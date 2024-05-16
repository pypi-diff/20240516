# Comparing `tmp/ckanext-create_typed_package-0.1.4.tar.gz` & `tmp/ckanext_create_typed_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-create_typed_package-0.1.4.tar", last modified: Wed Oct 19 06:04:37 2022, max compression
+gzip compressed data, was "ckanext_create_typed_package-0.2.0.tar", last modified: Thu May 16 11:39:06 2024, max compression
```

## Comparing `ckanext-create_typed_package-0.1.4.tar` & `ckanext_create_typed_package-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      174 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2470 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1960 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.104819 ckanext-create_typed_package-0.1.4/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.104819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.104819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      135 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/assets/resource.config
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.104819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/assets/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3023 2022-10-19 06:03:58.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/assets/scripts/package-type-selector.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      207 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      234 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1968 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      306 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1149 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.064819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/create_typed_package/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/create_typed_package/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       57 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/create_typed_package/snippets/asset.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/package/ctp_select_dataset_type.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/package/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      423 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/package/snippets/ctp_select_dataset_type_form.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      374 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      111 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      945 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/tests/test_view.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1012 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2470 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1379 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      156 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-10-19 06:04:37.000000 ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      218 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-11 12:48:41.000000 ckanext-create_typed_package-0.1.4/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      879 2022-10-19 06:04:37.114819 ckanext-create_typed_package-0.1.4/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3528 2022-10-19 06:04:20.000000 ckanext-create_typed_package-0.1.4/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.438988 ckanext_create_typed_package-0.2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      174 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2497 2024-05-16 11:39:06.438988 ckanext_create_typed_package-0.2.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1960 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      135 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/assets/resource.config
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/assets/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3047 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/assets/scripts/package-type-selector.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      207 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      234 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1968 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      306 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1149 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.432321 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/create_typed_package/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/create_typed_package/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       57 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/create_typed_package/snippets/asset.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/package/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/package/ctp_select_dataset_type.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/package/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      423 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/package/snippets/ctp_select_dataset_type_form.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      374 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      111 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      945 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/tests/test_view.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1012 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:39:06.435655 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2497 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1379 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      156 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       12 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-05-16 11:39:06.000000 ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      218 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-05-16 11:38:40.000000 ckanext_create_typed_package-0.2.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      879 2024-05-16 11:39:06.438988 ckanext_create_typed_package-0.2.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3528 2024-05-16 11:38:57.000000 ckanext_create_typed_package-0.2.0/setup.py
```

### Comparing `ckanext-create_typed_package-0.1.4/LICENSE` & `ckanext_create_typed_package-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/PKG-INFO` & `ckanext_create_typed_package-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ckanext-create_typed_package
-Version: 0.1.4
+Version: 0.2.0
 Summary: Select dataset type when adding new data
 Home-page: https://github.com/DataShades/ckanext-create_typed_package
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN extension
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ckantoolkit
 
 [![Tests](https://github.com/DataShades/ckanext-create_typed_package/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/DataShades/ckanext-create_typed_package/actions)
 
 # ckanext-create_typed_package
 
 
 Add dataset type selector to the "Add dataset" button.
```

### Comparing `ckanext-create_typed_package-0.1.4/README.md` & `ckanext_create_typed_package-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/assets/scripts/package-type-selector.js` & `ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/assets/scripts/package-type-selector.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 ckan.module("ctp-type-selector", function($, _) {
     "use strict";
     var modalTpl = [
         '<div role="alertdialog" aria-modal="true" aria-labelledby="ds_creation_label" aria-describedby="field-ctp-package-type" class="modal fade" tabindex="-1">',
         '<div class="modal-dialog">',
         '<div class="modal-content">',
         '<div class="modal-header">',
-        '<button type="button" class="close" data-dismiss="modal">×</button>',
         '<h3 id="ds_creation_label" class="modal-title"></h3>',
+        '<button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>',
         "</div>",
         '<div class="modal-body">',
 
         '<div class="control-group form-group control-medium">',
         '<label for="field-ctp-package-type" class="control-label"></label>',
         '<div class="controls">',
         '<select id="field-ctp-package-type" class="form-control">',
```

### Comparing `ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/logic/action.py` & `ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/plugin.py` & `ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/tests/test_view.py` & `ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/ckanext/create_typed_package/views.py` & `ckanext_create_typed_package-0.2.0/ckanext/create_typed_package/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/PKG-INFO` & `ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: ckanext-create-typed-package
-Version: 0.1.4
+Name: ckanext-create_typed_package
+Version: 0.2.0
 Summary: Select dataset type when adding new data
 Home-page: https://github.com/DataShades/ckanext-create_typed_package
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN extension
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ckantoolkit
 
 [![Tests](https://github.com/DataShades/ckanext-create_typed_package/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/DataShades/ckanext-create_typed_package/actions)
 
 # ckanext-create_typed_package
 
 
 Add dataset type selector to the "Add dataset" button.
```

### Comparing `ckanext-create_typed_package-0.1.4/ckanext_create_typed_package.egg-info/SOURCES.txt` & `ckanext_create_typed_package-0.2.0/ckanext_create_typed_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/setup.cfg` & `ckanext_create_typed_package-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-create_typed_package-0.1.4/setup.py` & `ckanext_create_typed_package-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='''ckanext-create_typed_package''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.1.4',
+    version='0.2.0',
 
     description='''Select dataset type when adding new data''',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/DataShades/'\
```

