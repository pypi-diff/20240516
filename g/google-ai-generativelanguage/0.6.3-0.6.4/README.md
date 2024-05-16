# Comparing `tmp/google-ai-generativelanguage-0.6.3.tar.gz` & `tmp/google-ai-generativelanguage-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ai-generativelanguage-0.6.3.tar", last modified: Tue May  7 20:43:16 2024, max compression
+gzip compressed data, was "google-ai-generativelanguage-0.6.4.tar", last modified: Thu May 16 20:56:30 2024, max compression
```

## Comparing `google-ai-generativelanguage-0.6.3.tar` & `google-ai-generativelanguage-0.6.4.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.958746 google-ai-generativelanguage-0.6.3/
--rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5604 2024-05-07 20:43:16.958746 google-ai-generativelanguage-0.6.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4216 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.878729 google-ai-generativelanguage-0.6.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.886731 google-ai-generativelanguage-0.6.3/google/ai/
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.890731 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage/
--rw-rw-r--   0 root         (0)     1003     9811 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.894732 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/
--rw-rw-r--   0 root         (0)     1003     2229 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3669 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.894732 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.894732 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    45630 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    61605 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.894732 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10725 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20180 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23467 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    46280 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.898733 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27688 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    43871 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5747 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.898733 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7270 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15957 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16817 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    26746 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.902734 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/
--rw-rw-r--   0 root         (0)     1003     1759 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2895 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/citation.py
--rw-rw-r--   0 root         (0)     1003     3720 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    20990 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/generative_service.py
--rw-rw-r--   0 root         (0)     1003     4802 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/model.py
--rw-rw-r--   0 root         (0)     1003     3143 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     6161 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/safety.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.902734 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/
--rw-rw-r--   0 root         (0)     1003     8304 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    21107 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.902734 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.902734 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24819 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41192 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.902734 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7451 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13961 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15520 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18401 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.906735 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25723 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41865 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/client.py
--rw-rw-r--   0 root         (0)     1003     5737 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.906735 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7453 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15587 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16871 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    24426 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.906735 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    46944 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62973 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.910735 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10886 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19199 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23056 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41119 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.910735 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    46546 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62699 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003    10950 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.910735 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11616 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20233 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24755 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41543 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.914736 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41591 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57782 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/client.py
--rw-rw-r--   0 root         (0)     1003     6013 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.914736 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10464 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18703 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22250 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41155 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.914736 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/
--rw-rw-r--   0 root         (0)     1003      777 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    96015 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   111634 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/client.py
--rw-rw-r--   0 root         (0)     1003    16011 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.918737 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20205 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33773 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    44233 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   105077 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.918737 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35603 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51755 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.918737 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9013 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16146 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18854 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28406 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.922738 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     7020 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2903 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/citation.py
--rw-rw-r--   0 root         (0)     1003    17562 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/content.py
--rw-rw-r--   0 root         (0)     1003    11601 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4234 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/file.py
--rw-rw-r--   0 root         (0)     1003     3555 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/file_service.py
--rw-rw-r--   0 root         (0)     1003    40746 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/generative_service.py
--rw-rw-r--   0 root         (0)     1003     4806 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/model.py
--rw-rw-r--   0 root         (0)     1003     9676 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     4530 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/permission.py
--rw-rw-r--   0 root         (0)     1003     6362 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/permission_service.py
--rw-rw-r--   0 root         (0)     1003    13703 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/retriever.py
--rw-rw-r--   0 root         (0)     1003    24469 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/retriever_service.py
--rw-rw-r--   0 root         (0)     1003     8594 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/safety.py
--rw-rw-r--   0 root         (0)     1003    14378 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/text_service.py
--rw-rw-r--   0 root         (0)     1003    13772 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/tuned_model.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.926739 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003     2426 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3627 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.926739 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.926739 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24772 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41145 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.926739 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7391 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13902 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15461 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18341 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.926739 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    21126 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37444 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5792 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.930740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7203 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13394 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14948 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    16216 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.930740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25081 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41409 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.930740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7273 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13650 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15194 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17420 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.934740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1847 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11613 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4670 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/model.py
--rw-rw-r--   0 root         (0)     1003     3158 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     7878 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/safety.py
--rw-rw-r--   0 root         (0)     1003    10981 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.934740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/
--rw-rw-r--   0 root         (0)     1003     4188 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003     8993 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.934740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.934740 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24835 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    41208 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.938741 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6769 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13964 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14829 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18404 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.938741 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    46589 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62742 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003    10967 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.938741 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9226 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20243 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22336 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41554 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.942742 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41568 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58077 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/client.py
--rw-rw-r--   0 root         (0)     1003     6022 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.942742 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8758 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18712 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20524 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40318 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.942742 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35729 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51881 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.946743 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7647 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16151 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17471 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28412 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.946743 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/
--rw-rw-r--   0 root         (0)     1003     3416 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11613 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4670 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/model.py
--rw-rw-r--   0 root         (0)     1003     8924 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     4460 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/permission.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/permission_service.py
--rw-rw-r--   0 root         (0)     1003     7974 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/safety.py
--rw-rw-r--   0 root         (0)     1003    13777 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/text_service.py
--rw-rw-r--   0 root         (0)     1003    12841 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/tuned_model.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.950744 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/
--rw-r--r--   0 root         (0)     1003     5604 2024-05-07 20:43:16.000000 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    15729 2024-05-07 20:43:16.000000 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:16.000000 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:16.000000 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-05-07 20:43:16.000000 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:43:16.000000 google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:43:16.958746 google-ai-generativelanguage-0.6.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.950744 google-ai-generativelanguage-0.6.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.950744 google-ai-generativelanguage-0.6.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.950744 google-ai-generativelanguage-0.6.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.950744 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   222708 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/test_generative_service.py
--rw-rw-r--   0 root         (0)     1003   144964 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/test_model_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.954745 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   122418 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   151192 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py
--rw-rw-r--   0 root         (0)     1003   228747 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py
--rw-rw-r--   0 root         (0)     1003   266003 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   236137 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py
--rw-rw-r--   0 root         (0)     1003   571435 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py
--rw-rw-r--   0 root         (0)     1003   168921 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.958746 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   122364 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   122910 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   118974 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:16.958746 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003   122426 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   265848 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   236707 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py
--rw-rw-r--   0 root         (0)     1003   169468 2024-05-07 20:40:10.000000 google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.812530 google-ai-generativelanguage-0.6.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5604 2024-05-16 20:56:30.808529 google-ai-generativelanguage-0.6.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4216 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.740523 google-ai-generativelanguage-0.6.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.748524 google-ai-generativelanguage-0.6.4/google/ai/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.752524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage/
+-rw-rw-r--   0 root         (0)     1003     9847 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.752524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/
+-rw-rw-r--   0 root         (0)     1003     2229 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3669 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.752524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.752524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45964 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    61939 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.752524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10729 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20434 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23725 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    46280 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.756524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27688 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43871 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5747 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.756524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7270 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15957 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16817 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    26746 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.756524 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1759 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2895 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/citation.py
+-rw-rw-r--   0 root         (0)     1003     3922 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    22648 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/generative_service.py
+-rw-rw-r--   0 root         (0)     1003     4802 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3143 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     6162 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/safety.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.760525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/
+-rw-rw-r--   0 root         (0)     1003     8340 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21107 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.760525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.760525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24819 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41192 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.760525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7451 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13961 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15520 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18401 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.760525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25773 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41915 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5737 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.764525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7453 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15587 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16871 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    24426 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.764525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47024 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63053 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.764525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10890 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19199 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23060 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41119 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.764525 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46546 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62699 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10950 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.768526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11616 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20233 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24755 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41543 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.768526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41591 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57782 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6013 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.768526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10464 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18703 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22250 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41155 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.772526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/
+-rw-rw-r--   0 root         (0)     1003      777 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    96015 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   111634 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16011 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.772526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20205 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33773 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    44233 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   105077 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.772526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35603 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51755 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.776526 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9013 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16146 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18854 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28406 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.780527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     7056 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2903 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    17562 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/content.py
+-rw-rw-r--   0 root         (0)     1003    11601 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     5422 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/file.py
+-rw-rw-r--   0 root         (0)     1003     3555 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/file_service.py
+-rw-rw-r--   0 root         (0)     1003    40810 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/generative_service.py
+-rw-rw-r--   0 root         (0)     1003     4806 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/model.py
+-rw-rw-r--   0 root         (0)     1003     9676 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     4530 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/permission.py
+-rw-rw-r--   0 root         (0)     1003     6362 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/permission_service.py
+-rw-rw-r--   0 root         (0)     1003    13703 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/retriever.py
+-rw-rw-r--   0 root         (0)     1003    24469 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/retriever_service.py
+-rw-rw-r--   0 root         (0)     1003     8595 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    14378 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/text_service.py
+-rw-rw-r--   0 root         (0)     1003    13772 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/tuned_model.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.780527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     2426 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3627 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.780527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.780527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24772 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41145 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.780527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7391 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13902 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15461 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18341 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.784527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21126 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37444 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5792 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.784527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7203 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13394 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14948 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    16216 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.784527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25081 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41409 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.784527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7273 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13650 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15194 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17420 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.788527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1847 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11613 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4670 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3158 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     7878 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    10981 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.788527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/
+-rw-rw-r--   0 root         (0)     1003     4188 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8993 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.788527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.788527 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24835 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    41208 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.792528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6769 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13964 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14829 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18404 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.792528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46589 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62742 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10967 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.792528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9226 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20243 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22336 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41554 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.792528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41568 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58077 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6022 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.796528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8758 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18712 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20524 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    40318 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.796528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35729 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51881 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.796528 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7647 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16151 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17471 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28412 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.800529 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/
+-rw-rw-r--   0 root         (0)     1003     3416 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11613 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4670 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/model.py
+-rw-rw-r--   0 root         (0)     1003     8924 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     4460 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/permission.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/permission_service.py
+-rw-rw-r--   0 root         (0)     1003     7974 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    13777 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/text_service.py
+-rw-rw-r--   0 root         (0)     1003    12841 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/tuned_model.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.800529 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/
+-rw-r--r--   0 root         (0)     1003     5604 2024-05-16 20:56:30.000000 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    15729 2024-05-16 20:56:30.000000 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 20:56:30.000000 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 20:56:30.000000 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-16 20:56:30.000000 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-16 20:56:30.000000 google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-16 20:56:30.812530 google-ai-generativelanguage-0.6.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.800529 google-ai-generativelanguage-0.6.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.800529 google-ai-generativelanguage-0.6.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.800529 google-ai-generativelanguage-0.6.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.804529 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   222606 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/test_generative_service.py
+-rw-rw-r--   0 root         (0)     1003   144964 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/test_model_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.804529 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   122418 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   151351 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py
+-rw-rw-r--   0 root         (0)     1003   228747 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py
+-rw-rw-r--   0 root         (0)     1003   266003 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   236137 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py
+-rw-rw-r--   0 root         (0)     1003   571435 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py
+-rw-rw-r--   0 root         (0)     1003   168921 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.808529 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   122364 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   122910 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   118974 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 20:56:30.808529 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   122426 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   265848 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   236707 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py
+-rw-rw-r--   0 root         (0)     1003   169468 2024-05-16 20:53:32.000000 google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py
```

### Comparing `google-ai-generativelanguage-0.6.3/LICENSE` & `google-ai-generativelanguage-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/MANIFEST.in` & `google-ai-generativelanguage-0.6.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/PKG-INFO` & `google-ai-generativelanguage-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.6.3
+Version: 0.6.4
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-ai-generativelanguage-0.6.3/README.rst` & `google-ai-generativelanguage-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     CountMessageTokensResponse,
     Example,
     GenerateMessageRequest,
     GenerateMessageResponse,
     Message,
     MessagePrompt,
 )
-from google.ai.generativelanguage_v1beta.types.file import File
+from google.ai.generativelanguage_v1beta.types.file import File, VideoMetadata
 from google.ai.generativelanguage_v1beta.types.file_service import (
     CreateFileRequest,
     CreateFileResponse,
     DeleteFileRequest,
     GetFileRequest,
     ListFilesRequest,
     ListFilesResponse,
@@ -247,14 +247,15 @@
     "CountMessageTokensResponse",
     "Example",
     "GenerateMessageRequest",
     "GenerateMessageResponse",
     "Message",
     "MessagePrompt",
     "File",
+    "VideoMetadata",
     "CreateFileRequest",
     "CreateFileResponse",
     "DeleteFileRequest",
     "GetFileRequest",
     "ListFilesRequest",
     "ListFilesResponse",
     "AttributionSourceId",
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage/gapic_version.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage/gapic_version.py`

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
-__version__ = "0.6.3"  # {x-release-please-version}
+__version__ = "0.6.4"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/gapic_metadata.json` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/gapic_version.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/gapic_version.py`

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
-__version__ = "0.6.3"  # {x-release-please-version}
+__version__ = "0.6.4"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,20 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> generative_service.GenerateContentResponse:
         r"""Generates a response from the model given an input
         ``GenerateContentRequest``.
 
+        Input capabilities differ between models, including tuned
+        models. See the `model
+        guide <https://ai.google.dev/models/gemini>`__ and `tuning
+        guide <https://ai.google.dev/docs/model_tuning_guidance>`__ for
+        details.
+
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
@@ -843,16 +849,17 @@
 
                 Format: ``models/{model}``
 
                 This corresponds to the ``model`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             contents (:class:`MutableSequence[google.ai.generativelanguage_v1.types.Content]`):
-                Required. The input given to the
-                model as a prompt.
+                Optional. The input given to the model as a prompt. This
+                field is ignored when ``generate_content_request`` is
+                set.
 
                 This corresponds to the ``contents`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,14 +692,20 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> generative_service.GenerateContentResponse:
         r"""Generates a response from the model given an input
         ``GenerateContentRequest``.
 
+        Input capabilities differ between models, including tuned
+        models. See the `model
+        guide <https://ai.google.dev/models/gemini>`__ and `tuning
+        guide <https://ai.google.dev/docs/model_tuning_guidance>`__ for
+        details.
+
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
@@ -1244,16 +1250,17 @@
 
                 Format: ``models/{model}``
 
                 This corresponds to the ``model`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             contents (MutableSequence[google.ai.generativelanguage_v1.types.Content]):
-                Required. The input given to the
-                model as a prompt.
+                Optional. The input given to the model as a prompt. This
+                field is ignored when ``generate_content_request`` is
+                set.
 
                 This corresponds to the ``contents`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,31 +132,31 @@
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.stream_generate_content: gapic_v1.method.wrap_method(
                 self.stream_generate_content,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.embed_content: gapic_v1.method.wrap_method(
                 self.embed_content,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,20 @@
         generative_service.GenerateContentResponse,
     ]:
         r"""Return a callable for the generate content method over gRPC.
 
         Generates a response from the model given an input
         ``GenerateContentRequest``.
 
+        Input capabilities differ between models, including tuned
+        models. See the `model
+        guide <https://ai.google.dev/models/gemini>`__ and `tuning
+        guide <https://ai.google.dev/docs/model_tuning_guidance>`__ for
+        details.
+
         Returns:
             Callable[[~.GenerateContentRequest],
                     ~.GenerateContentResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,20 @@
         Awaitable[generative_service.GenerateContentResponse],
     ]:
         r"""Return a callable for the generate content method over gRPC.
 
         Generates a response from the model given an input
         ``GenerateContentRequest``.
 
+        Input capabilities differ between models, including tuned
+        models. See the `model
+        guide <https://ai.google.dev/models/gemini>`__ and `tuning
+        guide <https://ai.google.dev/docs/model_tuning_guidance>`__ for
+        details.
+
         Returns:
             Callable[[~.GenerateContentRequest],
                     Awaitable[~.GenerateContentResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
@@ -397,31 +403,31 @@
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.stream_generate_content: gapic_v1.method_async.wrap_method(
                 self.stream_generate_content,
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.embed_content: gapic_v1.method_async.wrap_method(
                 self.embed_content,
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/citation.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/content.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/content.py`

 * *Files 18% similar despite different names*

```diff
@@ -105,18 +105,21 @@
 class Blob(proto.Message):
     r"""Raw media bytes.
 
     Text should not be sent as raw bytes, use the 'text' field.
 
     Attributes:
         mime_type (str):
-            The IANA standard MIME type of the source
-            data. Accepted types include: "image/png",
-            "image/jpeg", "image/heic", "image/heif",
-            "image/webp".
+            The IANA standard MIME type of the source data. Examples:
+
+            -  image/png
+            -  image/jpeg If an unsupported MIME type is provided, an
+               error will be returned. For a complete list of supported
+               types, see `Supported file
+               formats <https://ai.google.dev/gemini-api/docs/prompting_with_media#supported_file_formats>`__.
         data (bytes):
             Raw bytes for media formats.
     """
 
     mime_type: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/generative_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/generative_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,14 +269,17 @@
 
     Attributes:
         candidates (MutableSequence[google.ai.generativelanguage_v1.types.Candidate]):
             Candidate responses from the model.
         prompt_feedback (google.ai.generativelanguage_v1.types.GenerateContentResponse.PromptFeedback):
             Returns the prompt's feedback related to the
             content filters.
+        usage_metadata (google.ai.generativelanguage_v1.types.GenerateContentResponse.UsageMetadata):
+            Output only. Metadata on the generation
+            requests' token usage.
     """
 
     class PromptFeedback(proto.Message):
         r"""A set of the feedback metadata the prompt specified in
         ``GenerateContentRequest.content``.
 
         Attributes:
@@ -315,24 +318,56 @@
         )
         safety_ratings: MutableSequence[safety.SafetyRating] = proto.RepeatedField(
             proto.MESSAGE,
             number=2,
             message=safety.SafetyRating,
         )
 
+    class UsageMetadata(proto.Message):
+        r"""Metadata on the generation request's token usage.
+
+        Attributes:
+            prompt_token_count (int):
+                Number of tokens in the prompt.
+            candidates_token_count (int):
+                Total number of tokens across the generated
+                candidates.
+            total_token_count (int):
+                Total token count for the generation request
+                (prompt + candidates).
+        """
+
+        prompt_token_count: int = proto.Field(
+            proto.INT32,
+            number=1,
+        )
+        candidates_token_count: int = proto.Field(
+            proto.INT32,
+            number=2,
+        )
+        total_token_count: int = proto.Field(
+            proto.INT32,
+            number=3,
+        )
+
     candidates: MutableSequence["Candidate"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Candidate",
     )
     prompt_feedback: PromptFeedback = proto.Field(
         proto.MESSAGE,
         number=2,
         message=PromptFeedback,
     )
+    usage_metadata: UsageMetadata = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=UsageMetadata,
+    )
 
 
 class Candidate(proto.Message):
     r"""A response candidate generated from the model.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
@@ -454,16 +489,17 @@
             Note: Specifying a ``title`` for ``RETRIEVAL_DOCUMENT``
             provides better quality embeddings for retrieval.
 
             This field is a member of `oneof`_ ``_title``.
         output_dimensionality (int):
             Optional. Optional reduced dimension for the output
             embedding. If set, excessive values in the output embedding
-            are truncated from the end. Supported by
-            ``models/text-embedding-latest``.
+            are truncated from the end. Supported by newer models since
+            2024, and the earlier model (``models/embedding-001``)
+            cannot specify this value.
 
             This field is a member of `oneof`_ ``_output_dimensionality``.
     """
 
     model: str = proto.Field(
         proto.STRING,
         number=1,
@@ -580,27 +616,36 @@
             for the Model to use.
 
             This name should match a model name returned by the
             ``ListModels`` method.
 
             Format: ``models/{model}``
         contents (MutableSequence[google.ai.generativelanguage_v1.types.Content]):
-            Required. The input given to the model as a
-            prompt.
+            Optional. The input given to the model as a prompt. This
+            field is ignored when ``generate_content_request`` is set.
+        generate_content_request (google.ai.generativelanguage_v1.types.GenerateContentRequest):
+            Optional. The overall input given to the
+            model. CountTokens will count prompt, function
+            calling, etc.
     """
 
     model: str = proto.Field(
         proto.STRING,
         number=1,
     )
     contents: MutableSequence[gag_content.Content] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=gag_content.Content,
     )
+    generate_content_request: "GenerateContentRequest" = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message="GenerateContentRequest",
+    )
 
 
 class CountTokensResponse(proto.Message):
     r"""A response from ``CountTokens``.
 
     It returns the model's ``token_count`` for the ``prompt``.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/model.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/model_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1/types/safety.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1/types/safety.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     )
 
 
 class SafetySetting(proto.Message):
     r"""Safety setting, affecting the safety-blocking behavior.
 
     Passing a safety setting for a category changes the allowed
-    proability that content is blocked.
+    probability that content is blocked.
 
     Attributes:
         category (google.ai.generativelanguage_v1.types.HarmCategory):
             Required. The category for this setting.
         threshold (google.ai.generativelanguage_v1.types.SafetySetting.HarmBlockThreshold):
             Required. Controls the probability threshold
             at which harm is blocked.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     CountMessageTokensResponse,
     Example,
     GenerateMessageRequest,
     GenerateMessageResponse,
     Message,
     MessagePrompt,
 )
-from .types.file import File
+from .types.file import File, VideoMetadata
 from .types.file_service import (
     CreateFileRequest,
     CreateFileResponse,
     DeleteFileRequest,
     GetFileRequest,
     ListFilesRequest,
     ListFilesResponse,
@@ -321,8 +321,9 @@
     "TuningTask",
     "Type",
     "UpdateChunkRequest",
     "UpdateCorpusRequest",
     "UpdateDocumentRequest",
     "UpdatePermissionRequest",
     "UpdateTunedModelRequest",
+    "VideoMetadata",
 )
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/gapic_metadata.json` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/gapic_version.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/gapic_version.py`

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
-__version__ = "0.6.3"  # {x-release-please-version}
+__version__ = "0.6.4"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 try:
     OptionalRetry = Union[retries.AsyncRetry, gapic_v1.method._MethodDefault, None]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.AsyncRetry, object, None]  # type: ignore
 
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
+from google.rpc import status_pb2  # type: ignore
 
 from google.ai.generativelanguage_v1beta.services.file_service import pagers
 from google.ai.generativelanguage_v1beta.types import file, file_service
 
 from .client import FileServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, FileServiceTransport
 from .transports.grpc_asyncio import FileServiceGrpcAsyncIOTransport
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault, None]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object, None]  # type: ignore
 
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
+from google.rpc import status_pb2  # type: ignore
 
 from google.ai.generativelanguage_v1beta.services.file_service import pagers
 from google.ai.generativelanguage_v1beta.types import file, file_service
 
 from .transports.base import DEFAULT_CLIENT_INFO, FileServiceTransport
 from .transports.grpc import FileServiceGrpcTransport
 from .transports.grpc_asyncio import FileServiceGrpcAsyncIOTransport
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/file_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1014,16 +1014,17 @@
 
                 Format: ``models/{model}``
 
                 This corresponds to the ``model`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             contents (:class:`MutableSequence[google.ai.generativelanguage_v1beta.types.Content]`):
-                Optional. The input given to the
-                model as a prompt.
+                Optional. The input given to the model as a prompt. This
+                field is ignored when ``generate_content_request`` is
+                set.
 
                 This corresponds to the ``contents`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1412,16 +1412,17 @@
 
                 Format: ``models/{model}``
 
                 This corresponds to the ``model`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             contents (MutableSequence[google.ai.generativelanguage_v1beta.types.Content]):
-                Optional. The input given to the
-                model as a prompt.
+                Optional. The input given to the model as a prompt. This
+                field is ignored when ``generate_content_request`` is
+                set.
 
                 This corresponds to the ``contents`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,17 @@
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.generate_answer: gapic_v1.method.wrap_method(
                 self.generate_answer,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
@@ -160,17 +160,17 @@
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.embed_content: gapic_v1.method.wrap_method(
                 self.embed_content,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,17 +433,17 @@
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.generate_answer: gapic_v1.method_async.wrap_method(
                 self.generate_answer,
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
@@ -461,17 +461,17 @@
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
                         core_exceptions.ServiceUnavailable,
                     ),
-                    deadline=60.0,
+                    deadline=600.0,
                 ),
-                default_timeout=60.0,
+                default_timeout=600.0,
                 client_info=client_info,
             ),
             self.embed_content: gapic_v1.method_async.wrap_method(
                 self.embed_content,
                 default_retry=retries.AsyncRetry(
                     initial=1.0,
                     maximum=10.0,
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     CountMessageTokensResponse,
     Example,
     GenerateMessageRequest,
     GenerateMessageResponse,
     Message,
     MessagePrompt,
 )
-from .file import File
+from .file import File, VideoMetadata
 from .file_service import (
     CreateFileRequest,
     CreateFileResponse,
     DeleteFileRequest,
     GetFileRequest,
     ListFilesRequest,
     ListFilesResponse,
@@ -183,14 +183,15 @@
     "CountMessageTokensResponse",
     "Example",
     "GenerateMessageRequest",
     "GenerateMessageResponse",
     "Message",
     "MessagePrompt",
     "File",
+    "VideoMetadata",
     "CreateFileRequest",
     "CreateFileResponse",
     "DeleteFileRequest",
     "GetFileRequest",
     "ListFilesRequest",
     "ListFilesResponse",
     "AttributionSourceId",
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/citation.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/content.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/content.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/discuss_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/file.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/file.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,29 +13,38 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
+from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
+from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.ai.generativelanguage.v1beta",
     manifest={
         "File",
+        "VideoMetadata",
     },
 )
 
 
 class File(proto.Message):
     r"""A file uploaded to the API.
 
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
     Attributes:
+        video_metadata (google.ai.generativelanguage_v1beta.types.VideoMetadata):
+            Output only. Metadata for a video.
+
+            This field is a member of `oneof`_ ``metadata``.
         name (str):
             Immutable. Identifier. The ``File`` resource name. The ID
             (name excluding the "files/" prefix) can contain up to 40
             characters that are lowercase alphanumeric or dashes (-).
             The ID cannot start or end with a dash. If the name is empty
             on create, a unique name will be generated. Example:
             ``files/123-456``
@@ -58,14 +67,17 @@
         sha256_hash (bytes):
             Output only. SHA-256 hash of the uploaded
             bytes.
         uri (str):
             Output only. The uri of the ``File``.
         state (google.ai.generativelanguage_v1beta.types.File.State):
             Output only. Processing state of the File.
+        error (google.rpc.status_pb2.Status):
+            Output only. Error status if File processing
+            failed.
     """
 
     class State(proto.Enum):
         r"""States for the lifecycle of a File.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -81,14 +93,20 @@
                 File failed processing.
         """
         STATE_UNSPECIFIED = 0
         PROCESSING = 1
         ACTIVE = 2
         FAILED = 10
 
+    video_metadata: "VideoMetadata" = proto.Field(
+        proto.MESSAGE,
+        number=12,
+        oneof="metadata",
+        message="VideoMetadata",
+    )
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     display_name: str = proto.Field(
         proto.STRING,
         number=2,
@@ -125,10 +143,30 @@
         number=9,
     )
     state: State = proto.Field(
         proto.ENUM,
         number=10,
         enum=State,
     )
+    error: status_pb2.Status = proto.Field(
+        proto.MESSAGE,
+        number=11,
+        message=status_pb2.Status,
+    )
+
+
+class VideoMetadata(proto.Message):
+    r"""Metadata for a video ``File``.
+
+    Attributes:
+        video_duration (google.protobuf.duration_pb2.Duration):
+            Duration of the video.
+    """
+
+    video_duration: duration_pb2.Duration = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=duration_pb2.Duration,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/file_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/file_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/generative_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/generative_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1090,16 +1090,16 @@
             for the Model to use.
 
             This name should match a model name returned by the
             ``ListModels`` method.
 
             Format: ``models/{model}``
         contents (MutableSequence[google.ai.generativelanguage_v1beta.types.Content]):
-            Optional. The input given to the model as a
-            prompt.
+            Optional. The input given to the model as a prompt. This
+            field is ignored when ``generate_content_request`` is set.
         generate_content_request (google.ai.generativelanguage_v1beta.types.GenerateContentRequest):
             Optional. The overall input given to the
             model. CountTokens will count prompt, function
             calling, etc.
     """
 
     model: str = proto.Field(
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/model.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/model_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/permission.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/permission.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/permission_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/retriever.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/retriever.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/retriever_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/retriever_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/safety.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     )
 
 
 class SafetySetting(proto.Message):
     r"""Safety setting, affecting the safety-blocking behavior.
 
     Passing a safety setting for a category changes the allowed
-    proability that content is blocked.
+    probability that content is blocked.
 
     Attributes:
         category (google.ai.generativelanguage_v1beta.types.HarmCategory):
             Required. The category for this setting.
         threshold (google.ai.generativelanguage_v1beta.types.SafetySetting.HarmBlockThreshold):
             Required. Controls the probability threshold
             at which harm is blocked.
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/text_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta/types/tuned_model.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta/types/tuned_model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/gapic_metadata.json` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/gapic_version.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/gapic_version.py`

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
-__version__ = "0.6.3"  # {x-release-please-version}
+__version__ = "0.6.4"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/citation.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/discuss_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/model.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/model_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/safety.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/safety.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta2/types/text_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta2/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/gapic_metadata.json` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/gapic_version.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/gapic_version.py`

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
-__version__ = "0.6.3"  # {x-release-please-version}
+__version__ = "0.6.4"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/client.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/client.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/__init__.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/citation.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/citation.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/discuss_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/model.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/model_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/permission.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/permission.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/permission_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/safety.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/safety.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/text_service.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google/ai/generativelanguage_v1beta3/types/tuned_model.py` & `google-ai-generativelanguage-0.6.4/google/ai/generativelanguage_v1beta3/types/tuned_model.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/PKG-INFO` & `google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.6.3
+Version: 0.6.4
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-ai-generativelanguage-0.6.3/google_ai_generativelanguage.egg-info/SOURCES.txt` & `google-ai-generativelanguage-0.6.4/google_ai_generativelanguage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/setup.py` & `google-ai-generativelanguage-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/test_generative_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/test_generative_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -4494,23 +4494,15 @@
 
 def test_count_tokens_rest_unset_required_fields():
     transport = transports.GenerativeServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials
     )
 
     unset_fields = transport.count_tokens._get_unset_required_fields({})
-    assert set(unset_fields) == (
-        set(())
-        & set(
-            (
-                "model",
-                "contents",
-            )
-        )
-    )
+    assert set(unset_fields) == (set(()) & set(("model",)))
 
 
 @pytest.mark.parametrize("null_interceptor", [True, False])
 def test_count_tokens_rest_interceptors(null_interceptor):
     transport = transports.GenerativeServiceRestTransport(
         credentials=ga_credentials.AnonymousCredentials(),
         interceptor=None
```

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1/test_model_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_file_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,19 @@
 from google.api_core import api_core_version, client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account
+from google.protobuf import any_pb2  # type: ignore
+from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import json_format
 from google.protobuf import timestamp_pb2  # type: ignore
+from google.rpc import status_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
```

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/__init__.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.6.3/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py` & `google-ai-generativelanguage-0.6.4/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py`

 * *Files identical despite different names*

