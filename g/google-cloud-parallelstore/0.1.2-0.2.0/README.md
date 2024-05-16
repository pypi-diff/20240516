# Comparing `tmp/google-cloud-parallelstore-0.1.2.tar.gz` & `tmp/google-cloud-parallelstore-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-parallelstore-0.1.2.tar", last modified: Tue May  7 20:43:51 2024, max compression
+gzip compressed data, was "google-cloud-parallelstore-0.2.0.tar", last modified: Thu May 16 17:15:43 2024, max compression
```

## Comparing `google-cloud-parallelstore-0.1.2.tar` & `google-cloud-parallelstore-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/
--rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5258 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3876 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.669559 google-cloud-parallelstore-0.1.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.669559 google-cloud-parallelstore-0.1.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.673560 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/
--rw-rw-r--   0 root         (0)     1003     1932 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.673560 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/
--rw-rw-r--   0 root         (0)     1003     1767 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     3204 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       87 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/
--rw-rw-r--   0 root         (0)     1003      765 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py
--rw-rw-r--   0 root         (0)     1003    60808 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py
--rw-rw-r--   0 root         (0)     1003    77457 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/client.py
--rw-rw-r--   0 root         (0)     1003     5870 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10443 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25632 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27713 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    66171 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.677561 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1496 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26281 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/parallelstore.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/
--rw-r--r--   0 root         (0)     1003     5258 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1662 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-05-07 20:43:51.000000 google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3193 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 20:43:51.681561 google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   302813 2024-05-07 20:40:12.000000 google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5258 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3876 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.075510 google-cloud-parallelstore-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.079511 google-cloud-parallelstore-0.2.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.079511 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore/
+-rw-rw-r--   0 root         (0)     1003     2144 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.083511 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1979 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3204 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       87 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.083511 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.083511 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/
+-rw-rw-r--   0 root         (0)     1003      765 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60959 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py
+-rw-rw-r--   0 root         (0)     1003    77608 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/client.py
+-rw-rw-r--   0 root         (0)     1003     5870 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.083511 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10443 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25632 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27713 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    66171 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.083511 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1708 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32405 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/types/parallelstore.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/
+-rw-r--r--   0 root         (0)     1003     5258 2024-05-16 17:15:43.000000 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1662 2024-05-16 17:15:43.000000 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 17:15:43.000000 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-16 17:15:43.000000 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-16 17:15:43.000000 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-16 17:15:43.000000 google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3193 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-16 17:15:43.087511 google-cloud-parallelstore-0.2.0/tests/unit/gapic/parallelstore_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/tests/unit/gapic/parallelstore_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   302405 2024-05-16 17:11:29.000000 google-cloud-parallelstore-0.2.0/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py
```

### Comparing `google-cloud-parallelstore-0.1.2/LICENSE` & `google-cloud-parallelstore-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/MANIFEST.in` & `google-cloud-parallelstore-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/PKG-INFO` & `google-cloud-parallelstore-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-parallelstore
-Version: 0.1.2
+Version: 0.2.0
 Summary: Google Cloud Parallelstore API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-parallelstore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-parallelstore-0.1.2/README.rst` & `google-cloud-parallelstore-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/__init__.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,45 +23,53 @@
 )
 from google.cloud.parallelstore_v1beta.services.parallelstore.client import (
     ParallelstoreClient,
 )
 from google.cloud.parallelstore_v1beta.types.parallelstore import (
     CreateInstanceRequest,
     DeleteInstanceRequest,
+    DestinationGcsBucket,
+    DestinationParallelstore,
     ExportDataMetadata,
     ExportDataRequest,
     ExportDataResponse,
     GetInstanceRequest,
     ImportDataMetadata,
     ImportDataRequest,
     ImportDataResponse,
     Instance,
     ListInstancesRequest,
     ListInstancesResponse,
     OperationMetadata,
+    SourceGcsBucket,
+    SourceParallelstore,
     TransferCounters,
     TransferOperationMetadata,
     TransferType,
     UpdateInstanceRequest,
 )
 
 __all__ = (
     "ParallelstoreClient",
     "ParallelstoreAsyncClient",
     "CreateInstanceRequest",
     "DeleteInstanceRequest",
+    "DestinationGcsBucket",
+    "DestinationParallelstore",
     "ExportDataMetadata",
     "ExportDataRequest",
     "ExportDataResponse",
     "GetInstanceRequest",
     "ImportDataMetadata",
     "ImportDataRequest",
     "ImportDataResponse",
     "Instance",
     "ListInstancesRequest",
     "ListInstancesResponse",
     "OperationMetadata",
+    "SourceGcsBucket",
+    "SourceParallelstore",
     "TransferCounters",
     "TransferOperationMetadata",
     "UpdateInstanceRequest",
     "TransferType",
 )
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore/gapic_version.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/__init__.py`

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
-__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/__init__.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,45 +18,53 @@
 __version__ = package_version.__version__
 
 
 from .services.parallelstore import ParallelstoreAsyncClient, ParallelstoreClient
 from .types.parallelstore import (
     CreateInstanceRequest,
     DeleteInstanceRequest,
+    DestinationGcsBucket,
+    DestinationParallelstore,
     ExportDataMetadata,
     ExportDataRequest,
     ExportDataResponse,
     GetInstanceRequest,
     ImportDataMetadata,
     ImportDataRequest,
     ImportDataResponse,
     Instance,
     ListInstancesRequest,
     ListInstancesResponse,
     OperationMetadata,
+    SourceGcsBucket,
+    SourceParallelstore,
     TransferCounters,
     TransferOperationMetadata,
     TransferType,
     UpdateInstanceRequest,
 )
 
 __all__ = (
     "ParallelstoreAsyncClient",
     "CreateInstanceRequest",
     "DeleteInstanceRequest",
+    "DestinationGcsBucket",
+    "DestinationParallelstore",
     "ExportDataMetadata",
     "ExportDataRequest",
     "ExportDataResponse",
     "GetInstanceRequest",
     "ImportDataMetadata",
     "ImportDataRequest",
     "ImportDataResponse",
     "Instance",
     "ListInstancesRequest",
     "ListInstancesResponse",
     "OperationMetadata",
     "ParallelstoreClient",
+    "SourceGcsBucket",
+    "SourceParallelstore",
     "TransferCounters",
     "TransferOperationMetadata",
     "TransferType",
     "UpdateInstanceRequest",
 )
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_metadata.json` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/gapic_version.py` & `google-cloud-parallelstore-0.2.0/tests/__init__.py`

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
-__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/__init__.py` & `google-cloud-parallelstore-0.2.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -956,17 +956,19 @@
             from google.cloud import parallelstore_v1beta
 
             async def sample_import_data():
                 # Create a client
                 client = parallelstore_v1beta.ParallelstoreAsyncClient()
 
                 # Initialize request argument(s)
+                source_gcs_bucket = parallelstore_v1beta.SourceGcsBucket()
+                source_gcs_bucket.uri = "uri_value"
+
                 request = parallelstore_v1beta.ImportDataRequest(
-                    source_gcs_uri="source_gcs_uri_value",
-                    destination_path="destination_path_value",
+                    source_gcs_bucket=source_gcs_bucket,
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.import_data(request=request)
 
                 print("Waiting for operation to complete...")
@@ -1060,17 +1062,19 @@
             from google.cloud import parallelstore_v1beta
 
             async def sample_export_data():
                 # Create a client
                 client = parallelstore_v1beta.ParallelstoreAsyncClient()
 
                 # Initialize request argument(s)
+                destination_gcs_bucket = parallelstore_v1beta.DestinationGcsBucket()
+                destination_gcs_bucket.uri = "uri_value"
+
                 request = parallelstore_v1beta.ExportDataRequest(
-                    source_path="source_path_value",
-                    destination_gcs_uri="destination_gcs_uri_value",
+                    destination_gcs_bucket=destination_gcs_bucket,
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.export_data(request=request)
 
                 print("Waiting for operation to complete...")
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/client.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1396,17 +1396,19 @@
             from google.cloud import parallelstore_v1beta
 
             def sample_import_data():
                 # Create a client
                 client = parallelstore_v1beta.ParallelstoreClient()
 
                 # Initialize request argument(s)
+                source_gcs_bucket = parallelstore_v1beta.SourceGcsBucket()
+                source_gcs_bucket.uri = "uri_value"
+
                 request = parallelstore_v1beta.ImportDataRequest(
-                    source_gcs_uri="source_gcs_uri_value",
-                    destination_path="destination_path_value",
+                    source_gcs_bucket=source_gcs_bucket,
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.import_data(request=request)
 
                 print("Waiting for operation to complete...")
@@ -1498,17 +1500,19 @@
             from google.cloud import parallelstore_v1beta
 
             def sample_export_data():
                 # Create a client
                 client = parallelstore_v1beta.ParallelstoreClient()
 
                 # Initialize request argument(s)
+                destination_gcs_bucket = parallelstore_v1beta.DestinationGcsBucket()
+                destination_gcs_bucket.uri = "uri_value"
+
                 request = parallelstore_v1beta.ExportDataRequest(
-                    source_path="source_path_value",
-                    destination_gcs_uri="destination_gcs_uri_value",
+                    destination_gcs_bucket=destination_gcs_bucket,
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.export_data(request=request)
 
                 print("Waiting for operation to complete...")
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/services/parallelstore/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/__init__.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/types/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,43 +12,51 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .parallelstore import (
     CreateInstanceRequest,
     DeleteInstanceRequest,
+    DestinationGcsBucket,
+    DestinationParallelstore,
     ExportDataMetadata,
     ExportDataRequest,
     ExportDataResponse,
     GetInstanceRequest,
     ImportDataMetadata,
     ImportDataRequest,
     ImportDataResponse,
     Instance,
     ListInstancesRequest,
     ListInstancesResponse,
     OperationMetadata,
+    SourceGcsBucket,
+    SourceParallelstore,
     TransferCounters,
     TransferOperationMetadata,
     TransferType,
     UpdateInstanceRequest,
 )
 
 __all__ = (
     "CreateInstanceRequest",
     "DeleteInstanceRequest",
+    "DestinationGcsBucket",
+    "DestinationParallelstore",
     "ExportDataMetadata",
     "ExportDataRequest",
     "ExportDataResponse",
     "GetInstanceRequest",
     "ImportDataMetadata",
     "ImportDataRequest",
     "ImportDataResponse",
     "Instance",
     "ListInstancesRequest",
     "ListInstancesResponse",
     "OperationMetadata",
+    "SourceGcsBucket",
+    "SourceParallelstore",
     "TransferCounters",
     "TransferOperationMetadata",
     "UpdateInstanceRequest",
     "TransferType",
 )
```

### Comparing `google-cloud-parallelstore-0.1.2/google/cloud/parallelstore_v1beta/types/parallelstore.py` & `google-cloud-parallelstore-0.2.0/google/cloud/parallelstore_v1beta/types/parallelstore.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         "ListInstancesRequest",
         "ListInstancesResponse",
         "GetInstanceRequest",
         "CreateInstanceRequest",
         "UpdateInstanceRequest",
         "DeleteInstanceRequest",
         "OperationMetadata",
+        "SourceGcsBucket",
+        "DestinationGcsBucket",
+        "SourceParallelstore",
+        "DestinationParallelstore",
         "ImportDataRequest",
         "ExportDataRequest",
         "ImportDataResponse",
         "ImportDataMetadata",
         "ExportDataResponse",
         "ExportDataMetadata",
         "TransferOperationMetadata",
@@ -516,31 +520,90 @@
     )
     api_version: str = proto.Field(
         proto.STRING,
         number=7,
     )
 
 
+class SourceGcsBucket(proto.Message):
+    r"""Google Cloud Storage as a source.
+
+    Attributes:
+        uri (str):
+            Required. URI to a Cloud Storage object in format:
+            'gs://<bucket_name>/<path_inside_bucket>'.
+    """
+
+    uri: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class DestinationGcsBucket(proto.Message):
+    r"""Google Cloud Storage as a destination.
+
+    Attributes:
+        uri (str):
+            Required. URI to a Cloud Storage object in format:
+            'gs://<bucket_name>/<path_inside_bucket>'.
+    """
+
+    uri: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class SourceParallelstore(proto.Message):
+    r"""Pa as a source.
+
+    Attributes:
+        path (str):
+            Optional. Root directory path to the
+            Paralellstore filesystem, starting with '/'.
+            Defaults to '/' if unset.
+    """
+
+    path: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class DestinationParallelstore(proto.Message):
+    r"""Parallelstore as a destination.
+
+    Attributes:
+        path (str):
+            Optional. Root directory path to the
+            Paralellstore filesystem, starting with '/'.
+            Defaults to '/' if unset.
+    """
+
+    path: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
 class ImportDataRequest(proto.Message):
     r"""Message representing the request importing data from
     parallelstore to Cloud Storage.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        source_gcs_uri (str):
-            URI to a Cloud Storage object in format:
-            'gs://<bucket_name>/<path_inside_bucket>'.
+        source_gcs_bucket (google.cloud.parallelstore_v1beta.types.SourceGcsBucket):
+            Cloud Storage source.
 
             This field is a member of `oneof`_ ``source``.
-        destination_path (str):
-            Optional. Root directory path to the
-            Paralellstore filesystem, starting with '/'.
-            Sets to '/' if no value is set.
+        destination_parallelstore (google.cloud.parallelstore_v1beta.types.DestinationParallelstore):
+            Parallelstore destination.
 
             This field is a member of `oneof`_ ``destination``.
         name (str):
             Required. Name of the resource.
         request_id (str):
             Optional. An optional request ID to identify
             requests. Specify a unique request ID so that if
@@ -559,23 +622,25 @@
             duplicate commitments.
 
             The request ID must be a valid UUID with the
             exception that zero UUID is not supported
             (00000000-0000-0000-0000-000000000000).
     """
 
-    source_gcs_uri: str = proto.Field(
-        proto.STRING,
+    source_gcs_bucket: "SourceGcsBucket" = proto.Field(
+        proto.MESSAGE,
         number=2,
         oneof="source",
+        message="SourceGcsBucket",
     )
-    destination_path: str = proto.Field(
-        proto.STRING,
+    destination_parallelstore: "DestinationParallelstore" = proto.Field(
+        proto.MESSAGE,
         number=3,
         oneof="destination",
+        message="DestinationParallelstore",
     )
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     request_id: str = proto.Field(
         proto.STRING,
@@ -587,23 +652,20 @@
     r"""Message representing the request exporting data from Cloud
     Storage to parallelstore.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        source_path (str):
-            Optional. Root directory path to the
-            Paralellstore filesystem, starting with '/'.
-            Sets to '/' if no value is set.
+        source_parallelstore (google.cloud.parallelstore_v1beta.types.SourceParallelstore):
+            Parallelstore source.
 
             This field is a member of `oneof`_ ``source``.
-        destination_gcs_uri (str):
-            URI to a Cloud Storage object in format:
-            'gs://<bucket_name>/<path_inside_bucket>'.
+        destination_gcs_bucket (google.cloud.parallelstore_v1beta.types.DestinationGcsBucket):
+            Cloud Storage destination.
 
             This field is a member of `oneof`_ ``destination``.
         name (str):
             Required. Name of the resource.
         request_id (str):
             Optional. An optional request ID to identify
             requests. Specify a unique request ID so that if
@@ -622,23 +684,25 @@
             duplicate commitments.
 
             The request ID must be a valid UUID with the
             exception that zero UUID is not supported
             (00000000-0000-0000-0000-000000000000).
     """
 
-    source_path: str = proto.Field(
-        proto.STRING,
+    source_parallelstore: "SourceParallelstore" = proto.Field(
+        proto.MESSAGE,
         number=2,
         oneof="source",
+        message="SourceParallelstore",
     )
-    destination_gcs_uri: str = proto.Field(
-        proto.STRING,
+    destination_gcs_bucket: "DestinationGcsBucket" = proto.Field(
+        proto.MESSAGE,
         number=3,
         oneof="destination",
+        message="DestinationGcsBucket",
     )
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     request_id: str = proto.Field(
         proto.STRING,
@@ -656,21 +720,75 @@
 class ImportDataMetadata(proto.Message):
     r"""ImportDataMetadata contains import data operation metadata
 
     Attributes:
         operation_metadata (google.cloud.parallelstore_v1beta.types.TransferOperationMetadata):
             Contains the data transfer operation
             metadata.
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The time the operation was
+            created.
+        end_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The time the operation finished
+            running.
+        target (str):
+            Output only. Server-defined resource path for
+            the target of the operation.
+        verb (str):
+            Output only. Name of the verb executed by the
+            operation.
+        status_message (str):
+            Output only. Human-readable status of the
+            operation, if any.
+        requested_cancellation (bool):
+            Output only. Identifies whether the user has requested
+            cancellation of the operation. Operations that have
+            successfully been cancelled have [Operation.error][] value
+            with a [google.rpc.Status.code][google.rpc.Status.code] of
+            1, corresponding to ``Code.CANCELLED``.
+        api_version (str):
+            Output only. API version used to start the
+            operation.
     """
 
     operation_metadata: "TransferOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="TransferOperationMetadata",
     )
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
+    end_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=timestamp_pb2.Timestamp,
+    )
+    target: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    verb: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    status_message: str = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    requested_cancellation: bool = proto.Field(
+        proto.BOOL,
+        number=7,
+    )
+    api_version: str = proto.Field(
+        proto.STRING,
+        number=8,
+    )
 
 
 class ExportDataResponse(proto.Message):
     r"""ExportDataResponse is the response returned from ExportData
     rpc
 
     """
@@ -679,68 +797,140 @@
 class ExportDataMetadata(proto.Message):
     r"""ExportDataMetadata contains export data operation metadata
 
     Attributes:
         operation_metadata (google.cloud.parallelstore_v1beta.types.TransferOperationMetadata):
             Contains the data transfer operation
             metadata.
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The time the operation was
+            created.
+        end_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The time the operation finished
+            running.
+        target (str):
+            Output only. Server-defined resource path for
+            the target of the operation.
+        verb (str):
+            Output only. Name of the verb executed by the
+            operation.
+        status_message (str):
+            Output only. Human-readable status of the
+            operation, if any.
+        requested_cancellation (bool):
+            Output only. Identifies whether the user has requested
+            cancellation of the operation. Operations that have
+            successfully been cancelled have [Operation.error][] value
+            with a [google.rpc.Status.code][google.rpc.Status.code] of
+            1, corresponding to ``Code.CANCELLED``.
+        api_version (str):
+            Output only. API version used to start the
+            operation.
     """
 
     operation_metadata: "TransferOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="TransferOperationMetadata",
     )
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
+    end_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=timestamp_pb2.Timestamp,
+    )
+    target: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    verb: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    status_message: str = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    requested_cancellation: bool = proto.Field(
+        proto.BOOL,
+        number=7,
+    )
+    api_version: str = proto.Field(
+        proto.STRING,
+        number=8,
+    )
 
 
 class TransferOperationMetadata(proto.Message):
     r"""Represents the metadata of the long-running operation.
 
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
     Attributes:
-        create_time (google.protobuf.timestamp_pb2.Timestamp):
-            Output only. CCFE supplied fields BEGIN
-            The time the operation was created.
-        end_time (google.protobuf.timestamp_pb2.Timestamp):
-            Output only. The time the operation finished
-            running.
+        source_parallelstore (google.cloud.parallelstore_v1beta.types.SourceParallelstore):
+            Output only. Parallelstore source.
+
+            This field is a member of `oneof`_ ``source``.
+        source_gcs_bucket (google.cloud.parallelstore_v1beta.types.SourceGcsBucket):
+            Output only. Cloud Storage source.
+
+            This field is a member of `oneof`_ ``source``.
+        destination_gcs_bucket (google.cloud.parallelstore_v1beta.types.DestinationGcsBucket):
+            Output only. Cloud Storage destination.
+
+            This field is a member of `oneof`_ ``destination``.
+        destination_parallelstore (google.cloud.parallelstore_v1beta.types.DestinationParallelstore):
+            Output only. Parallelstore destination.
+
+            This field is a member of `oneof`_ ``destination``.
         counters (google.cloud.parallelstore_v1beta.types.TransferCounters):
-            Information about the progress of the
-            transfer operation.
-        source (str):
-            Required. The origin of the data transfer.
-        destination (str):
-            Required. The destination of the data
-            transfer.
+            Output only. Information about the progress
+            of the transfer operation.
         transfer_type (google.cloud.parallelstore_v1beta.types.TransferType):
-            The type of transfer occurring.
+            Output only. The type of transfer occurring.
     """
 
-    create_time: timestamp_pb2.Timestamp = proto.Field(
+    source_parallelstore: "SourceParallelstore" = proto.Field(
         proto.MESSAGE,
-        number=1,
-        message=timestamp_pb2.Timestamp,
+        number=7,
+        oneof="source",
+        message="SourceParallelstore",
     )
-    end_time: timestamp_pb2.Timestamp = proto.Field(
+    source_gcs_bucket: "SourceGcsBucket" = proto.Field(
         proto.MESSAGE,
-        number=2,
-        message=timestamp_pb2.Timestamp,
+        number=8,
+        oneof="source",
+        message="SourceGcsBucket",
+    )
+    destination_gcs_bucket: "DestinationGcsBucket" = proto.Field(
+        proto.MESSAGE,
+        number=9,
+        oneof="destination",
+        message="DestinationGcsBucket",
+    )
+    destination_parallelstore: "DestinationParallelstore" = proto.Field(
+        proto.MESSAGE,
+        number=10,
+        oneof="destination",
+        message="DestinationParallelstore",
     )
     counters: "TransferCounters" = proto.Field(
         proto.MESSAGE,
         number=3,
         message="TransferCounters",
     )
-    source: str = proto.Field(
-        proto.STRING,
-        number=4,
-    )
-    destination: str = proto.Field(
-        proto.STRING,
-        number=5,
-    )
     transfer_type: "TransferType" = proto.Field(
         proto.ENUM,
         number=6,
         enum="TransferType",
     )
```

### Comparing `google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/PKG-INFO` & `google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-parallelstore
-Version: 0.1.2
+Version: 0.2.0
 Summary: Google Cloud Parallelstore API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-parallelstore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-parallelstore-0.1.2/google_cloud_parallelstore.egg-info/SOURCES.txt` & `google-cloud-parallelstore-0.2.0/google_cloud_parallelstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/setup.py` & `google-cloud-parallelstore-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/tests/__init__.py` & `google-cloud-parallelstore-0.2.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/tests/unit/__init__.py` & `google-cloud-parallelstore-0.2.0/tests/unit/gapic/parallelstore_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-parallelstore-0.1.2/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py` & `google-cloud-parallelstore-0.2.0/tests/unit/gapic/parallelstore_v1beta/test_parallelstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -3308,30 +3308,26 @@
         transport="grpc",
     )
 
     # Populate all string fields in the request which are not UUID4
     # since we want to check that UUID4 are populated automatically
     # if they meet the requirements of AIP 4235.
     request = parallelstore.ImportDataRequest(
-        source_gcs_uri="source_gcs_uri_value",
-        destination_path="destination_path_value",
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.import_data), "__call__") as call:
         call.return_value.name = (
             "foo"  # operation_request.operation in compute client(s) expect a string.
         )
         client.import_data(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.ImportDataRequest(
-            source_gcs_uri="source_gcs_uri_value",
-            destination_path="destination_path_value",
             name="name_value",
         )
 
 
 def test_import_data_use_cached_wrapped_rpc():
     # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
     # instead of constructing them on each call
@@ -3599,30 +3595,26 @@
         transport="grpc",
     )
 
     # Populate all string fields in the request which are not UUID4
     # since we want to check that UUID4 are populated automatically
     # if they meet the requirements of AIP 4235.
     request = parallelstore.ExportDataRequest(
-        source_path="source_path_value",
-        destination_gcs_uri="destination_gcs_uri_value",
         name="name_value",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.export_data), "__call__") as call:
         call.return_value.name = (
             "foo"  # operation_request.operation in compute client(s) expect a string.
         )
         client.export_data(request=request)
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == parallelstore.ExportDataRequest(
-            source_path="source_path_value",
-            destination_gcs_uri="destination_gcs_uri_value",
             name="name_value",
         )
 
 
 def test_export_data_use_cached_wrapped_rpc():
     # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
     # instead of constructing them on each call
```

