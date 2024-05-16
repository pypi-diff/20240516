# Comparing `tmp/google-cloud-gke-multicloud-0.6.8.tar.gz` & `tmp/google-cloud-gke-multicloud-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-multicloud-0.6.8.tar", last modified: Thu Feb 22 22:38:46 2024, max compression
+gzip compressed data, was "google-cloud-gke-multicloud-0.6.9.tar", last modified: Tue Mar  5 18:55:25 2024, max compression
```

## Comparing `google-cloud-gke-multicloud-0.6.8.tar` & `google-cloud-gke-multicloud-0.6.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.690885 google-cloud-gke-multicloud-0.6.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5313 2024-02-22 22:38:46.690885 google-cloud-gke-multicloud-0.6.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3946 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.670884 google-cloud-gke-multicloud-0.6.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.670884 google-cloud-gke-multicloud-0.6.8/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.674884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud/
--rw-rw-r--   0 root         (0)     1003     9441 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.674884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/
--rw-rw-r--   0 root         (0)     1003     8844 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    19496 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       88 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.674884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.678884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/
--rw-rw-r--   0 root         (0)     1003      777 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py
--rw-rw-r--   0 root         (0)     1003    73200 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py
--rw-rw-r--   0 root         (0)     1003    89970 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py
--rw-rw-r--   0 root         (0)     1003     6153 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.678884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13297 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py
--rw-rw-r--   0 root         (0)     1003    27756 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28229 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    72756 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.678884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/
--rw-rw-r--   0 root         (0)     1003      757 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py
--rw-rw-r--   0 root         (0)     1003   110105 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py
--rw-rw-r--   0 root         (0)     1003   127041 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py
--rw-rw-r--   0 root         (0)     1003    11046 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.682884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17455 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36037 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    36785 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106038 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.682884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/
--rw-rw-r--   0 root         (0)     1003      765 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py
--rw-rw-r--   0 root         (0)     1003   130516 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py
--rw-rw-r--   0 root         (0)     1003   147900 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py
--rw-rw-r--   0 root         (0)     1003    16380 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.682884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19846 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py
--rw-rw-r--   0 root         (0)     1003    40690 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41520 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   123148 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.686884 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/
--rw-rw-r--   0 root         (0)     1003     8237 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    15401 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/attached_resources.py
--rw-rw-r--   0 root         (0)     1003    18179 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/attached_service.py
--rw-rw-r--   0 root         (0)     1003    47494 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/aws_resources.py
--rw-rw-r--   0 root         (0)     1003    27520 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/aws_service.py
--rw-rw-r--   0 root         (0)     1003    47344 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/azure_resources.py
--rw-rw-r--   0 root         (0)     1003    30904 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/azure_service.py
--rw-rw-r--   0 root         (0)     1003    11571 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/common_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.686884 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/
--rw-r--r--   0 root         (0)     1003     5313 2024-02-22 22:38:46.000000 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3398 2024-02-22 22:38:46.000000 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-22 22:38:46.000000 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-22 22:38:46.000000 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      287 2024-02-22 22:38:46.000000 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-02-22 22:38:46.000000 google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2024-02-22 22:38:46.694885 google-cloud-gke-multicloud-0.6.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3053 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.690885 google-cloud-gke-multicloud-0.6.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.690885 google-cloud-gke-multicloud-0.6.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.690885 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:38:46.690885 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   301400 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py
--rw-rw-r--   0 root         (0)     1003   432166 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py
--rw-rw-r--   0 root         (0)     1003   520371 2024-02-22 22:27:48.000000 google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.149818 google-cloud-gke-multicloud-0.6.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5331 2024-03-05 18:55:25.149818 google-cloud-gke-multicloud-0.6.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3946 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.129810 google-cloud-gke-multicloud-0.6.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.129810 google-cloud-gke-multicloud-0.6.9/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.133811 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud/
+-rw-rw-r--   0 root         (0)     1003     9441 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.133811 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/
+-rw-rw-r--   0 root         (0)     1003     8844 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19496 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       88 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.133811 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.137813 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/
+-rw-rw-r--   0 root         (0)     1003      777 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73200 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py
+-rw-rw-r--   0 root         (0)     1003    89970 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py
+-rw-rw-r--   0 root         (0)     1003     6153 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.137813 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13297 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27756 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28229 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    72756 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.137813 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/
+-rw-rw-r--   0 root         (0)     1003      757 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110105 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py
+-rw-rw-r--   0 root         (0)     1003   127041 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py
+-rw-rw-r--   0 root         (0)     1003    11046 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.141815 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17455 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36037 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    36785 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106038 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.141815 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/
+-rw-rw-r--   0 root         (0)     1003      765 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py
+-rw-rw-r--   0 root         (0)     1003   130516 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py
+-rw-rw-r--   0 root         (0)     1003   147900 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py
+-rw-rw-r--   0 root         (0)     1003    16380 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.141815 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19846 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    40690 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41520 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   123148 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.145816 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/
+-rw-rw-r--   0 root         (0)     1003     8237 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15401 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/attached_resources.py
+-rw-rw-r--   0 root         (0)     1003    18179 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/attached_service.py
+-rw-rw-r--   0 root         (0)     1003    47494 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/aws_resources.py
+-rw-rw-r--   0 root         (0)     1003    27520 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/aws_service.py
+-rw-rw-r--   0 root         (0)     1003    47344 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/azure_resources.py
+-rw-rw-r--   0 root         (0)     1003    30904 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/azure_service.py
+-rw-rw-r--   0 root         (0)     1003    11571 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/common_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.145816 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/
+-rw-r--r--   0 root         (0)     1003     5331 2024-03-05 18:55:25.000000 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3398 2024-03-05 18:55:25.000000 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:55:25.000000 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:55:25.000000 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-03-05 18:55:25.000000 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-03-05 18:55:25.000000 google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2024-03-05 18:55:25.149818 google-cloud-gke-multicloud-0.6.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3197 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.145816 google-cloud-gke-multicloud-0.6.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.145816 google-cloud-gke-multicloud-0.6.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.145816 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:55:25.149818 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   301400 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py
+-rw-rw-r--   0 root         (0)     1003   432166 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py
+-rw-rw-r--   0 root         (0)     1003   520371 2024-03-05 18:46:02.000000 google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py
```

### Comparing `google-cloud-gke-multicloud-0.6.8/LICENSE` & `google-cloud-gke-multicloud-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/MANIFEST.in` & `google-cloud-gke-multicloud-0.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/PKG-INFO` & `google-cloud-gke-multicloud-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-multicloud
-Version: 0.6.8
+Version: 0.6.9
 Summary: Google Cloud Gke Multicloud API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-multicloud
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
-Requires-Dist: google-auth<3.0.0dev,>=2.14.1
+Requires-Dist: google-auth!=2.24.0,!=2.25.0,<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
 Python Client for Anthos Multicloud
 ===================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-gke-multicloud-0.6.8/README.rst` & `google-cloud-gke-multicloud-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud/gapic_version.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.8"  # {x-release-please-version}
+__version__ = "0.6.9"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/gapic_metadata.json` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/gapic_version.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.8"  # {x-release-please-version}
+__version__ = "0.6.9"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/attached_clusters/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/aws_clusters/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/services/azure_clusters/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/__init__.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/attached_resources.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/attached_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/attached_service.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/attached_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/aws_resources.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/aws_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/aws_service.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/aws_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/azure_resources.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/azure_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/azure_service.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/azure_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google/cloud/gke_multicloud_v1/types/common_resources.py` & `google-cloud-gke-multicloud-0.6.9/google/cloud/gke_multicloud_v1/types/common_resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/PKG-INFO` & `google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-multicloud
-Version: 0.6.8
+Version: 0.6.9
 Summary: Google Cloud Gke Multicloud API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-multicloud
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
-Requires-Dist: google-auth<3.0.0dev,>=2.14.1
+Requires-Dist: google-auth!=2.24.0,!=2.25.0,<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
 Python Client for Anthos Multicloud
 ===================================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-gke-multicloud-0.6.8/google_cloud_gke_multicloud.egg-info/SOURCES.txt` & `google-cloud-gke-multicloud-0.6.9/google_cloud_gke_multicloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/setup.py` & `google-cloud-gke-multicloud-0.6.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.1, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
-    "google-auth >= 2.14.1, <3.0.0dev",
+    # Exclude incompatible versions of `google-auth`
+    # See https://github.com/googleapis/google-cloud-python/issues/12364
+    "google-auth >= 2.14.1, <3.0.0dev,!=2.24.0,!=2.25.0",
     "proto-plus >= 1.22.3, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 url = "https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-gke-multicloud"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/__init__.py` & `google-cloud-gke-multicloud-0.6.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/unit/__init__.py` & `google-cloud-gke-multicloud-0.6.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/__init__.py` & `google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/__init__.py` & `google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py` & `google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/test_attached_clusters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py` & `google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/test_aws_clusters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-multicloud-0.6.8/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py` & `google-cloud-gke-multicloud-0.6.9/tests/unit/gapic/gke_multicloud_v1/test_azure_clusters.py`

 * *Files identical despite different names*

