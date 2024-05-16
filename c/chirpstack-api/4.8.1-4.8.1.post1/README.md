# Comparing `tmp/chirpstack-api-4.8.1.tar.gz` & `tmp/chirpstack-api-4.8.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chirpstack-api-4.8.1.tar", last modified: Mon May 13 15:50:16 2024, max compression
+gzip compressed data, was "chirpstack-api-4.8.1.post1.tar", last modified: Thu May 16 10:54:14 2024, max compression
```

## Comparing `chirpstack-api-4.8.1.tar` & `chirpstack-api-4.8.1.post1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.731240 chirpstack-api-4.8.1/
--rw-r--r--   0 brocaar   (1000) users      (100)     1312 2024-05-13 15:50:16.730239 chirpstack-api-4.8.1/PKG-INFO
--rw-r--r--   0 brocaar   (1000) users      (100)      737 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1/README.md
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.712239 chirpstack-api-4.8.1/chirpstack_api/
--rw-r--r--   0 brocaar   (1000) users      (100)        0 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1/chirpstack_api/__init__.py
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.723240 chirpstack-api-4.8.1/chirpstack_api/api/
--rw-r--r--   0 brocaar   (1000) users      (100)      711 2024-03-25 10:51:04.000000 chirpstack-api-4.8.1/chirpstack_api/api/__init__.py
--rw-r--r--   0 brocaar   (1000) users      (100)    47688 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/application_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    94641 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/application_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)    22151 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/device_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    39252 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/device_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)    12860 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/device_profile_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    13523 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/device_profile_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)     9540 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/device_profile_template_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    12097 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/device_profile_template_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)    11582 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/gateway_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    17149 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/gateway_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)    13149 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/internal_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    33768 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/internal_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)    13404 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/multicast_group_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    25045 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/multicast_group_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)     5178 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/relay_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     9390 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/relay_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)    11306 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/tenant_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    20068 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/tenant_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)     6677 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/user_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)    12649 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/api/user_pb2_grpc.py
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.724239 chirpstack-api-4.8.1/chirpstack_api/common/
--rw-r--r--   0 brocaar   (1000) users      (100)       26 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1/chirpstack_api/common/__init__.py
--rw-r--r--   0 brocaar   (1000) users      (100)     5684 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/common/common_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1145 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/common/common_pb2_grpc.py
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.725240 chirpstack-api-4.8.1/chirpstack_api/gw/
--rw-r--r--   0 brocaar   (1000) users      (100)       22 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1/chirpstack_api/gw/__init__.py
--rw-r--r--   0 brocaar   (1000) users      (100)    20943 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/gw/gw_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1137 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/gw/gw_pb2_grpc.py
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.726240 chirpstack-api-4.8.1/chirpstack_api/integration/
--rw-r--r--   0 brocaar   (1000) users      (100)       31 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1/chirpstack_api/integration/__init__.py
--rw-r--r--   0 brocaar   (1000) users      (100)     8943 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/integration/integration_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1155 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/integration/integration_pb2_grpc.py
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.730239 chirpstack-api-4.8.1/chirpstack_api/stream/
--rw-r--r--   0 brocaar   (1000) users      (100)      118 2024-03-25 10:51:04.000000 chirpstack-api-4.8.1/chirpstack_api/stream/__init__.py
--rw-r--r--   0 brocaar   (1000) users      (100)     2315 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/stream/api_request_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1150 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/stream/api_request_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)     2024 2024-05-13 15:35:24.000000 chirpstack-api-4.8.1/chirpstack_api/stream/backend_interfaces_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1157 2024-05-13 15:35:24.000000 chirpstack-api-4.8.1/chirpstack_api/stream/backend_interfaces_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)     2871 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/stream/frame_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1144 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/stream/frame_pb2_grpc.py
--rw-r--r--   0 brocaar   (1000) users      (100)     2548 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/stream/meta_pb2.py
--rw-r--r--   0 brocaar   (1000) users      (100)     1143 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1/chirpstack_api/stream/meta_pb2_grpc.py
-drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-13 15:50:16.713240 chirpstack-api-4.8.1/chirpstack_api.egg-info/
--rw-r--r--   0 brocaar   (1000) users      (100)     1312 2024-05-13 15:50:16.000000 chirpstack-api-4.8.1/chirpstack_api.egg-info/PKG-INFO
--rw-r--r--   0 brocaar   (1000) users      (100)     1798 2024-05-13 15:50:16.000000 chirpstack-api-4.8.1/chirpstack_api.egg-info/SOURCES.txt
--rw-r--r--   0 brocaar   (1000) users      (100)        1 2024-05-13 15:50:16.000000 chirpstack-api-4.8.1/chirpstack_api.egg-info/dependency_links.txt
--rw-r--r--   0 brocaar   (1000) users      (100)        1 2024-05-13 15:50:16.000000 chirpstack-api-4.8.1/chirpstack_api.egg-info/not-zip-safe
--rw-r--r--   0 brocaar   (1000) users      (100)       23 2024-05-13 15:50:16.000000 chirpstack-api-4.8.1/chirpstack_api.egg-info/requires.txt
--rw-r--r--   0 brocaar   (1000) users      (100)       15 2024-05-13 15:50:16.000000 chirpstack-api-4.8.1/chirpstack_api.egg-info/top_level.txt
--rw-r--r--   0 brocaar   (1000) users      (100)       38 2024-05-13 15:50:16.731240 chirpstack-api-4.8.1/setup.cfg
--rw-r--r--   0 brocaar   (1000) users      (100)      868 2024-05-13 15:34:55.000000 chirpstack-api-4.8.1/setup.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.697800 chirpstack-api-4.8.1.post1/
+-rw-r--r--   0 brocaar   (1000) users      (100)     1318 2024-05-16 10:54:14.697800 chirpstack-api-4.8.1.post1/PKG-INFO
+-rw-r--r--   0 brocaar   (1000) users      (100)      737 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1.post1/README.md
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.674799 chirpstack-api-4.8.1.post1/chirpstack_api/
+-rw-r--r--   0 brocaar   (1000) users      (100)        0 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1.post1/chirpstack_api/__init__.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.687800 chirpstack-api-4.8.1.post1/chirpstack_api/api/
+-rw-r--r--   0 brocaar   (1000) users      (100)      648 2024-05-16 10:50:26.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/__init__.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    47688 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/application_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    94641 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/application_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    22151 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/device_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    39252 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/device_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    12860 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    13523 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     9540 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_template_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    12097 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_template_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    11582 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/gateway_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    17149 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/gateway_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    13149 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/internal_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    33768 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/internal_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    13404 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/multicast_group_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    25045 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/multicast_group_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     5178 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/relay_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     9390 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/relay_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    11306 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/tenant_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    20068 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/tenant_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     6677 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/user_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    12649 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/api/user_pb2_grpc.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.688799 chirpstack-api-4.8.1.post1/chirpstack_api/common/
+-rw-r--r--   0 brocaar   (1000) users      (100)       26 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1.post1/chirpstack_api/common/__init__.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     5684 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/common/common_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1145 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/common/common_pb2_grpc.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.690800 chirpstack-api-4.8.1.post1/chirpstack_api/gw/
+-rw-r--r--   0 brocaar   (1000) users      (100)       22 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1.post1/chirpstack_api/gw/__init__.py
+-rw-r--r--   0 brocaar   (1000) users      (100)    20943 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/gw/gw_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1137 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/gw/gw_pb2_grpc.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.691799 chirpstack-api-4.8.1.post1/chirpstack_api/integration/
+-rw-r--r--   0 brocaar   (1000) users      (100)       31 2024-02-22 12:45:56.000000 chirpstack-api-4.8.1.post1/chirpstack_api/integration/__init__.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     8943 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/integration/integration_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1155 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/integration/integration_pb2_grpc.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.696800 chirpstack-api-4.8.1.post1/chirpstack_api/stream/
+-rw-r--r--   0 brocaar   (1000) users      (100)      118 2024-03-25 10:51:04.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/__init__.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     2315 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/api_request_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1150 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/api_request_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     2024 2024-05-13 15:35:24.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/backend_interfaces_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1157 2024-05-13 15:35:24.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/backend_interfaces_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     2871 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/frame_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1144 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/frame_pb2_grpc.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     2548 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/meta_pb2.py
+-rw-r--r--   0 brocaar   (1000) users      (100)     1143 2024-05-13 15:35:23.000000 chirpstack-api-4.8.1.post1/chirpstack_api/stream/meta_pb2_grpc.py
+drwxr-xr-x   0 brocaar   (1000) users      (100)        0 2024-05-16 10:54:14.676799 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/
+-rw-r--r--   0 brocaar   (1000) users      (100)     1318 2024-05-16 10:54:14.000000 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/PKG-INFO
+-rw-r--r--   0 brocaar   (1000) users      (100)     1798 2024-05-16 10:54:14.000000 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/SOURCES.txt
+-rw-r--r--   0 brocaar   (1000) users      (100)        1 2024-05-16 10:54:14.000000 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/dependency_links.txt
+-rw-r--r--   0 brocaar   (1000) users      (100)        1 2024-05-16 10:54:14.000000 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/not-zip-safe
+-rw-r--r--   0 brocaar   (1000) users      (100)       23 2024-05-16 10:54:14.000000 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/requires.txt
+-rw-r--r--   0 brocaar   (1000) users      (100)       15 2024-05-16 10:54:14.000000 chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/top_level.txt
+-rw-r--r--   0 brocaar   (1000) users      (100)       38 2024-05-16 10:54:14.697800 chirpstack-api-4.8.1.post1/setup.cfg
+-rw-r--r--   0 brocaar   (1000) users      (100)      874 2024-05-16 10:53:44.000000 chirpstack-api-4.8.1.post1/setup.py
```

### Comparing `chirpstack-api-4.8.1/PKG-INFO` & `chirpstack-api-4.8.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chirpstack-api
-Version: 4.8.1
+Version: 4.8.1.post1
 Summary: Chirpstack Python API
 Home-page: https://github.com/brocaar/chirpstack-api
 Author: Orne Brocaar
 Author-email: info@brocaar.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `chirpstack-api-4.8.1/README.md` & `chirpstack-api-4.8.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/__init__.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from .application_pb2_grpc import *
 from .device_pb2 import *
 from .device_pb2_grpc import *
 from .device_profile_pb2 import *
 from .device_profile_pb2_grpc import *
 from .device_profile_template_pb2 import *
 from .device_profile_template_pb2_grpc import *
-from .frame_log_pb2 import *
-from .frame_log_pb2_grpc import *
 from .gateway_pb2 import *
 from .gateway_pb2_grpc import *
 from .internal_pb2 import *
 from .internal_pb2_grpc import *
 from .multicast_group_pb2 import *
 from .multicast_group_pb2_grpc import *
 from .tenant_pb2 import *
```

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/application_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/application_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/application_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/application_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/device_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/device_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/device_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/device_profile_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/device_profile_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/device_profile_template_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_template_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/device_profile_template_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/device_profile_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/gateway_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/gateway_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/gateway_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/internal_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/internal_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/internal_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/internal_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/multicast_group_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/multicast_group_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/multicast_group_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/multicast_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/relay_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/relay_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/relay_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/relay_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/tenant_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/tenant_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/user_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/user_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/api/user_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/api/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/common/common_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/common/common_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/common/common_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/gw/gw_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/gw/gw_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/gw/gw_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/gw/gw_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/integration/integration_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/integration/integration_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/integration/integration_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/integration/integration_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/api_request_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/api_request_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/api_request_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/api_request_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/backend_interfaces_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/backend_interfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/backend_interfaces_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/backend_interfaces_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/frame_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/frame_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/frame_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/frame_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/meta_pb2.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api/stream/meta_pb2_grpc.py` & `chirpstack-api-4.8.1.post1/chirpstack_api/stream/meta_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/chirpstack_api.egg-info/PKG-INFO` & `chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chirpstack-api
-Version: 4.8.1
+Version: 4.8.1.post1
 Summary: Chirpstack Python API
 Home-page: https://github.com/brocaar/chirpstack-api
 Author: Orne Brocaar
 Author-email: info@brocaar.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `chirpstack-api-4.8.1/chirpstack_api.egg-info/SOURCES.txt` & `chirpstack-api-4.8.1.post1/chirpstack_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chirpstack-api-4.8.1/setup.py` & `chirpstack-api-4.8.1.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'Topic :: Communications',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
 ]
 
 setup(
     name='chirpstack-api',
-    version = "4.8.1",
+    version = "4.8.1.post1",
     url='https://github.com/brocaar/chirpstack-api',
     author='Orne Brocaar',
     author_email='info@brocaar.com',
     license='MIT',
     description='Chirpstack Python API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

