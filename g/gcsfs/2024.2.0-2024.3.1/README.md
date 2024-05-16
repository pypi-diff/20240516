# Comparing `tmp/gcsfs-2024.2.0.tar.gz` & `tmp/gcsfs-2024.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsfs-2024.2.0.tar", last modified: Mon Feb  5 15:11:37 2024, max compression
+gzip compressed data, was "gcsfs-2024.3.1.tar", last modified: Mon Mar 18 20:04:18 2024, max compression
```

## Comparing `gcsfs-2024.2.0.tar` & `gcsfs-2024.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.760658 gcsfs-2024.2.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1593 2024-02-05 15:11:37.760569 gcsfs-2024.2.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.747564 gcsfs-2024.2.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.750996 gcsfs-2024.2.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2024.2.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     5203 2024-02-05 15:10:56.000000 gcsfs-2024.2.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/docs/source/developer.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2024.2.0/docs/source/fuse.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     6625 2024-02-05 15:10:56.000000 gcsfs-2024.2.0/docs/source/index.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.753591 gcsfs-2024.2.0/gcsfs/
--rw-r--r--   0 mdurant    (502) staff       (20)      266 2023-08-24 19:08:14.000000 gcsfs-2024.2.0/gcsfs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2024-02-05 15:11:37.761114 gcsfs-2024.2.0/gcsfs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/checkers.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.755021 gcsfs-2024.2.0/gcsfs/cli/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/gcsfs/cli/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/cli/gcsfuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    67542 2023-12-03 02:05:12.000000 gcsfs-2024.2.0/gcsfs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9137 2023-05-23 13:46:33.000000 gcsfs-2024.2.0/gcsfs/credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/gcsfs/dask_link.py
--rw-r--r--   0 mdurant    (502) staff       (20)    26286 2023-09-15 20:26:32.000000 gcsfs-2024.2.0/gcsfs/inventory_report.py
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/gcsfs/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5062 2023-10-06 19:10:11.000000 gcsfs-2024.2.0/gcsfs/retry.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.757822 gcsfs-2024.2.0/gcsfs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2024.2.0/gcsfs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/tests/conftest.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.758351 gcsfs-2024.2.0/gcsfs/tests/derived/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2023-08-25 15:30:21.000000 gcsfs-2024.2.0/gcsfs/tests/derived/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1163 2023-08-25 15:30:21.000000 gcsfs-2024.2.0/gcsfs/tests/derived/gcsfs_fixtures.py
--rw-r--r--   0 mdurant    (502) staff       (20)      324 2023-08-25 15:30:21.000000 gcsfs-2024.2.0/gcsfs/tests/derived/gcsfs_test.py
--rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/tests/settings.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/tests/test_checkers.py
--rw-r--r--   0 mdurant    (502) staff       (20)    45073 2023-12-03 02:05:12.000000 gcsfs-2024.2.0/gcsfs/tests/test_core.py
--rw-r--r--   0 mdurant    (502) staff       (20)      563 2023-05-23 13:46:33.000000 gcsfs-2024.2.0/gcsfs/tests/test_credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/tests/test_fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    28443 2023-09-15 20:26:32.000000 gcsfs-2024.2.0/gcsfs/tests/test_inventory_report.py
--rw-r--r--   0 mdurant    (502) staff       (20)      913 2023-09-15 20:26:32.000000 gcsfs-2024.2.0/gcsfs/tests/test_inventory_report_listing.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/tests/test_manyopens.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2677 2023-08-24 19:08:14.000000 gcsfs-2024.2.0/gcsfs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4377 2023-08-24 19:08:14.000000 gcsfs-2024.2.0/gcsfs/tests/test_retry.py
--rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2024.2.0/gcsfs/tests/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-05 15:11:37.760034 gcsfs-2024.2.0/gcsfs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1593 2024-02-05 15:11:37.000000 gcsfs-2024.2.0/gcsfs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1054 2024-02-05 15:11:37.000000 gcsfs-2024.2.0/gcsfs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-02-05 15:11:37.000000 gcsfs-2024.2.0/gcsfs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2024.2.0/gcsfs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2024-02-05 15:11:37.000000 gcsfs-2024.2.0/gcsfs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        6 2024-02-05 15:11:37.000000 gcsfs-2024.2.0/gcsfs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      129 2024-02-05 15:10:56.000000 gcsfs-2024.2.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      445 2024-02-05 15:11:37.760986 gcsfs-2024.2.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2024.2.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    86854 2023-08-24 19:08:14.000000 gcsfs-2024.2.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.089491 gcsfs-2024.3.1/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1593 2024-03-18 20:04:18.089400 gcsfs-2024.3.1/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.074098 gcsfs-2024.3.1/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.078510 gcsfs-2024.3.1/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2024.3.1/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     5427 2024-03-18 20:02:37.000000 gcsfs-2024.3.1/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/docs/source/developer.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2024.3.1/docs/source/fuse.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     7034 2024-03-18 19:46:49.000000 gcsfs-2024.3.1/docs/source/index.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.081213 gcsfs-2024.3.1/gcsfs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      266 2023-08-24 19:08:14.000000 gcsfs-2024.3.1/gcsfs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2024-03-18 20:04:18.089956 gcsfs-2024.3.1/gcsfs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/checkers.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.084240 gcsfs-2024.3.1/gcsfs/cli/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/gcsfs/cli/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/cli/gcsfuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    70545 2024-03-18 19:56:40.000000 gcsfs-2024.3.1/gcsfs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9137 2023-05-23 13:46:33.000000 gcsfs-2024.3.1/gcsfs/credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/gcsfs/dask_link.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    26286 2023-09-15 20:26:32.000000 gcsfs-2024.3.1/gcsfs/inventory_report.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/gcsfs/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5048 2024-03-18 19:56:40.000000 gcsfs-2024.3.1/gcsfs/retry.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.087808 gcsfs-2024.3.1/gcsfs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2024.3.1/gcsfs/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3876 2024-03-18 19:46:49.000000 gcsfs-2024.3.1/gcsfs/tests/conftest.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.088407 gcsfs-2024.3.1/gcsfs/tests/derived/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2023-08-25 15:30:21.000000 gcsfs-2024.3.1/gcsfs/tests/derived/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1163 2023-08-25 15:30:21.000000 gcsfs-2024.3.1/gcsfs/tests/derived/gcsfs_fixtures.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      324 2023-08-25 15:30:21.000000 gcsfs-2024.3.1/gcsfs/tests/derived/gcsfs_test.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/tests/settings.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/tests/test_checkers.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    46326 2024-03-18 20:02:37.000000 gcsfs-2024.3.1/gcsfs/tests/test_core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      563 2023-05-23 13:46:33.000000 gcsfs-2024.3.1/gcsfs/tests/test_credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/tests/test_fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    28443 2023-09-15 20:26:32.000000 gcsfs-2024.3.1/gcsfs/tests/test_inventory_report.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      913 2023-09-15 20:26:32.000000 gcsfs-2024.3.1/gcsfs/tests/test_inventory_report_listing.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/tests/test_manyopens.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2677 2023-08-24 19:08:14.000000 gcsfs-2024.3.1/gcsfs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4377 2023-08-24 19:08:14.000000 gcsfs-2024.3.1/gcsfs/tests/test_retry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2024.3.1/gcsfs/tests/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-18 20:04:18.088925 gcsfs-2024.3.1/gcsfs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1593 2024-03-18 20:04:18.000000 gcsfs-2024.3.1/gcsfs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1054 2024-03-18 20:04:18.000000 gcsfs-2024.3.1/gcsfs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-03-18 20:04:18.000000 gcsfs-2024.3.1/gcsfs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2024.3.1/gcsfs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2024-03-18 20:04:18.000000 gcsfs-2024.3.1/gcsfs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        6 2024-03-18 20:04:18.000000 gcsfs-2024.3.1/gcsfs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      129 2024-03-18 20:02:37.000000 gcsfs-2024.3.1/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      445 2024-03-18 20:04:18.089819 gcsfs-2024.3.1/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2024.3.1/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    86854 2023-08-24 19:08:14.000000 gcsfs-2024.3.1/versioneer.py
```

### Comparing `gcsfs-2024.2.0/LICENSE.txt` & `gcsfs-2024.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/PKG-INFO` & `gcsfs-2024.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2024.2.0
+Version: 2024.3.1
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: aiohttp!=4.0.0a0,!=4.0.0a1
 Requires-Dist: decorator>4.1.2
-Requires-Dist: fsspec==2024.2.0
+Requires-Dist: fsspec==2024.3.1
 Requires-Dist: google-auth>=1.2
 Requires-Dist: google-auth-oauthlib
 Requires-Dist: google-cloud-storage
 Requires-Dist: requests
 Provides-Extra: gcsfuse
 Requires-Dist: fusepy; extra == "gcsfuse"
 Provides-Extra: crc
```

### Comparing `gcsfs-2024.2.0/README.rst` & `gcsfs-2024.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/docs/source/api.rst` & `gcsfs-2024.3.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/docs/source/changelog.rst` & `gcsfs-2024.3.1/docs/source/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 Changelog
 =========
 
 Note: in some releases, there are no changes, because we always guarantee relasing in step
 with fsspec.
 
+2024.3.1
+--------
+
+* fix expiration= for sign() (#613)
+* do populate dircache in ls() (#612)
+* allow passing extra options to mkdir (#610)
+* credentials docs (#609)
+* retry in bulk rm (#608)
+* clean up loop on close (#606)
+
 2024.2.0
 --------
 
 * doc for passing tokens (#603)
 
 2023.12.2
 ---------
```

### Comparing `gcsfs-2024.2.0/docs/source/developer.rst` & `gcsfs-2024.3.1/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/docs/source/fuse.rst` & `gcsfs-2024.3.1/docs/source/fuse.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/docs/source/index.rst` & `gcsfs-2024.3.1/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -95,27 +95,41 @@
       be found, but it is often best to supply this anyway (only affects bucket-
       level operations).
 
     - if ``token='cloud'``, we assume we are running within google (compute
       or container engine) and fetch the credentials automatically from the
       metadata service.
 
-    - if ``token=dict(...)`` or ``token=<filepath>``, you may supply a token generated by the
-      gcloud_ utility; this is either a python dictionary, or the name of a file
-      containing the JSON returned by logging in with the gcloud CLI tool (e.g.,
-      ``~/.config/gcloud/application_default_credentials.json`` or
-      ``~/.config/gcloud/legacy_credentials/<YOUR GOOGLE USERNAME>/adc.json``)
-      or any value google ``Credentials`` object.
+    - if ``token=dict(...)`` or ``token=<filepath>``, you may supply a token
+      generated by the gcloud_ utility. This can be
+
+      - a python dictionary
+
+      - the path to a file containing the JSON returned by logging in with the
+        gcloud CLI tool (e.g.,
+        ``~/.config/gcloud/application_default_credentials.json`` or
+        ``~/.config/gcloud/legacy_credentials/<YOUR GOOGLE
+        USERNAME>/adc.json``)
+
+      - the path to a service account key
+
+      - a google.auth.credentials.Credentials_ object
+
+      Note that ``~`` will not be automatically expanded to the user home
+      directory, and must be manually expanded with a utility like
+      ``os.path.expanduser()``.
 
     - you can also generate tokens via Oauth2 in the browser using ``token='browser'``,
       which gcsfs then caches in a special file, ~/.gcs_tokens, and can subsequently be accessed with ``token='cache'``.
 
     - anonymous only access can be selected using ``token='anon'``, e.g. to access
       public resources such as 'anaconda-public-data'.
 
+.. _google.auth.credentials.Credentials: https://google-auth.readthedocs.io/en/master/reference/google.auth.credentials.html#google.auth.credentials.Credentials
+
 The acquired session tokens are *not* preserved when serializing the instances, so
 it is safe to pass them to worker processes on other machines if using in a
 distributed computation context. If credentials are given by a file path, however,
 then this file must exist on every machine.
 
 
 Integration
```

### Comparing `gcsfs-2024.2.0/gcsfs/checkers.py` & `gcsfs-2024.3.1/gcsfs/checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/cli/gcsfuse.py` & `gcsfs-2024.3.1/gcsfs/cli/gcsfuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/core.py` & `gcsfs-2024.3.1/gcsfs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 import json
 import logging
 import os
 import posixpath
 import re
 import warnings
 import weakref
-from datetime import datetime
+from datetime import datetime, timedelta
 from urllib.parse import parse_qs
 from urllib.parse import quote as quote_urllib
 from urllib.parse import urlsplit
 
 import fsspec
-from fsspec.asyn import AsyncFileSystem, sync, sync_wrapper
+from fsspec import asyn
 from fsspec.callbacks import NoOpCallback
 from fsspec.implementations.http import get_client
 from fsspec.utils import setup_logging, stringify_path
 
 from . import __version__ as version
 from .checkers import get_consistency_checker
 from .credentials import GoogleCredentials
 from .inventory_report import InventoryReport
-from .retry import retry_request, validate_response
+from .retry import errs, retry_request, validate_response
 
 logger = logging.getLogger("gcsfs")
 
 
 if "GCSFS_DEBUG" in os.environ:
     setup_logging(logger=logger, level=os.getenv("GCSFS_DEBUG"))
 
@@ -147,15 +147,15 @@
         )
     elif len(generations) == 0:
         return None
     else:
         return generations.pop()
 
 
-class GCSFileSystem(AsyncFileSystem):
+class GCSFileSystem(asyn.AsyncFileSystem):
     r"""
     Connect to Google Cloud Storage.
 
     The following modes of authentication are supported:
 
     - ``token=None``, GCSFS will attempt to guess your credentials in the
       following order: gcloud CLI default, gcsfs cached token, google compute
@@ -326,26 +326,34 @@
     def base(self):
         return f"{self._location}/storage/v1/"
 
     @property
     def project(self):
         return self.credentials.project
 
+    # Clean up the aiohttp session
+    #
+    # This can run from the main thread if invoked via the weakref callbcak.
+    # This can happen even if the `loop` parameter belongs to another thread
+    # (e.g. the fsspec IO worker). The control flow here is intended to attempt
+    # in-thread asynchronous cleanup first, then fallback to synchronous
+    # cleanup (which can handle cross-thread calls).
     @staticmethod
     def close_session(loop, session):
         if loop is not None and session is not None:
             if loop.is_running():
                 try:
-                    loop = asyncio.get_event_loop()
-                    loop.create_task(session.close())
+                    current_loop = asyncio.get_running_loop()
+                    current_loop.create_task(session.close())
                     return
                 except RuntimeError:
                     pass
+
                 try:
-                    sync(loop, session.close, timeout=0.1)
+                    asyn.sync(loop, session.close, timeout=0.1)
                 except fsspec.FSTimeoutError:
                     pass
             else:
                 pass
 
     async def _set_session(self):
         if self._session is None:
@@ -440,21 +448,22 @@
         if json_out:
             return json.loads(contents)
         elif info_out:
             return info
         else:
             return headers, contents
 
-    call = sync_wrapper(_call)
+    call = asyn.sync_wrapper(_call)
 
     @property
     def buckets(self):
         """Return list of available project buckets."""
         return [
-            b["name"] for b in sync(self.loop, self._list_buckets, timeout=self.timeout)
+            b["name"]
+            for b in asyn.sync(self.loop, self._list_buckets, timeout=self.timeout)
         ]
 
     def _process_object(self, bucket, object_metadata):
         """Process object resource into gcsfs object information format.
 
         Process GCS object resource via type casting and attribute updates to
         the cache-able gcsfs object information format. Returns an updated copy
@@ -480,15 +489,15 @@
 
     async def _make_bucket_requester_pays(self, path, state=True):
         # this is really some form of setACL/chmod
         # perhaps should be automatic if gcs.requester_pays
         json = {"billing": {"requesterPays": state}}
         await self._call("PATCH", f"b/{path}", json=json)
 
-    make_bucket_requester_pays = sync_wrapper(_make_bucket_requester_pays)
+    make_bucket_requester_pays = asyn.sync_wrapper(_make_bucket_requester_pays)
 
     async def _get_object(self, path):
         """Return object information at the given path."""
         bucket, key, generation = self.split_path(path)
 
         # Check if parent dir is in listing cache
         listing = self._ls_from_cache(path)
@@ -584,15 +593,15 @@
 
         use_snapshot_listing = inventory_report_info and inventory_report_info.get(
             "use_snapshot_listing"
         )
 
         # Don't cache prefixed/partial listings, in addition to
         # not using the inventory report service to do listing directly.
-        if not prefix and use_snapshot_listing is False:
+        if not prefix and not use_snapshot_listing:
             self.dircache[path] = out
         return out
 
     async def _do_list_objects(
         self, path, max_results=None, delimiter="/", prefix="", versions=False, **kwargs
     ):
         """Object listing for the given {bucket}/{prefix}/ path."""
@@ -825,42 +834,58 @@
         self,
         path,
         acl="projectPrivate",
         default_acl="bucketOwnerFullControl",
         location=None,
         create_parents=True,
         enable_versioning=False,
+        enable_object_retention=False,
+        iam_configuration=None,
         **kwargs,
     ):
         """
         New bucket
 
         If path is more than just a bucket, will create bucket if create_parents=True;
         otherwise is a noop. If create_parents is False and bucket does not exist,
-        will produce FileNotFFoundError.
+        will produce FileNotFoundError.
 
         Parameters
         ----------
         path: str
             bucket name. If contains '/' (i.e., looks like subdir), will
             have no effect because GCS doesn't have real directories.
         acl: string, one of bACLs
-            access for the bucket itself
+            access for the bucket itself. See:
+            https://cloud.google.com/storage/docs/access-control/lists#predefined-acl
         default_acl: str, one of ACLs
             default ACL for objects created in this bucket
         location: Optional[str]
             Location where buckets are created, like 'US' or 'EUROPE-WEST3'.
             If not provided, defaults to `self.default_location`.
             You can find a list of all available locations here:
             https://cloud.google.com/storage/docs/locations#available-locations
         create_parents: bool
             If True, creates the bucket in question, if it doesn't already exist
         enable_versioning: bool
             If True, creates the bucket in question with object versioning
             enabled.
+        enable_object_retention: bool
+            If True, creates the bucket in question with object retention
+            permanently enabled.
+        iam_configuration: dict
+            If provided, sets the IAM policy for the bucket. This argument
+            allows setting properties such as `{publicAccessPrevention: "enforced"}`
+            and `{"uniformBucketLevelAccess": {"enabled": True}}`. If passed, `acl`
+            and `default_acl` are explicitly ignored.
+        **kwargs
+            Additional parameters passed to the API call request body. See:
+            https://cloud.google.com/storage/docs/json_api/v1/buckets/insert#request-body
+            for all possible options. Pass nested parameters as dictionaries, e.g.:
+            `{"autoclass": {"enabled": True}}`
         """
         bucket, object, generation = self.split_path(path)
         if bucket in ["", "/"]:
             raise ValueError("Cannot create root bucket")
         if "/" in path and create_parents and await self._exists(bucket):
             # nothing to do
             return
@@ -871,26 +896,34 @@
 
         json_data = {"name": bucket}
         location = location or self.default_location
         if location:
             json_data["location"] = location
         if enable_versioning:
             json_data["versioning"] = {"enabled": True}
+        if iam_configuration:
+            json_data["iamConfiguration"] = iam_configuration
+            acl = None
+            default_acl = None
+        if kwargs:
+            json_data.update(kwargs)
+
         await self._call(
             method="POST",
             path="b",
             predefinedAcl=acl,
             project=self.project,
             predefinedDefaultObjectAcl=default_acl,
+            enableObjectRetention=str(enable_object_retention).lower(),
             json=json_data,
             json_out=True,
         )
         self.invalidate_cache(bucket)
 
-    mkdir = sync_wrapper(_mkdir)
+    mkdir = asyn.sync_wrapper(_mkdir)
 
     async def _rmdir(self, bucket):
         """Delete an empty bucket
 
         Parameters
         ----------
         bucket: str
@@ -900,15 +933,15 @@
         bucket = bucket.rstrip("/")
         if "/" in bucket:
             return
         await self._call("DELETE", "b/" + bucket, json_out=False)
         self.invalidate_cache(bucket)
         self.invalidate_cache("")
 
-    rmdir = sync_wrapper(_rmdir)
+    rmdir = asyn.sync_wrapper(_rmdir)
 
     def modified(self, path):
         return self.info(path)["mtime"]
 
     def created(self, path):
         return self.info(path)["ctime"]
 
@@ -1028,15 +1061,15 @@
         return out
 
     async def _getxattr(self, path, attr):
         """Get user-defined metadata attribute"""
         meta = (await self._info(path)).get("metadata", {})
         return meta[attr]
 
-    getxattr = sync_wrapper(_getxattr)
+    getxattr = asyn.sync_wrapper(_getxattr)
 
     async def _setxattrs(
         self,
         path,
         content_type=None,
         content_encoding=None,
         fixed_key_metadata=None,
@@ -1091,15 +1124,15 @@
             key,
             fields="metadata",
             json=i_json,
             json_out=True,
         )
         return o_json.get("metadata", {})
 
-    setxattrs = sync_wrapper(_setxattrs)
+    setxattrs = asyn.sync_wrapper(_setxattrs)
 
     async def _merge(self, path, paths, acl=None):
         """Concatenate objects within a single bucket"""
         bucket, key, generation = self.split_path(path)
         source = [{"name": self.split_path(p)[1]} for p in paths]
         await self._call(
             "POST",
@@ -1111,15 +1144,15 @@
             json={
                 "sourceObjects": source,
                 "kind": "storage#composeRequest",
                 "destination": {"name": key, "bucket": bucket},
             },
         )
 
-    merge = sync_wrapper(_merge)
+    merge = asyn.sync_wrapper(_merge)
 
     async def _cp_file(self, path1, path2, acl=None, **kwargs):
         """Duplicate remote file"""
         b1, k1, g1 = self.split_path(path1)
         b2, k2, g2 = self.split_path(path2)
         if g2:
             raise ValueError("Cannot write to specific object generation")
@@ -1156,27 +1189,31 @@
         if key:
             await self._call("DELETE", "b/{}/o/{}", bucket, key, generation=generation)
             self.invalidate_cache(posixpath.dirname(self._strip_protocol(path)))
         else:
             await self._rmdir(path)
 
     async def _rm_files(self, paths):
+        import random
+
         template = (
             "\n--===============7330845974216740156==\n"
             "Content-Type: application/http\n"
             "Content-Transfer-Encoding: binary\n"
             "Content-ID: <b29c5de2-0db4-490b-b421-6a51b598bd11+{i}>"
             "\n\nDELETE /storage/v1/b/{bucket}/o/{key}{query} HTTP/1.1\n"
             "Content-Type: application/json\n"
             "accept: application/json\ncontent-length: 0\n"
         )
-        errors = []
-        # Splitting requests into 100 chunk batches
+        out = []
+        # Splitting requests into batches
         # See https://cloud.google.com/storage/docs/batch
-        for chunk in _chunks(paths, 100):
+        for retry in range(1, 6):
+            remaining = []
+            chunk = paths
             parts = []
             for i, p in enumerate(chunk):
                 bucket, key, generation = self.split_path(p)
                 query = f"?generation={generation}" if generation else ""
                 parts.append(
                     template.format(
                         i=i + 1,
@@ -1193,65 +1230,93 @@
                     "Content-Type": 'multipart/mixed; boundary="=========='
                     '=====7330845974216740156=="'
                 },
                 data=body + "\n--===============7330845974216740156==--",
             )
 
             boundary = headers["Content-Type"].split("=", 1)[1]
-            parents = [self._parent(p) for p in paths]
-            [self.invalidate_cache(parent) for parent in parents + list(paths)]
+            parents = set(self._parent(p) for p in paths) | set(paths)
+            [self.invalidate_cache(parent) for parent in parents]
             txt = content.decode()
-            if any(
-                not ("200 OK" in c or "204 No Content" in c)
-                for c in txt.split(boundary)[1:-1]
-            ):
-                pattern = '"message": "([^"]+)"'
-                out = set(re.findall(pattern, txt))
-                errors.extend(out)
-
-        if errors:
-            raise OSError(errors)
+            responses = txt.split(boundary)[1:-1]
+            for path, response in zip(paths, responses):
+                m = re.search("HTTP/[0-9.]+ ([0-9]+)", response)
+                code = int(m.groups()[0]) if m else None
+                if code in [200, 204]:
+                    out.append(path)
+                elif code in errs and retry < 5:
+                    remaining.append(path)
+                else:
+                    msg = re.search("{(.*)}", response.replace("\n", ""))
+                    if msg:
+                        msg2 = re.search("({.*})", msg.groups()[0])
+                    else:
+                        msg2 = None
+                    if msg and msg2:
+                        out.append(OSError(msg2.groups()[0]))
+                    else:
+                        out.append(OSError(str(path, code)))
+            if remaining:
+                paths = remaining
+                await asyncio.sleep(min(random.random() + 2 ** (retry - 1), 32))
+            else:
+                break
+        return out
 
     @property
     def on_google(self):
         return "torage.googleapis.com" in self._location
 
     async def _rm(self, path, recursive=False, maxdepth=None, batchsize=20):
         paths = await self._expand_path(path, recursive=recursive, maxdepth=maxdepth)
         files = [p for p in paths if self.split_path(p)[1]]
         dirs = [p for p in paths if not self.split_path(p)[1]]
         if self.on_google:
             # emulators do not support batch
-            exs = await asyncio.gather(
-                *(
+            exs = sum(
+                await asyn._run_coros_in_chunks(
                     [
                         self._rm_files(files[i : i + batchsize])
                         for i in range(0, len(files), batchsize)
-                    ]
+                    ],
+                    return_exceptions=True,
                 ),
-                return_exceptions=True,
+                [],
             )
         else:
-            exs = await asyncio.gather(
-                *([self._rm_file(f) for f in files]),
-                return_exceptions=True,
+            exs = await asyn._run_coros_in_chunks(
+                [self._rm_file(f) for f in files], return_exceptions=True, batch_size=5
             )
 
-        exs = [
+        # buckets
+        exs.extend(
+            await asyncio.gather(
+                *[self._rmdir(d) for d in dirs], return_exceptions=True
+            )
+        )
+        errors = [
             ex
             for ex in exs
-            if ex is not None
+            if isinstance(ex, Exception)
             and "No such object" not in str(ex)
             and not isinstance(ex, FileNotFoundError)
         ]
-        if exs:
-            raise exs[0]
-        await asyncio.gather(*[self._rmdir(d) for d in dirs])
+        if errors:
+            raise errors[0]
+        exs = [
+            ex
+            for ex in exs
+            if "No such object" not in str(ex) and not isinstance(ex, FileNotFoundError)
+        ]
+        if not exs:
+            # nothing got deleted
+            raise FileNotFoundError(path)
+        return exs
 
-    rm = sync_wrapper(_rm)
+    rm = asyn.sync_wrapper(_rm)
 
     async def _pipe_file(
         self,
         path,
         data,
         metadata=None,
         consistency=None,
@@ -1591,22 +1656,28 @@
         Returns
         -------
         URL : str
             The signed URL
         """
         from google.cloud import storage
 
-        bucket, key, generation = self.split_path(path)
         client = storage.Client(
-            credentials=self.credentials.credentials, project=self.project
+            credentials=self.credentials.credentials,
+            project=self.project,
         )
+
+        bucket, key, generation = self.split_path(path)
         bucket = client.bucket(bucket)
         blob = bucket.blob(key)
+
         return blob.generate_signed_url(
-            expiration=expiration, generation=generation, **kwargs
+            expiration=timedelta(seconds=expiration),
+            generation=generation,
+            api_access_endpoint=self._endpoint,
+            **kwargs,
         )
 
 
 GoogleCredentials.load_tokens()
 
 
 class GCSFile(fsspec.spec.AbstractBufferedFile):
@@ -1792,15 +1863,15 @@
     def commit(self):
         """If not auto-committing, finalize file"""
         self.autocommit = True
         self._upload_chunk(final=True)
 
     def _initiate_upload(self):
         """Create multi-upload"""
-        self.location = sync(
+        self.location = asyn.sync(
             self.gcsfs.loop,
             initiate_upload,
             self.gcsfs,
             self.bucket,
             self.key,
             self.content_type,
             self.metadata,
@@ -1822,15 +1893,15 @@
         self.location = None
         self.closed = True
 
     def _simple_upload(self):
         """One-shot upload, less than 5MB"""
         self.buffer.seek(0)
         data = self.buffer.read()
-        sync(
+        asyn.sync(
             self.gcsfs.loop,
             simple_upload,
             self.gcsfs,
             self.bucket,
             self.key,
             data,
             self.metadata,
```

### Comparing `gcsfs-2024.2.0/gcsfs/credentials.py` & `gcsfs-2024.3.1/gcsfs/credentials.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/inventory_report.py` & `gcsfs-2024.3.1/gcsfs/inventory_report.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/retry.py` & `gcsfs-2024.3.1/gcsfs/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,26 @@
     requests.exceptions.ContentDecodingError,
     google.auth.exceptions.RefreshError,
     aiohttp.client_exceptions.ClientError,
     ChecksumError,
 )
 
 
+errs = list(range(500, 505)) + [
+    # Request Timeout
+    408,
+    # Too Many Requests
+    429,
+]
+errs = set(errs + [str(e) for e in errs])
+
+
 def is_retriable(exception):
     """Returns True if this exception is retriable."""
-    errs = list(range(500, 505)) + [
-        # Request Timeout
-        408,
-        # Too Many Requests
-        429,
-    ]
-    errs += [str(e) for e in errs]
+
     if isinstance(exception, HttpError):
         return exception.code in errs
 
     return isinstance(exception, RETRIABLE_EXCEPTIONS)
 
 
 def validate_response(status, content, path, args=None):
```

### Comparing `gcsfs-2024.2.0/gcsfs/tests/conftest.py` & `gcsfs-2024.3.1/gcsfs/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     if "STORAGE_EMULATOR_HOST" in os.environ:
         # assume using real API or otherwise have a server already set up
         yield os.getenv("STORAGE_EMULATOR_HOST")
         return
     container = "gcsfs_test"
     cmd = (
         "docker run -d -p 4443:4443 --name gcsfs_test fsouza/fake-gcs-server:latest -scheme "
-        "http -public-host http://localhost:4443 -external-url http://localhost:4443 "
+        "http -public-host 0.0.0.0:4443 -external-url http://localhost:4443 "
         "-backend memory"
     )
     stop_docker(container)
     subprocess.check_output(shlex.split(cmd))
     url = "http://0.0.0.0:4443"
     timeout = 10
     while True:
```

### Comparing `gcsfs-2024.2.0/gcsfs/tests/derived/gcsfs_fixtures.py` & `gcsfs-2024.3.1/gcsfs/tests/derived/gcsfs_fixtures.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_checkers.py` & `gcsfs-2024.3.1/gcsfs/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_core.py` & `gcsfs-2024.3.1/gcsfs/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import datetime
 import io
 import os
 from builtins import FileNotFoundError
+from datetime import datetime, timezone
 from itertools import chain
 from unittest import mock
 from urllib.parse import parse_qs, unquote, urlparse
 from uuid import uuid4
 
 import fsspec.core
 import pytest
@@ -22,20 +22,35 @@
 from gcsfs.tests.utils import tempdir, tmpfile
 
 TEST_BUCKET = gcsfs.tests.settings.TEST_BUCKET
 TEST_PROJECT = gcsfs.tests.settings.TEST_PROJECT
 TEST_REQUESTER_PAYS_BUCKET = gcsfs.tests.settings.TEST_REQUESTER_PAYS_BUCKET
 
 
-def test_simple(gcs):
-    assert not GoogleCredentials.tokens
+def test_simple(gcs, monkeypatch):
+    monkeypatch.setattr(GoogleCredentials, "tokens", None)
     gcs.ls(TEST_BUCKET)  # no error
     gcs.ls("/" + TEST_BUCKET)  # OK to lead with '/'
 
 
+def test_dircache_filled(gcs):
+    assert not dict(gcs.dircache)
+    gcs.ls(TEST_BUCKET)
+    assert len(gcs.dircache) == 1
+    gcs.dircache[TEST_BUCKET][0]["CHECK"] = True
+    out = gcs.ls(TEST_BUCKET, detail=True)
+    assert [o for o in out if o.get("CHECK", None)]
+
+    gcs.invalidate_cache()
+    assert not dict(gcs.dircache)
+
+    gcs.find(TEST_BUCKET)
+    assert len(gcs.dircache)
+
+
 def test_many_connect(docker_gcs):
     from multiprocessing.pool import ThreadPool
 
     GCSFileSystem(endpoint_url=docker_gcs)
 
     def task(i):
         GCSFileSystem(endpoint_url=docker_gcs).ls("")
@@ -121,15 +136,15 @@
     assert gcs.info(fn)["contentType"] == "application/octet-stream"
 
 
 def test_info(gcs):
     gcs.touch(a)
     assert gcs.info(a) == gcs.ls(a, detail=True)[0]
 
-    today = datetime.datetime.utcnow().date().isoformat()
+    today = datetime.utcnow().date().isoformat()
     assert gcs.created(a).isoformat().startswith(today)
     assert gcs.modified(a).isoformat().startswith(today)
     # Check conformance with expected info attribute names.
     assert gcs.info(a)["ctime"] == gcs.created(a)
     assert gcs.info(a)["mtime"] == gcs.modified(a)
 
 
@@ -179,17 +194,16 @@
 
 def test_rm(gcs):
     assert not gcs.exists(a)
     gcs.touch(a)
     assert gcs.exists(a)
     gcs.rm(a)
     assert not gcs.exists(a)
-    # silently ignored for now
-    # with pytest.raises((OSError, IOError)):
-    #    gcs.rm(TEST_BUCKET + "/nonexistent")
+    with pytest.raises((OSError, IOError)):
+        gcs.rm(TEST_BUCKET + "/nonexistent")
     with pytest.raises((OSError, IOError)):
         gcs.rm("nonexistent")
 
 
 def test_rm_batch(gcs):
     gcs.touch(a)
     gcs.touch(b)
@@ -933,16 +947,14 @@
         maxResults=100,
         info_out=True,
     )
     assert r.headers["User-Agent"] == "python-gcsfs/" + version
 
 
 def test_user_project_fallback_google_default(monkeypatch):
-    import fsspec
-
     monkeypatch.setattr(gcsfs.core, "DEFAULT_PROJECT", "my_default_project")
     monkeypatch.setattr(fsspec.config, "conf", {})
     monkeypatch.setattr(
         gcsfs.credentials.gauth,
         "default",
         lambda *__, **_: (requests.Session(), "my_default_project"),
     )
@@ -1474,7 +1486,32 @@
         f"{TEST_BUCKET}/nested/file1",
         f"{TEST_BUCKET}/nested/file2",
         f"{TEST_BUCKET}/nested/nested2",
     ]
 
     with pytest.raises(ValueError, match="maxdepth must be at least 1"):
         gcs.find(f"{TEST_BUCKET}/nested", maxdepth=0)
+
+
+def test_sign(gcs, monkeypatch):
+    file = TEST_BUCKET + "/test.jpg"
+    with gcs.open(file, "wb") as f:
+        f.write(b"This is a test string")
+    assert gcs.cat(file) == b"This is a test string"
+
+    # `sign` is creating a google Client on its own, it needs a realistically
+    # looking credentials file.
+    if not gcs.on_google:
+        monkeypatch.setenv(
+            "GOOGLE_APPLICATION_CREDENTIALS",
+            os.path.dirname(__file__) + "/fake-service-account-credentials.json",
+        )
+
+    current_ts_utc = int(datetime.now(tz=timezone.utc).timestamp())
+    result = gcs.sign(file)
+
+    # Check it here since emulator doesn't really validate those values
+    params = parse_qs(urlparse(result).query)
+    assert int(params["Expires"][0]) >= current_ts_utc + 100
+
+    response = requests.get(result)
+    assert response.text == "This is a test string"
```

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_credentials.py` & `gcsfs-2024.3.1/gcsfs/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_fuse.py` & `gcsfs-2024.3.1/gcsfs/tests/test_fuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_inventory_report.py` & `gcsfs-2024.3.1/gcsfs/tests/test_inventory_report.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_inventory_report_listing.py` & `gcsfs-2024.3.1/gcsfs/tests/test_inventory_report_listing.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_manyopens.py` & `gcsfs-2024.3.1/gcsfs/tests/test_manyopens.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_mapping.py` & `gcsfs-2024.3.1/gcsfs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/test_retry.py` & `gcsfs-2024.3.1/gcsfs/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs/tests/utils.py` & `gcsfs-2024.3.1/gcsfs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/gcsfs.egg-info/PKG-INFO` & `gcsfs-2024.3.1/gcsfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2024.2.0
+Version: 2024.3.1
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: aiohttp!=4.0.0a0,!=4.0.0a1
 Requires-Dist: decorator>4.1.2
-Requires-Dist: fsspec==2024.2.0
+Requires-Dist: fsspec==2024.3.1
 Requires-Dist: google-auth>=1.2
 Requires-Dist: google-auth-oauthlib
 Requires-Dist: google-cloud-storage
 Requires-Dist: requests
 Provides-Extra: gcsfuse
 Requires-Dist: fusepy; extra == "gcsfuse"
 Provides-Extra: crc
```

### Comparing `gcsfs-2024.2.0/gcsfs.egg-info/SOURCES.txt` & `gcsfs-2024.3.1/gcsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/setup.py` & `gcsfs-2024.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2024.2.0/versioneer.py` & `gcsfs-2024.3.1/versioneer.py`

 * *Files identical despite different names*

