# Comparing `tmp/google-maps-fleetengine-0.1.9.tar.gz` & `tmp/google-maps-fleetengine-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-fleetengine-0.1.9.tar", last modified: Tue Mar  5 19:01:29 2024, max compression
+gzip compressed data, was "google-maps-fleetengine-0.2.0.tar", last modified: Thu May 16 17:16:09 2024, max compression
```

## Comparing `google-maps-fleetengine-0.1.9.tar` & `google-maps-fleetengine-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.303316 google-maps-fleetengine-0.1.9/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5677 2024-03-05 19:01:29.303316 google-maps-fleetengine-0.1.9/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4256 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.287315 google-maps-fleetengine-0.1.9/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.287315 google-maps-fleetengine-0.1.9/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.291315 google-maps-fleetengine-0.1.9/google/maps/fleetengine/
--rw-rw-r--   0 root         (0)     1003     3891 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.291315 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/
--rw-rw-r--   0 root         (0)     1003     3457 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4057 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.291315 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.295316 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27756 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    44474 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/client.py
--rw-rw-r--   0 root         (0)     1003     5663 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.295316 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/
--rw-rw-r--   0 root         (0)     1003     1166 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9067 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15860 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16194 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.295316 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41288 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58945 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/client.py
--rw-rw-r--   0 root         (0)     1003     5753 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.295316 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11139 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21963 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22363 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.299316 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/
--rw-rw-r--   0 root         (0)     1003     2994 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    21382 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/fleetengine.py
--rw-rw-r--   0 root         (0)     1003     5319 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/header.py
--rw-rw-r--   0 root         (0)     1003     3519 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/traffic.py
--rw-rw-r--   0 root         (0)     1003    17503 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/trip_api.py
--rw-rw-r--   0 root         (0)     1003    19332 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/trips.py
--rw-rw-r--   0 root         (0)     1003    43717 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/vehicle_api.py
--rw-rw-r--   0 root         (0)     1003    20708 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/vehicles.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.299316 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/
--rw-r--r--   0 root         (0)     1003     5677 2024-03-05 19:01:29.000000 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2306 2024-03-05 19:01:29.000000 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:29.000000 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:29.000000 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      338 2024-03-05 19:01:29.000000 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:01:29.000000 google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 19:01:29.303316 google-maps-fleetengine-0.1.9/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3218 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.299316 google-maps-fleetengine-0.1.9/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.299316 google-maps-fleetengine-0.1.9/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.299316 google-maps-fleetengine-0.1.9/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:29.299316 google-maps-fleetengine-0.1.9/tests/unit/gapic/fleetengine_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/tests/unit/gapic/fleetengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    97728 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/tests/unit/gapic/fleetengine_v1/test_trip_service.py
--rw-rw-r--   0 root         (0)     1003   113856 2024-03-05 18:46:03.000000 google-maps-fleetengine-0.1.9/tests/unit/gapic/fleetengine_v1/test_vehicle_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.304919 google-maps-fleetengine-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5677 2024-05-16 17:16:09.304919 google-maps-fleetengine-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4256 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.288918 google-maps-fleetengine-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.288918 google-maps-fleetengine-0.2.0/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.292918 google-maps-fleetengine-0.2.0/google/maps/fleetengine/
+-rw-rw-r--   0 root         (0)     1003     3821 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.292918 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/
+-rw-rw-r--   0 root         (0)     1003     3387 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3505 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.292918 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.296919 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27577 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44758 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5663 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.296919 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1166 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9067 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16407 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19332 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.296919 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34038 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51415 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5753 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.296919 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10145 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20028 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23535 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.300919 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2924 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21504 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/fleetengine.py
+-rw-rw-r--   0 root         (0)     1003     5319 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/header.py
+-rw-rw-r--   0 root         (0)     1003     3519 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/traffic.py
+-rw-rw-r--   0 root         (0)     1003    17503 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/trip_api.py
+-rw-rw-r--   0 root         (0)     1003    19332 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/trips.py
+-rw-rw-r--   0 root         (0)     1003    42139 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/vehicle_api.py
+-rw-rw-r--   0 root         (0)     1003    20708 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/vehicles.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.300919 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     5677 2024-05-16 17:16:09.000000 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2306 2024-05-16 17:16:09.000000 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 17:16:09.000000 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 17:16:09.000000 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      338 2024-05-16 17:16:09.000000 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-16 17:16:09.000000 google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-16 17:16:09.304919 google-maps-fleetengine-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3218 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.300919 google-maps-fleetengine-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.300919 google-maps-fleetengine-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.300919 google-maps-fleetengine-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:16:09.304919 google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   124464 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/test_trip_service.py
+-rw-rw-r--   0 root         (0)     1003   136717 2024-05-16 17:11:30.000000 google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/test_vehicle_service.py
```

### Comparing `google-maps-fleetengine-0.1.9/LICENSE` & `google-maps-fleetengine-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-0.1.9/MANIFEST.in` & `google-maps-fleetengine-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-0.1.9/PKG-INFO` & `google-maps-fleetengine-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-fleetengine
-Version: 0.1.9
+Version: 0.2.0
 Summary: Google Maps Fleetengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-fleetengine-0.1.9/README.rst` & `google-maps-fleetengine-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -65,15 +65,14 @@
     GetVehicleRequest,
     ListVehiclesRequest,
     ListVehiclesResponse,
     SearchVehiclesRequest,
     SearchVehiclesResponse,
     UpdateVehicleAttributesRequest,
     UpdateVehicleAttributesResponse,
-    UpdateVehicleLocationRequest,
     UpdateVehicleRequest,
     VehicleAttributeList,
     VehicleMatch,
     Waypoint,
 )
 from google.maps.fleetengine_v1.types.vehicles import (
     BatteryInfo,
@@ -121,15 +120,14 @@
     "GetVehicleRequest",
     "ListVehiclesRequest",
     "ListVehiclesResponse",
     "SearchVehiclesRequest",
     "SearchVehiclesResponse",
     "UpdateVehicleAttributesRequest",
     "UpdateVehicleAttributesResponse",
-    "UpdateVehicleLocationRequest",
     "UpdateVehicleRequest",
     "VehicleAttributeList",
     "VehicleMatch",
     "Waypoint",
     "BatteryInfo",
     "DeviceSettings",
     "LicensePlate",
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine/gapic_version.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -54,15 +54,14 @@
     GetVehicleRequest,
     ListVehiclesRequest,
     ListVehiclesResponse,
     SearchVehiclesRequest,
     SearchVehiclesResponse,
     UpdateVehicleAttributesRequest,
     UpdateVehicleAttributesResponse,
-    UpdateVehicleLocationRequest,
     UpdateVehicleRequest,
     VehicleAttributeList,
     VehicleMatch,
     Waypoint,
 )
 from .types.vehicles import (
     BatteryInfo,
@@ -113,15 +112,14 @@
     "TripStatus",
     "TripType",
     "TripView",
     "TripWaypoint",
     "UpdateTripRequest",
     "UpdateVehicleAttributesRequest",
     "UpdateVehicleAttributesResponse",
-    "UpdateVehicleLocationRequest",
     "UpdateVehicleRequest",
     "Vehicle",
     "VehicleAttribute",
     "VehicleAttributeList",
     "VehicleLocation",
     "VehicleMatch",
     "VehicleServiceClient",
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/gapic_metadata.json` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/gapic_metadata.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996744791666666%*

 * *Differences: {"'services'": "{'VehicleService': {'clients': {'grpc': {'rpcs': {delete: ['SearchFuzzedVehicles', "*

 * *               "'UpdateVehicleLocation']}}, 'grpc-async': {'rpcs': {delete: "*

 * *               "['SearchFuzzedVehicles', 'UpdateVehicleLocation']}}}}}"}*

```diff
@@ -85,38 +85,28 @@
                             ]
                         },
                         "ListVehicles": {
                             "methods": [
                                 "list_vehicles"
                             ]
                         },
-                        "SearchFuzzedVehicles": {
-                            "methods": [
-                                "search_fuzzed_vehicles"
-                            ]
-                        },
                         "SearchVehicles": {
                             "methods": [
                                 "search_vehicles"
                             ]
                         },
                         "UpdateVehicle": {
                             "methods": [
                                 "update_vehicle"
                             ]
                         },
                         "UpdateVehicleAttributes": {
                             "methods": [
                                 "update_vehicle_attributes"
                             ]
-                        },
-                        "UpdateVehicleLocation": {
-                            "methods": [
-                                "update_vehicle_location"
-                            ]
                         }
                     }
                 },
                 "grpc-async": {
                     "libraryClient": "VehicleServiceAsyncClient",
                     "rpcs": {
                         "CreateVehicle": {
@@ -130,38 +120,28 @@
                             ]
                         },
                         "ListVehicles": {
                             "methods": [
                                 "list_vehicles"
                             ]
                         },
-                        "SearchFuzzedVehicles": {
-                            "methods": [
-                                "search_fuzzed_vehicles"
-                            ]
-                        },
                         "SearchVehicles": {
                             "methods": [
                                 "search_vehicles"
                             ]
                         },
                         "UpdateVehicle": {
                             "methods": [
                                 "update_vehicle"
                             ]
                         },
                         "UpdateVehicleAttributes": {
                             "methods": [
                                 "update_vehicle_attributes"
                             ]
-                        },
-                        "UpdateVehicleLocation": {
-                            "methods": [
-                                "update_vehicle_location"
-                            ]
                         }
                     }
                 }
             }
         }
     }
 }
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/gapic_version.py` & `google-maps-fleetengine-0.2.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/__init__.py` & `google-maps-fleetengine-0.2.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/async_client.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
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
@@ -191,29 +192,33 @@
         type(TripServiceClient).get_transport_class, type(TripServiceClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, TripServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, TripServiceTransport, Callable[..., TripServiceTransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the trip service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.TripServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,TripServiceTransport,Callable[..., TripServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the TripServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -301,32 +306,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Trip:
                 Trip metadata.
         """
         # Create or coerce a protobuf request object.
-        request = trip_api.CreateTripRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, trip_api.CreateTripRequest):
+            request = trip_api.CreateTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_trip,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_trip
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -390,32 +387,22 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Trip:
                 Trip metadata.
         """
         # Create or coerce a protobuf request object.
-        request = trip_api.GetTripRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, trip_api.GetTripRequest):
+            request = trip_api.GetTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_trip,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[self._client._transport.get_trip]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -473,23 +460,24 @@
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        request = trip_api.ReportBillableTripRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, trip_api.ReportBillableTripRequest):
+            request = trip_api.ReportBillableTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.report_billable_trip,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.report_billable_trip
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -556,32 +544,24 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        request = trip_api.SearchTripsRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, trip_api.SearchTripsRequest):
+            request = trip_api.SearchTripsRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.search_trips,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.search_trips
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -654,32 +634,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Trip:
                 Trip metadata.
         """
         # Create or coerce a protobuf request object.
-        request = trip_api.UpdateTripRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, trip_api.UpdateTripRequest):
+            request = trip_api.UpdateTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_trip,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_trip
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/client.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
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
@@ -521,29 +522,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, TripServiceTransport]] = None,
+        transport: Optional[
+            Union[str, TripServiceTransport, Callable[..., TripServiceTransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the trip service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, TripServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,TripServiceTransport,Callable[..., TripServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the TripServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -641,16 +646,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[TripServiceTransport], Callable[..., TripServiceTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., TripServiceTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -706,18 +718,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Trip:
                 Trip metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a trip_api.CreateTripRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, trip_api.CreateTripRequest):
             request = trip_api.CreateTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.create_trip]
 
@@ -793,18 +803,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Trip:
                 Trip metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a trip_api.GetTripRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, trip_api.GetTripRequest):
             request = trip_api.GetTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.get_trip]
 
@@ -874,18 +882,16 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a trip_api.ReportBillableTripRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, trip_api.ReportBillableTripRequest):
             request = trip_api.ReportBillableTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.report_billable_trip]
 
@@ -964,18 +970,16 @@
 
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a trip_api.SearchTripsRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, trip_api.SearchTripsRequest):
             request = trip_api.SearchTripsRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.search_trips]
 
@@ -1060,18 +1064,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Trip:
                 Trip metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a trip_api.UpdateTripRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, trip_api.UpdateTripRequest):
             request = trip_api.UpdateTripRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_trip]
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/pagers.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/base.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/grpc.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -46,15 +46,15 @@
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
@@ -66,36 +66,39 @@
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
@@ -113,15 +116,15 @@
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
@@ -154,15 +157,17 @@
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
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/trip_service/transports/grpc_asyncio.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/trip_service/transports/grpc_asyncio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
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
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.maps.fleetengine_v1.types import trip_api, trips
@@ -61,15 +63,14 @@
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
@@ -91,15 +92,15 @@
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
@@ -111,37 +112,40 @@
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
@@ -159,15 +163,15 @@
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
@@ -199,15 +203,17 @@
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
@@ -359,12 +365,78 @@
             self._stubs["update_trip"] = self.grpc_channel.unary_unary(
                 "/maps.fleetengine.v1.TripService/UpdateTrip",
                 request_serializer=trip_api.UpdateTripRequest.serialize,
                 response_deserializer=trips.Trip.deserialize,
             )
         return self._stubs["update_trip"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.create_trip: gapic_v1.method_async.wrap_method(
+                self.create_trip,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.get_trip: gapic_v1.method_async.wrap_method(
+                self.get_trip,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.report_billable_trip: gapic_v1.method_async.wrap_method(
+                self.report_billable_trip,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.search_trips: gapic_v1.method_async.wrap_method(
+                self.search_trips,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.update_trip: gapic_v1.method_async.wrap_method(
+                self.update_trip,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("TripServiceGrpcAsyncIOTransport",)
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/async_client.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/async_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,25 +13,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
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
 )
-import warnings
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry_async as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -41,15 +41,14 @@
 try:
     OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault, None]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.AsyncRetry, object, None]  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
-from google.type import latlng_pb2  # type: ignore
 
 from google.maps.fleetengine_v1.services.vehicle_service import pagers
 from google.maps.fleetengine_v1.types import fleetengine, vehicle_api, vehicles
 
 from .client import VehicleServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, VehicleServiceTransport
 from .transports.grpc_asyncio import VehicleServiceGrpcAsyncIOTransport
@@ -195,29 +194,33 @@
         type(VehicleServiceClient).get_transport_class, type(VehicleServiceClient)
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, VehicleServiceTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[str, VehicleServiceTransport, Callable[..., VehicleServiceTransport]]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the vehicle service async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.VehicleServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,VehicleServiceTransport,Callable[..., VehicleServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the VehicleServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -334,32 +337,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Vehicle:
                 Vehicle metadata.
         """
         # Create or coerce a protobuf request object.
-        request = vehicle_api.CreateVehicleRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, vehicle_api.CreateVehicleRequest):
+            request = vehicle_api.CreateVehicleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_vehicle,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_vehicle
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -423,32 +418,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Vehicle:
                 Vehicle metadata.
         """
         # Create or coerce a protobuf request object.
-        request = vehicle_api.GetVehicleRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, vehicle_api.GetVehicleRequest):
+            request = vehicle_api.GetVehicleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_vehicle,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_vehicle
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -529,120 +516,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Vehicle:
                 Vehicle metadata.
         """
         # Create or coerce a protobuf request object.
-        request = vehicle_api.UpdateVehicleRequest(request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_vehicle,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
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
-    async def update_vehicle_location(
-        self,
-        request: Optional[Union[vehicle_api.UpdateVehicleLocationRequest, dict]] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> fleetengine.VehicleLocation:
-        r"""Deprecated: Use the ``UpdateVehicle`` method instead.
-        UpdateVehicleLocation updates the location of the vehicle.
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
-            from google.maps import fleetengine_v1
-
-            async def sample_update_vehicle_location():
-                # Create a client
-                client = fleetengine_v1.VehicleServiceAsyncClient()
-
-                # Initialize request argument(s)
-                request = fleetengine_v1.UpdateVehicleLocationRequest(
-                    name="name_value",
-                )
-
-                # Make the request
-                response = await client.update_vehicle_location(request=request)
-
-                # Handle the response
-                print(response)
-
-        Args:
-            request (Optional[Union[google.maps.fleetengine_v1.types.UpdateVehicleLocationRequest, dict]]):
-                The request object. ``UpdateVehicleLocation`` request message.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.maps.fleetengine_v1.types.VehicleLocation:
-                The location, speed, and heading of a
-                vehicle at a point in time.
-
-        """
-        warnings.warn(
-            "VehicleServiceAsyncClient.update_vehicle_location is deprecated",
-            DeprecationWarning,
-        )
-
-        # Create or coerce a protobuf request object.
-        request = vehicle_api.UpdateVehicleLocationRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, vehicle_api.UpdateVehicleRequest):
+            request = vehicle_api.UpdateVehicleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_vehicle_location,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_vehicle
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -717,32 +608,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.UpdateVehicleAttributesResponse:
                 UpdateVehicleAttributes response message.
         """
         # Create or coerce a protobuf request object.
-        request = vehicle_api.UpdateVehicleAttributesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, vehicle_api.UpdateVehicleAttributesRequest):
+            request = vehicle_api.UpdateVehicleAttributesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_vehicle_attributes,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_vehicle_attributes
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -813,23 +696,24 @@
                 ListVehicles response message.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        request = vehicle_api.ListVehiclesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, vehicle_api.ListVehiclesRequest):
+            request = vehicle_api.ListVehiclesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_vehicles,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_vehicles
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -908,122 +792,24 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.SearchVehiclesResponse:
                 SearchVehicles response message.
         """
         # Create or coerce a protobuf request object.
-        request = vehicle_api.SearchVehiclesRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, vehicle_api.SearchVehiclesRequest):
+            request = vehicle_api.SearchVehiclesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.search_vehicles,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=15.0,
-            ),
-            default_timeout=15.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
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
-    async def search_fuzzed_vehicles(
-        self,
-        request: Optional[Union[vehicle_api.SearchVehiclesRequest, dict]] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> vehicle_api.SearchVehiclesResponse:
-        r"""Deprecated: Use ``SearchVehicles`` instead.
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
-            from google.maps import fleetengine_v1
-
-            async def sample_search_fuzzed_vehicles():
-                # Create a client
-                client = fleetengine_v1.VehicleServiceAsyncClient()
-
-                # Initialize request argument(s)
-                request = fleetengine_v1.SearchVehiclesRequest(
-                    parent="parent_value",
-                    pickup_radius_meters=2146,
-                    count=553,
-                    minimum_capacity=1705,
-                    trip_types=['EXCLUSIVE'],
-                    order_by="COST",
-                )
-
-                # Make the request
-                response = await client.search_fuzzed_vehicles(request=request)
-
-                # Handle the response
-                print(response)
-
-        Args:
-            request (Optional[Union[google.maps.fleetengine_v1.types.SearchVehiclesRequest, dict]]):
-                The request object. ``SearchVehicles`` request message.
-            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.maps.fleetengine_v1.types.SearchVehiclesResponse:
-                SearchVehicles response message.
-        """
-        warnings.warn(
-            "VehicleServiceAsyncClient.search_fuzzed_vehicles is deprecated",
-            DeprecationWarning,
-        )
-
-        # Create or coerce a protobuf request object.
-        request = vehicle_api.SearchVehiclesRequest(request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.search_fuzzed_vehicles,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.search_vehicles
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/client.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
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
@@ -45,15 +46,14 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault, None]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object, None]  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
-from google.type import latlng_pb2  # type: ignore
 
 from google.maps.fleetengine_v1.services.vehicle_service import pagers
 from google.maps.fleetengine_v1.types import fleetengine, vehicle_api, vehicles
 
 from .transports.base import DEFAULT_CLIENT_INFO, VehicleServiceTransport
 from .transports.grpc import VehicleServiceGrpcTransport
 from .transports.grpc_asyncio import VehicleServiceGrpcAsyncIOTransport
@@ -522,29 +522,33 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, VehicleServiceTransport]] = None,
+        transport: Optional[
+            Union[str, VehicleServiceTransport, Callable[..., VehicleServiceTransport]]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the vehicle service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, VehicleServiceTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,VehicleServiceTransport,Callable[..., VehicleServiceTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the VehicleServiceTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -645,16 +649,23 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[VehicleServiceTransport], Callable[..., VehicleServiceTransport]
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., VehicleServiceTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -739,18 +750,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Vehicle:
                 Vehicle metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.CreateVehicleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, vehicle_api.CreateVehicleRequest):
             request = vehicle_api.CreateVehicleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.create_vehicle]
 
@@ -826,18 +835,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Vehicle:
                 Vehicle metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.GetVehicleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, vehicle_api.GetVehicleRequest):
             request = vehicle_api.GetVehicleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.get_vehicle]
 
@@ -930,18 +937,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.Vehicle:
                 Vehicle metadata.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.UpdateVehicleRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, vehicle_api.UpdateVehicleRequest):
             request = vehicle_api.UpdateVehicleRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.update_vehicle]
 
@@ -967,109 +972,14 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def update_vehicle_location(
-        self,
-        request: Optional[Union[vehicle_api.UpdateVehicleLocationRequest, dict]] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> fleetengine.VehicleLocation:
-        r"""Deprecated: Use the ``UpdateVehicle`` method instead.
-        UpdateVehicleLocation updates the location of the vehicle.
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
-            from google.maps import fleetengine_v1
-
-            def sample_update_vehicle_location():
-                # Create a client
-                client = fleetengine_v1.VehicleServiceClient()
-
-                # Initialize request argument(s)
-                request = fleetengine_v1.UpdateVehicleLocationRequest(
-                    name="name_value",
-                )
-
-                # Make the request
-                response = client.update_vehicle_location(request=request)
-
-                # Handle the response
-                print(response)
-
-        Args:
-            request (Union[google.maps.fleetengine_v1.types.UpdateVehicleLocationRequest, dict]):
-                The request object. ``UpdateVehicleLocation`` request message.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.maps.fleetengine_v1.types.VehicleLocation:
-                The location, speed, and heading of a
-                vehicle at a point in time.
-
-        """
-        warnings.warn(
-            "VehicleServiceClient.update_vehicle_location is deprecated",
-            DeprecationWarning,
-        )
-
-        # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.UpdateVehicleLocationRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, vehicle_api.UpdateVehicleLocationRequest):
-            request = vehicle_api.UpdateVehicleLocationRequest(request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.update_vehicle_location]
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
     def update_vehicle_attributes(
         self,
         request: Optional[
             Union[vehicle_api.UpdateVehicleAttributesRequest, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
@@ -1123,18 +1033,16 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.UpdateVehicleAttributesResponse:
                 UpdateVehicleAttributes response message.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.UpdateVehicleAttributesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, vehicle_api.UpdateVehicleAttributesRequest):
             request = vehicle_api.UpdateVehicleAttributesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[
             self._transport.update_vehicle_attributes
@@ -1219,18 +1127,16 @@
                 ListVehicles response message.
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.ListVehiclesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, vehicle_api.ListVehiclesRequest):
             request = vehicle_api.ListVehiclesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.list_vehicles]
 
@@ -1321,128 +1227,29 @@
                 sent along with the request as metadata.
 
         Returns:
             google.maps.fleetengine_v1.types.SearchVehiclesResponse:
                 SearchVehicles response message.
         """
         # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.SearchVehiclesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, vehicle_api.SearchVehiclesRequest):
             request = vehicle_api.SearchVehiclesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.search_vehicles]
 
         header_params = {}
 
         routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
         regex_match = routing_param_regex.match(request.parent)
         if regex_match and regex_match.group("provider_id"):
             header_params["provider_id"] = regex_match.group("provider_id")
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
-    def search_fuzzed_vehicles(
-        self,
-        request: Optional[Union[vehicle_api.SearchVehiclesRequest, dict]] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> vehicle_api.SearchVehiclesResponse:
-        r"""Deprecated: Use ``SearchVehicles`` instead.
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
-            from google.maps import fleetengine_v1
-
-            def sample_search_fuzzed_vehicles():
-                # Create a client
-                client = fleetengine_v1.VehicleServiceClient()
-
-                # Initialize request argument(s)
-                request = fleetengine_v1.SearchVehiclesRequest(
-                    parent="parent_value",
-                    pickup_radius_meters=2146,
-                    count=553,
-                    minimum_capacity=1705,
-                    trip_types=['EXCLUSIVE'],
-                    order_by="COST",
-                )
-
-                # Make the request
-                response = client.search_fuzzed_vehicles(request=request)
-
-                # Handle the response
-                print(response)
-
-        Args:
-            request (Union[google.maps.fleetengine_v1.types.SearchVehiclesRequest, dict]):
-                The request object. ``SearchVehicles`` request message.
-            retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-
-        Returns:
-            google.maps.fleetengine_v1.types.SearchVehiclesResponse:
-                SearchVehicles response message.
-        """
-        warnings.warn(
-            "VehicleServiceClient.search_fuzzed_vehicles is deprecated",
-            DeprecationWarning,
-        )
-
-        # Create or coerce a protobuf request object.
-        # Minor optimization to avoid making a copy if the user passes
-        # in a vehicle_api.SearchVehiclesRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
-        if not isinstance(request, vehicle_api.SearchVehiclesRequest):
-            request = vehicle_api.SearchVehiclesRequest(request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = self._transport._wrapped_methods[self._transport.search_fuzzed_vehicles]
-
-        header_params = {}
-
-        routing_param_regex = re.compile("^(?P<provider_id>providers/[^/]+)$")
-        regex_match = routing_param_regex.match(request.parent)
-        if regex_match and regex_match.group("provider_id"):
-            header_params["provider_id"] = regex_match.group("provider_id")
 
         if header_params:
             metadata = tuple(metadata) + (
                 gapic_v1.routing_header.to_grpc_metadata(header_params),
             )
 
         # Validate the universe domain.
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/pagers.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/pagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/base.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.maps.fleetengine_v1 import gapic_version as package_version
-from google.maps.fleetengine_v1.types import fleetengine, vehicle_api, vehicles
+from google.maps.fleetengine_v1.types import vehicle_api, vehicles
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class VehicleServiceTransport(abc.ABC):
@@ -164,19 +164,14 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=15.0,
                 ),
                 default_timeout=15.0,
                 client_info=client_info,
             ),
-            self.update_vehicle_location: gapic_v1.method.wrap_method(
-                self.update_vehicle_location,
-                default_timeout=None,
-                client_info=client_info,
-            ),
             self.update_vehicle_attributes: gapic_v1.method.wrap_method(
                 self.update_vehicle_attributes,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
@@ -202,19 +197,14 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=15.0,
                 ),
                 default_timeout=15.0,
                 client_info=client_info,
             ),
-            self.search_fuzzed_vehicles: gapic_v1.method.wrap_method(
-                self.search_fuzzed_vehicles,
-                default_timeout=None,
-                client_info=client_info,
-            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -246,23 +236,14 @@
     ) -> Callable[
         [vehicle_api.UpdateVehicleRequest],
         Union[vehicles.Vehicle, Awaitable[vehicles.Vehicle]],
     ]:
         raise NotImplementedError()
 
     @property
-    def update_vehicle_location(
-        self,
-    ) -> Callable[
-        [vehicle_api.UpdateVehicleLocationRequest],
-        Union[fleetengine.VehicleLocation, Awaitable[fleetengine.VehicleLocation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
     def update_vehicle_attributes(
         self,
     ) -> Callable[
         [vehicle_api.UpdateVehicleAttributesRequest],
         Union[
             vehicle_api.UpdateVehicleAttributesResponse,
             Awaitable[vehicle_api.UpdateVehicleAttributesResponse],
@@ -287,26 +268,14 @@
         self,
     ) -> Callable[
         [vehicle_api.SearchVehiclesRequest],
         Union[
             vehicle_api.SearchVehiclesResponse,
             Awaitable[vehicle_api.SearchVehiclesResponse],
         ],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def search_fuzzed_vehicles(
-        self,
-    ) -> Callable[
-        [vehicle_api.SearchVehiclesRequest],
-        Union[
-            vehicle_api.SearchVehiclesResponse,
-            Awaitable[vehicle_api.SearchVehiclesResponse],
-        ],
     ]:
         raise NotImplementedError()
 
     @property
     def kind(self) -> str:
         raise NotImplementedError()
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc_asyncio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,105 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers
-import google.auth  # type: ignore
+from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
-from google.maps.fleetengine_v1.types import fleetengine, vehicle_api, vehicles
+from google.maps.fleetengine_v1.types import vehicle_api, vehicles
 
 from .base import DEFAULT_CLIENT_INFO, VehicleServiceTransport
+from .grpc import VehicleServiceGrpcTransport
 
 
-class VehicleServiceGrpcTransport(VehicleServiceTransport):
-    """gRPC backend transport for VehicleService.
+class VehicleServiceGrpcAsyncIOTransport(VehicleServiceTransport):
+    """gRPC AsyncIO backend transport for VehicleService.
 
     Vehicle management service.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "fleetengine.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "fleetengine.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -65,68 +111,71 @@
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
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                This argument is ignored if a ``channel`` instance is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
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
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
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
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -153,15 +202,17 @@
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
@@ -172,70 +223,28 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "fleetengine.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
     def create_vehicle(
         self,
-    ) -> Callable[[vehicle_api.CreateVehicleRequest], vehicles.Vehicle]:
+    ) -> Callable[[vehicle_api.CreateVehicleRequest], Awaitable[vehicles.Vehicle]]:
         r"""Return a callable for the create vehicle method over gRPC.
 
         Instantiates a new vehicle associated with an on-demand
         rideshare or deliveries provider. Each ``Vehicle`` must have a
         unique vehicle ID.
 
         The following ``Vehicle`` fields are required when creating a
@@ -264,15 +273,15 @@
         -  ``eta_to_next_waypoint``
         -  ``navigation_status``
 
         All other fields are optional and used if provided.
 
         Returns:
             Callable[[~.CreateVehicleRequest],
-                    ~.Vehicle]:
+                    Awaitable[~.Vehicle]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -283,22 +292,22 @@
                 response_deserializer=vehicles.Vehicle.deserialize,
             )
         return self._stubs["create_vehicle"]
 
     @property
     def get_vehicle(
         self,
-    ) -> Callable[[vehicle_api.GetVehicleRequest], vehicles.Vehicle]:
+    ) -> Callable[[vehicle_api.GetVehicleRequest], Awaitable[vehicles.Vehicle]]:
         r"""Return a callable for the get vehicle method over gRPC.
 
         Returns a vehicle from the Fleet Engine.
 
         Returns:
             Callable[[~.GetVehicleRequest],
-                    ~.Vehicle]:
+                    Awaitable[~.Vehicle]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -309,15 +318,15 @@
                 response_deserializer=vehicles.Vehicle.deserialize,
             )
         return self._stubs["get_vehicle"]
 
     @property
     def update_vehicle(
         self,
-    ) -> Callable[[vehicle_api.UpdateVehicleRequest], vehicles.Vehicle]:
+    ) -> Callable[[vehicle_api.UpdateVehicleRequest], Awaitable[vehicles.Vehicle]]:
         r"""Return a callable for the update vehicle method over gRPC.
 
         Writes updated vehicle data to the Fleet Engine.
 
         When updating a ``Vehicle``, the following fields cannot be
         updated since they are managed by the server:
 
@@ -333,15 +342,15 @@
         request. If you want to update only some attributes, see the
         ``UpdateVehicleAttributes`` method. Likewise, the ``waypoints``
         field can be updated, but must contain all the waypoints
         currently on the vehicle, and no other waypoints.
 
         Returns:
             Callable[[~.UpdateVehicleRequest],
-                    ~.Vehicle]:
+                    Awaitable[~.Vehicle]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -350,61 +359,32 @@
                 "/maps.fleetengine.v1.VehicleService/UpdateVehicle",
                 request_serializer=vehicle_api.UpdateVehicleRequest.serialize,
                 response_deserializer=vehicles.Vehicle.deserialize,
             )
         return self._stubs["update_vehicle"]
 
     @property
-    def update_vehicle_location(
-        self,
-    ) -> Callable[
-        [vehicle_api.UpdateVehicleLocationRequest], fleetengine.VehicleLocation
-    ]:
-        r"""Return a callable for the update vehicle location method over gRPC.
-
-        Deprecated: Use the ``UpdateVehicle`` method instead.
-        UpdateVehicleLocation updates the location of the vehicle.
-
-        Returns:
-            Callable[[~.UpdateVehicleLocationRequest],
-                    ~.VehicleLocation]:
-                A function that, when called, will call the underlying RPC
-                on the server.
-        """
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "update_vehicle_location" not in self._stubs:
-            self._stubs["update_vehicle_location"] = self.grpc_channel.unary_unary(
-                "/maps.fleetengine.v1.VehicleService/UpdateVehicleLocation",
-                request_serializer=vehicle_api.UpdateVehicleLocationRequest.serialize,
-                response_deserializer=fleetengine.VehicleLocation.deserialize,
-            )
-        return self._stubs["update_vehicle_location"]
-
-    @property
     def update_vehicle_attributes(
         self,
     ) -> Callable[
         [vehicle_api.UpdateVehicleAttributesRequest],
-        vehicle_api.UpdateVehicleAttributesResponse,
+        Awaitable[vehicle_api.UpdateVehicleAttributesResponse],
     ]:
         r"""Return a callable for the update vehicle attributes method over gRPC.
 
         Partially updates a vehicle's attributes. Only the attributes
         mentioned in the request will be updated, other attributes will
         NOT be altered. Note: this is different in ``UpdateVehicle``,
         where the whole ``attributes`` field will be replaced by the one
         in ``UpdateVehicleRequest``, attributes not in the request would
         be removed.
 
         Returns:
             Callable[[~.UpdateVehicleAttributesRequest],
-                    ~.UpdateVehicleAttributesResponse]:
+                    Awaitable[~.UpdateVehicleAttributesResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -415,23 +395,25 @@
                 response_deserializer=vehicle_api.UpdateVehicleAttributesResponse.deserialize,
             )
         return self._stubs["update_vehicle_attributes"]
 
     @property
     def list_vehicles(
         self,
-    ) -> Callable[[vehicle_api.ListVehiclesRequest], vehicle_api.ListVehiclesResponse]:
+    ) -> Callable[
+        [vehicle_api.ListVehiclesRequest], Awaitable[vehicle_api.ListVehiclesResponse]
+    ]:
         r"""Return a callable for the list vehicles method over gRPC.
 
         Returns a paginated list of vehicles associated with
         a provider that match the request options.
 
         Returns:
             Callable[[~.ListVehiclesRequest],
-                    ~.ListVehiclesResponse]:
+                    Awaitable[~.ListVehiclesResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -443,24 +425,25 @@
             )
         return self._stubs["list_vehicles"]
 
     @property
     def search_vehicles(
         self,
     ) -> Callable[
-        [vehicle_api.SearchVehiclesRequest], vehicle_api.SearchVehiclesResponse
+        [vehicle_api.SearchVehiclesRequest],
+        Awaitable[vehicle_api.SearchVehiclesResponse],
     ]:
         r"""Return a callable for the search vehicles method over gRPC.
 
         Returns a list of vehicles that match the request
         options.
 
         Returns:
             Callable[[~.SearchVehiclesRequest],
-                    ~.SearchVehiclesResponse]:
+                    Awaitable[~.SearchVehiclesResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -468,44 +451,92 @@
             self._stubs["search_vehicles"] = self.grpc_channel.unary_unary(
                 "/maps.fleetengine.v1.VehicleService/SearchVehicles",
                 request_serializer=vehicle_api.SearchVehiclesRequest.serialize,
                 response_deserializer=vehicle_api.SearchVehiclesResponse.deserialize,
             )
         return self._stubs["search_vehicles"]
 
-    @property
-    def search_fuzzed_vehicles(
-        self,
-    ) -> Callable[
-        [vehicle_api.SearchVehiclesRequest], vehicle_api.SearchVehiclesResponse
-    ]:
-        r"""Return a callable for the search fuzzed vehicles method over gRPC.
-
-        Deprecated: Use ``SearchVehicles`` instead.
-
-        Returns:
-            Callable[[~.SearchVehiclesRequest],
-                    ~.SearchVehiclesResponse]:
-                A function that, when called, will call the underlying RPC
-                on the server.
-        """
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "search_fuzzed_vehicles" not in self._stubs:
-            self._stubs["search_fuzzed_vehicles"] = self.grpc_channel.unary_unary(
-                "/maps.fleetengine.v1.VehicleService/SearchFuzzedVehicles",
-                request_serializer=vehicle_api.SearchVehiclesRequest.serialize,
-                response_deserializer=vehicle_api.SearchVehiclesResponse.deserialize,
-            )
-        return self._stubs["search_fuzzed_vehicles"]
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.create_vehicle: gapic_v1.method_async.wrap_method(
+                self.create_vehicle,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.get_vehicle: gapic_v1.method_async.wrap_method(
+                self.get_vehicle,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.update_vehicle: gapic_v1.method_async.wrap_method(
+                self.update_vehicle,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.update_vehicle_attributes: gapic_v1.method_async.wrap_method(
+                self.update_vehicle_attributes,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+            self.list_vehicles: gapic_v1.method_async.wrap_method(
+                self.list_vehicles,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.search_vehicles: gapic_v1.method_async.wrap_method(
+                self.search_vehicles,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=15.0,
+                ),
+                default_timeout=15.0,
+                client_info=client_info,
+            ),
+        }
 
     def close(self):
-        self.grpc_channel.close()
-
-    @property
-    def kind(self) -> str:
-        return "grpc"
+        return self.grpc_channel.close()
 
 
-__all__ = ("VehicleServiceGrpcTransport",)
+__all__ = ("VehicleServiceGrpcAsyncIOTransport",)
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc_asyncio.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/services/vehicle_service/transports/grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,59 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import gapic_v1, grpc_helpers
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
-from google.maps.fleetengine_v1.types import fleetengine, vehicle_api, vehicles
+from google.maps.fleetengine_v1.types import vehicle_api, vehicles
 
 from .base import DEFAULT_CLIENT_INFO, VehicleServiceTransport
-from .grpc import VehicleServiceGrpcTransport
 
 
-class VehicleServiceGrpcAsyncIOTransport(VehicleServiceTransport):
-    """gRPC AsyncIO backend transport for VehicleService.
+class VehicleServiceGrpcTransport(VehicleServiceTransport):
+    """gRPC backend transport for VehicleService.
 
     Vehicle management service.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "fleetengine.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "fleetengine.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -110,68 +65,71 @@
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
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+                This argument is ignored if a ``channel`` instance is provided.
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
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
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
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
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -198,15 +156,17 @@
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
@@ -217,28 +177,70 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "fleetengine.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def create_vehicle(
         self,
-    ) -> Callable[[vehicle_api.CreateVehicleRequest], Awaitable[vehicles.Vehicle]]:
+    ) -> Callable[[vehicle_api.CreateVehicleRequest], vehicles.Vehicle]:
         r"""Return a callable for the create vehicle method over gRPC.
 
         Instantiates a new vehicle associated with an on-demand
         rideshare or deliveries provider. Each ``Vehicle`` must have a
         unique vehicle ID.
 
         The following ``Vehicle`` fields are required when creating a
@@ -267,15 +269,15 @@
         -  ``eta_to_next_waypoint``
         -  ``navigation_status``
 
         All other fields are optional and used if provided.
 
         Returns:
             Callable[[~.CreateVehicleRequest],
-                    Awaitable[~.Vehicle]]:
+                    ~.Vehicle]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -286,22 +288,22 @@
                 response_deserializer=vehicles.Vehicle.deserialize,
             )
         return self._stubs["create_vehicle"]
 
     @property
     def get_vehicle(
         self,
-    ) -> Callable[[vehicle_api.GetVehicleRequest], Awaitable[vehicles.Vehicle]]:
+    ) -> Callable[[vehicle_api.GetVehicleRequest], vehicles.Vehicle]:
         r"""Return a callable for the get vehicle method over gRPC.
 
         Returns a vehicle from the Fleet Engine.
 
         Returns:
             Callable[[~.GetVehicleRequest],
-                    Awaitable[~.Vehicle]]:
+                    ~.Vehicle]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -312,15 +314,15 @@
                 response_deserializer=vehicles.Vehicle.deserialize,
             )
         return self._stubs["get_vehicle"]
 
     @property
     def update_vehicle(
         self,
-    ) -> Callable[[vehicle_api.UpdateVehicleRequest], Awaitable[vehicles.Vehicle]]:
+    ) -> Callable[[vehicle_api.UpdateVehicleRequest], vehicles.Vehicle]:
         r"""Return a callable for the update vehicle method over gRPC.
 
         Writes updated vehicle data to the Fleet Engine.
 
         When updating a ``Vehicle``, the following fields cannot be
         updated since they are managed by the server:
 
@@ -336,15 +338,15 @@
         request. If you want to update only some attributes, see the
         ``UpdateVehicleAttributes`` method. Likewise, the ``waypoints``
         field can be updated, but must contain all the waypoints
         currently on the vehicle, and no other waypoints.
 
         Returns:
             Callable[[~.UpdateVehicleRequest],
-                    Awaitable[~.Vehicle]]:
+                    ~.Vehicle]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -353,62 +355,32 @@
                 "/maps.fleetengine.v1.VehicleService/UpdateVehicle",
                 request_serializer=vehicle_api.UpdateVehicleRequest.serialize,
                 response_deserializer=vehicles.Vehicle.deserialize,
             )
         return self._stubs["update_vehicle"]
 
     @property
-    def update_vehicle_location(
-        self,
-    ) -> Callable[
-        [vehicle_api.UpdateVehicleLocationRequest],
-        Awaitable[fleetengine.VehicleLocation],
-    ]:
-        r"""Return a callable for the update vehicle location method over gRPC.
-
-        Deprecated: Use the ``UpdateVehicle`` method instead.
-        UpdateVehicleLocation updates the location of the vehicle.
-
-        Returns:
-            Callable[[~.UpdateVehicleLocationRequest],
-                    Awaitable[~.VehicleLocation]]:
-                A function that, when called, will call the underlying RPC
-                on the server.
-        """
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "update_vehicle_location" not in self._stubs:
-            self._stubs["update_vehicle_location"] = self.grpc_channel.unary_unary(
-                "/maps.fleetengine.v1.VehicleService/UpdateVehicleLocation",
-                request_serializer=vehicle_api.UpdateVehicleLocationRequest.serialize,
-                response_deserializer=fleetengine.VehicleLocation.deserialize,
-            )
-        return self._stubs["update_vehicle_location"]
-
-    @property
     def update_vehicle_attributes(
         self,
     ) -> Callable[
         [vehicle_api.UpdateVehicleAttributesRequest],
-        Awaitable[vehicle_api.UpdateVehicleAttributesResponse],
+        vehicle_api.UpdateVehicleAttributesResponse,
     ]:
         r"""Return a callable for the update vehicle attributes method over gRPC.
 
         Partially updates a vehicle's attributes. Only the attributes
         mentioned in the request will be updated, other attributes will
         NOT be altered. Note: this is different in ``UpdateVehicle``,
         where the whole ``attributes`` field will be replaced by the one
         in ``UpdateVehicleRequest``, attributes not in the request would
         be removed.
 
         Returns:
             Callable[[~.UpdateVehicleAttributesRequest],
-                    Awaitable[~.UpdateVehicleAttributesResponse]]:
+                    ~.UpdateVehicleAttributesResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -419,25 +391,23 @@
                 response_deserializer=vehicle_api.UpdateVehicleAttributesResponse.deserialize,
             )
         return self._stubs["update_vehicle_attributes"]
 
     @property
     def list_vehicles(
         self,
-    ) -> Callable[
-        [vehicle_api.ListVehiclesRequest], Awaitable[vehicle_api.ListVehiclesResponse]
-    ]:
+    ) -> Callable[[vehicle_api.ListVehiclesRequest], vehicle_api.ListVehiclesResponse]:
         r"""Return a callable for the list vehicles method over gRPC.
 
         Returns a paginated list of vehicles associated with
         a provider that match the request options.
 
         Returns:
             Callable[[~.ListVehiclesRequest],
-                    Awaitable[~.ListVehiclesResponse]]:
+                    ~.ListVehiclesResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -449,25 +419,24 @@
             )
         return self._stubs["list_vehicles"]
 
     @property
     def search_vehicles(
         self,
     ) -> Callable[
-        [vehicle_api.SearchVehiclesRequest],
-        Awaitable[vehicle_api.SearchVehiclesResponse],
+        [vehicle_api.SearchVehiclesRequest], vehicle_api.SearchVehiclesResponse
     ]:
         r"""Return a callable for the search vehicles method over gRPC.
 
         Returns a list of vehicles that match the request
         options.
 
         Returns:
             Callable[[~.SearchVehiclesRequest],
-                    Awaitable[~.SearchVehiclesResponse]]:
+                    ~.SearchVehiclesResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -475,41 +444,16 @@
             self._stubs["search_vehicles"] = self.grpc_channel.unary_unary(
                 "/maps.fleetengine.v1.VehicleService/SearchVehicles",
                 request_serializer=vehicle_api.SearchVehiclesRequest.serialize,
                 response_deserializer=vehicle_api.SearchVehiclesResponse.deserialize,
             )
         return self._stubs["search_vehicles"]
 
-    @property
-    def search_fuzzed_vehicles(
-        self,
-    ) -> Callable[
-        [vehicle_api.SearchVehiclesRequest],
-        Awaitable[vehicle_api.SearchVehiclesResponse],
-    ]:
-        r"""Return a callable for the search fuzzed vehicles method over gRPC.
-
-        Deprecated: Use ``SearchVehicles`` instead.
-
-        Returns:
-            Callable[[~.SearchVehiclesRequest],
-                    Awaitable[~.SearchVehiclesResponse]]:
-                A function that, when called, will call the underlying RPC
-                on the server.
-        """
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "search_fuzzed_vehicles" not in self._stubs:
-            self._stubs["search_fuzzed_vehicles"] = self.grpc_channel.unary_unary(
-                "/maps.fleetengine.v1.VehicleService/SearchFuzzedVehicles",
-                request_serializer=vehicle_api.SearchVehiclesRequest.serialize,
-                response_deserializer=vehicle_api.SearchVehiclesResponse.deserialize,
-            )
-        return self._stubs["search_fuzzed_vehicles"]
-
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
+
+    @property
+    def kind(self) -> str:
+        return "grpc"
 
 
-__all__ = ("VehicleServiceGrpcAsyncIOTransport",)
+__all__ = ("VehicleServiceGrpcTransport",)
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/__init__.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -41,15 +41,14 @@
     GetVehicleRequest,
     ListVehiclesRequest,
     ListVehiclesResponse,
     SearchVehiclesRequest,
     SearchVehiclesResponse,
     UpdateVehicleAttributesRequest,
     UpdateVehicleAttributesResponse,
-    UpdateVehicleLocationRequest,
     UpdateVehicleRequest,
     VehicleAttributeList,
     VehicleMatch,
     Waypoint,
 )
 from .vehicles import (
     BatteryInfo,
@@ -93,15 +92,14 @@
     "GetVehicleRequest",
     "ListVehiclesRequest",
     "ListVehiclesResponse",
     "SearchVehiclesRequest",
     "SearchVehiclesResponse",
     "UpdateVehicleAttributesRequest",
     "UpdateVehicleAttributesResponse",
-    "UpdateVehicleLocationRequest",
     "UpdateVehicleRequest",
     "VehicleAttributeList",
     "VehicleMatch",
     "Waypoint",
     "BatteryInfo",
     "DeviceSettings",
     "LicensePlate",
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/fleetengine.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/fleetengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -165,15 +165,16 @@
     CUSTOMER_SUPPLIED_LOCATION = 5
     FLEET_ENGINE_LOCATION = 6
     FUSED_LOCATION_PROVIDER = 100
     CORE_LOCATION = 200
 
 
 class TerminalPointId(proto.Message):
-    r"""Identifies a terminal point.
+    r"""Deprecated: TerminalPoints are no longer supported in Fleet Engine.
+    Use ``TerminalLocation.point`` instead.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
@@ -184,15 +185,15 @@
 
             This field is a member of `oneof`_ ``Id``.
         generated_id (str):
             Deprecated.
 
             This field is a member of `oneof`_ ``Id``.
         value (str):
-            Unique ID of the terminal point.
+            Deprecated.
     """
 
     place_id: str = proto.Field(
         proto.STRING,
         number=2,
         oneof="Id",
     )
@@ -211,17 +212,17 @@
     r"""Describes the location of a waypoint.
 
     Attributes:
         point (google.type.latlng_pb2.LatLng):
             Required. Denotes the location of a trip
             waypoint.
         terminal_point_id (google.maps.fleetengine_v1.types.TerminalPointId):
-            ID of the terminal point.
+            Deprecated: Specify the ``point`` field instead.
         access_point_id (str):
-            Deprecated.
+            Deprecated: Specify the ``point`` field instead.
         trip_id (str):
             Deprecated.
         terminal_location_type (google.maps.fleetengine_v1.types.WaypointType):
             Deprecated: ``Vehicle.waypoint`` will have this data.
     """
 
     point: latlng_pb2.LatLng = proto.Field(
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/header.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/traffic.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/traffic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/trip_api.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/trip_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/trips.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/trips.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/vehicle_api.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/vehicle_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,15 +31,14 @@
 
 __protobuf__ = proto.module(
     package="maps.fleetengine.v1",
     manifest={
         "CreateVehicleRequest",
         "GetVehicleRequest",
         "UpdateVehicleRequest",
-        "UpdateVehicleLocationRequest",
         "UpdateVehicleAttributesRequest",
         "UpdateVehicleAttributesResponse",
         "SearchVehiclesRequest",
         "SearchVehiclesResponse",
         "ListVehiclesRequest",
         "ListVehiclesResponse",
         "Waypoint",
@@ -222,56 +221,14 @@
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=5,
         message=field_mask_pb2.FieldMask,
     )
 
 
-class UpdateVehicleLocationRequest(proto.Message):
-    r"""``UpdateVehicleLocation`` request message.
-
-    Attributes:
-        header (google.maps.fleetengine_v1.types.RequestHeader):
-            The standard Fleet Engine request header.
-        name (str):
-            Required. Must be in the format
-            ``providers/{provider}/vehicles/{vehicle}``. The {provider}
-            must be the Project ID (for example,
-            ``sample-cloud-project``) of the Google Cloud Project of
-            which the service account making this call is a member.
-        current_location (google.maps.fleetengine_v1.types.VehicleLocation):
-            Required. The vehicle's most recent location. The
-            ``location`` and ``update_time`` subfields are required.
-        current_state (google.maps.fleetengine_v1.types.VehicleState):
-            Set the vehicle's state to either ``ONLINE`` or ``OFFLINE``.
-            If set to ``UNKNOWN_VEHICLE_STATE``, the vehicle's state
-            will not be altered.
-    """
-
-    header: mf_header.RequestHeader = proto.Field(
-        proto.MESSAGE,
-        number=1,
-        message=mf_header.RequestHeader,
-    )
-    name: str = proto.Field(
-        proto.STRING,
-        number=3,
-    )
-    current_location: fleetengine.VehicleLocation = proto.Field(
-        proto.MESSAGE,
-        number=4,
-        message=fleetengine.VehicleLocation,
-    )
-    current_state: mf_vehicles.VehicleState = proto.Field(
-        proto.ENUM,
-        number=5,
-        enum=mf_vehicles.VehicleState,
-    )
-
-
 class UpdateVehicleAttributesRequest(proto.Message):
     r"""``UpdateVehicleAttributes`` request message.
 
     Attributes:
         header (google.maps.fleetengine_v1.types.RequestHeader):
             The standard Fleet Engine request header.
         name (str):
```

### Comparing `google-maps-fleetengine-0.1.9/google/maps/fleetengine_v1/types/vehicles.py` & `google-maps-fleetengine-0.2.0/google/maps/fleetengine_v1/types/vehicles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/PKG-INFO` & `google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-fleetengine
-Version: 0.1.9
+Version: 0.2.0
 Summary: Google Maps Fleetengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-fleetengine
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-fleetengine-0.1.9/google_maps_fleetengine.egg-info/SOURCES.txt` & `google-maps-fleetengine-0.2.0/google_maps_fleetengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-fleetengine-0.1.9/setup.py` & `google-maps-fleetengine-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/tests/__init__.py` & `google-maps-fleetengine-0.2.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/tests/unit/__init__.py` & `google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-fleetengine-0.1.9/tests/unit/gapic/fleetengine_v1/test_trip_service.py` & `google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/test_trip_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1099,15 +1099,16 @@
             view=trips.TripView.SDK,
         )
         response = client.create_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.CreateTripRequest()
+        request = trip_api.CreateTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, trips.Trip)
     assert response.name == "name_value"
     assert response.vehicle_id == "vehicle_id_value"
     assert response.trip_status == trips.TripStatus.NEW
     assert response.trip_type == fleetengine.TripType.SHARED
@@ -1124,20 +1125,165 @@
     client = TripServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_trip), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_trip()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == trip_api.CreateTripRequest()
 
 
+def test_create_trip_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = TripServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = trip_api.CreateTripRequest(
+        parent="parent_value",
+        trip_id="trip_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_trip), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.create_trip(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.CreateTripRequest(
+            parent="parent_value",
+            trip_id="trip_id_value",
+        )
+
+
+def test_create_trip_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = TripServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_trip in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_trip] = mock_rpc
+        request = {}
+        client.create_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_create_trip_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = TripServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_trip), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            trips.Trip(
+                name="name_value",
+                vehicle_id="vehicle_id_value",
+                trip_status=trips.TripStatus.NEW,
+                trip_type=fleetengine.TripType.SHARED,
+                intermediate_destination_index=3187,
+                current_route_segment="current_route_segment_value",
+                number_of_passengers=2135,
+                last_location_snappable=True,
+                view=trips.TripView.SDK,
+            )
+        )
+        response = await client.create_trip()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.CreateTripRequest()
+
+
+@pytest.mark.asyncio
+async def test_create_trip_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = TripServiceAsyncClient(
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
+            client._client._transport.create_trip
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
+            client._client._transport.create_trip
+        ] = mock_object
+
+        request = {}
+        await client.create_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_trip_async(
     transport: str = "grpc_asyncio", request_type=trip_api.CreateTripRequest
 ):
     client = TripServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1164,15 +1310,16 @@
             )
         )
         response = await client.create_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.CreateTripRequest()
+        request = trip_api.CreateTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, trips.Trip)
     assert response.name == "name_value"
     assert response.vehicle_id == "vehicle_id_value"
     assert response.trip_status == trips.TripStatus.NEW
     assert response.trip_type == fleetengine.TripType.SHARED
@@ -1244,15 +1391,16 @@
             view=trips.TripView.SDK,
         )
         response = client.get_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.GetTripRequest()
+        request = trip_api.GetTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, trips.Trip)
     assert response.name == "name_value"
     assert response.vehicle_id == "vehicle_id_value"
     assert response.trip_status == trips.TripStatus.NEW
     assert response.trip_type == fleetengine.TripType.SHARED
@@ -1269,20 +1417,161 @@
     client = TripServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_trip), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_trip()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == trip_api.GetTripRequest()
 
 
+def test_get_trip_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = TripServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = trip_api.GetTripRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_trip), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_trip(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.GetTripRequest(
+            name="name_value",
+        )
+
+
+def test_get_trip_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = TripServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_trip in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_trip] = mock_rpc
+        request = {}
+        client.get_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_trip_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = TripServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_trip), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            trips.Trip(
+                name="name_value",
+                vehicle_id="vehicle_id_value",
+                trip_status=trips.TripStatus.NEW,
+                trip_type=fleetengine.TripType.SHARED,
+                intermediate_destination_index=3187,
+                current_route_segment="current_route_segment_value",
+                number_of_passengers=2135,
+                last_location_snappable=True,
+                view=trips.TripView.SDK,
+            )
+        )
+        response = await client.get_trip()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.GetTripRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_trip_async_use_cached_wrapped_rpc(transport: str = "grpc_asyncio"):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = TripServiceAsyncClient(
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
+            client._client._transport.get_trip
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
+            client._client._transport.get_trip
+        ] = mock_object
+
+        request = {}
+        await client.get_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_trip_async(
     transport: str = "grpc_asyncio", request_type=trip_api.GetTripRequest
 ):
     client = TripServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1309,15 +1598,16 @@
             )
         )
         response = await client.get_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.GetTripRequest()
+        request = trip_api.GetTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, trips.Trip)
     assert response.name == "name_value"
     assert response.vehicle_id == "vehicle_id_value"
     assert response.trip_status == trips.TripStatus.NEW
     assert response.trip_type == fleetengine.TripType.SHARED
@@ -1381,15 +1671,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.report_billable_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.ReportBillableTripRequest()
+        request = trip_api.ReportBillableTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_report_billable_trip_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1399,20 +1690,161 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.report_billable_trip), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.report_billable_trip()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == trip_api.ReportBillableTripRequest()
 
 
+def test_report_billable_trip_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = TripServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = trip_api.ReportBillableTripRequest(
+        name="name_value",
+        country_code="country_code_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.report_billable_trip), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.report_billable_trip(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.ReportBillableTripRequest(
+            name="name_value",
+            country_code="country_code_value",
+        )
+
+
+def test_report_billable_trip_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = TripServiceClient(
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
+            client._transport.report_billable_trip in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.report_billable_trip
+        ] = mock_rpc
+        request = {}
+        client.report_billable_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.report_billable_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_report_billable_trip_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = TripServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.report_billable_trip), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.report_billable_trip()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.ReportBillableTripRequest()
+
+
+@pytest.mark.asyncio
+async def test_report_billable_trip_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = TripServiceAsyncClient(
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
+            client._client._transport.report_billable_trip
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
+            client._client._transport.report_billable_trip
+        ] = mock_object
+
+        request = {}
+        await client.report_billable_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.report_billable_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_report_billable_trip_async(
     transport: str = "grpc_asyncio", request_type=trip_api.ReportBillableTripRequest
 ):
     client = TripServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1429,15 +1861,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.report_billable_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.ReportBillableTripRequest()
+        request = trip_api.ReportBillableTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_report_billable_trip_async_from_dict():
@@ -1494,15 +1927,16 @@
             next_page_token="next_page_token_value",
         )
         response = client.search_trips(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.SearchTripsRequest()
+        request = trip_api.SearchTripsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchTripsPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_search_trips_empty_call():
@@ -1511,20 +1945,159 @@
     client = TripServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search_trips), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.search_trips()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == trip_api.SearchTripsRequest()
 
 
+def test_search_trips_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = TripServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = trip_api.SearchTripsRequest(
+        parent="parent_value",
+        vehicle_id="vehicle_id_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.search_trips), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.search_trips(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.SearchTripsRequest(
+            parent="parent_value",
+            vehicle_id="vehicle_id_value",
+            page_token="page_token_value",
+        )
+
+
+def test_search_trips_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = TripServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.search_trips in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.search_trips] = mock_rpc
+        request = {}
+        client.search_trips(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.search_trips(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_search_trips_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = TripServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.search_trips), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            trip_api.SearchTripsResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.search_trips()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.SearchTripsRequest()
+
+
+@pytest.mark.asyncio
+async def test_search_trips_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = TripServiceAsyncClient(
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
+            client._client._transport.search_trips
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
+            client._client._transport.search_trips
+        ] = mock_object
+
+        request = {}
+        await client.search_trips(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.search_trips(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_search_trips_async(
     transport: str = "grpc_asyncio", request_type=trip_api.SearchTripsRequest
 ):
     client = TripServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1543,15 +2116,16 @@
             )
         )
         response = await client.search_trips(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.SearchTripsRequest()
+        request = trip_api.SearchTripsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.SearchTripsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
@@ -1802,15 +2376,16 @@
             view=trips.TripView.SDK,
         )
         response = client.update_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.UpdateTripRequest()
+        request = trip_api.UpdateTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, trips.Trip)
     assert response.name == "name_value"
     assert response.vehicle_id == "vehicle_id_value"
     assert response.trip_status == trips.TripStatus.NEW
     assert response.trip_type == fleetengine.TripType.SHARED
@@ -1827,20 +2402,163 @@
     client = TripServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_trip), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_trip()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == trip_api.UpdateTripRequest()
 
 
+def test_update_trip_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = TripServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = trip_api.UpdateTripRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_trip), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_trip(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.UpdateTripRequest(
+            name="name_value",
+        )
+
+
+def test_update_trip_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = TripServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_trip in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_trip] = mock_rpc
+        request = {}
+        client.update_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_trip_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = TripServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_trip), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            trips.Trip(
+                name="name_value",
+                vehicle_id="vehicle_id_value",
+                trip_status=trips.TripStatus.NEW,
+                trip_type=fleetengine.TripType.SHARED,
+                intermediate_destination_index=3187,
+                current_route_segment="current_route_segment_value",
+                number_of_passengers=2135,
+                last_location_snappable=True,
+                view=trips.TripView.SDK,
+            )
+        )
+        response = await client.update_trip()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == trip_api.UpdateTripRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_trip_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = TripServiceAsyncClient(
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
+            client._client._transport.update_trip
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
+            client._client._transport.update_trip
+        ] = mock_object
+
+        request = {}
+        await client.update_trip(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_trip(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_trip_async(
     transport: str = "grpc_asyncio", request_type=trip_api.UpdateTripRequest
 ):
     client = TripServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1867,15 +2585,16 @@
             )
         )
         response = await client.update_trip(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == trip_api.UpdateTripRequest()
+        request = trip_api.UpdateTripRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, trips.Trip)
     assert response.name == "name_value"
     assert response.vehicle_id == "vehicle_id_value"
     assert response.trip_status == trips.TripStatus.NEW
     assert response.trip_type == fleetengine.TripType.SHARED
```

### Comparing `google-maps-fleetengine-0.1.9/tests/unit/gapic/fleetengine_v1/test_vehicle_service.py` & `google-maps-fleetengine-0.2.0/tests/unit/gapic/fleetengine_v1/test_vehicle_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1136,15 +1136,16 @@
             navigation_status=fleetengine.NavigationStatus.NO_GUIDANCE,
         )
         response = client.create_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.CreateVehicleRequest()
+        request = vehicle_api.CreateVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicles.Vehicle)
     assert response.name == "name_value"
     assert response.vehicle_state == vehicles.VehicleState.OFFLINE
     assert response.supported_trip_types == [fleetengine.TripType.SHARED]
     assert response.current_trips == ["current_trips_value"]
@@ -1160,20 +1161,164 @@
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_vehicle), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.CreateVehicleRequest()
 
 
+def test_create_vehicle_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = VehicleServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = vehicle_api.CreateVehicleRequest(
+        parent="parent_value",
+        vehicle_id="vehicle_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_vehicle), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.create_vehicle(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.CreateVehicleRequest(
+            parent="parent_value",
+            vehicle_id="vehicle_id_value",
+        )
+
+
+def test_create_vehicle_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = VehicleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_vehicle in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_vehicle] = mock_rpc
+        request = {}
+        client.create_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_create_vehicle_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VehicleServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_vehicle), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vehicles.Vehicle(
+                name="name_value",
+                vehicle_state=vehicles.VehicleState.OFFLINE,
+                supported_trip_types=[fleetengine.TripType.SHARED],
+                current_trips=["current_trips_value"],
+                maximum_capacity=1707,
+                current_route_segment="current_route_segment_value",
+                back_to_back_enabled=True,
+                navigation_status=fleetengine.NavigationStatus.NO_GUIDANCE,
+            )
+        )
+        response = await client.create_vehicle()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.CreateVehicleRequest()
+
+
+@pytest.mark.asyncio
+async def test_create_vehicle_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = VehicleServiceAsyncClient(
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
+            client._client._transport.create_vehicle
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
+            client._client._transport.create_vehicle
+        ] = mock_object
+
+        request = {}
+        await client.create_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_vehicle_async(
     transport: str = "grpc_asyncio", request_type=vehicle_api.CreateVehicleRequest
 ):
     client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1199,15 +1344,16 @@
             )
         )
         response = await client.create_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.CreateVehicleRequest()
+        request = vehicle_api.CreateVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicles.Vehicle)
     assert response.name == "name_value"
     assert response.vehicle_state == vehicles.VehicleState.OFFLINE
     assert response.supported_trip_types == [fleetengine.TripType.SHARED]
     assert response.current_trips == ["current_trips_value"]
@@ -1277,15 +1423,16 @@
             navigation_status=fleetengine.NavigationStatus.NO_GUIDANCE,
         )
         response = client.get_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.GetVehicleRequest()
+        request = vehicle_api.GetVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicles.Vehicle)
     assert response.name == "name_value"
     assert response.vehicle_state == vehicles.VehicleState.OFFLINE
     assert response.supported_trip_types == [fleetengine.TripType.SHARED]
     assert response.current_trips == ["current_trips_value"]
@@ -1301,20 +1448,162 @@
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_vehicle), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.GetVehicleRequest()
 
 
+def test_get_vehicle_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = VehicleServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = vehicle_api.GetVehicleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_vehicle), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_vehicle(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.GetVehicleRequest(
+            name="name_value",
+        )
+
+
+def test_get_vehicle_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = VehicleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_vehicle in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_vehicle] = mock_rpc
+        request = {}
+        client.get_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_vehicle_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VehicleServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_vehicle), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vehicles.Vehicle(
+                name="name_value",
+                vehicle_state=vehicles.VehicleState.OFFLINE,
+                supported_trip_types=[fleetengine.TripType.SHARED],
+                current_trips=["current_trips_value"],
+                maximum_capacity=1707,
+                current_route_segment="current_route_segment_value",
+                back_to_back_enabled=True,
+                navigation_status=fleetengine.NavigationStatus.NO_GUIDANCE,
+            )
+        )
+        response = await client.get_vehicle()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.GetVehicleRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_vehicle_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = VehicleServiceAsyncClient(
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
+            client._client._transport.get_vehicle
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
+            client._client._transport.get_vehicle
+        ] = mock_object
+
+        request = {}
+        await client.get_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_vehicle_async(
     transport: str = "grpc_asyncio", request_type=vehicle_api.GetVehicleRequest
 ):
     client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1340,15 +1629,16 @@
             )
         )
         response = await client.get_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.GetVehicleRequest()
+        request = vehicle_api.GetVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicles.Vehicle)
     assert response.name == "name_value"
     assert response.vehicle_state == vehicles.VehicleState.OFFLINE
     assert response.supported_trip_types == [fleetengine.TripType.SHARED]
     assert response.current_trips == ["current_trips_value"]
@@ -1418,15 +1708,16 @@
             navigation_status=fleetengine.NavigationStatus.NO_GUIDANCE,
         )
         response = client.update_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleRequest()
+        request = vehicle_api.UpdateVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicles.Vehicle)
     assert response.name == "name_value"
     assert response.vehicle_state == vehicles.VehicleState.OFFLINE
     assert response.supported_trip_types == [fleetengine.TripType.SHARED]
     assert response.current_trips == ["current_trips_value"]
@@ -1442,20 +1733,162 @@
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_vehicle), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_vehicle()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.UpdateVehicleRequest()
 
 
+def test_update_vehicle_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = VehicleServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = vehicle_api.UpdateVehicleRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_vehicle), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_vehicle(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.UpdateVehicleRequest(
+            name="name_value",
+        )
+
+
+def test_update_vehicle_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = VehicleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.update_vehicle in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.update_vehicle] = mock_rpc
+        request = {}
+        client.update_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_vehicle_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VehicleServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_vehicle), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vehicles.Vehicle(
+                name="name_value",
+                vehicle_state=vehicles.VehicleState.OFFLINE,
+                supported_trip_types=[fleetengine.TripType.SHARED],
+                current_trips=["current_trips_value"],
+                maximum_capacity=1707,
+                current_route_segment="current_route_segment_value",
+                back_to_back_enabled=True,
+                navigation_status=fleetengine.NavigationStatus.NO_GUIDANCE,
+            )
+        )
+        response = await client.update_vehicle()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.UpdateVehicleRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_vehicle_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = VehicleServiceAsyncClient(
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
+            client._client._transport.update_vehicle
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
+            client._client._transport.update_vehicle
+        ] = mock_object
+
+        request = {}
+        await client.update_vehicle(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_vehicle(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_vehicle_async(
     transport: str = "grpc_asyncio", request_type=vehicle_api.UpdateVehicleRequest
 ):
     client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1481,15 +1914,16 @@
             )
         )
         response = await client.update_vehicle(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleRequest()
+        request = vehicle_api.UpdateVehicleRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicles.Vehicle)
     assert response.name == "name_value"
     assert response.vehicle_state == vehicles.VehicleState.OFFLINE
     assert response.supported_trip_types == [fleetengine.TripType.SHARED]
     assert response.current_trips == ["current_trips_value"]
@@ -1527,195 +1961,204 @@
     # This test doesn't assert anything useful.
     assert kw["metadata"]
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
-        vehicle_api.UpdateVehicleLocationRequest,
+        vehicle_api.UpdateVehicleAttributesRequest,
         dict,
     ],
 )
-def test_update_vehicle_location(request_type, transport: str = "grpc"):
+def test_update_vehicle_attributes(request_type, transport: str = "grpc"):
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
-        type(client.transport.update_vehicle_location), "__call__"
+        type(client.transport.update_vehicle_attributes), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
-        call.return_value = fleetengine.VehicleLocation(
-            location_sensor=fleetengine.LocationSensor.GPS,
-            raw_location_sensor=fleetengine.LocationSensor.GPS,
-            supplemental_location_sensor=fleetengine.LocationSensor.GPS,
-            road_snapped=True,
-        )
-        response = client.update_vehicle_location(request)
+        call.return_value = vehicle_api.UpdateVehicleAttributesResponse()
+        response = client.update_vehicle_attributes(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleLocationRequest()
+        request = vehicle_api.UpdateVehicleAttributesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
-    assert isinstance(response, fleetengine.VehicleLocation)
-    assert response.location_sensor == fleetengine.LocationSensor.GPS
-    assert response.raw_location_sensor == fleetengine.LocationSensor.GPS
-    assert response.supplemental_location_sensor == fleetengine.LocationSensor.GPS
-    assert response.road_snapped is True
+    assert isinstance(response, vehicle_api.UpdateVehicleAttributesResponse)
 
 
-def test_update_vehicle_location_empty_call():
+def test_update_vehicle_attributes_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
-        type(client.transport.update_vehicle_location), "__call__"
+        type(client.transport.update_vehicle_attributes), "__call__"
     ) as call:
-        client.update_vehicle_location()
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_vehicle_attributes()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleLocationRequest()
+        assert args[0] == vehicle_api.UpdateVehicleAttributesRequest()
 
 
-@pytest.mark.asyncio
-async def test_update_vehicle_location_async(
-    transport: str = "grpc_asyncio",
-    request_type=vehicle_api.UpdateVehicleLocationRequest,
-):
-    client = VehicleServiceAsyncClient(
+def test_update_vehicle_attributes_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
+        transport="grpc",
     )
 
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = request_type()
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = vehicle_api.UpdateVehicleAttributesRequest(
+        name="name_value",
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
-        type(client.transport.update_vehicle_location), "__call__"
+        type(client.transport.update_vehicle_attributes), "__call__"
     ) as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            fleetengine.VehicleLocation(
-                location_sensor=fleetengine.LocationSensor.GPS,
-                raw_location_sensor=fleetengine.LocationSensor.GPS,
-                supplemental_location_sensor=fleetengine.LocationSensor.GPS,
-                road_snapped=True,
-            )
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
         )
-        response = await client.update_vehicle_location(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls)
+        client.update_vehicle_attributes(request=request)
+        call.assert_called()
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleLocationRequest()
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, fleetengine.VehicleLocation)
-    assert response.location_sensor == fleetengine.LocationSensor.GPS
-    assert response.raw_location_sensor == fleetengine.LocationSensor.GPS
-    assert response.supplemental_location_sensor == fleetengine.LocationSensor.GPS
-    assert response.road_snapped is True
-
+        assert args[0] == vehicle_api.UpdateVehicleAttributesRequest(
+            name="name_value",
+        )
 
-@pytest.mark.asyncio
-async def test_update_vehicle_location_async_from_dict():
-    await test_update_vehicle_location_async(request_type=dict)
 
+def test_update_vehicle_attributes_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = VehicleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
 
-def test_update_vehicle_location_routing_parameters():
-    client = VehicleServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
 
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = vehicle_api.UpdateVehicleLocationRequest(**{"name": "providers/sample1"})
+        # Ensure method has been cached
+        assert (
+            client._transport.update_vehicle_attributes
+            in client._transport._wrapped_methods
+        )
 
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.update_vehicle_location), "__call__"
-    ) as call:
-        call.return_value = fleetengine.VehicleLocation()
-        client.update_vehicle_location(request)
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_vehicle_attributes
+        ] = mock_rpc
+        request = {}
+        client.update_vehicle_attributes(request)
 
         # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
+        assert mock_rpc.call_count == 1
 
-    _, _, kw = call.mock_calls[0]
-    # This test doesn't assert anything useful.
-    assert kw["metadata"]
+        client.update_vehicle_attributes(request)
 
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
 
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        vehicle_api.UpdateVehicleAttributesRequest,
-        dict,
-    ],
-)
-def test_update_vehicle_attributes(request_type, transport: str = "grpc"):
-    client = VehicleServiceClient(
+
+@pytest.mark.asyncio
+async def test_update_vehicle_attributes_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
+        transport="grpc_asyncio",
     )
 
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = request_type()
-
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_vehicle_attributes), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
-        call.return_value = vehicle_api.UpdateVehicleAttributesResponse()
-        response = client.update_vehicle_attributes(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vehicle_api.UpdateVehicleAttributesResponse()
+        )
+        response = await client.update_vehicle_attributes()
+        call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.UpdateVehicleAttributesRequest()
 
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, vehicle_api.UpdateVehicleAttributesResponse)
 
+@pytest.mark.asyncio
+async def test_update_vehicle_attributes_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = VehicleServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
 
-def test_update_vehicle_attributes_empty_call():
-    # This test is a coverage failsafe to make sure that totally empty calls,
-    # i.e. request == None and no flattened fields passed, work.
-    client = VehicleServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="grpc",
-    )
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
 
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.update_vehicle_attributes), "__call__"
-    ) as call:
-        client.update_vehicle_attributes()
-        call.assert_called()
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleAttributesRequest()
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_vehicle_attributes
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
+            client._client._transport.update_vehicle_attributes
+        ] = mock_object
+
+        request = {}
+        await client.update_vehicle_attributes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_vehicle_attributes(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
 
 
 @pytest.mark.asyncio
 async def test_update_vehicle_attributes_async(
     transport: str = "grpc_asyncio",
     request_type=vehicle_api.UpdateVehicleAttributesRequest,
 ):
@@ -1737,15 +2180,16 @@
             vehicle_api.UpdateVehicleAttributesResponse()
         )
         response = await client.update_vehicle_attributes(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.UpdateVehicleAttributesRequest()
+        request = vehicle_api.UpdateVehicleAttributesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicle_api.UpdateVehicleAttributesResponse)
 
 
 @pytest.mark.asyncio
 async def test_update_vehicle_attributes_async_from_dict():
@@ -1805,15 +2249,16 @@
             total_size=1086,
         )
         response = client.list_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.ListVehiclesRequest()
+        request = vehicle_api.ListVehiclesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListVehiclesPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -1823,20 +2268,160 @@
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_vehicles), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_vehicles()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.ListVehiclesRequest()
 
 
+def test_list_vehicles_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = VehicleServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = vehicle_api.ListVehiclesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_vehicles), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_vehicles(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.ListVehiclesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+        )
+
+
+def test_list_vehicles_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = VehicleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_vehicles in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_vehicles] = mock_rpc
+        request = {}
+        client.list_vehicles(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_vehicles(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_vehicles_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VehicleServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_vehicles), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vehicle_api.ListVehiclesResponse(
+                next_page_token="next_page_token_value",
+                total_size=1086,
+            )
+        )
+        response = await client.list_vehicles()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vehicle_api.ListVehiclesRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_vehicles_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = VehicleServiceAsyncClient(
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
+            client._client._transport.list_vehicles
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
+            client._client._transport.list_vehicles
+        ] = mock_object
+
+        request = {}
+        await client.list_vehicles(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_vehicles(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_vehicles_async(
     transport: str = "grpc_asyncio", request_type=vehicle_api.ListVehiclesRequest
 ):
     client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1856,15 +2441,16 @@
             )
         )
         response = await client.list_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.ListVehiclesRequest()
+        request = vehicle_api.ListVehiclesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListVehiclesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -2106,15 +2692,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = vehicle_api.SearchVehiclesResponse()
         response = client.search_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.SearchVehiclesRequest()
+        request = vehicle_api.SearchVehiclesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicle_api.SearchVehiclesResponse)
 
 
 def test_search_vehicles_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -2122,183 +2709,206 @@
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search_vehicles), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.search_vehicles()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.SearchVehiclesRequest()
 
 
-@pytest.mark.asyncio
-async def test_search_vehicles_async(
-    transport: str = "grpc_asyncio", request_type=vehicle_api.SearchVehiclesRequest
-):
-    client = VehicleServiceAsyncClient(
+def test_search_vehicles_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
+        transport="grpc",
     )
 
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = request_type()
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = vehicle_api.SearchVehiclesRequest(
+        parent="parent_value",
+        trip_id="trip_id_value",
+        filter="filter_value",
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.search_vehicles), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            vehicle_api.SearchVehiclesResponse()
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
         )
-        response = await client.search_vehicles(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls)
+        client.search_vehicles(request=request)
+        call.assert_called()
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.SearchVehiclesRequest()
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, vehicle_api.SearchVehiclesResponse)
+        assert args[0] == vehicle_api.SearchVehiclesRequest(
+            parent="parent_value",
+            trip_id="trip_id_value",
+            filter="filter_value",
+        )
 
 
-@pytest.mark.asyncio
-async def test_search_vehicles_async_from_dict():
-    await test_search_vehicles_async(request_type=dict)
+def test_search_vehicles_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = VehicleServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
 
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
 
-def test_search_vehicles_routing_parameters():
-    client = VehicleServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
+        # Ensure method has been cached
+        assert client._transport.search_vehicles in client._transport._wrapped_methods
 
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = vehicle_api.SearchVehiclesRequest(**{"parent": "providers/sample1"})
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.search_vehicles), "__call__") as call:
-        call.return_value = vehicle_api.SearchVehiclesResponse()
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.search_vehicles] = mock_rpc
+        request = {}
         client.search_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
+        assert mock_rpc.call_count == 1
 
-    _, _, kw = call.mock_calls[0]
-    # This test doesn't assert anything useful.
-    assert kw["metadata"]
+        client.search_vehicles(request)
 
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
 
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        vehicle_api.SearchVehiclesRequest,
-        dict,
-    ],
-)
-def test_search_fuzzed_vehicles(request_type, transport: str = "grpc"):
-    client = VehicleServiceClient(
+
+@pytest.mark.asyncio
+async def test_search_vehicles_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
+        transport="grpc_asyncio",
     )
 
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = request_type()
-
     # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.search_fuzzed_vehicles), "__call__"
-    ) as call:
+    with mock.patch.object(type(client.transport.search_vehicles), "__call__") as call:
         # Designate an appropriate return value for the call.
-        call.return_value = vehicle_api.SearchVehiclesResponse()
-        response = client.search_fuzzed_vehicles(request)
-
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vehicle_api.SearchVehiclesResponse()
+        )
+        response = await client.search_vehicles()
+        call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == vehicle_api.SearchVehiclesRequest()
 
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, vehicle_api.SearchVehiclesResponse)
 
+@pytest.mark.asyncio
+async def test_search_vehicles_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = VehicleServiceAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
 
-def test_search_fuzzed_vehicles_empty_call():
-    # This test is a coverage failsafe to make sure that totally empty calls,
-    # i.e. request == None and no flattened fields passed, work.
-    client = VehicleServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="grpc",
-    )
+        # Ensure method has been cached
+        assert (
+            client._client._transport.search_vehicles
+            in client._client._transport._wrapped_methods
+        )
 
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.search_fuzzed_vehicles), "__call__"
-    ) as call:
-        client.search_fuzzed_vehicles()
-        call.assert_called()
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.SearchVehiclesRequest()
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.search_vehicles
+        ] = mock_object
+
+        request = {}
+        await client.search_vehicles(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.search_vehicles(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
 
 
 @pytest.mark.asyncio
-async def test_search_fuzzed_vehicles_async(
+async def test_search_vehicles_async(
     transport: str = "grpc_asyncio", request_type=vehicle_api.SearchVehiclesRequest
 ):
     client = VehicleServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.search_fuzzed_vehicles), "__call__"
-    ) as call:
+    with mock.patch.object(type(client.transport.search_vehicles), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             vehicle_api.SearchVehiclesResponse()
         )
-        response = await client.search_fuzzed_vehicles(request)
+        response = await client.search_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == vehicle_api.SearchVehiclesRequest()
+        request = vehicle_api.SearchVehiclesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vehicle_api.SearchVehiclesResponse)
 
 
 @pytest.mark.asyncio
-async def test_search_fuzzed_vehicles_async_from_dict():
-    await test_search_fuzzed_vehicles_async(request_type=dict)
+async def test_search_vehicles_async_from_dict():
+    await test_search_vehicles_async(request_type=dict)
 
 
-def test_search_fuzzed_vehicles_routing_parameters():
+def test_search_vehicles_routing_parameters():
     client = VehicleServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = vehicle_api.SearchVehiclesRequest(**{"parent": "providers/sample1"})
 
     # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(
-        type(client.transport.search_fuzzed_vehicles), "__call__"
-    ) as call:
+    with mock.patch.object(type(client.transport.search_vehicles), "__call__") as call:
         call.return_value = vehicle_api.SearchVehiclesResponse()
-        client.search_fuzzed_vehicles(request)
+        client.search_vehicles(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     _, _, kw = call.mock_calls[0]
@@ -2442,19 +3052,17 @@
 
     # Every method on the transport should just blindly
     # raise NotImplementedError.
     methods = (
         "create_vehicle",
         "get_vehicle",
         "update_vehicle",
-        "update_vehicle_location",
         "update_vehicle_attributes",
         "list_vehicles",
         "search_vehicles",
-        "search_fuzzed_vehicles",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
```

