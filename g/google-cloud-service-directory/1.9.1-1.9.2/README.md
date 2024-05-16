# Comparing `tmp/google-cloud-service-directory-1.9.1.tar.gz` & `tmp/google-cloud-service-directory-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-directory-1.9.1.tar", last modified: Thu Aug  3 19:07:25 2023, max compression
+gzip compressed data, was "google-cloud-service-directory-1.9.2.tar", last modified: Tue Sep 19 16:32:18 2023, max compression
```

## Comparing `google-cloud-service-directory-1.9.1.tar` & `google-cloud-service-directory-1.9.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4751 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3810 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.594971 google-cloud-service-directory-1.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.594971 google-cloud-service-directory-1.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/
--rw-rw-r--   0 root         (0)     1003     2830 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003     2391 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8096 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17303 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27720 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6688 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13705 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13918 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19691 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.602970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   100610 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   113993 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16223 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.602970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14825 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34111 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34839 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   116750 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.602970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4109 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     4601 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     1971 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    22554 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     3634 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2396 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8106 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17361 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27778 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6698 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13728 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13941 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19721 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   101232 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   114615 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16348 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14865 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34203 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34931 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   117717 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4728 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     4608 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     2622 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    23224 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     4453 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/
--rw-r--r--   0 root         (0)     1003     4751 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4919 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3008 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    82594 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   428124 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    82624 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   429655 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.281792 google-cloud-service-directory-1.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4751 2023-09-19 16:32:18.281792 google-cloud-service-directory-1.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3810 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.261783 google-cloud-service-directory-1.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.261783 google-cloud-service-directory-1.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.265785 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory/
+-rw-rw-r--   0 root         (0)     1003     2830 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.265785 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003     2391 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8096 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.265785 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.265785 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17303 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27720 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.265785 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6688 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13705 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13918 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19691 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.269787 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   100610 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   113993 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16223 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.269787 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14825 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34111 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34839 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116750 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.269787 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4109 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4601 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     1971 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    22554 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     3634 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.273789 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2396 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8106 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.273789 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.273789 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17361 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27778 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.273789 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6698 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13728 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13941 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19721 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.273789 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   101232 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   114615 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16348 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.273789 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14865 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34203 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34931 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   117717 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.277790 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4728 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4608 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     2622 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    23224 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     4452 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.277790 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/
+-rw-r--r--   0 root         (0)     1003     4751 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4919 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-09-19 16:32:18.000000 google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-09-19 16:32:18.281792 google-cloud-service-directory-1.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3008 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.277790 google-cloud-service-directory-1.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.277790 google-cloud-service-directory-1.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.277790 google-cloud-service-directory-1.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.277790 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    82594 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   428124 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-09-19 16:32:18.281792 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    82624 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   429655 2023-09-19 16:22:09.000000 google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
```

### Comparing `google-cloud-service-directory-1.9.1/LICENSE` & `google-cloud-service-directory-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/MANIFEST.in` & `google-cloud-service-directory-1.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/PKG-INFO` & `google-cloud-service-directory-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.9.1
+Version: 1.9.2
 Summary: Google Cloud Service Directory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-service-directory-1.9.1/README.rst` & `google-cloud-service-directory-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/gapic_version.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_metadata.json` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_version.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/endpoint.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/endpoint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/lookup_service.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/namespace.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/namespace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/registration_service.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/service.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_metadata.json` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_version.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/__init__.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/endpoint.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/endpoint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/lookup_service.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/namespace.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/namespace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/registration_service.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/service.py` & `google-cloud-service-directory-1.9.2/google/cloud/servicedirectory_v1beta1/types/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,19 +70,18 @@
             Control plane clients should use
             [RegistrationService.ListEndpoints][google.cloud.servicedirectory.v1beta1.RegistrationService.ListEndpoints].
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the service
             was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when the service
-            was last updated. Note:
-
-            endpoints being created/deleted/updated within
-            the service are not considered service updates
-            for the purpose of this timestamp.
+            was last updated. Note: endpoints being
+            created/deleted/updated within the service are
+            not considered service updates for the purpose
+            of this timestamp.
         uid (str):
             Output only. A globally unique identifier (in
             UUID4 format) for this service.
     """
 
     name: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/PKG-INFO` & `google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.9.1
+Version: 1.9.2
 Summary: Google Cloud Service Directory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/SOURCES.txt` & `google-cloud-service-directory-1.9.2/google_cloud_service_directory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/setup.py` & `google-cloud-service-directory-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/__init__.py` & `google-cloud-service-directory-1.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/__init__.py` & `google-cloud-service-directory-1.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/__init__.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_registration_service.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1/test_registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py` & `google-cloud-service-directory-1.9.2/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py`

 * *Files identical despite different names*

