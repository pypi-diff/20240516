# Comparing `tmp/google-maps-fleetengine-delivery-0.1.8.tar.gz` & `tmp/google-maps-fleetengine-delivery-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-fleetengine-delivery-0.1.8.tar", last modified: Tue May  7 20:43:59 2024, max compression
+gzip compressed data, was "google-maps-fleetengine-delivery-0.2.0.tar", last modified: Thu May 16 17:16:01 2024, max compression
```

## Comparing `google-maps-fleetengine-delivery-0.1.8.tar` & `google-maps-fleetengine-delivery-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5839 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4391 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.571007 google-maps-fleetengine-delivery-0.1.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.571007 google-maps-fleetengine-delivery-0.1.8/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.571007 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/
--rw-rw-r--   0 root         (0)     1003     2996 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/
--rw-rw-r--   0 root         (0)     1003     2634 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4838 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/
--rw-rw-r--   0 root         (0)     1003      773 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    75315 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    93141 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py
--rw-rw-r--   0 root         (0)     1003    16072 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.575008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14692 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23901 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24445 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    68054 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/
--rw-rw-r--   0 root         (0)     1003     2320 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16752 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    25036 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_api.py
--rw-rw-r--   0 root         (0)     1003    17286 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py
--rw-rw-r--   0 root         (0)     1003     5374 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/header.py
--rw-rw-r--   0 root         (0)     1003     6215 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py
--rw-rw-r--   0 root         (0)     1003    19744 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/
--rw-r--r--   0 root         (0)     1003     5839 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2065 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      338 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:43:59.000000 google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3260 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.579008 google-maps-fleetengine-delivery-0.1.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:59.583009 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   349414 2024-05-07 20:40:13.000000 google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5839 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4391 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.936533 google-maps-fleetengine-delivery-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.936533 google-maps-fleetengine-delivery-0.2.0/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.940533 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery/
+-rw-rw-r--   0 root         (0)     1003     2894 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.940533 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/
+-rw-rw-r--   0 root         (0)     1003     2532 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4484 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.940533 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.944533 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/
+-rw-rw-r--   0 root         (0)     1003      773 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    68819 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    87661 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11092 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.944533 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13876 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23327 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29575 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    62974 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.944533 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2218 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16752 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    21735 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/delivery_api.py
+-rw-rw-r--   0 root         (0)     1003    17149 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py
+-rw-rw-r--   0 root         (0)     1003     5374 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/header.py
+-rw-rw-r--   0 root         (0)     1003     6215 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py
+-rw-rw-r--   0 root         (0)     1003    19744 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/
+-rw-r--r--   0 root         (0)     1003     5839 2024-05-16 17:16:01.000000 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2065 2024-05-16 17:16:01.000000 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 17:16:01.000000 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 17:16:01.000000 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      338 2024-05-16 17:16:01.000000 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-16 17:16:01.000000 google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3260 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:01.948533 google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/fleetengine_delivery_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/fleetengine_delivery_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   367088 2024-05-16 17:11:30.000000 google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/LICENSE` & `google-maps-fleetengine-delivery-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/MANIFEST.in` & `google-maps-fleetengine-delivery-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/PKG-INFO` & `google-maps-fleetengine-delivery-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-fleetengine-delivery
-Version: 0.1.8
+Version: 0.2.0
 Summary: Google Maps Fleetengine Delivery API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine-delivery
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/README.rst` & `google-maps-fleetengine-delivery-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,16 +40,14 @@
     GetDeliveryVehicleRequest,
     GetTaskRequest,
     GetTaskTrackingInfoRequest,
     ListDeliveryVehiclesRequest,
     ListDeliveryVehiclesResponse,
     ListTasksRequest,
     ListTasksResponse,
-    SearchTasksRequest,
-    SearchTasksResponse,
     UpdateDeliveryVehicleRequest,
     UpdateTaskRequest,
 )
 from google.maps.fleetengine_delivery_v1.types.delivery_vehicles import (
     DeliveryVehicle,
     LocationInfo,
     VehicleJourneySegment,
@@ -77,16 +75,14 @@
     "GetDeliveryVehicleRequest",
     "GetTaskRequest",
     "GetTaskTrackingInfoRequest",
     "ListDeliveryVehiclesRequest",
     "ListDeliveryVehiclesResponse",
     "ListTasksRequest",
     "ListTasksResponse",
-    "SearchTasksRequest",
-    "SearchTasksResponse",
     "UpdateDeliveryVehicleRequest",
     "UpdateTaskRequest",
     "DeliveryVehicle",
     "LocationInfo",
     "VehicleJourneySegment",
     "VehicleStop",
     "DeliveryRequestHeader",
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery/gapic_version.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,16 +35,14 @@
     GetDeliveryVehicleRequest,
     GetTaskRequest,
     GetTaskTrackingInfoRequest,
     ListDeliveryVehiclesRequest,
     ListDeliveryVehiclesResponse,
     ListTasksRequest,
     ListTasksResponse,
-    SearchTasksRequest,
-    SearchTasksResponse,
     UpdateDeliveryVehicleRequest,
     UpdateTaskRequest,
 )
 from .types.delivery_vehicles import (
     DeliveryVehicle,
     LocationInfo,
     VehicleJourneySegment,
@@ -71,16 +69,14 @@
     "GetTaskRequest",
     "GetTaskTrackingInfoRequest",
     "ListDeliveryVehiclesRequest",
     "ListDeliveryVehiclesResponse",
     "ListTasksRequest",
     "ListTasksResponse",
     "LocationInfo",
-    "SearchTasksRequest",
-    "SearchTasksResponse",
     "Task",
     "TaskAttribute",
     "TaskTrackingInfo",
     "TaskTrackingViewConfig",
     "TimeWindow",
     "UpdateDeliveryVehicleRequest",
     "UpdateTaskRequest",
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_metadata.json` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/gapic_metadata.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997632575757575%*

 * *Differences: {"'services'": "{'DeliveryService': {'clients': {'grpc': {'rpcs': {delete: ['SearchTasks']}}, "*

 * *               "'grpc-async': {'rpcs': {delete: ['SearchTasks']}}, 'rest': {'rpcs': {delete: "*

 * *               "['SearchTasks']}}}}}"}*

```diff
@@ -46,19 +46,14 @@
                             ]
                         },
                         "ListTasks": {
                             "methods": [
                                 "list_tasks"
                             ]
                         },
-                        "SearchTasks": {
-                            "methods": [
-                                "search_tasks"
-                            ]
-                        },
                         "UpdateDeliveryVehicle": {
                             "methods": [
                                 "update_delivery_vehicle"
                             ]
                         },
                         "UpdateTask": {
                             "methods": [
@@ -106,19 +101,14 @@
                             ]
                         },
                         "ListTasks": {
                             "methods": [
                                 "list_tasks"
                             ]
                         },
-                        "SearchTasks": {
-                            "methods": [
-                                "search_tasks"
-                            ]
-                        },
                         "UpdateDeliveryVehicle": {
                             "methods": [
                                 "update_delivery_vehicle"
                             ]
                         },
                         "UpdateTask": {
                             "methods": [
@@ -166,19 +156,14 @@
                             ]
                         },
                         "ListTasks": {
                             "methods": [
                                 "list_tasks"
                             ]
                         },
-                        "SearchTasks": {
-                            "methods": [
-                                "search_tasks"
-                            ]
-                        },
                         "UpdateDeliveryVehicle": {
                             "methods": [
                                 "update_delivery_vehicle"
                             ]
                         },
                         "UpdateTask": {
                             "methods": [
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/gapic_version.py` & `google-maps-fleetengine-delivery-0.2.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,42 +10,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-import functools
+import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
+    cast,
 )
 import warnings
 
+from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry_async as retries
-from google.api_core.client_options import ClientOptions
+from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.auth.exceptions import MutualTLSChannelError  # type: ignore
+from google.auth.transport import mtls  # type: ignore
+from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.maps.fleetengine_delivery_v1 import gapic_version as package_version
 
 try:
-    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault, None]
+    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault, None]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.AsyncRetry, object, None]  # type: ignore
+    OptionalRetry = Union[retries.Retry, object, None]  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 from google.type import latlng_pb2  # type: ignore
 
@@ -54,106 +59,283 @@
     common,
     delivery_api,
     delivery_vehicles,
     task_tracking_info,
     tasks,
 )
 
-from .client import DeliveryServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, DeliveryServiceTransport
+from .transports.grpc import DeliveryServiceGrpcTransport
 from .transports.grpc_asyncio import DeliveryServiceGrpcAsyncIOTransport
+from .transports.rest import DeliveryServiceRestTransport
 
 
-class DeliveryServiceAsyncClient:
+class DeliveryServiceClientMeta(type):
+    """Metaclass for the DeliveryService client.
+
+    This provides class-level methods for building and retrieving
+    support objects (e.g. transport) without polluting the client instance
+    objects.
+    """
+
+    _transport_registry = (
+        OrderedDict()
+    )  # type: Dict[str, Type[DeliveryServiceTransport]]
+    _transport_registry["grpc"] = DeliveryServiceGrpcTransport
+    _transport_registry["grpc_asyncio"] = DeliveryServiceGrpcAsyncIOTransport
+    _transport_registry["rest"] = DeliveryServiceRestTransport
+
+    def get_transport_class(
+        cls,
+        label: Optional[str] = None,
+    ) -> Type[DeliveryServiceTransport]:
+        """Returns an appropriate transport class.
+
+        Args:
+            label: The name of the desired transport. If none is
+                provided, then the first transport in the registry is used.
+
+        Returns:
+            The transport class to use.
+        """
+        # If a specific transport is requested, return that one.
+        if label:
+            return cls._transport_registry[label]
+
+        # No transport is requested; return the default (that is, the first one
+        # in the dictionary).
+        return next(iter(cls._transport_registry.values()))
+
+
+class DeliveryServiceClient(metaclass=DeliveryServiceClientMeta):
     """The Last Mile Delivery service."""
 
-    _client: DeliveryServiceClient
+    @staticmethod
+    def _get_default_mtls_endpoint(api_endpoint):
+        """Converts api endpoint to mTLS endpoint.
+
+        Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
+        "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
+        Args:
+            api_endpoint (Optional[str]): the api endpoint to convert.
+        Returns:
+            str: converted mTLS api endpoint.
+        """
+        if not api_endpoint:
+            return api_endpoint
+
+        mtls_endpoint_re = re.compile(
+            r"(?P<name>[^.]+)(?P<mtls>\.mtls)?(?P<sandbox>\.sandbox)?(?P<googledomain>\.googleapis\.com)?"
+        )
+
+        m = mtls_endpoint_re.match(api_endpoint)
+        name, mtls, sandbox, googledomain = m.groups()
+        if mtls or not googledomain:
+            return api_endpoint
+
+        if sandbox:
+            return api_endpoint.replace(
+                "sandbox.googleapis.com", "mtls.sandbox.googleapis.com"
+            )
+
+        return api_endpoint.replace(".googleapis.com", ".mtls.googleapis.com")
 
-    # Copy defaults from the synchronous client for use here.
     # Note: DEFAULT_ENDPOINT is deprecated. Use _DEFAULT_ENDPOINT_TEMPLATE instead.
-    DEFAULT_ENDPOINT = DeliveryServiceClient.DEFAULT_ENDPOINT
-    DEFAULT_MTLS_ENDPOINT = DeliveryServiceClient.DEFAULT_MTLS_ENDPOINT
-    _DEFAULT_ENDPOINT_TEMPLATE = DeliveryServiceClient._DEFAULT_ENDPOINT_TEMPLATE
-    _DEFAULT_UNIVERSE = DeliveryServiceClient._DEFAULT_UNIVERSE
-
-    delivery_vehicle_path = staticmethod(DeliveryServiceClient.delivery_vehicle_path)
-    parse_delivery_vehicle_path = staticmethod(
-        DeliveryServiceClient.parse_delivery_vehicle_path
-    )
-    task_path = staticmethod(DeliveryServiceClient.task_path)
-    parse_task_path = staticmethod(DeliveryServiceClient.parse_task_path)
-    task_tracking_info_path = staticmethod(
-        DeliveryServiceClient.task_tracking_info_path
-    )
-    parse_task_tracking_info_path = staticmethod(
-        DeliveryServiceClient.parse_task_tracking_info_path
-    )
-    common_billing_account_path = staticmethod(
-        DeliveryServiceClient.common_billing_account_path
-    )
-    parse_common_billing_account_path = staticmethod(
-        DeliveryServiceClient.parse_common_billing_account_path
-    )
-    common_folder_path = staticmethod(DeliveryServiceClient.common_folder_path)
-    parse_common_folder_path = staticmethod(
-        DeliveryServiceClient.parse_common_folder_path
-    )
-    common_organization_path = staticmethod(
-        DeliveryServiceClient.common_organization_path
-    )
-    parse_common_organization_path = staticmethod(
-        DeliveryServiceClient.parse_common_organization_path
-    )
-    common_project_path = staticmethod(DeliveryServiceClient.common_project_path)
-    parse_common_project_path = staticmethod(
-        DeliveryServiceClient.parse_common_project_path
-    )
-    common_location_path = staticmethod(DeliveryServiceClient.common_location_path)
-    parse_common_location_path = staticmethod(
-        DeliveryServiceClient.parse_common_location_path
+    DEFAULT_ENDPOINT = "fleetengine.googleapis.com"
+    DEFAULT_MTLS_ENDPOINT = _get_default_mtls_endpoint.__func__(  # type: ignore
+        DEFAULT_ENDPOINT
     )
 
+    _DEFAULT_ENDPOINT_TEMPLATE = "fleetengine.{UNIVERSE_DOMAIN}"
+    _DEFAULT_UNIVERSE = "googleapis.com"
+
     @classmethod
     def from_service_account_info(cls, info: dict, *args, **kwargs):
         """Creates an instance of this client using the provided credentials
             info.
 
         Args:
             info (dict): The service account private key info.
             args: Additional arguments to pass to the constructor.
             kwargs: Additional arguments to pass to the constructor.
 
         Returns:
-            DeliveryServiceAsyncClient: The constructed client.
+            DeliveryServiceClient: The constructed client.
         """
-        return DeliveryServiceClient.from_service_account_info.__func__(DeliveryServiceAsyncClient, info, *args, **kwargs)  # type: ignore
+        credentials = service_account.Credentials.from_service_account_info(info)
+        kwargs["credentials"] = credentials
+        return cls(*args, **kwargs)
 
     @classmethod
     def from_service_account_file(cls, filename: str, *args, **kwargs):
         """Creates an instance of this client using the provided credentials
             file.
 
         Args:
             filename (str): The path to the service account private key json
                 file.
             args: Additional arguments to pass to the constructor.
             kwargs: Additional arguments to pass to the constructor.
 
         Returns:
-            DeliveryServiceAsyncClient: The constructed client.
+            DeliveryServiceClient: The constructed client.
         """
-        return DeliveryServiceClient.from_service_account_file.__func__(DeliveryServiceAsyncClient, filename, *args, **kwargs)  # type: ignore
+        credentials = service_account.Credentials.from_service_account_file(filename)
+        kwargs["credentials"] = credentials
+        return cls(*args, **kwargs)
 
     from_service_account_json = from_service_account_file
 
+    @property
+    def transport(self) -> DeliveryServiceTransport:
+        """Returns the transport used by the client instance.
+
+        Returns:
+            DeliveryServiceTransport: The transport used by the client
+                instance.
+        """
+        return self._transport
+
+    @staticmethod
+    def delivery_vehicle_path(
+        provider: str,
+        vehicle: str,
+    ) -> str:
+        """Returns a fully-qualified delivery_vehicle string."""
+        return "providers/{provider}/deliveryVehicles/{vehicle}".format(
+            provider=provider,
+            vehicle=vehicle,
+        )
+
+    @staticmethod
+    def parse_delivery_vehicle_path(path: str) -> Dict[str, str]:
+        """Parses a delivery_vehicle path into its component segments."""
+        m = re.match(
+            r"^providers/(?P<provider>.+?)/deliveryVehicles/(?P<vehicle>.+?)$", path
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def task_path(
+        provider: str,
+        task: str,
+    ) -> str:
+        """Returns a fully-qualified task string."""
+        return "providers/{provider}/tasks/{task}".format(
+            provider=provider,
+            task=task,
+        )
+
+    @staticmethod
+    def parse_task_path(path: str) -> Dict[str, str]:
+        """Parses a task path into its component segments."""
+        m = re.match(r"^providers/(?P<provider>.+?)/tasks/(?P<task>.+?)$", path)
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def task_tracking_info_path(
+        provider: str,
+        tracking: str,
+    ) -> str:
+        """Returns a fully-qualified task_tracking_info string."""
+        return "providers/{provider}/taskTrackingInfo/{tracking}".format(
+            provider=provider,
+            tracking=tracking,
+        )
+
+    @staticmethod
+    def parse_task_tracking_info_path(path: str) -> Dict[str, str]:
+        """Parses a task_tracking_info path into its component segments."""
+        m = re.match(
+            r"^providers/(?P<provider>.+?)/taskTrackingInfo/(?P<tracking>.+?)$", path
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
+        """Returns a fully-qualified billing_account string."""
+        return "billingAccounts/{billing_account}".format(
+            billing_account=billing_account,
+        )
+
+    @staticmethod
+    def parse_common_billing_account_path(path: str) -> Dict[str, str]:
+        """Parse a billing_account path into its component segments."""
+        m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def common_folder_path(
+        folder: str,
+    ) -> str:
+        """Returns a fully-qualified folder string."""
+        return "folders/{folder}".format(
+            folder=folder,
+        )
+
+    @staticmethod
+    def parse_common_folder_path(path: str) -> Dict[str, str]:
+        """Parse a folder path into its component segments."""
+        m = re.match(r"^folders/(?P<folder>.+?)$", path)
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def common_organization_path(
+        organization: str,
+    ) -> str:
+        """Returns a fully-qualified organization string."""
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
+
+    @staticmethod
+    def parse_common_organization_path(path: str) -> Dict[str, str]:
+        """Parse a organization path into its component segments."""
+        m = re.match(r"^organizations/(?P<organization>.+?)$", path)
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def common_project_path(
+        project: str,
+    ) -> str:
+        """Returns a fully-qualified project string."""
+        return "projects/{project}".format(
+            project=project,
+        )
+
+    @staticmethod
+    def parse_common_project_path(path: str) -> Dict[str, str]:
+        """Parse a project path into its component segments."""
+        m = re.match(r"^projects/(?P<project>.+?)$", path)
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
+        """Returns a fully-qualified location string."""
+        return "projects/{project}/locations/{location}".format(
+            project=project,
+            location=location,
+        )
+
+    @staticmethod
+    def parse_common_location_path(path: str) -> Dict[str, str]:
+        """Parse a location path into its component segments."""
+        m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
+        return m.groupdict() if m else {}
+
     @classmethod
     def get_mtls_endpoint_and_cert_source(
-        cls, client_options: Optional[ClientOptions] = None
+        cls, client_options: Optional[client_options_lib.ClientOptions] = None
     ):
-        """Return the API endpoint and client cert source for mutual TLS.
+        """Deprecated. Return the API endpoint and client cert source for mutual TLS.
 
         The client cert source is determined in the following order:
         (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
         client cert source is None.
         (2) if `client_options.client_cert_source` is provided, use the provided one; if the
         default client cert source exists, use the default one; otherwise the client cert
         source is None.
@@ -175,67 +357,249 @@
         Returns:
             Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
                 client cert source to use.
 
         Raises:
             google.auth.exceptions.MutualTLSChannelError: If any errors happen.
         """
-        return DeliveryServiceClient.get_mtls_endpoint_and_cert_source(client_options)  # type: ignore
 
-    @property
-    def transport(self) -> DeliveryServiceTransport:
-        """Returns the transport used by the client instance.
+        warnings.warn(
+            "get_mtls_endpoint_and_cert_source is deprecated. Use the api_endpoint property instead.",
+            DeprecationWarning,
+        )
+        if client_options is None:
+            client_options = client_options_lib.ClientOptions()
+        use_client_cert = os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false")
+        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
+        if use_client_cert not in ("true", "false"):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        if use_mtls_endpoint not in ("auto", "never", "always"):
+            raise MutualTLSChannelError(
+                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
+            )
+
+        # Figure out the client cert source to use.
+        client_cert_source = None
+        if use_client_cert == "true":
+            if client_options.client_cert_source:
+                client_cert_source = client_options.client_cert_source
+            elif mtls.has_default_client_cert_source():
+                client_cert_source = mtls.default_client_cert_source()
+
+        # Figure out which api endpoint to use.
+        if client_options.api_endpoint is not None:
+            api_endpoint = client_options.api_endpoint
+        elif use_mtls_endpoint == "always" or (
+            use_mtls_endpoint == "auto" and client_cert_source
+        ):
+            api_endpoint = cls.DEFAULT_MTLS_ENDPOINT
+        else:
+            api_endpoint = cls.DEFAULT_ENDPOINT
+
+        return api_endpoint, client_cert_source
+
+    @staticmethod
+    def _read_environment_variables():
+        """Returns the environment variables used by the client.
 
         Returns:
-            DeliveryServiceTransport: The transport used by the client instance.
+            Tuple[bool, str, str]: returns the GOOGLE_API_USE_CLIENT_CERTIFICATE,
+            GOOGLE_API_USE_MTLS_ENDPOINT, and GOOGLE_CLOUD_UNIVERSE_DOMAIN environment variables.
+
+        Raises:
+            ValueError: If GOOGLE_API_USE_CLIENT_CERTIFICATE is not
+                any of ["true", "false"].
+            google.auth.exceptions.MutualTLSChannelError: If GOOGLE_API_USE_MTLS_ENDPOINT
+                is not any of ["auto", "never", "always"].
         """
-        return self._client.transport
+        use_client_cert = os.getenv(
+            "GOOGLE_API_USE_CLIENT_CERTIFICATE", "false"
+        ).lower()
+        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto").lower()
+        universe_domain_env = os.getenv("GOOGLE_CLOUD_UNIVERSE_DOMAIN")
+        if use_client_cert not in ("true", "false"):
+            raise ValueError(
+                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
+            )
+        if use_mtls_endpoint not in ("auto", "never", "always"):
+            raise MutualTLSChannelError(
+                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
+            )
+        return use_client_cert == "true", use_mtls_endpoint, universe_domain_env
+
+    @staticmethod
+    def _get_client_cert_source(provided_cert_source, use_cert_flag):
+        """Return the client cert source to be used by the client.
+
+        Args:
+            provided_cert_source (bytes): The client certificate source provided.
+            use_cert_flag (bool): A flag indicating whether to use the client certificate.
+
+        Returns:
+            bytes or None: The client cert source to be used by the client.
+        """
+        client_cert_source = None
+        if use_cert_flag:
+            if provided_cert_source:
+                client_cert_source = provided_cert_source
+            elif mtls.has_default_client_cert_source():
+                client_cert_source = mtls.default_client_cert_source()
+        return client_cert_source
+
+    @staticmethod
+    def _get_api_endpoint(
+        api_override, client_cert_source, universe_domain, use_mtls_endpoint
+    ):
+        """Return the API endpoint used by the client.
+
+        Args:
+            api_override (str): The API endpoint override. If specified, this is always
+                the return value of this function and the other arguments are not used.
+            client_cert_source (bytes): The client certificate source used by the client.
+            universe_domain (str): The universe domain used by the client.
+            use_mtls_endpoint (str): How to use the mTLS endpoint, which depends also on the other parameters.
+                Possible values are "always", "auto", or "never".
+
+        Returns:
+            str: The API endpoint to be used by the client.
+        """
+        if api_override is not None:
+            api_endpoint = api_override
+        elif use_mtls_endpoint == "always" or (
+            use_mtls_endpoint == "auto" and client_cert_source
+        ):
+            _default_universe = DeliveryServiceClient._DEFAULT_UNIVERSE
+            if universe_domain != _default_universe:
+                raise MutualTLSChannelError(
+                    f"mTLS is not supported in any universe other than {_default_universe}."
+                )
+            api_endpoint = DeliveryServiceClient.DEFAULT_MTLS_ENDPOINT
+        else:
+            api_endpoint = DeliveryServiceClient._DEFAULT_ENDPOINT_TEMPLATE.format(
+                UNIVERSE_DOMAIN=universe_domain
+            )
+        return api_endpoint
+
+    @staticmethod
+    def _get_universe_domain(
+        client_universe_domain: Optional[str], universe_domain_env: Optional[str]
+    ) -> str:
+        """Return the universe domain used by the client.
+
+        Args:
+            client_universe_domain (Optional[str]): The universe domain configured via the client options.
+            universe_domain_env (Optional[str]): The universe domain configured via the "GOOGLE_CLOUD_UNIVERSE_DOMAIN" environment variable.
+
+        Returns:
+            str: The universe domain to be used by the client.
+
+        Raises:
+            ValueError: If the universe domain is an empty string.
+        """
+        universe_domain = DeliveryServiceClient._DEFAULT_UNIVERSE
+        if client_universe_domain is not None:
+            universe_domain = client_universe_domain
+        elif universe_domain_env is not None:
+            universe_domain = universe_domain_env
+        if len(universe_domain.strip()) == 0:
+            raise ValueError("Universe Domain cannot be an empty string.")
+        return universe_domain
+
+    @staticmethod
+    def _compare_universes(
+        client_universe: str, credentials: ga_credentials.Credentials
+    ) -> bool:
+        """Returns True iff the universe domains used by the client and credentials match.
+
+        Args:
+            client_universe (str): The universe domain configured via the client options.
+            credentials (ga_credentials.Credentials): The credentials being used in the client.
+
+        Returns:
+            bool: True iff client_universe matches the universe in credentials.
+
+        Raises:
+            ValueError: when client_universe does not match the universe in credentials.
+        """
+
+        default_universe = DeliveryServiceClient._DEFAULT_UNIVERSE
+        credentials_universe = getattr(credentials, "universe_domain", default_universe)
+
+        if client_universe != credentials_universe:
+            raise ValueError(
+                "The configured universe domain "
+                f"({client_universe}) does not match the universe domain "
+                f"found in the credentials ({credentials_universe}). "
+                "If you haven't configured the universe domain explicitly, "
+                f"`{default_universe}` is the default."
+            )
+        return True
+
+    def _validate_universe_domain(self):
+        """Validates client's and credentials' universe domains are consistent.
+
+        Returns:
+            bool: True iff the configured universe domain is valid.
+
+        Raises:
+            ValueError: If the configured universe domain is not valid.
+        """
+        self._is_universe_domain_valid = (
+            self._is_universe_domain_valid
+            or DeliveryServiceClient._compare_universes(
+                self.universe_domain, self.transport._credentials
+            )
+        )
+        return self._is_universe_domain_valid
 
     @property
     def api_endpoint(self):
         """Return the API endpoint used by the client instance.
 
         Returns:
             str: The API endpoint used by the client instance.
         """
-        return self._client._api_endpoint
+        return self._api_endpoint
 
     @property
     def universe_domain(self) -> str:
         """Return the universe domain used by the client instance.
 
         Returns:
-            str: The universe domain used
-                by the client instance.
+            str: The universe domain used by the client instance.
         """
-        return self._client._universe_domain
-
-    get_transport_class = functools.partial(
-        type(DeliveryServiceClient).get_transport_class, type(DeliveryServiceClient)
-    )
+        return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, DeliveryServiceTransport] = "grpc_asyncio",
-        client_options: Optional[ClientOptions] = None,
+        transport: Optional[
+            Union[
+                str, DeliveryServiceTransport, Callable[..., DeliveryServiceTransport]
+            ]
+        ] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
-        """Instantiates the delivery service async client.
+        """Instantiates the delivery service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.DeliveryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,DeliveryServiceTransport,Callable[..., DeliveryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the DeliveryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -250,36 +614,121 @@
                 is "true", then the ``client_cert_source`` property can be used
                 to provide a client certificate for mTLS transport. If
                 not provided, the default SSL client certificate will be used if
                 present. If GOOGLE_API_USE_CLIENT_CERTIFICATE is "false" or not
                 set, no client certificate will be used.
 
                 3. The ``universe_domain`` property can be used to override the
-                default "googleapis.com" universe. Note that ``api_endpoint``
+                default "googleapis.com" universe. Note that the ``api_endpoint``
                 property still takes precedence; and ``universe_domain`` is
                 currently not supported for mTLS.
 
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
-        self._client = DeliveryServiceClient(
-            credentials=credentials,
-            transport=transport,
-            client_options=client_options,
-            client_info=client_info,
+        self._client_options = client_options
+        if isinstance(self._client_options, dict):
+            self._client_options = client_options_lib.from_dict(self._client_options)
+        if self._client_options is None:
+            self._client_options = client_options_lib.ClientOptions()
+        self._client_options = cast(
+            client_options_lib.ClientOptions, self._client_options
+        )
+
+        universe_domain_opt = getattr(self._client_options, "universe_domain", None)
+
+        (
+            self._use_client_cert,
+            self._use_mtls_endpoint,
+            self._universe_domain_env,
+        ) = DeliveryServiceClient._read_environment_variables()
+        self._client_cert_source = DeliveryServiceClient._get_client_cert_source(
+            self._client_options.client_cert_source, self._use_client_cert
+        )
+        self._universe_domain = DeliveryServiceClient._get_universe_domain(
+            universe_domain_opt, self._universe_domain_env
         )
+        self._api_endpoint = None  # updated below, depending on `transport`
+
+        # Initialize the universe domain validation.
+        self._is_universe_domain_valid = False
+
+        api_key_value = getattr(self._client_options, "api_key", None)
+        if api_key_value and credentials:
+            raise ValueError(
+                "client_options.api_key and credentials are mutually exclusive"
+            )
+
+        # Save or instantiate the transport.
+        # Ordinarily, we provide the transport, but allowing a custom transport
+        # instance provides an extensibility point for unusual situations.
+        transport_provided = isinstance(transport, DeliveryServiceTransport)
+        if transport_provided:
+            # transport is a DeliveryServiceTransport instance.
+            if credentials or self._client_options.credentials_file or api_key_value:
+                raise ValueError(
+                    "When providing a transport instance, "
+                    "provide its credentials directly."
+                )
+            if self._client_options.scopes:
+                raise ValueError(
+                    "When providing a transport instance, provide its scopes "
+                    "directly."
+                )
+            self._transport = cast(DeliveryServiceTransport, transport)
+            self._api_endpoint = self._transport.host
+
+        self._api_endpoint = (
+            self._api_endpoint
+            or DeliveryServiceClient._get_api_endpoint(
+                self._client_options.api_endpoint,
+                self._client_cert_source,
+                self._universe_domain,
+                self._use_mtls_endpoint,
+            )
+        )
+
+        if not transport_provided:
+            import google.auth._default  # type: ignore
 
-    async def create_delivery_vehicle(
+            if api_key_value and hasattr(
+                google.auth._default, "get_api_key_credentials"
+            ):
+                credentials = google.auth._default.get_api_key_credentials(
+                    api_key_value
+                )
+
+            transport_init: Union[
+                Type[DeliveryServiceTransport], Callable[..., DeliveryServiceTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., DeliveryServiceTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
+                credentials=credentials,
+                credentials_file=self._client_options.credentials_file,
+                host=self._api_endpoint,
+                scopes=self._client_options.scopes,
+                client_cert_source_for_mtls=self._client_cert_source,
+                quota_project_id=self._client_options.quota_project_id,
+                client_info=client_info,
+                always_use_jwt_access=True,
+                api_audience=self._client_options.api_audience,
+            )
+
+    def create_delivery_vehicle(
         self,
         request: Optional[
             Union[delivery_api.CreateDeliveryVehicleRequest, dict]
         ] = None,
         *,
         parent: Optional[str] = None,
         delivery_vehicle: Optional[delivery_vehicles.DeliveryVehicle] = None,
@@ -297,72 +746,72 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_create_delivery_vehicle():
+            def sample_create_delivery_vehicle():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.CreateDeliveryVehicleRequest(
                     parent="parent_value",
                     delivery_vehicle_id="delivery_vehicle_id_value",
                 )
 
                 # Make the request
-                response = await client.create_delivery_vehicle(request=request)
+                response = client.create_delivery_vehicle(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.CreateDeliveryVehicleRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.CreateDeliveryVehicleRequest, dict]):
                 The request object. The ``CreateDeliveryVehicle`` request message.
-            parent (:class:`str`):
+            parent (str):
                 Required. Must be in the format
                 ``providers/{provider}``. The provider must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            delivery_vehicle (:class:`google.maps.fleetengine_delivery_v1.types.DeliveryVehicle`):
+            delivery_vehicle (google.maps.fleetengine_delivery_v1.types.DeliveryVehicle):
                 Required. The ``DeliveryVehicle`` entity to create. When
                 creating a new delivery vehicle, you may set the
                 following optional fields:
 
                 -  last_location
                 -  attributes
 
                 Note: The DeliveryVehicle's ``name`` field is ignored.
                 All other DeliveryVehicle fields must not be set;
                 otherwise, an error is returned.
 
                 This corresponds to the ``delivery_vehicle`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            delivery_vehicle_id (:class:`str`):
+            delivery_vehicle_id (str):
                 Required. The Delivery Vehicle ID must be unique and
                 subject to the following restrictions:
 
                 -  Must be a valid Unicode string.
                 -  Limited to a maximum length of 64 characters.
                 -  Normalized according to [Unicode Normalization Form
                    C] (http://www.unicode.org/reports/tr15/).
                 -  May not contain any of the following ASCII
                    characters: '/', ':', '?', ',', or '#'.
 
                 This corresponds to the ``delivery_vehicle_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.DeliveryVehicle:
@@ -376,72 +825,67 @@
                    conventions. For example, the
                    DeliveryVehicle.current_route_segment field in the
                    gRPC API and the DeliveryVehicle.currentRouteSegment
                    field in the REST API refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, delivery_vehicle, delivery_vehicle_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.CreateDeliveryVehicleRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if parent is not None:
-            request.parent = parent
-        if delivery_vehicle is not None:
-            request.delivery_vehicle = delivery_vehicle
-        if delivery_vehicle_id is not None:
-            request.delivery_vehicle_id = delivery_vehicle_id
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.CreateDeliveryVehicleRequest):
+            request = delivery_api.CreateDeliveryVehicleRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+            if delivery_vehicle is not None:
+                request.delivery_vehicle = delivery_vehicle
+            if delivery_vehicle_id is not None:
+                request.delivery_vehicle_id = delivery_vehicle_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_delivery_vehicle,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.create_delivery_vehicle]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def get_delivery_vehicle(
+    def get_delivery_vehicle(
         self,
         request: Optional[Union[delivery_api.GetDeliveryVehicleRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -455,42 +899,42 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_get_delivery_vehicle():
+            def sample_get_delivery_vehicle():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.GetDeliveryVehicleRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = await client.get_delivery_vehicle(request=request)
+                response = client.get_delivery_vehicle(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.GetDeliveryVehicleRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.GetDeliveryVehicleRequest, dict]):
                 The request object. The ``GetDeliveryVehicle`` request message.
-            name (:class:`str`):
+            name (str):
                 Required. Must be in the format
                 ``providers/{provider}/deliveryVehicles/{delivery_vehicle}``.
                 The ``provider`` must be the Google Cloud Project ID.
                 For example, ``sample-cloud-project``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.DeliveryVehicle:
@@ -504,68 +948,63 @@
                    conventions. For example, the
                    DeliveryVehicle.current_route_segment field in the
                    gRPC API and the DeliveryVehicle.currentRouteSegment
                    field in the REST API refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.GetDeliveryVehicleRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if name is not None:
-            request.name = name
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.GetDeliveryVehicleRequest):
+            request = delivery_api.GetDeliveryVehicleRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_delivery_vehicle,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.get_delivery_vehicle]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.name)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def update_delivery_vehicle(
+    def update_delivery_vehicle(
         self,
         request: Optional[
             Union[delivery_api.UpdateDeliveryVehicleRequest, dict]
         ] = None,
         *,
         delivery_vehicle: Optional[delivery_vehicles.DeliveryVehicle] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
@@ -590,52 +1029,52 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_update_delivery_vehicle():
+            def sample_update_delivery_vehicle():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.UpdateDeliveryVehicleRequest(
                 )
 
                 # Make the request
-                response = await client.update_delivery_vehicle(request=request)
+                response = client.update_delivery_vehicle(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.UpdateDeliveryVehicleRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.UpdateDeliveryVehicleRequest, dict]):
                 The request object. The ``UpdateDeliveryVehicle`` request message.
-            delivery_vehicle (:class:`google.maps.fleetengine_delivery_v1.types.DeliveryVehicle`):
+            delivery_vehicle (google.maps.fleetengine_delivery_v1.types.DeliveryVehicle):
                 Required. The ``DeliveryVehicle`` entity update to
                 apply. Note: You cannot update the name of the
                 ``DeliveryVehicle``.
 
                 This corresponds to the ``delivery_vehicle`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. A field mask that indicates which
                 ``DeliveryVehicle`` fields to update. Note that the
                 update_mask must contain at least one field.
 
                 This is a comma-separated list of fully qualified names
                 of fields. Example:
                 ``"remaining_vehicle_journey_segments"``.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.DeliveryVehicle:
@@ -649,72 +1088,65 @@
                    conventions. For example, the
                    DeliveryVehicle.current_route_segment field in the
                    gRPC API and the DeliveryVehicle.currentRouteSegment
                    field in the REST API refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([delivery_vehicle, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.UpdateDeliveryVehicleRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if delivery_vehicle is not None:
-            request.delivery_vehicle = delivery_vehicle
-        if update_mask is not None:
-            request.update_mask = update_mask
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.UpdateDeliveryVehicleRequest):
+            request = delivery_api.UpdateDeliveryVehicleRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if delivery_vehicle is not None:
+                request.delivery_vehicle = delivery_vehicle
+            if update_mask is not None:
+                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_delivery_vehicle,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata(
-                (("delivery_vehicle.name", request.delivery_vehicle.name),)
-            ),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.update_delivery_vehicle]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.delivery_vehicle.name)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def batch_create_tasks(
+    def batch_create_tasks(
         self,
         request: Optional[Union[delivery_api.BatchCreateTasksRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> delivery_api.BatchCreateTasksResponse:
@@ -727,90 +1159,86 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_batch_create_tasks():
+            def sample_batch_create_tasks():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 requests = fleetengine_delivery_v1.CreateTaskRequest()
                 requests.parent = "parent_value"
                 requests.task_id = "task_id_value"
                 requests.task.type_ = "UNAVAILABLE"
                 requests.task.state = "CLOSED"
 
                 request = fleetengine_delivery_v1.BatchCreateTasksRequest(
                     parent="parent_value",
                     requests=requests,
                 )
 
                 # Make the request
-                response = await client.batch_create_tasks(request=request)
+                response = client.batch_create_tasks(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.BatchCreateTasksRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.BatchCreateTasksRequest, dict]):
                 The request object. The ``BatchCreateTask`` request message.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.BatchCreateTasksResponse:
                 The BatchCreateTask response message.
         """
         # Create or coerce a protobuf request object.
-        request = delivery_api.BatchCreateTasksRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.BatchCreateTasksRequest):
+            request = delivery_api.BatchCreateTasksRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.batch_create_tasks,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.batch_create_tasks]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def create_task(
+    def create_task(
         self,
         request: Optional[Union[delivery_api.CreateTaskRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         task: Optional[tasks.Task] = None,
         task_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
@@ -826,48 +1254,48 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_create_task():
+            def sample_create_task():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 task = fleetengine_delivery_v1.Task()
                 task.type_ = "UNAVAILABLE"
                 task.state = "CLOSED"
 
                 request = fleetengine_delivery_v1.CreateTaskRequest(
                     parent="parent_value",
                     task_id="task_id_value",
                     task=task,
                 )
 
                 # Make the request
-                response = await client.create_task(request=request)
+                response = client.create_task(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.CreateTaskRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.CreateTaskRequest, dict]):
                 The request object. The ``CreateTask`` request message.
-            parent (:class:`str`):
+            parent (str):
                 Required. Must be in the format
                 ``providers/{provider}``. The ``provider`` must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            task (:class:`google.maps.fleetengine_delivery_v1.types.Task`):
+            task (google.maps.fleetengine_delivery_v1.types.Task):
                 Required. The Task entity to create. When creating a
                 Task, the following fields are required:
 
                 -  ``type``
                 -  ``state`` (must be set to ``OPEN``)
                 -  ``tracking_id`` (must not be set for ``UNAVAILABLE``
                    or ``SCHEDULED_STOP`` tasks, but required for all
@@ -879,15 +1307,15 @@
                 Note: The Task's ``name`` field is ignored. All other
                 Task fields must not be set; otherwise, an error is
                 returned.
 
                 This corresponds to the ``task`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            task_id (:class:`str`):
+            task_id (str):
                 Required. The Task ID must be unique, but it should be
                 not a shipment tracking ID. To store a shipment tracking
                 ID, use the ``tracking_id`` field. Note that multiple
                 tasks can have the same ``tracking_id``. Task IDs are
                 subject to the following restrictions:
 
                 -  Must be a valid Unicode string.
@@ -896,15 +1324,15 @@
                    C] (http://www.unicode.org/reports/tr15/).
                 -  May not contain any of the following ASCII
                    characters: '/', ':', '?', ',', or '#'.
 
                 This corresponds to the ``task_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.Task:
@@ -923,72 +1351,67 @@
                    conventions. For example, the
                    Task.journey_sharing_info field in the gRPC API and
                    the Task.journeySharingInfo field in the REST API
                    refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, task, task_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.CreateTaskRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if parent is not None:
-            request.parent = parent
-        if task is not None:
-            request.task = task
-        if task_id is not None:
-            request.task_id = task_id
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.CreateTaskRequest):
+            request = delivery_api.CreateTaskRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+            if task is not None:
+                request.task = task
+            if task_id is not None:
+                request.task_id = task_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_task,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.create_task]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def get_task(
+    def get_task(
         self,
         request: Optional[Union[delivery_api.GetTaskRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1002,42 +1425,42 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_get_task():
+            def sample_get_task():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.GetTaskRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = await client.get_task(request=request)
+                response = client.get_task(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.GetTaskRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.GetTaskRequest, dict]):
                 The request object. The ``GetTask`` request message.
-            name (:class:`str`):
+            name (str):
                 Required. Must be in the format
                 ``providers/{provider}/tasks/{task}``. The ``provider``
                 must be the Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.Task:
@@ -1056,202 +1479,63 @@
                    conventions. For example, the
                    Task.journey_sharing_info field in the gRPC API and
                    the Task.journeySharingInfo field in the REST API
                    refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.GetTaskRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if name is not None:
-            request.name = name
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.GetTaskRequest):
+            request = delivery_api.GetTaskRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_task,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Validate the universe domain.
-        self._client._validate_universe_domain()
-
-        # Send the request.
-        response = await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    async def search_tasks(
-        self,
-        request: Optional[Union[delivery_api.SearchTasksRequest, dict]] = None,
-        *,
-        parent: Optional[str] = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.SearchTasksAsyncPager:
-        r"""Deprecated: Use ``GetTaskTrackingInfo`` instead.
-
-        .. code-block:: python
-
-            # This snippet has been automatically generated and should be regarded as a
-            # code template only.
-            # It will require modifications to work:
-            # - It may require correct/in-range values for request initialization.
-            # - It may require specifying regional endpoints when creating the service
-            #   client as shown in:
-            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.maps import fleetengine_delivery_v1
-
-            async def sample_search_tasks():
-                # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
-
-                # Initialize request argument(s)
-                request = fleetengine_delivery_v1.SearchTasksRequest(
-                    parent="parent_value",
-                    tracking_id="tracking_id_value",
-                )
-
-                # Make the request
-                page_result = client.search_tasks(request=request)
-
-                # Handle the response
-                async for response in page_result:
-                    print(response)
-
-        Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.SearchTasksRequest, dict]]):
-                The request object. Deprecated: Issue ``GetTaskTrackingInfoRequest``\ s to
-                ``GetTaskTrackingInfo`` instead.
-            parent (:class:`str`):
-                Required. Must be in the format
-                ``providers/{provider}``. The provider must be the
-                Google Cloud Project ID. For example,
-                ``sample-cloud-project``.
-
-                This corresponds to the ``parent`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.SearchTasksAsyncPager:
-                The SearchTasks response. It contains the set of Tasks that meet the search
-                   criteria in the SearchTasksRequest.
-
-                Iterating over this object will yield results and
-                resolve additional pages automatically.
+        rpc = self._transport._wrapped_methods[self._transport.get_task]
 
-        """
-        warnings.warn(
-            "DeliveryServiceAsyncClient.search_tasks is deprecated", DeprecationWarning
-        )
+        header_params = {}
 
-        # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([parent])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.name)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
             )
 
-        request = delivery_api.SearchTasksRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if parent is not None:
-            request.parent = parent
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.search_tasks,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
-
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-        # This method is paged; wrap the response in a pager, which provides
-        # an `__aiter__` convenience method.
-        response = pagers.SearchTasksAsyncPager(
-            method=rpc,
-            request=request,
-            response=response,
-            metadata=metadata,
-        )
-
         # Done; return the response.
         return response
 
-    async def update_task(
+    def update_task(
         self,
         request: Optional[Union[delivery_api.UpdateTaskRequest, dict]] = None,
         *,
         task: Optional[tasks.Task] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
@@ -1266,37 +1550,37 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_update_task():
+            def sample_update_task():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 task = fleetengine_delivery_v1.Task()
                 task.type_ = "UNAVAILABLE"
                 task.state = "CLOSED"
 
                 request = fleetengine_delivery_v1.UpdateTaskRequest(
                     task=task,
                 )
 
                 # Make the request
-                response = await client.update_task(request=request)
+                response = client.update_task(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.UpdateTaskRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.UpdateTaskRequest, dict]):
                 The request object. The ``UpdateTask`` request message.
-            task (:class:`google.maps.fleetengine_delivery_v1.types.Task`):
+            task (google.maps.fleetengine_delivery_v1.types.Task):
                 Required. The Task associated with the update. The
                 following fields are maintained by Fleet Engine. Do not
                 update them using ``Task.update``.
 
                 -  ``last_location``.
                 -  ``last_location_snappable``.
                 -  ``name``.
@@ -1311,27 +1595,27 @@
                 ``Task.update``. Instead, remove the ``VehicleStop``
                 that contains the Task from the delivery vehicle, which
                 automatically sets the Task state to CLOSED.
 
                 This corresponds to the ``task`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. The field mask that indicates which Task
                 fields to update. Note: The ``update_mask`` must contain
                 at least one field.
 
                 This is a comma-separated list of fully qualified names
                 of fields. Example:
                 ``"task_outcome,task_outcome_time,task_outcome_location"``.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.Task:
@@ -1350,200 +1634,188 @@
                    conventions. For example, the
                    Task.journey_sharing_info field in the gRPC API and
                    the Task.journeySharingInfo field in the REST API
                    refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([task, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.UpdateTaskRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if task is not None:
-            request.task = task
-        if update_mask is not None:
-            request.update_mask = update_mask
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.UpdateTaskRequest):
+            request = delivery_api.UpdateTaskRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if task is not None:
+                request.task = task
+            if update_mask is not None:
+                request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_task,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata(
-                (("task.name", request.task.name),)
-            ),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.update_task]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.task.name)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def list_tasks(
+    def list_tasks(
         self,
         request: Optional[Union[delivery_api.ListTasksRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.ListTasksAsyncPager:
+    ) -> pagers.ListTasksPager:
         r"""Gets all ``Task``\ s that meet the specified filtering criteria.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_list_tasks():
+            def sample_list_tasks():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.ListTasksRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_tasks(request=request)
 
                 # Handle the response
-                async for response in page_result:
+                for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.ListTasksRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.ListTasksRequest, dict]):
                 The request object. The ``ListTasks`` request message.
-            parent (:class:`str`):
+            parent (str):
                 Required. Must be in the format
                 ``providers/{provider}``. The ``provider`` must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListTasksAsyncPager:
+            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListTasksPager:
                 The ListTasks response that contains the set of Tasks that meet the filter
                    criteria in the ListTasksRequest.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.ListTasksRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if parent is not None:
-            request.parent = parent
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.ListTasksRequest):
+            request = delivery_api.ListTasksRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_tasks,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.list_tasks]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # This method is paged; wrap the response in a pager, which provides
-        # an `__aiter__` convenience method.
-        response = pagers.ListTasksAsyncPager(
+        # an `__iter__` convenience method.
+        response = pagers.ListTasksPager(
             method=rpc,
             request=request,
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def get_task_tracking_info(
+    def get_task_tracking_info(
         self,
         request: Optional[Union[delivery_api.GetTaskTrackingInfoRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1557,44 +1829,44 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_get_task_tracking_info():
+            def sample_get_task_tracking_info():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.GetTaskTrackingInfoRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = await client.get_task_tracking_info(request=request)
+                response = client.get_task_tracking_info(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.GetTaskTrackingInfoRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.GetTaskTrackingInfoRequest, dict]):
                 The request object. The ``GetTaskTrackingInfoRequest`` request message.
-            name (:class:`str`):
+            name (str):
                 Required. Must be in the format
                 ``providers/{provider}/taskTrackingInfo/{tracking_id}``.
                 The ``provider`` must be the Google Cloud Project ID,
                 and the ``tracking_id`` must be the tracking ID
                 associated with the task. An example name can be
                 ``providers/sample-cloud-project/taskTrackingInfo/sample-tracking-id``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.TaskTrackingInfo:
@@ -1602,201 +1874,198 @@
                    information which will be used for display. If a
                    tracking ID is associated with multiple Tasks, Fleet
                    Engine uses a heuristic to decide which Task's
                    TaskTrackingInfo to select.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.GetTaskTrackingInfoRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if name is not None:
-            request.name = name
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.GetTaskTrackingInfoRequest):
+            request = delivery_api.GetTaskTrackingInfoRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_task_tracking_info,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.get_task_tracking_info]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.name)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def list_delivery_vehicles(
+    def list_delivery_vehicles(
         self,
         request: Optional[Union[delivery_api.ListDeliveryVehiclesRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.ListDeliveryVehiclesAsyncPager:
+    ) -> pagers.ListDeliveryVehiclesPager:
         r"""Gets all ``DeliveryVehicle``\ s that meet the specified
         filtering criteria.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            async def sample_list_delivery_vehicles():
+            def sample_list_delivery_vehicles():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
+                client = fleetengine_delivery_v1.DeliveryServiceClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.ListDeliveryVehiclesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_delivery_vehicles(request=request)
 
                 # Handle the response
-                async for response in page_result:
+                for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.ListDeliveryVehiclesRequest, dict]]):
+            request (Union[google.maps.fleetengine_delivery_v1.types.ListDeliveryVehiclesRequest, dict]):
                 The request object. The ``ListDeliveryVehicles`` request message.
-            parent (:class:`str`):
+            parent (str):
                 Required. Must be in the format
                 ``providers/{provider}``. The ``provider`` must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListDeliveryVehiclesAsyncPager:
+            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListDeliveryVehiclesPager:
                 The ListDeliveryVehicles response message.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = delivery_api.ListDeliveryVehiclesRequest(request)
-
-        # If we have keyword arguments corresponding to fields on the
-        # request, apply these.
-        if parent is not None:
-            request.parent = parent
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, delivery_api.ListDeliveryVehiclesRequest):
+            request = delivery_api.ListDeliveryVehiclesRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_delivery_vehicles,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
-        )
+        rpc = self._transport._wrapped_methods[self._transport.list_delivery_vehicles]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("provider_id"):
+            header_params["provider_id"] = regex_match.group("provider_id")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
 
         # Validate the universe domain.
-        self._client._validate_universe_domain()
+        self._validate_universe_domain()
 
         # Send the request.
-        response = await rpc(
+        response = rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # This method is paged; wrap the response in a pager, which provides
-        # an `__aiter__` convenience method.
-        response = pagers.ListDeliveryVehiclesAsyncPager(
+        # an `__iter__` convenience method.
+        response = pagers.ListDeliveryVehiclesPager(
             method=rpc,
             request=request,
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self) -> "DeliveryServiceAsyncClient":
+    def __enter__(self) -> "DeliveryServiceClient":
         return self
 
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.transport.close()
+    def __exit__(self, type, value, traceback):
+        """Releases underlying transport's resources.
+
+        .. warning::
+            ONLY use as a context manager if the transport is NOT shared
+            with other clients! Exiting the with block will CLOSE the transport
+            and may cause errors in other clients!
+        """
+        self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
-__all__ = ("DeliveryServiceAsyncClient",)
+__all__ = ("DeliveryServiceClient",)
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/client.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/async_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,46 +10,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-import os
+import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
-    cast,
 )
-import warnings
 
-from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
-from google.api_core import retry as retries
+from google.api_core import retry_async as retries
+from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
-from google.auth.exceptions import MutualTLSChannelError  # type: ignore
-from google.auth.transport import mtls  # type: ignore
-from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.maps.fleetengine_delivery_v1 import gapic_version as package_version
 
 try:
-    OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault, None]
+    OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault, None]
 except AttributeError:  # pragma: NO COVER
-    OptionalRetry = Union[retries.Retry, object, None]  # type: ignore
+    OptionalRetry = Union[retries.AsyncRetry, object, None]  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 from google.type import latlng_pb2  # type: ignore
 
@@ -58,283 +54,106 @@
     common,
     delivery_api,
     delivery_vehicles,
     task_tracking_info,
     tasks,
 )
 
+from .client import DeliveryServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, DeliveryServiceTransport
-from .transports.grpc import DeliveryServiceGrpcTransport
 from .transports.grpc_asyncio import DeliveryServiceGrpcAsyncIOTransport
-from .transports.rest import DeliveryServiceRestTransport
 
 
-class DeliveryServiceClientMeta(type):
-    """Metaclass for the DeliveryService client.
-
-    This provides class-level methods for building and retrieving
-    support objects (e.g. transport) without polluting the client instance
-    objects.
-    """
-
-    _transport_registry = (
-        OrderedDict()
-    )  # type: Dict[str, Type[DeliveryServiceTransport]]
-    _transport_registry["grpc"] = DeliveryServiceGrpcTransport
-    _transport_registry["grpc_asyncio"] = DeliveryServiceGrpcAsyncIOTransport
-    _transport_registry["rest"] = DeliveryServiceRestTransport
-
-    def get_transport_class(
-        cls,
-        label: Optional[str] = None,
-    ) -> Type[DeliveryServiceTransport]:
-        """Returns an appropriate transport class.
-
-        Args:
-            label: The name of the desired transport. If none is
-                provided, then the first transport in the registry is used.
-
-        Returns:
-            The transport class to use.
-        """
-        # If a specific transport is requested, return that one.
-        if label:
-            return cls._transport_registry[label]
-
-        # No transport is requested; return the default (that is, the first one
-        # in the dictionary).
-        return next(iter(cls._transport_registry.values()))
-
-
-class DeliveryServiceClient(metaclass=DeliveryServiceClientMeta):
+class DeliveryServiceAsyncClient:
     """The Last Mile Delivery service."""
 
-    @staticmethod
-    def _get_default_mtls_endpoint(api_endpoint):
-        """Converts api endpoint to mTLS endpoint.
-
-        Convert "*.sandbox.googleapis.com" and "*.googleapis.com" to
-        "*.mtls.sandbox.googleapis.com" and "*.mtls.googleapis.com" respectively.
-        Args:
-            api_endpoint (Optional[str]): the api endpoint to convert.
-        Returns:
-            str: converted mTLS api endpoint.
-        """
-        if not api_endpoint:
-            return api_endpoint
-
-        mtls_endpoint_re = re.compile(
-            r"(?P<name>[^.]+)(?P<mtls>\.mtls)?(?P<sandbox>\.sandbox)?(?P<googledomain>\.googleapis\.com)?"
-        )
-
-        m = mtls_endpoint_re.match(api_endpoint)
-        name, mtls, sandbox, googledomain = m.groups()
-        if mtls or not googledomain:
-            return api_endpoint
-
-        if sandbox:
-            return api_endpoint.replace(
-                "sandbox.googleapis.com", "mtls.sandbox.googleapis.com"
-            )
-
-        return api_endpoint.replace(".googleapis.com", ".mtls.googleapis.com")
+    _client: DeliveryServiceClient
 
+    # Copy defaults from the synchronous client for use here.
     # Note: DEFAULT_ENDPOINT is deprecated. Use _DEFAULT_ENDPOINT_TEMPLATE instead.
-    DEFAULT_ENDPOINT = "fleetengine.googleapis.com"
-    DEFAULT_MTLS_ENDPOINT = _get_default_mtls_endpoint.__func__(  # type: ignore
-        DEFAULT_ENDPOINT
+    DEFAULT_ENDPOINT = DeliveryServiceClient.DEFAULT_ENDPOINT
+    DEFAULT_MTLS_ENDPOINT = DeliveryServiceClient.DEFAULT_MTLS_ENDPOINT
+    _DEFAULT_ENDPOINT_TEMPLATE = DeliveryServiceClient._DEFAULT_ENDPOINT_TEMPLATE
+    _DEFAULT_UNIVERSE = DeliveryServiceClient._DEFAULT_UNIVERSE
+
+    delivery_vehicle_path = staticmethod(DeliveryServiceClient.delivery_vehicle_path)
+    parse_delivery_vehicle_path = staticmethod(
+        DeliveryServiceClient.parse_delivery_vehicle_path
+    )
+    task_path = staticmethod(DeliveryServiceClient.task_path)
+    parse_task_path = staticmethod(DeliveryServiceClient.parse_task_path)
+    task_tracking_info_path = staticmethod(
+        DeliveryServiceClient.task_tracking_info_path
+    )
+    parse_task_tracking_info_path = staticmethod(
+        DeliveryServiceClient.parse_task_tracking_info_path
+    )
+    common_billing_account_path = staticmethod(
+        DeliveryServiceClient.common_billing_account_path
+    )
+    parse_common_billing_account_path = staticmethod(
+        DeliveryServiceClient.parse_common_billing_account_path
+    )
+    common_folder_path = staticmethod(DeliveryServiceClient.common_folder_path)
+    parse_common_folder_path = staticmethod(
+        DeliveryServiceClient.parse_common_folder_path
+    )
+    common_organization_path = staticmethod(
+        DeliveryServiceClient.common_organization_path
+    )
+    parse_common_organization_path = staticmethod(
+        DeliveryServiceClient.parse_common_organization_path
+    )
+    common_project_path = staticmethod(DeliveryServiceClient.common_project_path)
+    parse_common_project_path = staticmethod(
+        DeliveryServiceClient.parse_common_project_path
+    )
+    common_location_path = staticmethod(DeliveryServiceClient.common_location_path)
+    parse_common_location_path = staticmethod(
+        DeliveryServiceClient.parse_common_location_path
     )
-
-    _DEFAULT_ENDPOINT_TEMPLATE = "fleetengine.{UNIVERSE_DOMAIN}"
-    _DEFAULT_UNIVERSE = "googleapis.com"
 
     @classmethod
     def from_service_account_info(cls, info: dict, *args, **kwargs):
         """Creates an instance of this client using the provided credentials
             info.
 
         Args:
             info (dict): The service account private key info.
             args: Additional arguments to pass to the constructor.
             kwargs: Additional arguments to pass to the constructor.
 
         Returns:
-            DeliveryServiceClient: The constructed client.
+            DeliveryServiceAsyncClient: The constructed client.
         """
-        credentials = service_account.Credentials.from_service_account_info(info)
-        kwargs["credentials"] = credentials
-        return cls(*args, **kwargs)
+        return DeliveryServiceClient.from_service_account_info.__func__(DeliveryServiceAsyncClient, info, *args, **kwargs)  # type: ignore
 
     @classmethod
     def from_service_account_file(cls, filename: str, *args, **kwargs):
         """Creates an instance of this client using the provided credentials
             file.
 
         Args:
             filename (str): The path to the service account private key json
                 file.
             args: Additional arguments to pass to the constructor.
             kwargs: Additional arguments to pass to the constructor.
 
         Returns:
-            DeliveryServiceClient: The constructed client.
+            DeliveryServiceAsyncClient: The constructed client.
         """
-        credentials = service_account.Credentials.from_service_account_file(filename)
-        kwargs["credentials"] = credentials
-        return cls(*args, **kwargs)
+        return DeliveryServiceClient.from_service_account_file.__func__(DeliveryServiceAsyncClient, filename, *args, **kwargs)  # type: ignore
 
     from_service_account_json = from_service_account_file
 
-    @property
-    def transport(self) -> DeliveryServiceTransport:
-        """Returns the transport used by the client instance.
-
-        Returns:
-            DeliveryServiceTransport: The transport used by the client
-                instance.
-        """
-        return self._transport
-
-    @staticmethod
-    def delivery_vehicle_path(
-        provider: str,
-        vehicle: str,
-    ) -> str:
-        """Returns a fully-qualified delivery_vehicle string."""
-        return "providers/{provider}/deliveryVehicles/{vehicle}".format(
-            provider=provider,
-            vehicle=vehicle,
-        )
-
-    @staticmethod
-    def parse_delivery_vehicle_path(path: str) -> Dict[str, str]:
-        """Parses a delivery_vehicle path into its component segments."""
-        m = re.match(
-            r"^providers/(?P<provider>.+?)/deliveryVehicles/(?P<vehicle>.+?)$", path
-        )
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def task_path(
-        provider: str,
-        task: str,
-    ) -> str:
-        """Returns a fully-qualified task string."""
-        return "providers/{provider}/tasks/{task}".format(
-            provider=provider,
-            task=task,
-        )
-
-    @staticmethod
-    def parse_task_path(path: str) -> Dict[str, str]:
-        """Parses a task path into its component segments."""
-        m = re.match(r"^providers/(?P<provider>.+?)/tasks/(?P<task>.+?)$", path)
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def task_tracking_info_path(
-        provider: str,
-        tracking: str,
-    ) -> str:
-        """Returns a fully-qualified task_tracking_info string."""
-        return "providers/{provider}/taskTrackingInfo/{tracking}".format(
-            provider=provider,
-            tracking=tracking,
-        )
-
-    @staticmethod
-    def parse_task_tracking_info_path(path: str) -> Dict[str, str]:
-        """Parses a task_tracking_info path into its component segments."""
-        m = re.match(
-            r"^providers/(?P<provider>.+?)/taskTrackingInfo/(?P<tracking>.+?)$", path
-        )
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def common_billing_account_path(
-        billing_account: str,
-    ) -> str:
-        """Returns a fully-qualified billing_account string."""
-        return "billingAccounts/{billing_account}".format(
-            billing_account=billing_account,
-        )
-
-    @staticmethod
-    def parse_common_billing_account_path(path: str) -> Dict[str, str]:
-        """Parse a billing_account path into its component segments."""
-        m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def common_folder_path(
-        folder: str,
-    ) -> str:
-        """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(
-            folder=folder,
-        )
-
-    @staticmethod
-    def parse_common_folder_path(path: str) -> Dict[str, str]:
-        """Parse a folder path into its component segments."""
-        m = re.match(r"^folders/(?P<folder>.+?)$", path)
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def common_organization_path(
-        organization: str,
-    ) -> str:
-        """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(
-            organization=organization,
-        )
-
-    @staticmethod
-    def parse_common_organization_path(path: str) -> Dict[str, str]:
-        """Parse a organization path into its component segments."""
-        m = re.match(r"^organizations/(?P<organization>.+?)$", path)
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def common_project_path(
-        project: str,
-    ) -> str:
-        """Returns a fully-qualified project string."""
-        return "projects/{project}".format(
-            project=project,
-        )
-
-    @staticmethod
-    def parse_common_project_path(path: str) -> Dict[str, str]:
-        """Parse a project path into its component segments."""
-        m = re.match(r"^projects/(?P<project>.+?)$", path)
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def common_location_path(
-        project: str,
-        location: str,
-    ) -> str:
-        """Returns a fully-qualified location string."""
-        return "projects/{project}/locations/{location}".format(
-            project=project,
-            location=location,
-        )
-
-    @staticmethod
-    def parse_common_location_path(path: str) -> Dict[str, str]:
-        """Parse a location path into its component segments."""
-        m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
-        return m.groupdict() if m else {}
-
     @classmethod
     def get_mtls_endpoint_and_cert_source(
-        cls, client_options: Optional[client_options_lib.ClientOptions] = None
+        cls, client_options: Optional[ClientOptions] = None
     ):
-        """Deprecated. Return the API endpoint and client cert source for mutual TLS.
+        """Return the API endpoint and client cert source for mutual TLS.
 
         The client cert source is determined in the following order:
         (1) if `GOOGLE_API_USE_CLIENT_CERTIFICATE` environment variable is not "true", the
         client cert source is None.
         (2) if `client_options.client_cert_source` is provided, use the provided one; if the
         default client cert source exists, use the default one; otherwise the client cert
         source is None.
@@ -356,243 +175,73 @@
         Returns:
             Tuple[str, Callable[[], Tuple[bytes, bytes]]]: returns the API endpoint and the
                 client cert source to use.
 
         Raises:
             google.auth.exceptions.MutualTLSChannelError: If any errors happen.
         """
+        return DeliveryServiceClient.get_mtls_endpoint_and_cert_source(client_options)  # type: ignore
 
-        warnings.warn(
-            "get_mtls_endpoint_and_cert_source is deprecated. Use the api_endpoint property instead.",
-            DeprecationWarning,
-        )
-        if client_options is None:
-            client_options = client_options_lib.ClientOptions()
-        use_client_cert = os.getenv("GOOGLE_API_USE_CLIENT_CERTIFICATE", "false")
-        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto")
-        if use_client_cert not in ("true", "false"):
-            raise ValueError(
-                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
-            )
-        if use_mtls_endpoint not in ("auto", "never", "always"):
-            raise MutualTLSChannelError(
-                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
-            )
-
-        # Figure out the client cert source to use.
-        client_cert_source = None
-        if use_client_cert == "true":
-            if client_options.client_cert_source:
-                client_cert_source = client_options.client_cert_source
-            elif mtls.has_default_client_cert_source():
-                client_cert_source = mtls.default_client_cert_source()
-
-        # Figure out which api endpoint to use.
-        if client_options.api_endpoint is not None:
-            api_endpoint = client_options.api_endpoint
-        elif use_mtls_endpoint == "always" or (
-            use_mtls_endpoint == "auto" and client_cert_source
-        ):
-            api_endpoint = cls.DEFAULT_MTLS_ENDPOINT
-        else:
-            api_endpoint = cls.DEFAULT_ENDPOINT
-
-        return api_endpoint, client_cert_source
-
-    @staticmethod
-    def _read_environment_variables():
-        """Returns the environment variables used by the client.
-
-        Returns:
-            Tuple[bool, str, str]: returns the GOOGLE_API_USE_CLIENT_CERTIFICATE,
-            GOOGLE_API_USE_MTLS_ENDPOINT, and GOOGLE_CLOUD_UNIVERSE_DOMAIN environment variables.
-
-        Raises:
-            ValueError: If GOOGLE_API_USE_CLIENT_CERTIFICATE is not
-                any of ["true", "false"].
-            google.auth.exceptions.MutualTLSChannelError: If GOOGLE_API_USE_MTLS_ENDPOINT
-                is not any of ["auto", "never", "always"].
-        """
-        use_client_cert = os.getenv(
-            "GOOGLE_API_USE_CLIENT_CERTIFICATE", "false"
-        ).lower()
-        use_mtls_endpoint = os.getenv("GOOGLE_API_USE_MTLS_ENDPOINT", "auto").lower()
-        universe_domain_env = os.getenv("GOOGLE_CLOUD_UNIVERSE_DOMAIN")
-        if use_client_cert not in ("true", "false"):
-            raise ValueError(
-                "Environment variable `GOOGLE_API_USE_CLIENT_CERTIFICATE` must be either `true` or `false`"
-            )
-        if use_mtls_endpoint not in ("auto", "never", "always"):
-            raise MutualTLSChannelError(
-                "Environment variable `GOOGLE_API_USE_MTLS_ENDPOINT` must be `never`, `auto` or `always`"
-            )
-        return use_client_cert == "true", use_mtls_endpoint, universe_domain_env
-
-    @staticmethod
-    def _get_client_cert_source(provided_cert_source, use_cert_flag):
-        """Return the client cert source to be used by the client.
-
-        Args:
-            provided_cert_source (bytes): The client certificate source provided.
-            use_cert_flag (bool): A flag indicating whether to use the client certificate.
-
-        Returns:
-            bytes or None: The client cert source to be used by the client.
-        """
-        client_cert_source = None
-        if use_cert_flag:
-            if provided_cert_source:
-                client_cert_source = provided_cert_source
-            elif mtls.has_default_client_cert_source():
-                client_cert_source = mtls.default_client_cert_source()
-        return client_cert_source
-
-    @staticmethod
-    def _get_api_endpoint(
-        api_override, client_cert_source, universe_domain, use_mtls_endpoint
-    ):
-        """Return the API endpoint used by the client.
-
-        Args:
-            api_override (str): The API endpoint override. If specified, this is always
-                the return value of this function and the other arguments are not used.
-            client_cert_source (bytes): The client certificate source used by the client.
-            universe_domain (str): The universe domain used by the client.
-            use_mtls_endpoint (str): How to use the mTLS endpoint, which depends also on the other parameters.
-                Possible values are "always", "auto", or "never".
-
-        Returns:
-            str: The API endpoint to be used by the client.
-        """
-        if api_override is not None:
-            api_endpoint = api_override
-        elif use_mtls_endpoint == "always" or (
-            use_mtls_endpoint == "auto" and client_cert_source
-        ):
-            _default_universe = DeliveryServiceClient._DEFAULT_UNIVERSE
-            if universe_domain != _default_universe:
-                raise MutualTLSChannelError(
-                    f"mTLS is not supported in any universe other than {_default_universe}."
-                )
-            api_endpoint = DeliveryServiceClient.DEFAULT_MTLS_ENDPOINT
-        else:
-            api_endpoint = DeliveryServiceClient._DEFAULT_ENDPOINT_TEMPLATE.format(
-                UNIVERSE_DOMAIN=universe_domain
-            )
-        return api_endpoint
-
-    @staticmethod
-    def _get_universe_domain(
-        client_universe_domain: Optional[str], universe_domain_env: Optional[str]
-    ) -> str:
-        """Return the universe domain used by the client.
-
-        Args:
-            client_universe_domain (Optional[str]): The universe domain configured via the client options.
-            universe_domain_env (Optional[str]): The universe domain configured via the "GOOGLE_CLOUD_UNIVERSE_DOMAIN" environment variable.
-
-        Returns:
-            str: The universe domain to be used by the client.
-
-        Raises:
-            ValueError: If the universe domain is an empty string.
-        """
-        universe_domain = DeliveryServiceClient._DEFAULT_UNIVERSE
-        if client_universe_domain is not None:
-            universe_domain = client_universe_domain
-        elif universe_domain_env is not None:
-            universe_domain = universe_domain_env
-        if len(universe_domain.strip()) == 0:
-            raise ValueError("Universe Domain cannot be an empty string.")
-        return universe_domain
-
-    @staticmethod
-    def _compare_universes(
-        client_universe: str, credentials: ga_credentials.Credentials
-    ) -> bool:
-        """Returns True iff the universe domains used by the client and credentials match.
-
-        Args:
-            client_universe (str): The universe domain configured via the client options.
-            credentials (ga_credentials.Credentials): The credentials being used in the client.
-
-        Returns:
-            bool: True iff client_universe matches the universe in credentials.
-
-        Raises:
-            ValueError: when client_universe does not match the universe in credentials.
-        """
-
-        default_universe = DeliveryServiceClient._DEFAULT_UNIVERSE
-        credentials_universe = getattr(credentials, "universe_domain", default_universe)
-
-        if client_universe != credentials_universe:
-            raise ValueError(
-                "The configured universe domain "
-                f"({client_universe}) does not match the universe domain "
-                f"found in the credentials ({credentials_universe}). "
-                "If you haven't configured the universe domain explicitly, "
-                f"`{default_universe}` is the default."
-            )
-        return True
-
-    def _validate_universe_domain(self):
-        """Validates client's and credentials' universe domains are consistent.
+    @property
+    def transport(self) -> DeliveryServiceTransport:
+        """Returns the transport used by the client instance.
 
         Returns:
-            bool: True iff the configured universe domain is valid.
-
-        Raises:
-            ValueError: If the configured universe domain is not valid.
+            DeliveryServiceTransport: The transport used by the client instance.
         """
-        self._is_universe_domain_valid = (
-            self._is_universe_domain_valid
-            or DeliveryServiceClient._compare_universes(
-                self.universe_domain, self.transport._credentials
-            )
-        )
-        return self._is_universe_domain_valid
+        return self._client.transport
 
     @property
     def api_endpoint(self):
         """Return the API endpoint used by the client instance.
 
         Returns:
             str: The API endpoint used by the client instance.
         """
-        return self._api_endpoint
+        return self._client._api_endpoint
 
     @property
     def universe_domain(self) -> str:
         """Return the universe domain used by the client instance.
 
         Returns:
-            str: The universe domain used by the client instance.
+            str: The universe domain used
+                by the client instance.
         """
-        return self._universe_domain
+        return self._client._universe_domain
+
+    get_transport_class = functools.partial(
+        type(DeliveryServiceClient).get_transport_class, type(DeliveryServiceClient)
+    )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, DeliveryServiceTransport]] = None,
-        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
+        transport: Optional[
+            Union[
+                str, DeliveryServiceTransport, Callable[..., DeliveryServiceTransport]
+            ]
+        ] = "grpc_asyncio",
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
-        """Instantiates the delivery service client.
+        """Instantiates the delivery service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, DeliveryServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,DeliveryServiceTransport,Callable[..., DeliveryServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the DeliveryServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -607,114 +256,36 @@
                 is "true", then the ``client_cert_source`` property can be used
                 to provide a client certificate for mTLS transport. If
                 not provided, the default SSL client certificate will be used if
                 present. If GOOGLE_API_USE_CLIENT_CERTIFICATE is "false" or not
                 set, no client certificate will be used.
 
                 3. The ``universe_domain`` property can be used to override the
-                default "googleapis.com" universe. Note that the ``api_endpoint``
+                default "googleapis.com" universe. Note that ``api_endpoint``
                 property still takes precedence; and ``universe_domain`` is
                 currently not supported for mTLS.
 
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
 
         Raises:
-            google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
-        self._client_options = client_options
-        if isinstance(self._client_options, dict):
-            self._client_options = client_options_lib.from_dict(self._client_options)
-        if self._client_options is None:
-            self._client_options = client_options_lib.ClientOptions()
-        self._client_options = cast(
-            client_options_lib.ClientOptions, self._client_options
-        )
-
-        universe_domain_opt = getattr(self._client_options, "universe_domain", None)
-
-        (
-            self._use_client_cert,
-            self._use_mtls_endpoint,
-            self._universe_domain_env,
-        ) = DeliveryServiceClient._read_environment_variables()
-        self._client_cert_source = DeliveryServiceClient._get_client_cert_source(
-            self._client_options.client_cert_source, self._use_client_cert
-        )
-        self._universe_domain = DeliveryServiceClient._get_universe_domain(
-            universe_domain_opt, self._universe_domain_env
+        self._client = DeliveryServiceClient(
+            credentials=credentials,
+            transport=transport,
+            client_options=client_options,
+            client_info=client_info,
         )
-        self._api_endpoint = None  # updated below, depending on `transport`
-
-        # Initialize the universe domain validation.
-        self._is_universe_domain_valid = False
-
-        api_key_value = getattr(self._client_options, "api_key", None)
-        if api_key_value and credentials:
-            raise ValueError(
-                "client_options.api_key and credentials are mutually exclusive"
-            )
-
-        # Save or instantiate the transport.
-        # Ordinarily, we provide the transport, but allowing a custom transport
-        # instance provides an extensibility point for unusual situations.
-        transport_provided = isinstance(transport, DeliveryServiceTransport)
-        if transport_provided:
-            # transport is a DeliveryServiceTransport instance.
-            if credentials or self._client_options.credentials_file or api_key_value:
-                raise ValueError(
-                    "When providing a transport instance, "
-                    "provide its credentials directly."
-                )
-            if self._client_options.scopes:
-                raise ValueError(
-                    "When providing a transport instance, provide its scopes "
-                    "directly."
-                )
-            self._transport = cast(DeliveryServiceTransport, transport)
-            self._api_endpoint = self._transport.host
-
-        self._api_endpoint = (
-            self._api_endpoint
-            or DeliveryServiceClient._get_api_endpoint(
-                self._client_options.api_endpoint,
-                self._client_cert_source,
-                self._universe_domain,
-                self._use_mtls_endpoint,
-            )
-        )
-
-        if not transport_provided:
-            import google.auth._default  # type: ignore
-
-            if api_key_value and hasattr(
-                google.auth._default, "get_api_key_credentials"
-            ):
-                credentials = google.auth._default.get_api_key_credentials(
-                    api_key_value
-                )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
-                credentials=credentials,
-                credentials_file=self._client_options.credentials_file,
-                host=self._api_endpoint,
-                scopes=self._client_options.scopes,
-                client_cert_source_for_mtls=self._client_cert_source,
-                quota_project_id=self._client_options.quota_project_id,
-                client_info=client_info,
-                always_use_jwt_access=True,
-                api_audience=self._client_options.api_audience,
-            )
-
-    def create_delivery_vehicle(
+    async def create_delivery_vehicle(
         self,
         request: Optional[
             Union[delivery_api.CreateDeliveryVehicleRequest, dict]
         ] = None,
         *,
         parent: Optional[str] = None,
         delivery_vehicle: Optional[delivery_vehicles.DeliveryVehicle] = None,
@@ -732,72 +303,72 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_create_delivery_vehicle():
+            async def sample_create_delivery_vehicle():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.CreateDeliveryVehicleRequest(
                     parent="parent_value",
                     delivery_vehicle_id="delivery_vehicle_id_value",
                 )
 
                 # Make the request
-                response = client.create_delivery_vehicle(request=request)
+                response = await client.create_delivery_vehicle(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.CreateDeliveryVehicleRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.CreateDeliveryVehicleRequest, dict]]):
                 The request object. The ``CreateDeliveryVehicle`` request message.
-            parent (str):
+            parent (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}``. The provider must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            delivery_vehicle (google.maps.fleetengine_delivery_v1.types.DeliveryVehicle):
+            delivery_vehicle (:class:`google.maps.fleetengine_delivery_v1.types.DeliveryVehicle`):
                 Required. The ``DeliveryVehicle`` entity to create. When
                 creating a new delivery vehicle, you may set the
                 following optional fields:
 
                 -  last_location
                 -  attributes
 
                 Note: The DeliveryVehicle's ``name`` field is ignored.
                 All other DeliveryVehicle fields must not be set;
                 otherwise, an error is returned.
 
                 This corresponds to the ``delivery_vehicle`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            delivery_vehicle_id (str):
+            delivery_vehicle_id (:class:`str`):
                 Required. The Delivery Vehicle ID must be unique and
                 subject to the following restrictions:
 
                 -  Must be a valid Unicode string.
                 -  Limited to a maximum length of 64 characters.
                 -  Normalized according to [Unicode Normalization Form
                    C] (http://www.unicode.org/reports/tr15/).
                 -  May not contain any of the following ASCII
                    characters: '/', ':', '?', ',', or '#'.
 
                 This corresponds to the ``delivery_vehicle_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.DeliveryVehicle:
@@ -811,69 +382,64 @@
                    conventions. For example, the
                    DeliveryVehicle.current_route_segment field in the
                    gRPC API and the DeliveryVehicle.currentRouteSegment
                    field in the REST API refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, delivery_vehicle, delivery_vehicle_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.CreateDeliveryVehicleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.CreateDeliveryVehicleRequest):
             request = delivery_api.CreateDeliveryVehicleRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
-            if delivery_vehicle is not None:
-                request.delivery_vehicle = delivery_vehicle
-            if delivery_vehicle_id is not None:
-                request.delivery_vehicle_id = delivery_vehicle_id
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+        if delivery_vehicle is not None:
+            request.delivery_vehicle = delivery_vehicle
+        if delivery_vehicle_id is not None:
+            request.delivery_vehicle_id = delivery_vehicle_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.create_delivery_vehicle]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_delivery_vehicle
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def get_delivery_vehicle(
+    async def get_delivery_vehicle(
         self,
         request: Optional[Union[delivery_api.GetDeliveryVehicleRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -887,42 +453,42 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_get_delivery_vehicle():
+            async def sample_get_delivery_vehicle():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.GetDeliveryVehicleRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_delivery_vehicle(request=request)
+                response = await client.get_delivery_vehicle(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.GetDeliveryVehicleRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.GetDeliveryVehicleRequest, dict]]):
                 The request object. The ``GetDeliveryVehicle`` request message.
-            name (str):
+            name (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}/deliveryVehicles/{delivery_vehicle}``.
                 The ``provider`` must be the Google Cloud Project ID.
                 For example, ``sample-cloud-project``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.DeliveryVehicle:
@@ -936,65 +502,60 @@
                    conventions. For example, the
                    DeliveryVehicle.current_route_segment field in the
                    gRPC API and the DeliveryVehicle.currentRouteSegment
                    field in the REST API refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.GetDeliveryVehicleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.GetDeliveryVehicleRequest):
             request = delivery_api.GetDeliveryVehicleRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if name is not None:
-                request.name = name
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.get_delivery_vehicle]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.name)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_delivery_vehicle
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def update_delivery_vehicle(
+    async def update_delivery_vehicle(
         self,
         request: Optional[
             Union[delivery_api.UpdateDeliveryVehicleRequest, dict]
         ] = None,
         *,
         delivery_vehicle: Optional[delivery_vehicles.DeliveryVehicle] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
@@ -1019,52 +580,52 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_update_delivery_vehicle():
+            async def sample_update_delivery_vehicle():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.UpdateDeliveryVehicleRequest(
                 )
 
                 # Make the request
-                response = client.update_delivery_vehicle(request=request)
+                response = await client.update_delivery_vehicle(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.UpdateDeliveryVehicleRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.UpdateDeliveryVehicleRequest, dict]]):
                 The request object. The ``UpdateDeliveryVehicle`` request message.
-            delivery_vehicle (google.maps.fleetengine_delivery_v1.types.DeliveryVehicle):
+            delivery_vehicle (:class:`google.maps.fleetengine_delivery_v1.types.DeliveryVehicle`):
                 Required. The ``DeliveryVehicle`` entity update to
                 apply. Note: You cannot update the name of the
                 ``DeliveryVehicle``.
 
                 This corresponds to the ``delivery_vehicle`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. A field mask that indicates which
                 ``DeliveryVehicle`` fields to update. Note that the
                 update_mask must contain at least one field.
 
                 This is a comma-separated list of fully qualified names
                 of fields. Example:
                 ``"remaining_vehicle_journey_segments"``.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.DeliveryVehicle:
@@ -1078,67 +639,64 @@
                    conventions. For example, the
                    DeliveryVehicle.current_route_segment field in the
                    gRPC API and the DeliveryVehicle.currentRouteSegment
                    field in the REST API refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([delivery_vehicle, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.UpdateDeliveryVehicleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.UpdateDeliveryVehicleRequest):
             request = delivery_api.UpdateDeliveryVehicleRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if delivery_vehicle is not None:
-                request.delivery_vehicle = delivery_vehicle
-            if update_mask is not None:
-                request.update_mask = update_mask
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if delivery_vehicle is not None:
+            request.delivery_vehicle = delivery_vehicle
+        if update_mask is not None:
+            request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.update_delivery_vehicle]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.delivery_vehicle.name)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_delivery_vehicle
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("delivery_vehicle.name", request.delivery_vehicle.name),)
+            ),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def batch_create_tasks(
+    async def batch_create_tasks(
         self,
         request: Optional[Union[delivery_api.BatchCreateTasksRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> delivery_api.BatchCreateTasksResponse:
@@ -1151,88 +709,82 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_batch_create_tasks():
+            async def sample_batch_create_tasks():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 requests = fleetengine_delivery_v1.CreateTaskRequest()
                 requests.parent = "parent_value"
                 requests.task_id = "task_id_value"
                 requests.task.type_ = "UNAVAILABLE"
                 requests.task.state = "CLOSED"
 
                 request = fleetengine_delivery_v1.BatchCreateTasksRequest(
                     parent="parent_value",
                     requests=requests,
                 )
 
                 # Make the request
-                response = client.batch_create_tasks(request=request)
+                response = await client.batch_create_tasks(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.BatchCreateTasksRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.BatchCreateTasksRequest, dict]]):
                 The request object. The ``BatchCreateTask`` request message.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.BatchCreateTasksResponse:
                 The BatchCreateTask response message.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.BatchCreateTasksRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.BatchCreateTasksRequest):
             request = delivery_api.BatchCreateTasksRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.batch_create_tasks]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.batch_create_tasks
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def create_task(
+    async def create_task(
         self,
         request: Optional[Union[delivery_api.CreateTaskRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         task: Optional[tasks.Task] = None,
         task_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
@@ -1248,48 +800,48 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_create_task():
+            async def sample_create_task():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 task = fleetengine_delivery_v1.Task()
                 task.type_ = "UNAVAILABLE"
                 task.state = "CLOSED"
 
                 request = fleetengine_delivery_v1.CreateTaskRequest(
                     parent="parent_value",
                     task_id="task_id_value",
                     task=task,
                 )
 
                 # Make the request
-                response = client.create_task(request=request)
+                response = await client.create_task(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.CreateTaskRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.CreateTaskRequest, dict]]):
                 The request object. The ``CreateTask`` request message.
-            parent (str):
+            parent (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}``. The ``provider`` must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            task (google.maps.fleetengine_delivery_v1.types.Task):
+            task (:class:`google.maps.fleetengine_delivery_v1.types.Task`):
                 Required. The Task entity to create. When creating a
                 Task, the following fields are required:
 
                 -  ``type``
                 -  ``state`` (must be set to ``OPEN``)
                 -  ``tracking_id`` (must not be set for ``UNAVAILABLE``
                    or ``SCHEDULED_STOP`` tasks, but required for all
@@ -1301,15 +853,15 @@
                 Note: The Task's ``name`` field is ignored. All other
                 Task fields must not be set; otherwise, an error is
                 returned.
 
                 This corresponds to the ``task`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            task_id (str):
+            task_id (:class:`str`):
                 Required. The Task ID must be unique, but it should be
                 not a shipment tracking ID. To store a shipment tracking
                 ID, use the ``tracking_id`` field. Note that multiple
                 tasks can have the same ``tracking_id``. Task IDs are
                 subject to the following restrictions:
 
                 -  Must be a valid Unicode string.
@@ -1318,15 +870,15 @@
                    C] (http://www.unicode.org/reports/tr15/).
                 -  May not contain any of the following ASCII
                    characters: '/', ':', '?', ',', or '#'.
 
                 This corresponds to the ``task_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.Task:
@@ -1345,69 +897,64 @@
                    conventions. For example, the
                    Task.journey_sharing_info field in the gRPC API and
                    the Task.journeySharingInfo field in the REST API
                    refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, task, task_id])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.CreateTaskRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.CreateTaskRequest):
             request = delivery_api.CreateTaskRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
-            if task is not None:
-                request.task = task
-            if task_id is not None:
-                request.task_id = task_id
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+        if task is not None:
+            request.task = task
+        if task_id is not None:
+            request.task_id = task_id
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.create_task]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_task
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def get_task(
+    async def get_task(
         self,
         request: Optional[Union[delivery_api.GetTaskRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1421,42 +968,42 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_get_task():
+            async def sample_get_task():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.GetTaskRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_task(request=request)
+                response = await client.get_task(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.GetTaskRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.GetTaskRequest, dict]]):
                 The request object. The ``GetTask`` request message.
-            name (str):
+            name (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}/tasks/{task}``. The ``provider``
                 must be the Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.Task:
@@ -1475,196 +1022,58 @@
                    conventions. For example, the
                    Task.journey_sharing_info field in the gRPC API and
                    the Task.journeySharingInfo field in the REST API
                    refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.GetTaskRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.GetTaskRequest):
             request = delivery_api.GetTaskRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if name is not None:
-                request.name = name
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.get_task]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.name)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
-
-        # Validate the universe domain.
-        self._validate_universe_domain()
-
-        # Send the request.
-        response = rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    def search_tasks(
-        self,
-        request: Optional[Union[delivery_api.SearchTasksRequest, dict]] = None,
-        *,
-        parent: Optional[str] = None,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.SearchTasksPager:
-        r"""Deprecated: Use ``GetTaskTrackingInfo`` instead.
-
-        .. code-block:: python
-
-            # This snippet has been automatically generated and should be regarded as a
-            # code template only.
-            # It will require modifications to work:
-            # - It may require correct/in-range values for request initialization.
-            # - It may require specifying regional endpoints when creating the service
-            #   client as shown in:
-            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.maps import fleetengine_delivery_v1
-
-            def sample_search_tasks():
-                # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
-
-                # Initialize request argument(s)
-                request = fleetengine_delivery_v1.SearchTasksRequest(
-                    parent="parent_value",
-                    tracking_id="tracking_id_value",
-                )
-
-                # Make the request
-                page_result = client.search_tasks(request=request)
-
-                # Handle the response
-                for response in page_result:
-                    print(response)
-
-        Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.SearchTasksRequest, dict]):
-                The request object. Deprecated: Issue ``GetTaskTrackingInfoRequest``\ s to
-                ``GetTaskTrackingInfo`` instead.
-            parent (str):
-                Required. Must be in the format
-                ``providers/{provider}``. The provider must be the
-                Google Cloud Project ID. For example,
-                ``sample-cloud-project``.
-
-                This corresponds to the ``parent`` field
-                on the ``request`` instance; if ``request`` is provided, this
-                should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.SearchTasksPager:
-                The SearchTasks response. It contains the set of Tasks that meet the search
-                   criteria in the SearchTasksRequest.
-
-                Iterating over this object will yield results and
-                resolve additional pages automatically.
 
-        """
-        warnings.warn(
-            "DeliveryServiceClient.search_tasks is deprecated", DeprecationWarning
-        )
-
-        # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
-        has_flattened_params = any([parent])
-        if request is not None and has_flattened_params:
-            raise ValueError(
-                "If the `request` argument is set, then none of "
-                "the individual field arguments should be set."
-            )
-
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.SearchTasksRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, delivery_api.SearchTasksRequest):
-            request = delivery_api.SearchTasksRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.search_tasks]
-
-        header_params = {}
+        rpc = self._client._transport._wrapped_methods[self._client._transport.get_task]
 
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-        # This method is paged; wrap the response in a pager, which provides
-        # an `__iter__` convenience method.
-        response = pagers.SearchTasksPager(
-            method=rpc,
-            request=request,
-            response=response,
-            metadata=metadata,
-        )
-
         # Done; return the response.
         return response
 
-    def update_task(
+    async def update_task(
         self,
         request: Optional[Union[delivery_api.UpdateTaskRequest, dict]] = None,
         *,
         task: Optional[tasks.Task] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
@@ -1679,37 +1088,37 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_update_task():
+            async def sample_update_task():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 task = fleetengine_delivery_v1.Task()
                 task.type_ = "UNAVAILABLE"
                 task.state = "CLOSED"
 
                 request = fleetengine_delivery_v1.UpdateTaskRequest(
                     task=task,
                 )
 
                 # Make the request
-                response = client.update_task(request=request)
+                response = await client.update_task(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.UpdateTaskRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.UpdateTaskRequest, dict]]):
                 The request object. The ``UpdateTask`` request message.
-            task (google.maps.fleetengine_delivery_v1.types.Task):
+            task (:class:`google.maps.fleetengine_delivery_v1.types.Task`):
                 Required. The Task associated with the update. The
                 following fields are maintained by Fleet Engine. Do not
                 update them using ``Task.update``.
 
                 -  ``last_location``.
                 -  ``last_location_snappable``.
                 -  ``name``.
@@ -1724,27 +1133,27 @@
                 ``Task.update``. Instead, remove the ``VehicleStop``
                 that contains the Task from the delivery vehicle, which
                 automatically sets the Task state to CLOSED.
 
                 This corresponds to the ``task`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. The field mask that indicates which Task
                 fields to update. Note: The ``update_mask`` must contain
                 at least one field.
 
                 This is a comma-separated list of fully qualified names
                 of fields. Example:
                 ``"task_outcome,task_outcome_time,task_outcome_location"``.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.Task:
@@ -1763,192 +1172,184 @@
                    conventions. For example, the
                    Task.journey_sharing_info field in the gRPC API and
                    the Task.journeySharingInfo field in the REST API
                    refer to the same field.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([task, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.UpdateTaskRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.UpdateTaskRequest):
             request = delivery_api.UpdateTaskRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if task is not None:
-                request.task = task
-            if update_mask is not None:
-                request.update_mask = update_mask
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if task is not None:
+            request.task = task
+        if update_mask is not None:
+            request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.update_task]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.task.name)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_task
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("task.name", request.task.name),)
+            ),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def list_tasks(
+    async def list_tasks(
         self,
         request: Optional[Union[delivery_api.ListTasksRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.ListTasksPager:
+    ) -> pagers.ListTasksAsyncPager:
         r"""Gets all ``Task``\ s that meet the specified filtering criteria.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_list_tasks():
+            async def sample_list_tasks():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.ListTasksRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_tasks(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.ListTasksRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.ListTasksRequest, dict]]):
                 The request object. The ``ListTasks`` request message.
-            parent (str):
+            parent (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}``. The ``provider`` must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListTasksPager:
+            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListTasksAsyncPager:
                 The ListTasks response that contains the set of Tasks that meet the filter
                    criteria in the ListTasksRequest.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.ListTasksRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.ListTasksRequest):
             request = delivery_api.ListTasksRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.list_tasks]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_tasks
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # This method is paged; wrap the response in a pager, which provides
-        # an `__iter__` convenience method.
-        response = pagers.ListTasksPager(
+        # an `__aiter__` convenience method.
+        response = pagers.ListTasksAsyncPager(
             method=rpc,
             request=request,
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def get_task_tracking_info(
+    async def get_task_tracking_info(
         self,
         request: Optional[Union[delivery_api.GetTaskTrackingInfoRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1962,44 +1363,44 @@
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_get_task_tracking_info():
+            async def sample_get_task_tracking_info():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.GetTaskTrackingInfoRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_task_tracking_info(request=request)
+                response = await client.get_task_tracking_info(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.GetTaskTrackingInfoRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.GetTaskTrackingInfoRequest, dict]]):
                 The request object. The ``GetTaskTrackingInfoRequest`` request message.
-            name (str):
+            name (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}/taskTrackingInfo/{tracking_id}``.
                 The ``provider`` must be the Google Cloud Project ID,
                 and the ``tracking_id`` must be the tracking ID
                 associated with the task. An example name can be
                 ``providers/sample-cloud-project/taskTrackingInfo/sample-tracking-id``.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_delivery_v1.types.TaskTrackingInfo:
@@ -2007,202 +1408,185 @@
                    information which will be used for display. If a
                    tracking ID is associated with multiple Tasks, Fleet
                    Engine uses a heuristic to decide which Task's
                    TaskTrackingInfo to select.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.GetTaskTrackingInfoRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.GetTaskTrackingInfoRequest):
             request = delivery_api.GetTaskTrackingInfoRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if name is not None:
-                request.name = name
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.get_task_tracking_info]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.name)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_task_tracking_info
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def list_delivery_vehicles(
+    async def list_delivery_vehicles(
         self,
         request: Optional[Union[delivery_api.ListDeliveryVehiclesRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
-    ) -> pagers.ListDeliveryVehiclesPager:
+    ) -> pagers.ListDeliveryVehiclesAsyncPager:
         r"""Gets all ``DeliveryVehicle``\ s that meet the specified
         filtering criteria.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
             from google.maps import fleetengine_delivery_v1
 
-            def sample_list_delivery_vehicles():
+            async def sample_list_delivery_vehicles():
                 # Create a client
-                client = fleetengine_delivery_v1.DeliveryServiceClient()
+                client = fleetengine_delivery_v1.DeliveryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = fleetengine_delivery_v1.ListDeliveryVehiclesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_delivery_vehicles(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.maps.fleetengine_delivery_v1.types.ListDeliveryVehiclesRequest, dict]):
+            request (Optional[Union[google.maps.fleetengine_delivery_v1.types.ListDeliveryVehiclesRequest, dict]]):
                 The request object. The ``ListDeliveryVehicles`` request message.
-            parent (str):
+            parent (:class:`str`):
                 Required. Must be in the format
                 ``providers/{provider}``. The ``provider`` must be the
                 Google Cloud Project ID. For example,
                 ``sample-cloud-project``.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListDeliveryVehiclesPager:
+            google.maps.fleetengine_delivery_v1.services.delivery_service.pagers.ListDeliveryVehiclesAsyncPager:
                 The ListDeliveryVehicles response message.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a delivery_api.ListDeliveryVehiclesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, delivery_api.ListDeliveryVehiclesRequest):
             request = delivery_api.ListDeliveryVehiclesRequest(request)
-            # If we have keyword arguments corresponding to fields on the
-            # request, apply these.
-            if parent is not None:
-                request.parent = parent
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.list_delivery_vehicles]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
-
-        if header_params:
-            metadata = tuple(metadata) + (
-                gapic_v1.routing_header.to_grpc_metadata(header_params),
-            )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_delivery_vehicles
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
 
         # Validate the universe domain.
-        self._validate_universe_domain()
+        self._client._validate_universe_domain()
 
         # Send the request.
-        response = rpc(
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # This method is paged; wrap the response in a pager, which provides
-        # an `__iter__` convenience method.
-        response = pagers.ListDeliveryVehiclesPager(
+        # an `__aiter__` convenience method.
+        response = pagers.ListDeliveryVehiclesAsyncPager(
             method=rpc,
             request=request,
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self) -> "DeliveryServiceClient":
+    async def __aenter__(self) -> "DeliveryServiceAsyncClient":
         return self
 
-    def __exit__(self, type, value, traceback):
-        """Releases underlying transport's resources.
-
-        .. warning::
-            ONLY use as a context manager if the transport is NOT shared
-            with other clients! Exiting the with block will CLOSE the transport
-            and may cause errors in other clients!
-        """
-        self.transport.close()
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
-__all__ = ("DeliveryServiceClient",)
+__all__ = ("DeliveryServiceAsyncClient",)
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/pagers.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,142 +27,14 @@
 from google.maps.fleetengine_delivery_v1.types import (
     delivery_api,
     delivery_vehicles,
     tasks,
 )
 
 
-class SearchTasksPager:
-    """A pager for iterating through ``search_tasks`` requests.
-
-    This class thinly wraps an initial
-    :class:`google.maps.fleetengine_delivery_v1.types.SearchTasksResponse` object, and
-    provides an ``__iter__`` method to iterate through its
-    ``tasks`` field.
-
-    If there are more pages, the ``__iter__`` method will make additional
-    ``SearchTasks`` requests and continue to iterate
-    through the ``tasks`` field on the
-    corresponding responses.
-
-    All the usual :class:`google.maps.fleetengine_delivery_v1.types.SearchTasksResponse`
-    attributes are available on the pager. If multiple requests are made, only
-    the most recent response is retained, and thus used for attribute lookup.
-    """
-
-    def __init__(
-        self,
-        method: Callable[..., delivery_api.SearchTasksResponse],
-        request: delivery_api.SearchTasksRequest,
-        response: delivery_api.SearchTasksResponse,
-        *,
-        metadata: Sequence[Tuple[str, str]] = ()
-    ):
-        """Instantiate the pager.
-
-        Args:
-            method (Callable): The method that was originally called, and
-                which instantiated this pager.
-            request (google.maps.fleetengine_delivery_v1.types.SearchTasksRequest):
-                The initial request object.
-            response (google.maps.fleetengine_delivery_v1.types.SearchTasksResponse):
-                The initial response object.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        """
-        self._method = method
-        self._request = delivery_api.SearchTasksRequest(request)
-        self._response = response
-        self._metadata = metadata
-
-    def __getattr__(self, name: str) -> Any:
-        return getattr(self._response, name)
-
-    @property
-    def pages(self) -> Iterator[delivery_api.SearchTasksResponse]:
-        yield self._response
-        while self._response.next_page_token:
-            self._request.page_token = self._response.next_page_token
-            self._response = self._method(self._request, metadata=self._metadata)
-            yield self._response
-
-    def __iter__(self) -> Iterator[tasks.Task]:
-        for page in self.pages:
-            yield from page.tasks
-
-    def __repr__(self) -> str:
-        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
-
-
-class SearchTasksAsyncPager:
-    """A pager for iterating through ``search_tasks`` requests.
-
-    This class thinly wraps an initial
-    :class:`google.maps.fleetengine_delivery_v1.types.SearchTasksResponse` object, and
-    provides an ``__aiter__`` method to iterate through its
-    ``tasks`` field.
-
-    If there are more pages, the ``__aiter__`` method will make additional
-    ``SearchTasks`` requests and continue to iterate
-    through the ``tasks`` field on the
-    corresponding responses.
-
-    All the usual :class:`google.maps.fleetengine_delivery_v1.types.SearchTasksResponse`
-    attributes are available on the pager. If multiple requests are made, only
-    the most recent response is retained, and thus used for attribute lookup.
-    """
-
-    def __init__(
-        self,
-        method: Callable[..., Awaitable[delivery_api.SearchTasksResponse]],
-        request: delivery_api.SearchTasksRequest,
-        response: delivery_api.SearchTasksResponse,
-        *,
-        metadata: Sequence[Tuple[str, str]] = ()
-    ):
-        """Instantiates the pager.
-
-        Args:
-            method (Callable): The method that was originally called, and
-                which instantiated this pager.
-            request (google.maps.fleetengine_delivery_v1.types.SearchTasksRequest):
-                The initial request object.
-            response (google.maps.fleetengine_delivery_v1.types.SearchTasksResponse):
-                The initial response object.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        """
-        self._method = method
-        self._request = delivery_api.SearchTasksRequest(request)
-        self._response = response
-        self._metadata = metadata
-
-    def __getattr__(self, name: str) -> Any:
-        return getattr(self._response, name)
-
-    @property
-    async def pages(self) -> AsyncIterator[delivery_api.SearchTasksResponse]:
-        yield self._response
-        while self._response.next_page_token:
-            self._request.page_token = self._response.next_page_token
-            self._response = await self._method(self._request, metadata=self._metadata)
-            yield self._response
-
-    def __aiter__(self) -> AsyncIterator[tasks.Task]:
-        async def async_generator():
-            async for page in self.pages:
-                for response in page.tasks:
-                    yield response
-
-        return async_generator()
-
-    def __repr__(self) -> str:
-        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
-
-
 class ListTasksPager:
     """A pager for iterating through ``list_tasks`` requests.
 
     This class thinly wraps an initial
     :class:`google.maps.fleetengine_delivery_v1.types.ListTasksResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``tasks`` field.
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -211,28 +211,14 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=60.0,
                 ),
                 default_timeout=60.0,
                 client_info=client_info,
             ),
-            self.search_tasks: gapic_v1.method.wrap_method(
-                self.search_tasks,
-                default_retry=retries.Retry(
-                    initial=1.0,
-                    maximum=10.0,
-                    multiplier=1.3,
-                    predicate=retries.if_exception_type(
-                        core_exceptions.ServiceUnavailable,
-                    ),
-                    deadline=60.0,
-                ),
-                default_timeout=60.0,
-                client_info=client_info,
-            ),
             self.update_task: gapic_v1.method.wrap_method(
                 self.update_task,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
@@ -357,26 +343,14 @@
         self,
     ) -> Callable[
         [delivery_api.GetTaskRequest], Union[tasks.Task, Awaitable[tasks.Task]]
     ]:
         raise NotImplementedError()
 
     @property
-    def search_tasks(
-        self,
-    ) -> Callable[
-        [delivery_api.SearchTasksRequest],
-        Union[
-            delivery_api.SearchTasksResponse,
-            Awaitable[delivery_api.SearchTasksResponse],
-        ],
-    ]:
-        raise NotImplementedError()
-
-    @property
     def update_task(
         self,
     ) -> Callable[
         [delivery_api.UpdateTaskRequest], Union[tasks.Task, Awaitable[tasks.Task]]
     ]:
         raise NotImplementedError()
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def __init__(
         self,
         *,
         host: str = "fleetengine.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -70,36 +70,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'fleetengine.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -117,15 +120,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -158,15 +161,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -398,40 +403,14 @@
                 "/maps.fleetengine.delivery.v1.DeliveryService/GetTask",
                 request_serializer=delivery_api.GetTaskRequest.serialize,
                 response_deserializer=tasks.Task.deserialize,
             )
         return self._stubs["get_task"]
 
     @property
-    def search_tasks(
-        self,
-    ) -> Callable[[delivery_api.SearchTasksRequest], delivery_api.SearchTasksResponse]:
-        r"""Return a callable for the search tasks method over gRPC.
-
-        Deprecated: Use ``GetTaskTrackingInfo`` instead.
-
-        Returns:
-            Callable[[~.SearchTasksRequest],
-                    ~.SearchTasksResponse]:
-                A function that, when called, will call the underlying RPC
-                on the server.
-        """
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "search_tasks" not in self._stubs:
-            self._stubs["search_tasks"] = self.grpc_channel.unary_unary(
-                "/maps.fleetengine.delivery.v1.DeliveryService/SearchTasks",
-                request_serializer=delivery_api.SearchTasksRequest.serialize,
-                response_deserializer=delivery_api.SearchTasksResponse.deserialize,
-            )
-        return self._stubs["search_tasks"]
-
-    @property
     def update_task(self) -> Callable[[delivery_api.UpdateTaskRequest], tasks.Task]:
         r"""Return a callable for the update task method over gRPC.
 
         Updates ``Task`` data.
 
         Returns:
             Callable[[~.UpdateTaskRequest],
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/grpc_asyncio.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.maps.fleetengine_delivery_v1.types import (
     delivery_api,
@@ -65,15 +67,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -95,15 +96,15 @@
     def __init__(
         self,
         *,
         host: str = "fleetengine.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -115,37 +116,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'fleetengine.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -163,15 +167,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -203,15 +207,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -409,42 +415,14 @@
                 "/maps.fleetengine.delivery.v1.DeliveryService/GetTask",
                 request_serializer=delivery_api.GetTaskRequest.serialize,
                 response_deserializer=tasks.Task.deserialize,
             )
         return self._stubs["get_task"]
 
     @property
-    def search_tasks(
-        self,
-    ) -> Callable[
-        [delivery_api.SearchTasksRequest], Awaitable[delivery_api.SearchTasksResponse]
-    ]:
-        r"""Return a callable for the search tasks method over gRPC.
-
-        Deprecated: Use ``GetTaskTrackingInfo`` instead.
-
-        Returns:
-            Callable[[~.SearchTasksRequest],
-                    Awaitable[~.SearchTasksResponse]]:
-                A function that, when called, will call the underlying RPC
-                on the server.
-        """
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "search_tasks" not in self._stubs:
-            self._stubs["search_tasks"] = self.grpc_channel.unary_unary(
-                "/maps.fleetengine.delivery.v1.DeliveryService/SearchTasks",
-                request_serializer=delivery_api.SearchTasksRequest.serialize,
-                response_deserializer=delivery_api.SearchTasksResponse.deserialize,
-            )
-        return self._stubs["search_tasks"]
-
-    @property
     def update_task(
         self,
     ) -> Callable[[delivery_api.UpdateTaskRequest], Awaitable[tasks.Task]]:
         r"""Return a callable for the update task method over gRPC.
 
         Updates ``Task`` data.
 
@@ -549,12 +527,157 @@
             self._stubs["list_delivery_vehicles"] = self.grpc_channel.unary_unary(
                 "/maps.fleetengine.delivery.v1.DeliveryService/ListDeliveryVehicles",
                 request_serializer=delivery_api.ListDeliveryVehiclesRequest.serialize,
                 response_deserializer=delivery_api.ListDeliveryVehiclesResponse.deserialize,
             )
         return self._stubs["list_delivery_vehicles"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.create_delivery_vehicle: gapic_v1.method_async.wrap_method(
+                self.create_delivery_vehicle,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_delivery_vehicle: gapic_v1.method_async.wrap_method(
+                self.get_delivery_vehicle,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_delivery_vehicle: gapic_v1.method_async.wrap_method(
+                self.update_delivery_vehicle,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.batch_create_tasks: gapic_v1.method_async.wrap_method(
+                self.batch_create_tasks,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.create_task: gapic_v1.method_async.wrap_method(
+                self.create_task,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_task: gapic_v1.method_async.wrap_method(
+                self.get_task,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_task: gapic_v1.method_async.wrap_method(
+                self.update_task,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_tasks: gapic_v1.method_async.wrap_method(
+                self.list_tasks,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_task_tracking_info: gapic_v1.method_async.wrap_method(
+                self.get_task_tracking_info,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_delivery_vehicles: gapic_v1.method_async.wrap_method(
+                self.list_delivery_vehicles,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("DeliveryServiceGrpcAsyncIOTransport",)
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/services/delivery_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,22 +128,14 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_tasks(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
-            def pre_search_tasks(self, request, metadata):
-                logging.log(f"Received request: {request}")
-                return request, metadata
-
-            def post_search_tasks(self, response):
-                logging.log(f"Received response: {response}")
-                return response
-
             def pre_update_delivery_vehicle(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_delivery_vehicle(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -336,37 +328,14 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the DeliveryService server but before
         it is returned to user code.
         """
         return response
 
-    def pre_search_tasks(
-        self,
-        request: delivery_api.SearchTasksRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[delivery_api.SearchTasksRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for search_tasks
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the DeliveryService server.
-        """
-        return request, metadata
-
-    def post_search_tasks(
-        self, response: delivery_api.SearchTasksResponse
-    ) -> delivery_api.SearchTasksResponse:
-        """Post-rpc interceptor for search_tasks
-
-        Override in a subclass to manipulate the response
-        after it is returned by the DeliveryService server but before
-        it is returned to user code.
-        """
-        return response
-
     def pre_update_delivery_vehicle(
         self,
         request: delivery_api.UpdateDeliveryVehicleRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[delivery_api.UpdateDeliveryVehicleRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for update_delivery_vehicle
 
@@ -1279,105 +1248,14 @@
             resp = delivery_api.ListTasksResponse()
             pb_resp = delivery_api.ListTasksResponse.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_list_tasks(resp)
             return resp
 
-    class _SearchTasks(DeliveryServiceRestStub):
-        def __hash__(self):
-            return hash("SearchTasks")
-
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
-            "trackingId": "",
-        }
-
-        @classmethod
-        def _get_unset_required_fields(cls, message_dict):
-            return {
-                k: v
-                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
-                if k not in message_dict
-            }
-
-        def __call__(
-            self,
-            request: delivery_api.SearchTasksRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> delivery_api.SearchTasksResponse:
-            r"""Call the search tasks method over HTTP.
-
-            Args:
-                request (~.delivery_api.SearchTasksRequest):
-                    The request object. Deprecated: Issue ``GetTaskTrackingInfoRequest``\ s to
-                ``GetTaskTrackingInfo`` instead.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-
-            Returns:
-                ~.delivery_api.SearchTasksResponse:
-                    The ``SearchTasks`` response. It contains the set of
-                Tasks that meet the search criteria in the
-                ``SearchTasksRequest``.
-
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "get",
-                    "uri": "/v1/{parent=providers/*}/tasks:search",
-                },
-            ]
-            request, metadata = self._interceptor.pre_search_tasks(request, metadata)
-            pb_request = delivery_api.SearchTasksRequest.pb(request)
-            transcoded_request = path_template.transcode(http_options, pb_request)
-
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(
-                json_format.MessageToJson(
-                    transcoded_request["query_params"],
-                    use_integers_for_enums=True,
-                )
-            )
-            query_params.update(self._get_unset_required_fields(query_params))
-
-            query_params["$alt"] = "json;enum-encoding=int"
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params, strict=True),
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            # Return the response
-            resp = delivery_api.SearchTasksResponse()
-            pb_resp = delivery_api.SearchTasksResponse.pb(resp)
-
-            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
-            resp = self._interceptor.post_search_tasks(resp)
-            return resp
-
     class _UpdateDeliveryVehicle(DeliveryServiceRestStub):
         def __hash__(self):
             return hash("UpdateDeliveryVehicle")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "updateMask": {},
         }
@@ -1660,22 +1538,14 @@
         self,
     ) -> Callable[[delivery_api.ListTasksRequest], delivery_api.ListTasksResponse]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ListTasks(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
-    def search_tasks(
-        self,
-    ) -> Callable[[delivery_api.SearchTasksRequest], delivery_api.SearchTasksResponse]:
-        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
-        # In C++ this would require a dynamic_cast
-        return self._SearchTasks(self._session, self._host, self._interceptor)  # type: ignore
-
-    @property
     def update_delivery_vehicle(
         self,
     ) -> Callable[
         [delivery_api.UpdateDeliveryVehicleRequest], delivery_vehicles.DeliveryVehicle
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,14 @@
     GetDeliveryVehicleRequest,
     GetTaskRequest,
     GetTaskTrackingInfoRequest,
     ListDeliveryVehiclesRequest,
     ListDeliveryVehiclesResponse,
     ListTasksRequest,
     ListTasksResponse,
-    SearchTasksRequest,
-    SearchTasksResponse,
     UpdateDeliveryVehicleRequest,
     UpdateTaskRequest,
 )
 from .delivery_vehicles import (
     DeliveryVehicle,
     LocationInfo,
     VehicleJourneySegment,
@@ -62,16 +60,14 @@
     "GetDeliveryVehicleRequest",
     "GetTaskRequest",
     "GetTaskTrackingInfoRequest",
     "ListDeliveryVehiclesRequest",
     "ListDeliveryVehiclesResponse",
     "ListTasksRequest",
     "ListTasksResponse",
-    "SearchTasksRequest",
-    "SearchTasksResponse",
     "UpdateDeliveryVehicleRequest",
     "UpdateTaskRequest",
     "DeliveryVehicle",
     "LocationInfo",
     "VehicleJourneySegment",
     "VehicleStop",
     "DeliveryRequestHeader",
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/common.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_api.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/delivery_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,14 @@
         "ListDeliveryVehiclesRequest",
         "ListDeliveryVehiclesResponse",
         "UpdateDeliveryVehicleRequest",
         "BatchCreateTasksRequest",
         "BatchCreateTasksResponse",
         "CreateTaskRequest",
         "GetTaskRequest",
-        "SearchTasksRequest",
-        "SearchTasksResponse",
         "UpdateTaskRequest",
         "ListTasksRequest",
         "ListTasksResponse",
         "GetTaskTrackingInfoRequest",
     },
 )
 
@@ -422,108 +420,14 @@
     )
     name: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
-class SearchTasksRequest(proto.Message):
-    r"""Deprecated: Issue ``GetTaskTrackingInfoRequest``\ s to
-    ``GetTaskTrackingInfo`` instead.
-
-    Attributes:
-        header (google.maps.fleetengine_delivery_v1.types.DeliveryRequestHeader):
-            Optional. The standard Delivery API request
-            header.
-        parent (str):
-            Required. Must be in the format ``providers/{provider}``.
-            The provider must be the Google Cloud Project ID. For
-            example, ``sample-cloud-project``.
-        tracking_id (str):
-            Required. The identifier of the set of related Tasks being
-            requested. Tracking IDs are subject to the following
-            restrictions:
-
-            -  Must be a valid Unicode string.
-            -  Limited to a maximum length of 64 characters.
-            -  Normalized according to [Unicode Normalization Form C]
-               (http://www.unicode.org/reports/tr15/).
-            -  May not contain any of the following ASCII characters:
-               '/', ':', '?', ',', or '#'.
-        page_size (int):
-            Optional. The maximum number of Tasks to
-            return. The service may return fewer than this
-            value. If you don't specify this value, then the
-            server determines the number of results to
-            return.
-        page_token (str):
-            Optional. A page token, received from a previous
-            ``SearchTasks`` call. You must provide this value to
-            retrieve the subsequent page.
-
-            When paginating, all other parameters provided to
-            ``SearchTasks`` must match the call that provided the page
-            token.
-    """
-
-    header: mfd_header.DeliveryRequestHeader = proto.Field(
-        proto.MESSAGE,
-        number=1,
-        message=mfd_header.DeliveryRequestHeader,
-    )
-    parent: str = proto.Field(
-        proto.STRING,
-        number=3,
-    )
-    tracking_id: str = proto.Field(
-        proto.STRING,
-        number=4,
-    )
-    page_size: int = proto.Field(
-        proto.INT32,
-        number=5,
-    )
-    page_token: str = proto.Field(
-        proto.STRING,
-        number=6,
-    )
-
-
-class SearchTasksResponse(proto.Message):
-    r"""The ``SearchTasks`` response. It contains the set of Tasks that meet
-    the search criteria in the ``SearchTasksRequest``.
-
-    Attributes:
-        tasks (MutableSequence[google.maps.fleetengine_delivery_v1.types.Task]):
-            The set of Tasks for the requested ``tracking_id``. A
-            successful response can also be empty. An empty response
-            indicates that no Tasks are associated with the supplied
-            ``tracking_id``.
-        next_page_token (str):
-            Pass this token in the ``SearchTasksRequest`` to continue to
-            list results. If all results have been returned, then this
-            field is either an empty string, or it doesn't appear in the
-            response.
-    """
-
-    @property
-    def raw_page(self):
-        return self
-
-    tasks: MutableSequence[mfd_tasks.Task] = proto.RepeatedField(
-        proto.MESSAGE,
-        number=1,
-        message=mfd_tasks.Task,
-    )
-    next_page_token: str = proto.Field(
-        proto.STRING,
-        number=2,
-    )
-
-
 class UpdateTaskRequest(proto.Message):
     r"""The ``UpdateTask`` request message.
 
     Attributes:
         header (google.maps.fleetengine_delivery_v1.types.DeliveryRequestHeader):
             Optional. The standard Delivery API request
             header.
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/delivery_vehicles.py`

 * *Files 3% similar despite different names*

```diff
@@ -324,24 +324,22 @@
     ``Task``\ s.
 
     Attributes:
         planned_location (google.maps.fleetengine_delivery_v1.types.LocationInfo):
             Required. The location of the stop. Note that the locations
             in the ``Task``\ s might not exactly match this location,
             but will be within a short distance of it. This field won't
-            be populated in the response of either a ``GetTask``, or a
-            ``SearchTasks`` call.
+            be populated in the response of a ``GetTask`` call.
         tasks (MutableSequence[google.maps.fleetengine_delivery_v1.types.VehicleStop.TaskInfo]):
             The list of ``Task``\ s to be performed at this stop. This
-            field won't be populated in the response of either a
-            ``GetTask`` or ``SearchTasks`` call.
+            field won't be populated in the response of a ``GetTask``
+            call.
         state (google.maps.fleetengine_delivery_v1.types.VehicleStop.State):
             The state of the ``VehicleStop``. This field won't be
-            populated in the response of either a ``GetTask``, or a
-            ``SearchTasks`` call.
+            populated in the response of a ``GetTask`` call.
     """
 
     class State(proto.Enum):
         r"""The current state of a ``VehicleStop``.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -362,16 +360,16 @@
 
     class TaskInfo(proto.Message):
         r"""Additional information about the Task performed at this stop.
 
         Attributes:
             task_id (str):
                 The Task ID. This field won't be populated in the response
-                of either a ``GetTask``, or a ``SearchTasks`` call. Task IDs
-                are subject to the following restrictions:
+                of a ``GetTask`` call. Task IDs are subject to the following
+                restrictions:
 
                 -  Must be a valid Unicode string.
                 -  Limited to a maximum length of 64 characters.
                 -  Normalized according to [Unicode Normalization Form C]
                    (http://www.unicode.org/reports/tr15/).
                 -  May not contain any of the following ASCII characters:
                    '/', ':', '?', ',', or '#'.
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/header.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/header.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/task_tracking_info.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google/maps/fleetengine_delivery_v1/types/tasks.py` & `google-maps-fleetengine-delivery-0.2.0/google/maps/fleetengine_delivery_v1/types/tasks.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/PKG-INFO` & `google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-fleetengine-delivery
-Version: 0.1.8
+Version: 0.2.0
 Summary: Google Maps Fleetengine Delivery API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine-delivery
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-fleetengine-delivery-0.1.8/google_maps_fleetengine_delivery.egg-info/SOURCES.txt` & `google-maps-fleetengine-delivery-0.2.0/google_maps_fleetengine_delivery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/setup.py` & `google-maps-fleetengine-delivery-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/tests/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/tests/unit/__init__.py` & `google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/fleetengine_delivery_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-delivery-0.1.8/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py` & `google-maps-fleetengine-delivery-0.2.0/tests/unit/gapic/fleetengine_delivery_v1/test_delivery_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1207,14 +1207,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_delivery_vehicle), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateDeliveryVehicleRequest()
 
 
 def test_create_delivery_vehicle_non_empty_request_with_auto_populated_field():
@@ -1233,23 +1236,66 @@
         delivery_vehicle_id="delivery_vehicle_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_delivery_vehicle), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_delivery_vehicle(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateDeliveryVehicleRequest(
             parent="parent_value",
             delivery_vehicle_id="delivery_vehicle_id_value",
         )
 
 
+def test_create_delivery_vehicle_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_delivery_vehicle
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_delivery_vehicle
+        ] = mock_rpc
+        request = {}
+        client.create_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_delivery_vehicle_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1271,14 +1317,60 @@
         response = await client.create_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateDeliveryVehicleRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_delivery_vehicle_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_delivery_vehicle
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_delivery_vehicle
+        ] = mock_object
+
+        request = {}
+        await client.create_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_delivery_vehicle_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.CreateDeliveryVehicleRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1512,14 +1604,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_delivery_vehicle), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetDeliveryVehicleRequest()
 
 
 def test_get_delivery_vehicle_non_empty_request_with_auto_populated_field():
@@ -1537,22 +1632,64 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_delivery_vehicle), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_delivery_vehicle(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetDeliveryVehicleRequest(
             name="name_value",
         )
 
 
+def test_get_delivery_vehicle_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_delivery_vehicle in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_delivery_vehicle
+        ] = mock_rpc
+        request = {}
+        client.get_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_delivery_vehicle_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1574,14 +1711,60 @@
         response = await client.get_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetDeliveryVehicleRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_delivery_vehicle_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_delivery_vehicle
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_delivery_vehicle
+        ] = mock_object
+
+        request = {}
+        await client.get_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_delivery_vehicle_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.GetDeliveryVehicleRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -1792,14 +1975,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_delivery_vehicle), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
 
 
 def test_update_delivery_vehicle_non_empty_request_with_auto_populated_field():
@@ -1815,20 +2001,63 @@
     # if they meet the requirements of AIP 4235.
     request = delivery_api.UpdateDeliveryVehicleRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_delivery_vehicle), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_delivery_vehicle(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
 
 
+def test_update_delivery_vehicle_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_delivery_vehicle
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_delivery_vehicle
+        ] = mock_rpc
+        request = {}
+        client.update_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_delivery_vehicle_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -1850,14 +2079,60 @@
         response = await client.update_delivery_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateDeliveryVehicleRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_delivery_vehicle_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_delivery_vehicle
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_delivery_vehicle
+        ] = mock_object
+
+        request = {}
+        await client.update_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_delivery_vehicle_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.UpdateDeliveryVehicleRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2070,14 +2345,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.batch_create_tasks), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.batch_create_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.BatchCreateTasksRequest()
 
 
 def test_batch_create_tasks_non_empty_request_with_auto_populated_field():
@@ -2095,22 +2373,64 @@
         parent="parent_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.batch_create_tasks), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.batch_create_tasks(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.BatchCreateTasksRequest(
             parent="parent_value",
         )
 
 
+def test_batch_create_tasks_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.batch_create_tasks in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.batch_create_tasks
+        ] = mock_rpc
+        request = {}
+        client.batch_create_tasks(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.batch_create_tasks(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_batch_create_tasks_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2127,14 +2447,60 @@
         response = await client.batch_create_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.BatchCreateTasksRequest()
 
 
 @pytest.mark.asyncio
+async def test_batch_create_tasks_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.batch_create_tasks
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.batch_create_tasks
+        ] = mock_object
+
+        request = {}
+        await client.batch_create_tasks(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.batch_create_tasks(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_batch_create_tasks_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.BatchCreateTasksRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2251,14 +2617,17 @@
     client = DeliveryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_task), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateTaskRequest()
 
 
 def test_create_task_non_empty_request_with_auto_populated_field():
@@ -2275,23 +2644,61 @@
     request = delivery_api.CreateTaskRequest(
         parent="parent_value",
         task_id="task_id_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_task), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_task(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateTaskRequest(
             parent="parent_value",
             task_id="task_id_value",
         )
 
 
+def test_create_task_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_task in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_task] = mock_rpc
+        request = {}
+        client.create_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_task_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2314,14 +2721,60 @@
         response = await client.create_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.CreateTaskRequest()
 
 
 @pytest.mark.asyncio
+async def test_create_task_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_task
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_task
+        ] = mock_object
+
+        request = {}
+        await client.create_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_create_task_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.CreateTaskRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2552,14 +3005,17 @@
     client = DeliveryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_task), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskRequest()
 
 
 def test_get_task_non_empty_request_with_auto_populated_field():
@@ -2575,22 +3031,60 @@
     # if they meet the requirements of AIP 4235.
     request = delivery_api.GetTaskRequest(
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_task), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_task(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskRequest(
             name="name_value",
         )
 
 
+def test_get_task_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_task in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_task] = mock_rpc
+        request = {}
+        client.get_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_task_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -2613,14 +3107,58 @@
         response = await client.get_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_task_async_use_cached_wrapped_rpc(transport: str = "grpc_asyncio"):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_task
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_task
+        ] = mock_object
+
+        request = {}
+        await client.get_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_task_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.GetTaskRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -2773,450 +3311,14 @@
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
-        delivery_api.SearchTasksRequest,
-        dict,
-    ],
-)
-def test_search_tasks(request_type, transport: str = "grpc"):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = request_type()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = delivery_api.SearchTasksResponse(
-            next_page_token="next_page_token_value",
-        )
-        response = client.search_tasks(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        request = delivery_api.SearchTasksRequest()
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, pagers.SearchTasksPager)
-    assert response.next_page_token == "next_page_token_value"
-
-
-def test_search_tasks_empty_call():
-    # This test is a coverage failsafe to make sure that totally empty calls,
-    # i.e. request == None and no flattened fields passed, work.
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="grpc",
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        client.search_tasks()
-        call.assert_called()
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.SearchTasksRequest()
-
-
-def test_search_tasks_non_empty_request_with_auto_populated_field():
-    # This test is a coverage failsafe to make sure that UUID4 fields are
-    # automatically populated, according to AIP-4235, with non-empty requests.
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="grpc",
-    )
-
-    # Populate all string fields in the request which are not UUID4
-    # since we want to check that UUID4 are populated automatically
-    # if they meet the requirements of AIP 4235.
-    request = delivery_api.SearchTasksRequest(
-        parent="parent_value",
-        tracking_id="tracking_id_value",
-        page_token="page_token_value",
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        client.search_tasks(request=request)
-        call.assert_called()
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.SearchTasksRequest(
-            parent="parent_value",
-            tracking_id="tracking_id_value",
-            page_token="page_token_value",
-        )
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_empty_call_async():
-    # This test is a coverage failsafe to make sure that totally empty calls,
-    # i.e. request == None and no flattened fields passed, work.
-    client = DeliveryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="grpc_asyncio",
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            delivery_api.SearchTasksResponse(
-                next_page_token="next_page_token_value",
-            )
-        )
-        response = await client.search_tasks()
-        call.assert_called()
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == delivery_api.SearchTasksRequest()
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_async(
-    transport: str = "grpc_asyncio", request_type=delivery_api.SearchTasksRequest
-):
-    client = DeliveryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = request_type()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            delivery_api.SearchTasksResponse(
-                next_page_token="next_page_token_value",
-            )
-        )
-        response = await client.search_tasks(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls)
-        _, args, _ = call.mock_calls[0]
-        request = delivery_api.SearchTasksRequest()
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, pagers.SearchTasksAsyncPager)
-    assert response.next_page_token == "next_page_token_value"
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_async_from_dict():
-    await test_search_tasks_async(request_type=dict)
-
-
-def test_search_tasks_routing_parameters():
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = delivery_api.SearchTasksRequest(**{"parent": "providers/sample1"})
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        call.return_value = delivery_api.SearchTasksResponse()
-        client.search_tasks(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    _, _, kw = call.mock_calls[0]
-    # This test doesn't assert anything useful.
-    assert kw["metadata"]
-
-
-def test_search_tasks_flattened():
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = delivery_api.SearchTasksResponse()
-        # Call the method with a truthy value for each flattened field,
-        # using the keyword arguments to the method.
-        client.search_tasks(
-            parent="parent_value",
-        )
-
-        # Establish that the underlying call was made with the expected
-        # request object values.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        arg = args[0].parent
-        mock_val = "parent_value"
-        assert arg == mock_val
-
-
-def test_search_tasks_flattened_error():
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Attempting to call a method with both a request object and flattened
-    # fields is an error.
-    with pytest.raises(ValueError):
-        client.search_tasks(
-            delivery_api.SearchTasksRequest(),
-            parent="parent_value",
-        )
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_flattened_async():
-    client = DeliveryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = delivery_api.SearchTasksResponse()
-
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            delivery_api.SearchTasksResponse()
-        )
-        # Call the method with a truthy value for each flattened field,
-        # using the keyword arguments to the method.
-        response = await client.search_tasks(
-            parent="parent_value",
-        )
-
-        # Establish that the underlying call was made with the expected
-        # request object values.
-        assert len(call.mock_calls)
-        _, args, _ = call.mock_calls[0]
-        arg = args[0].parent
-        mock_val = "parent_value"
-        assert arg == mock_val
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_flattened_error_async():
-    client = DeliveryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Attempting to call a method with both a request object and flattened
-    # fields is an error.
-    with pytest.raises(ValueError):
-        await client.search_tasks(
-            delivery_api.SearchTasksRequest(),
-            parent="parent_value",
-        )
-
-
-def test_search_tasks_pager(transport_name: str = "grpc"):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport_name,
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Set the response to a series of pages.
-        call.side_effect = (
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-                next_page_token="abc",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[],
-                next_page_token="def",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                ],
-                next_page_token="ghi",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-            ),
-            RuntimeError,
-        )
-
-        metadata = ()
-        pager = client.search_tasks(request={})
-
-        assert pager._metadata == metadata
-
-        results = list(pager)
-        assert len(results) == 6
-        assert all(isinstance(i, tasks.Task) for i in results)
-
-
-def test_search_tasks_pages(transport_name: str = "grpc"):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport_name,
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_tasks), "__call__") as call:
-        # Set the response to a series of pages.
-        call.side_effect = (
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-                next_page_token="abc",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[],
-                next_page_token="def",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                ],
-                next_page_token="ghi",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-            ),
-            RuntimeError,
-        )
-        pages = list(client.search_tasks(request={}).pages)
-        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
-            assert page_.raw_page.next_page_token == token
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_async_pager():
-    client = DeliveryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.search_tasks), "__call__", new_callable=mock.AsyncMock
-    ) as call:
-        # Set the response to a series of pages.
-        call.side_effect = (
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-                next_page_token="abc",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[],
-                next_page_token="def",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                ],
-                next_page_token="ghi",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-            ),
-            RuntimeError,
-        )
-        async_pager = await client.search_tasks(
-            request={},
-        )
-        assert async_pager.next_page_token == "abc"
-        responses = []
-        async for response in async_pager:  # pragma: no branch
-            responses.append(response)
-
-        assert len(responses) == 6
-        assert all(isinstance(i, tasks.Task) for i in responses)
-
-
-@pytest.mark.asyncio
-async def test_search_tasks_async_pages():
-    client = DeliveryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.search_tasks), "__call__", new_callable=mock.AsyncMock
-    ) as call:
-        # Set the response to a series of pages.
-        call.side_effect = (
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-                next_page_token="abc",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[],
-                next_page_token="def",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                ],
-                next_page_token="ghi",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-            ),
-            RuntimeError,
-        )
-        pages = []
-        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
-        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
-        async for page_ in (  # pragma: no branch
-            await client.search_tasks(request={})
-        ).pages:
-            pages.append(page_)
-        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
-            assert page_.raw_page.next_page_token == token
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
         delivery_api.UpdateTaskRequest,
         dict,
     ],
 )
 def test_update_task(request_type, transport: str = "grpc"):
     client = DeliveryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3267,14 +3369,17 @@
     client = DeliveryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_task), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateTaskRequest()
 
 
 def test_update_task_non_empty_request_with_auto_populated_field():
@@ -3288,20 +3393,58 @@
     # Populate all string fields in the request which are not UUID4
     # since we want to check that UUID4 are populated automatically
     # if they meet the requirements of AIP 4235.
     request = delivery_api.UpdateTaskRequest()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_task), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_task(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateTaskRequest()
 
 
+def test_update_task_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_task in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_task] = mock_rpc
+        request = {}
+        client.update_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_task_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3324,14 +3467,60 @@
         response = await client.update_task()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.UpdateTaskRequest()
 
 
 @pytest.mark.asyncio
+async def test_update_task_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_task
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_task
+        ] = mock_object
+
+        request = {}
+        await client.update_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_update_task_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.UpdateTaskRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -3539,14 +3728,17 @@
     client = DeliveryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_tasks), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListTasksRequest()
 
 
 def test_list_tasks_non_empty_request_with_auto_populated_field():
@@ -3564,24 +3756,62 @@
         parent="parent_value",
         page_token="page_token_value",
         filter="filter_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_tasks), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_tasks(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListTasksRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
         )
 
 
+def test_list_tasks_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_tasks in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_tasks] = mock_rpc
+        request = {}
+        client.list_tasks(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_tasks(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_tasks_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -3599,14 +3829,58 @@
         response = await client.list_tasks()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListTasksRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_tasks_async_use_cached_wrapped_rpc(transport: str = "grpc_asyncio"):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_tasks
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_tasks
+        ] = mock_object
+
+        request = {}
+        await client.list_tasks(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_tasks(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_tasks_async(
     transport: str = "grpc_asyncio", request_type=delivery_api.ListTasksRequest
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
@@ -3988,14 +4262,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_task_tracking_info), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_task_tracking_info()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskTrackingInfoRequest()
 
 
 def test_get_task_tracking_info_non_empty_request_with_auto_populated_field():
@@ -4013,22 +4290,65 @@
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_task_tracking_info), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_task_tracking_info(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskTrackingInfoRequest(
             name="name_value",
         )
 
 
+def test_get_task_tracking_info_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_task_tracking_info
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_task_tracking_info
+        ] = mock_rpc
+        request = {}
+        client.get_task_tracking_info(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_task_tracking_info(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_task_tracking_info_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -4050,14 +4370,60 @@
         response = await client.get_task_tracking_info()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.GetTaskTrackingInfoRequest()
 
 
 @pytest.mark.asyncio
+async def test_get_task_tracking_info_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_task_tracking_info
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_task_tracking_info
+        ] = mock_object
+
+        request = {}
+        await client.get_task_tracking_info(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_task_tracking_info(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_get_task_tracking_info_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.GetTaskTrackingInfoRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4261,14 +4627,17 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_delivery_vehicles), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_delivery_vehicles()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListDeliveryVehiclesRequest()
 
 
 def test_list_delivery_vehicles_non_empty_request_with_auto_populated_field():
@@ -4288,24 +4657,67 @@
         filter="filter_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_delivery_vehicles), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_delivery_vehicles(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListDeliveryVehiclesRequest(
             parent="parent_value",
             page_token="page_token_value",
             filter="filter_value",
         )
 
 
+def test_list_delivery_vehicles_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_delivery_vehicles
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_delivery_vehicles
+        ] = mock_rpc
+        request = {}
+        client.list_delivery_vehicles(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_delivery_vehicles(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_delivery_vehicles_empty_call_async():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc_asyncio",
@@ -4325,14 +4737,60 @@
         response = await client.list_delivery_vehicles()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == delivery_api.ListDeliveryVehiclesRequest()
 
 
 @pytest.mark.asyncio
+async def test_list_delivery_vehicles_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = DeliveryServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_delivery_vehicles
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_delivery_vehicles
+        ] = mock_object
+
+        request = {}
+        await client.list_delivery_vehicles(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_delivery_vehicles(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
+@pytest.mark.asyncio
 async def test_list_delivery_vehicles_async(
     transport: str = "grpc_asyncio",
     request_type=delivery_api.ListDeliveryVehiclesRequest,
 ):
     client = DeliveryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4860,14 +5318,55 @@
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
     assert response.current_route_segment == b"current_route_segment_blob"
     assert response.type_ == delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO
 
 
+def test_create_delivery_vehicle_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.create_delivery_vehicle
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.create_delivery_vehicle
+        ] = mock_rpc
+
+        request = {}
+        client.create_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_delivery_vehicle_rest_required_fields(
     request_type=delivery_api.CreateDeliveryVehicleRequest,
 ):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -5173,14 +5672,54 @@
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
     assert response.current_route_segment == b"current_route_segment_blob"
     assert response.type_ == delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO
 
 
+def test_get_delivery_vehicle_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_delivery_vehicle in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_delivery_vehicle
+        ] = mock_rpc
+
+        request = {}
+        client.get_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_delivery_vehicle_rest_required_fields(
     request_type=delivery_api.GetDeliveryVehicleRequest,
 ):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -5586,14 +6125,55 @@
     assert (
         response.navigation_status == common.DeliveryVehicleNavigationStatus.NO_GUIDANCE
     )
     assert response.current_route_segment == b"current_route_segment_blob"
     assert response.type_ == delivery_vehicles.DeliveryVehicle.DeliveryVehicleType.AUTO
 
 
+def test_update_delivery_vehicle_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_delivery_vehicle
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_delivery_vehicle
+        ] = mock_rpc
+
+        request = {}
+        client.update_delivery_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_delivery_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_delivery_vehicle_rest_required_fields(
     request_type=delivery_api.UpdateDeliveryVehicleRequest,
 ):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -5872,14 +6452,54 @@
         req.return_value = response_value
         response = client.batch_create_tasks(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, delivery_api.BatchCreateTasksResponse)
 
 
+def test_batch_create_tasks_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.batch_create_tasks in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.batch_create_tasks
+        ] = mock_rpc
+
+        request = {}
+        client.batch_create_tasks(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.batch_create_tasks(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_batch_create_tasks_rest_required_fields(
     request_type=delivery_api.BatchCreateTasksRequest,
 ):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -6260,14 +6880,50 @@
         response.task_outcome_location_source
         == tasks.Task.TaskOutcomeLocationSource.PROVIDER
     )
     assert response.tracking_id == "tracking_id_value"
     assert response.delivery_vehicle_id == "delivery_vehicle_id_value"
 
 
+def test_create_task_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_task in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_task] = mock_rpc
+
+        request = {}
+        client.create_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_task_rest_required_fields(request_type=delivery_api.CreateTaskRequest):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
     request_init["task_id"] = ""
     request = request_type(**request_init)
@@ -6573,14 +7229,50 @@
         response.task_outcome_location_source
         == tasks.Task.TaskOutcomeLocationSource.PROVIDER
     )
     assert response.tracking_id == "tracking_id_value"
     assert response.delivery_vehicle_id == "delivery_vehicle_id_value"
 
 
+def test_get_task_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_task in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_task] = mock_rpc
+
+        request = {}
+        client.get_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_task_rest_required_fields(request_type=delivery_api.GetTaskRequest):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -6797,371 +7489,14 @@
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
-        delivery_api.SearchTasksRequest,
-        dict,
-    ],
-)
-def test_search_tasks_rest(request_type):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-
-    # send a request that will satisfy transcoding
-    request_init = {"parent": "providers/sample1"}
-    request = request_type(**request_init)
-
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = delivery_api.SearchTasksResponse(
-            next_page_token="next_page_token_value",
-        )
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        # Convert return value to protobuf type
-        return_value = delivery_api.SearchTasksResponse.pb(return_value)
-        json_return_value = json_format.MessageToJson(return_value)
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-        response = client.search_tasks(request)
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, pagers.SearchTasksPager)
-    assert response.next_page_token == "next_page_token_value"
-
-
-def test_search_tasks_rest_required_fields(
-    request_type=delivery_api.SearchTasksRequest,
-):
-    transport_class = transports.DeliveryServiceRestTransport
-
-    request_init = {}
-    request_init["parent"] = ""
-    request_init["tracking_id"] = ""
-    request = request_type(**request_init)
-    pb_request = request_type.pb(request)
-    jsonified_request = json.loads(
-        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
-    )
-
-    # verify fields with default values are dropped
-    assert "trackingId" not in jsonified_request
-
-    unset_fields = transport_class(
-        credentials=ga_credentials.AnonymousCredentials()
-    ).search_tasks._get_unset_required_fields(jsonified_request)
-    jsonified_request.update(unset_fields)
-
-    # verify required fields with default values are now present
-    assert "trackingId" in jsonified_request
-    assert jsonified_request["trackingId"] == request_init["tracking_id"]
-
-    jsonified_request["parent"] = "parent_value"
-    jsonified_request["trackingId"] = "tracking_id_value"
-
-    unset_fields = transport_class(
-        credentials=ga_credentials.AnonymousCredentials()
-    ).search_tasks._get_unset_required_fields(jsonified_request)
-    # Check that path parameters and body parameters are not mixing in.
-    assert not set(unset_fields) - set(
-        (
-            "header",
-            "page_size",
-            "page_token",
-            "tracking_id",
-        )
-    )
-    jsonified_request.update(unset_fields)
-
-    # verify required fields with non-default values are left alone
-    assert "parent" in jsonified_request
-    assert jsonified_request["parent"] == "parent_value"
-    assert "trackingId" in jsonified_request
-    assert jsonified_request["trackingId"] == "tracking_id_value"
-
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request = request_type(**request_init)
-
-    # Designate an appropriate value for the returned response.
-    return_value = delivery_api.SearchTasksResponse()
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(Session, "request") as req:
-        # We need to mock transcode() because providing default values
-        # for required fields will fail the real version if the http_options
-        # expect actual values for those fields.
-        with mock.patch.object(path_template, "transcode") as transcode:
-            # A uri without fields and an empty body will force all the
-            # request fields to show up in the query_params.
-            pb_request = request_type.pb(request)
-            transcode_result = {
-                "uri": "v1/sample_method",
-                "method": "get",
-                "query_params": pb_request,
-            }
-            transcode.return_value = transcode_result
-
-            response_value = Response()
-            response_value.status_code = 200
-
-            # Convert return value to protobuf type
-            return_value = delivery_api.SearchTasksResponse.pb(return_value)
-            json_return_value = json_format.MessageToJson(return_value)
-
-            response_value._content = json_return_value.encode("UTF-8")
-            req.return_value = response_value
-
-            response = client.search_tasks(request)
-
-            expected_params = [
-                (
-                    "trackingId",
-                    "",
-                ),
-                ("$alt", "json;enum-encoding=int"),
-            ]
-            actual_params = req.call_args.kwargs["params"]
-            assert expected_params == actual_params
-
-
-def test_search_tasks_rest_unset_required_fields():
-    transport = transports.DeliveryServiceRestTransport(
-        credentials=ga_credentials.AnonymousCredentials
-    )
-
-    unset_fields = transport.search_tasks._get_unset_required_fields({})
-    assert set(unset_fields) == (
-        set(
-            (
-                "header",
-                "pageSize",
-                "pageToken",
-                "trackingId",
-            )
-        )
-        & set(
-            (
-                "parent",
-                "trackingId",
-            )
-        )
-    )
-
-
-@pytest.mark.parametrize("null_interceptor", [True, False])
-def test_search_tasks_rest_interceptors(null_interceptor):
-    transport = transports.DeliveryServiceRestTransport(
-        credentials=ga_credentials.AnonymousCredentials(),
-        interceptor=None
-        if null_interceptor
-        else transports.DeliveryServiceRestInterceptor(),
-    )
-    client = DeliveryServiceClient(transport=transport)
-    with mock.patch.object(
-        type(client.transport._session), "request"
-    ) as req, mock.patch.object(
-        path_template, "transcode"
-    ) as transcode, mock.patch.object(
-        transports.DeliveryServiceRestInterceptor, "post_search_tasks"
-    ) as post, mock.patch.object(
-        transports.DeliveryServiceRestInterceptor, "pre_search_tasks"
-    ) as pre:
-        pre.assert_not_called()
-        post.assert_not_called()
-        pb_message = delivery_api.SearchTasksRequest.pb(
-            delivery_api.SearchTasksRequest()
-        )
-        transcode.return_value = {
-            "method": "post",
-            "uri": "my_uri",
-            "body": pb_message,
-            "query_params": pb_message,
-        }
-
-        req.return_value = Response()
-        req.return_value.status_code = 200
-        req.return_value.request = PreparedRequest()
-        req.return_value._content = delivery_api.SearchTasksResponse.to_json(
-            delivery_api.SearchTasksResponse()
-        )
-
-        request = delivery_api.SearchTasksRequest()
-        metadata = [
-            ("key", "val"),
-            ("cephalopod", "squid"),
-        ]
-        pre.return_value = request, metadata
-        post.return_value = delivery_api.SearchTasksResponse()
-
-        client.search_tasks(
-            request,
-            metadata=[
-                ("key", "val"),
-                ("cephalopod", "squid"),
-            ],
-        )
-
-        pre.assert_called_once()
-        post.assert_called_once()
-
-
-def test_search_tasks_rest_bad_request(
-    transport: str = "rest", request_type=delivery_api.SearchTasksRequest
-):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # send a request that will satisfy transcoding
-    request_init = {"parent": "providers/sample1"}
-    request = request_type(**request_init)
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.search_tasks(request)
-
-
-def test_search_tasks_rest_flattened():
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = delivery_api.SearchTasksResponse()
-
-        # get arguments that satisfy an http rule for this method
-        sample_request = {"parent": "providers/sample1"}
-
-        # get truthy value for each flattened field
-        mock_args = dict(
-            parent="parent_value",
-        )
-        mock_args.update(sample_request)
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        # Convert return value to protobuf type
-        return_value = delivery_api.SearchTasksResponse.pb(return_value)
-        json_return_value = json_format.MessageToJson(return_value)
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        client.search_tasks(**mock_args)
-
-        # Establish that the underlying call was made with the expected
-        # request object values.
-        assert len(req.mock_calls) == 1
-        _, args, _ = req.mock_calls[0]
-        assert path_template.validate(
-            "%s/v1/{parent=providers/*}/tasks:search" % client.transport._host, args[1]
-        )
-
-
-def test_search_tasks_rest_flattened_error(transport: str = "rest"):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Attempting to call a method with both a request object and flattened
-    # fields is an error.
-    with pytest.raises(ValueError):
-        client.search_tasks(
-            delivery_api.SearchTasksRequest(),
-            parent="parent_value",
-        )
-
-
-def test_search_tasks_rest_pager(transport: str = "rest"):
-    client = DeliveryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(Session, "request") as req:
-        # TODO(kbandes): remove this mock unless there's a good reason for it.
-        # with mock.patch.object(path_template, 'transcode') as transcode:
-        # Set the response as a series of pages
-        response = (
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-                next_page_token="abc",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[],
-                next_page_token="def",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                ],
-                next_page_token="ghi",
-            ),
-            delivery_api.SearchTasksResponse(
-                tasks=[
-                    tasks.Task(),
-                    tasks.Task(),
-                ],
-            ),
-        )
-        # Two responses for two calls
-        response = response + response
-
-        # Wrap the values into proper Response objs
-        response = tuple(delivery_api.SearchTasksResponse.to_json(x) for x in response)
-        return_values = tuple(Response() for i in response)
-        for return_val, response_val in zip(return_values, response):
-            return_val._content = response_val.encode("UTF-8")
-            return_val.status_code = 200
-        req.side_effect = return_values
-
-        sample_request = {"parent": "providers/sample1"}
-
-        pager = client.search_tasks(request=sample_request)
-
-        results = list(pager)
-        assert len(results) == 6
-        assert all(isinstance(i, tasks.Task) for i in results)
-
-        pages = list(client.search_tasks(request=sample_request).pages)
-        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
-            assert page_.raw_page.next_page_token == token
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
         delivery_api.UpdateTaskRequest,
         dict,
     ],
 )
 def test_update_task_rest(request_type):
     client = DeliveryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -7360,14 +7695,50 @@
         response.task_outcome_location_source
         == tasks.Task.TaskOutcomeLocationSource.PROVIDER
     )
     assert response.tracking_id == "tracking_id_value"
     assert response.delivery_vehicle_id == "delivery_vehicle_id_value"
 
 
+def test_update_task_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_task in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_task] = mock_rpc
+
+        request = {}
+        client.update_task(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_task(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_task_rest_required_fields(request_type=delivery_api.UpdateTaskRequest):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
     jsonified_request = json.loads(
@@ -7639,14 +8010,50 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListTasksPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
+def test_list_tasks_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_tasks in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_tasks] = mock_rpc
+
+        request = {}
+        client.list_tasks(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_tasks(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_tasks_rest_required_fields(request_type=delivery_api.ListTasksRequest):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
@@ -7980,14 +8387,55 @@
     assert isinstance(response, task_tracking_info.TaskTrackingInfo)
     assert response.name == "name_value"
     assert response.tracking_id == "tracking_id_value"
     assert response.state == tasks.Task.State.OPEN
     assert response.task_outcome == tasks.Task.TaskOutcome.SUCCEEDED
 
 
+def test_get_task_tracking_info_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.get_task_tracking_info
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.get_task_tracking_info
+        ] = mock_rpc
+
+        request = {}
+        client.get_task_tracking_info(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_task_tracking_info(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_task_tracking_info_rest_required_fields(
     request_type=delivery_api.GetTaskTrackingInfoRequest,
 ):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -8250,14 +8698,55 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDeliveryVehiclesPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
+def test_list_delivery_vehicles_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = DeliveryServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.list_delivery_vehicles
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.list_delivery_vehicles
+        ] = mock_rpc
+
+        request = {}
+        client.list_delivery_vehicles(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_delivery_vehicles(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_delivery_vehicles_rest_required_fields(
     request_type=delivery_api.ListDeliveryVehiclesRequest,
 ):
     transport_class = transports.DeliveryServiceRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -8699,15 +9188,14 @@
     methods = (
         "create_delivery_vehicle",
         "get_delivery_vehicle",
         "update_delivery_vehicle",
         "batch_create_tasks",
         "create_task",
         "get_task",
-        "search_tasks",
         "update_task",
         "list_tasks",
         "get_task_tracking_info",
         "list_delivery_vehicles",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
@@ -8980,17 +9468,14 @@
     assert session1 != session2
     session1 = client1.transport.create_task._session
     session2 = client2.transport.create_task._session
     assert session1 != session2
     session1 = client1.transport.get_task._session
     session2 = client2.transport.get_task._session
     assert session1 != session2
-    session1 = client1.transport.search_tasks._session
-    session2 = client2.transport.search_tasks._session
-    assert session1 != session2
     session1 = client1.transport.update_task._session
     session2 = client2.transport.update_task._session
     assert session1 != session2
     session1 = client1.transport.list_tasks._session
     session2 = client2.transport.list_tasks._session
     assert session1 != session2
     session1 = client1.transport.get_task_tracking_info._session
```

