# Comparing `tmp/openobd_protocol-0.0.46.tar.gz` & `tmp/openobd_protocol-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.0.46.tar", last modified: Tue May  7 14:32:34 2024, max compression
+gzip compressed data, was "openobd_protocol-0.1.0.tar", last modified: Wed May  8 11:52:32 2024, max compression
```

## Comparing `openobd_protocol-0.0.46.tar` & `openobd_protocol-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.531825 openobd_protocol-0.0.46/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 14:32:34.531825 openobd_protocol-0.0.46/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 14:32:34.531825 openobd_protocol-0.0.46/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.516825 openobd_protocol-0.0.46/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.522825 openobd_protocol-0.0.46/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1359 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.525825 openobd_protocol-0.0.46/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     1978 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2565 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.527825 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     2466 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    10384 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2512 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2494 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.530825 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.530825 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.846830 openobd_protocol-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-05-08 11:52:32.845829 openobd_protocol-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 11:52:32.846830 openobd_protocol-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.826829 openobd_protocol-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.834829 openobd_protocol-0.1.0/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.838829 openobd_protocol-0.1.0/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.841829 openobd_protocol-0.1.0/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.843829 openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-08 11:52:27.000000 openobd_protocol-0.1.0/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 11:52:32.844829 openobd_protocol-0.1.0/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-05-08 11:52:32.000000 openobd_protocol-0.1.0/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-08 11:52:32.000000 openobd_protocol-0.1.0/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 11:52:32.000000 openobd_protocol-0.1.0/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-08 11:52:32.000000 openobd_protocol-0.1.0/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-08 11:52:32.000000 openobd_protocol-0.1.0/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.0.46/LICENSE` & `openobd_protocol-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/PKG-INFO` & `openobd_protocol-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.46
+Version: 0.1.0
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.46/pyproject.toml` & `openobd_protocol-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/BasicResponse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.1.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.1.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.1.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/SessionController/Session_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\'\n\x0cStartSession\x12\x17\n\x0f\x63onnection_uuid\x18\x01 \x01(\t\"\x85\x01\n\x0bSessionInfo\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x16\n\x0esession_status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x18\n\x10session_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"N\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x1a\n\x12\x63lient_credentials\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\"%\n\x0cSessionToken\x12\x15\n\rsession_token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x1f\n\tSessionId\x12\x12\n\nsession_id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\'\n\x0cStartSession\x12\x17\n\x0f\x63onnection_uuid\x18\x01 \x01(\t\"r\n\x0bSessionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x15\n\rgrpc_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"b\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x1a\n\x12\x63lient_credentials\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\x12\x12\n\ncluster_id\x18\x04 \x01(\t\"\x1d\n\x0cSessionToken\x12\r\n\x05token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x17\n\tSessionId\x12\n\n\x02id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.Session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_STARTSESSION']._serialized_start=132
   _globals['_STARTSESSION']._serialized_end=171
-  _globals['_SESSIONINFO']._serialized_start=174
-  _globals['_SESSIONINFO']._serialized_end=307
-  _globals['_AUTHENTICATE']._serialized_start=309
+  _globals['_SESSIONINFO']._serialized_start=173
+  _globals['_SESSIONINFO']._serialized_end=287
+  _globals['_AUTHENTICATE']._serialized_start=289
   _globals['_AUTHENTICATE']._serialized_end=387
   _globals['_SESSIONTOKEN']._serialized_start=389
-  _globals['_SESSIONTOKEN']._serialized_end=426
-  _globals['_SESSIONINFOLIST']._serialized_start=428
-  _globals['_SESSIONINFOLIST']._serialized_end=525
-  _globals['_SESSIONID']._serialized_start=527
-  _globals['_SESSIONID']._serialized_end=558
+  _globals['_SESSIONTOKEN']._serialized_end=418
+  _globals['_SESSIONINFOLIST']._serialized_start=420
+  _globals['_SESSIONINFOLIST']._serialized_end=517
+  _globals['_SESSIONID']._serialized_start=519
+  _globals['_SESSIONID']._serialized_end=542
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/SessionController/Session_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -9,47 +9,49 @@
 class StartSession(_message.Message):
     __slots__ = ("connection_uuid",)
     CONNECTION_UUID_FIELD_NUMBER: _ClassVar[int]
     connection_uuid: str
     def __init__(self, connection_uuid: _Optional[str] = ...) -> None: ...
 
 class SessionInfo(_message.Message):
-    __slots__ = ("session_id", "session_status", "created_at", "session_endpoint", "authentication_token")
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    SESSION_STATUS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ("id", "status", "created_at", "grpc_endpoint", "authentication_token")
+    ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    SESSION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
+    GRPC_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     AUTHENTICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    session_id: str
-    session_status: str
+    id: str
+    status: str
     created_at: str
-    session_endpoint: str
+    grpc_endpoint: str
     authentication_token: str
-    def __init__(self, session_id: _Optional[str] = ..., session_status: _Optional[str] = ..., created_at: _Optional[str] = ..., session_endpoint: _Optional[str] = ..., authentication_token: _Optional[str] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., status: _Optional[str] = ..., created_at: _Optional[str] = ..., grpc_endpoint: _Optional[str] = ..., authentication_token: _Optional[str] = ...) -> None: ...
 
 class Authenticate(_message.Message):
-    __slots__ = ("client_id", "client_credentials", "api_key")
+    __slots__ = ("client_id", "client_credentials", "api_key", "cluster_id")
     CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
     CLIENT_CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
     API_KEY_FIELD_NUMBER: _ClassVar[int]
+    CLUSTER_ID_FIELD_NUMBER: _ClassVar[int]
     client_id: str
     client_credentials: str
     api_key: str
-    def __init__(self, client_id: _Optional[str] = ..., client_credentials: _Optional[str] = ..., api_key: _Optional[str] = ...) -> None: ...
+    cluster_id: str
+    def __init__(self, client_id: _Optional[str] = ..., client_credentials: _Optional[str] = ..., api_key: _Optional[str] = ..., cluster_id: _Optional[str] = ...) -> None: ...
 
 class SessionToken(_message.Message):
-    __slots__ = ("session_token",)
-    SESSION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    session_token: str
-    def __init__(self, session_token: _Optional[str] = ...) -> None: ...
+    __slots__ = ("token",)
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    token: str
+    def __init__(self, token: _Optional[str] = ...) -> None: ...
 
 class SessionInfoList(_message.Message):
     __slots__ = ("sessions",)
     SESSIONS_FIELD_NUMBER: _ClassVar[int]
     sessions: _containers.RepeatedCompositeFieldContainer[SessionInfo]
     def __init__(self, sessions: _Optional[_Iterable[_Union[SessionInfo, _Mapping]]] = ...) -> None: ...
 
 class SessionId(_message.Message):
-    __slots__ = ("session_id",)
-    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    session_id: str
-    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+    __slots__ = ("id",)
+    ID_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    def __init__(self, id: _Optional[str] = ...) -> None: ...
```

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.1.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.1.0/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.46
+Version: 0.1.0
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.46/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.1.0/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

