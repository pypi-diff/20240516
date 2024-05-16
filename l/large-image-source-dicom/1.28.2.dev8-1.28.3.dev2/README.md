# Comparing `tmp/large-image-source-dicom-1.28.2.dev8.tar.gz` & `tmp/large-image-source-dicom-1.28.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.28.2.dev8.tar", last modified: Wed Apr 24 20:02:10 2024, max compression
+gzip compressed data, was "large-image-source-dicom-1.28.3.dev2.tar", last modified: Thu May 16 16:47:00 2024, max compression
```

## Comparing `large-image-source-dicom-1.28.2.dev8.tar` & `large-image-source-dicom-1.28.3.dev2.tar`

### file list

```diff
@@ -1,49 +1,46 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.510041 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15406 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.514042 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/assetstore/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3142 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/assetstore/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22975 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3912 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/assetstore/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/dicom_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/dicom_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/dicomweb_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/girder_plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3319 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.514042 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/constants.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.514042 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/models/AssetstoreModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.514042 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/assetstoreImport.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/AssetstoresView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      236 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/AuthOptions.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3469 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/DICOMwebImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1774 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-24 20:02:10.000000 large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2753 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/test_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/test_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1407 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/test_dicom/test_web_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:02:10.518041 large-image-source-dicom-1.28.2.dev8/test_dicom/web_client_specs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9427 2024-04-24 19:59:45.000000 large-image-source-dicom-1.28.2.dev8/test_dicom/web_client_specs/dicomWebSpec.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.853803 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15406 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.853803 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/assetstore/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3142 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/assetstore/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24183 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3130 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/assetstore/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/dicom_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/dicom_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2625 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/dicomweb_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/girder_plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3319 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       96 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/constants.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4098 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/assetstoreImport.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      257 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/AssetstoresView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      236 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/AuthOptions.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3739 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/DICOMwebImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1659 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1097 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1666 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-05-16 16:47:00.000000 large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2828 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/test_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/test_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1407 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/test_dicom/test_web_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:47:00.857803 large-image-source-dicom-1.28.3.dev2/test_dicom/web_client_specs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9436 2024-05-16 16:44:45.000000 large-image-source-dicom-1.28.3.dev2/test_dicom/web_client_specs/dicomWebSpec.js
```

### Comparing `large-image-source-dicom-1.28.2.dev8/LICENSE` & `large-image-source-dicom-1.28.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/PKG-INFO` & `large-image-source-dicom-1.28.3.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: wsidicom>=0.9.0
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
+Requires-Dist: girder>=3.2.3; extra == "girder"
 
 A DICOM tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-dicom-1.28.2.dev8/README.rst` & `large-image-source-dicom-1.28.3.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/assetstore/__init__.py` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/assetstore/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import cherrypy
 import requests
 from large_image_source_dicom.dicom_tags import dicom_key_to_tag
 from large_image_source_dicom.dicomweb_utils import get_dicomweb_metadata
 from requests.exceptions import HTTPError
 
 from girder.api.rest import setContentDisposition, setResponseHeader
@@ -390,39 +392,18 @@
 
         try:
             # The DICOM file size is equal to the Content-Length
             return int(content_length)
         except ValueError:
             return
 
-    def importData(self, parent, parentType, params, progress, user, **kwargs):
-        """
-        Import DICOMweb WSI instances from a DICOMweb server.
-
-        :param parent: The parent object to import into.
-        :param parentType: The model type of the parent object.
-        :type parentType: str
-        :param params: Additional parameters required for the import process.
-            This dictionary may include the following keys:
-
-            :limit: (optional) limit the number of studies imported.
-            :search_filters: (optional) a dictionary of additional search
-                filters to use with dicomweb_client's `search_for_series()`
-                function.
-
-        :type params: dict
-        :param progress: Object on which to record progress if possible.
-        :type progress: :py:class:`girder.utility.progress.ProgressContext`
-        :param user: The Girder user performing the import.
-        :type user: dict or None
-        :return: a list of items that were created
-        """
+    def _importData(self, parent, parentType, params, progress, user):
         if parentType not in ('folder', 'user', 'collection'):
             msg = f'Invalid parent type: {parentType}'
-            raise RuntimeError(msg)
+            raise ValidationException(msg)
 
         limit = params.get('limit')
         search_filters = params.get('search_filters', {})
 
         meta = self.assetstore_meta
 
         client = _create_dicomweb_client(meta)
@@ -508,14 +489,73 @@
                 # file['size'] = self._infer_file_size(file)
                 file = File().save(file)
 
             items.append(item)
 
         return items
 
+    def importData(self, parent, parentType, params, progress, user, **kwargs):
+        """
+        Import DICOMweb WSI instances from a DICOMweb server.
+
+        :param parent: The parent object to import into.
+        :param parentType: The model type of the parent object.
+        :type parentType: str
+        :param params: Additional parameters required for the import process.
+            This dictionary may include the following keys:
+
+            :limit: (optional) limit the number of studies imported.
+            :filters: (optional) a dictionary/JSON string of additional search
+                filters to use with dicomweb_client's `search_for_series()`
+                function.
+
+        :type params: dict
+        :param progress: Object on which to record progress if possible.
+        :type progress: :py:class:`girder.utility.progress.ProgressContext`
+        :param user: The Girder user performing the import.
+        :type user: dict or None
+        :return: a list of items that were created
+        """
+        # Validate the parameters
+        limit = params.get('limit') or None
+        if limit is not None:
+            error_msg = f'Invalid limit: {limit}'
+            try:
+                limit = int(limit)
+            except ValueError:
+                raise ValidationException(error_msg)
+
+            if limit < 1:
+                raise ValidationException(error_msg)
+
+        search_filters = params.get('filters', {})
+        if isinstance(search_filters, str):
+            try:
+                search_filters = json.loads(search_filters)
+            except json.JSONDecodeError as e:
+                msg = f'Invalid filters: "{params.get("filters")}". {e}'
+                raise ValidationException(msg)
+
+        items = self._importData(
+            parent,
+            parentType,
+            {
+                'limit': limit,
+                'search_filters': search_filters,
+            },
+            progress,
+            user,
+        )
+
+        if not items:
+            msg = 'No studies matching the search filters were found'
+            raise ValidationException(msg)
+
+        return items
+
     @property
     def auth_session(self):
         return _create_auth_session(self.assetstore_meta)
 
     def getFileSize(self, file):
         # This function will compute the size of the DICOM file (a potentially
         # expensive operation, since it may have to stream the whole file).
```

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/dicom_metadata.py` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/dicomweb_utils.py` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/dicomweb_utils.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/package.json` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/package.json`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/assetstoreImport.pug` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/assetstoreImport.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/AssetstoresView.js` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/DICOMwebImportView.js` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/DICOMwebImportView.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -3,14 +3,21 @@
 import BrowserWidget from '@girder/core/views/widgets/BrowserWidget';
 import router from '@girder/core/router';
 import View from '@girder/core/views/View';
 import {
     restRequest
 } from '@girder/core/rest';
 
+import {
+    assetstoreImportViewMap
+} from '@girder/core/views/body/AssetstoresView';
+import {
+    AssetstoreType
+} from '@girder/core/constants';
+
 import DWASImportTemplate from '../templates/assetstoreImport.pug';
 
 const DICOMwebImportView = View.extend({
     events: {
         'submit .g-dwas-import-form': function(e) {
             e.preventDefault();
             this.$('.g-validation-failed-message').empty();
@@ -22,33 +29,33 @@
 
             if (!destinationId) {
                 this.$('.g-validation-failed-message').html('Invalid Destination ID');
                 return;
             }
 
             this.$('.g-submit-dwas-import').addClass('disabled');
-            this.model.off().on('g:imported', function() {
+            this.assetstore.off().on('g:imported', function() {
                 router.navigate(destinationType + '/' + destinationId, {
                     trigger: true
                 });
             }, this).on('g:error', function(err) {
                 this.$('.g-submit-dwas-import').removeClass('disabled');
                 this.$('.g-validation-failed-message').html(err.responseJSON.message);
-            }, this).dicomwebImport({
+            }, this).import({
                 destinationId,
                 destinationType,
                 limit,
                 filters,
                 progress: true
             });
         },
         'click .g-open-browser': '_openBrowser'
     },
 
-    initialize: function() {
+    initialize: function(settings) {
         this._browserWidgetView = new BrowserWidget({
             parentView: this,
             titleText: 'Destination',
             helpText: 'Browse to a location to select it as the destination.',
             submitText: 'Select Destination',
             validate: function(model) {
                 const isValid = $.Deferred();
@@ -77,24 +84,27 @@
             }).done((result) => {
                 // Only add the resource path if the value wasn't altered
                 if (this.$('#g-dwas-import-dest-id').val() === val.id) {
                     this.$('#g-dwas-import-dest-id').val(`${val.id} (${result})`);
                 }
             });
         });
+        this.assetstore = settings.assetstore;
         this.render();
     },
 
     render: function() {
         this.$el.html(DWASImportTemplate({
-            assetstore: this.model
+            assetstore: this.assetstore
         }));
 
         return this;
     },
 
     _openBrowser: function() {
         this._browserWidgetView.setElement($('#g-dialog-container')).render();
     }
 });
 
+assetstoreImportViewMap[AssetstoreType.DICOMWEB] = DICOMwebImportView;
+
 export default DICOMwebImportView;
```

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/EditAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom/web_client/views/NewAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: wsidicom>=0.9.0
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
+Requires-Dist: girder>=3.2.3; extra == "girder"
 
 A DICOM tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-dicom-1.28.2.dev8/large_image_source_dicom.egg-info/SOURCES.txt` & `large-image-source-dicom-1.28.3.dev2/large_image_source_dicom.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 large_image_source_dicom.egg-info/top_level.txt
 large_image_source_dicom/assetstore/__init__.py
 large_image_source_dicom/assetstore/dicomweb_assetstore_adapter.py
 large_image_source_dicom/assetstore/rest.py
 large_image_source_dicom/web_client/constants.js
 large_image_source_dicom/web_client/main.js
 large_image_source_dicom/web_client/package.json
-large_image_source_dicom/web_client/routes.js
-large_image_source_dicom/web_client/models/AssetstoreModel.js
 large_image_source_dicom/web_client/templates/assetstoreImport.pug
 large_image_source_dicom/web_client/templates/dicomwebAssetstoreCreate.pug
 large_image_source_dicom/web_client/templates/dicomwebAssetstoreEditFields.pug
 large_image_source_dicom/web_client/templates/dicomwebAssetstoreImportButton.pug
 large_image_source_dicom/web_client/templates/dicomwebAssetstoreMixins.pug
 large_image_source_dicom/web_client/views/AssetstoresView.js
 large_image_source_dicom/web_client/views/AuthOptions.js
```

### Comparing `large-image-source-dicom-1.28.2.dev8/setup.py` & `large-image-source-dicom-1.28.3.dev2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,19 +37,22 @@
         'dicom = large_image_source_dicom:DICOMFileTileSource',
     ],
     'girder_large_image.source': [
         'dicom = large_image_source_dicom.girder_source:DICOMGirderTileSource',
     ],
 }
 
+girder_extras = [f'girder-large-image{limit_version}']
+
 if sys.version_info >= (3, 9):
     # For Python >= 3.9, include the DICOMweb plugin
     entry_points['girder.plugin'] = [
         'dicomweb = large_image_source_dicom.girder_plugin:DICOMwebPlugin',
     ]
+    girder_extras.append('girder>=3.2.3')
 
 setup(
     name='large-image-source-dicom',
     use_scm_version={'root': '../..', 'local_scheme': prerelease_local_scheme,
                      'fallback_version': '0.0.0'},
     description=description,
     long_description=long_description,
@@ -67,15 +70,15 @@
         'Programming Language :: Python :: 3.12',
     ],
     install_requires=[
         f'large-image{limit_version}',
         'wsidicom>=0.9.0',
     ],
     extras_require={
-        'girder': f'girder-large-image{limit_version}',
+        'girder': girder_extras,
     },
     include_package_data=True,
     keywords='large_image, tile source',
     packages=find_packages(exclude=['test', 'test.*', 'test_dicom', 'test_dicom.*']),
     url='https://github.com/girder/large_image',
     python_requires='>=3.8',
     entry_points=entry_points,
```

### Comparing `large-image-source-dicom-1.28.2.dev8/test_dicom/test_web_client.py` & `large-image-source-dicom-1.28.3.dev2/test_dicom/test_web_client.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.28.2.dev8/test_dicom/web_client_specs/dicomWebSpec.js` & `large-image-source-dicom-1.28.3.dev2/test_dicom/web_client_specs/dicomWebSpec.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -139,28 +139,28 @@
 
             // Test error for an invalid limit
             $('#g-dwas-import-limit').val('1.3');
             $('.g-submit-assetstore-import').trigger('click');
         });
 
         waitsFor(function() {
-            return $('.g-validation-failed-message').html() === 'Invalid limit';
+            return $('.g-validation-failed-message').html() === 'Invalid limit: 1.3';
         }, 'Invalid limit check (float)');
 
         runs(function() {
             // Make sure this is cleared (we will be checking the same message).
             $('.g-validation-failed-message').html('');
 
             // Test error for negative limit
             $('#g-dwas-import-limit').val('-1');
             $('.g-submit-assetstore-import').trigger('click');
         });
 
         waitsFor(function() {
-            return $('.g-validation-failed-message').html() === 'Invalid limit';
+            return $('.g-validation-failed-message').html() === 'Invalid limit: -1';
         }, 'Invalid limit check (negative)');
 
         runs(function() {
             // Fix the limit
             $('#g-dwas-import-limit').val('1');
 
             // Test error for invalid JSON in the filters parameter
```

