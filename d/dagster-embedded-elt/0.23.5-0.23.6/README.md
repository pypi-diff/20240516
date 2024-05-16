# Comparing `tmp/dagster-embedded-elt-0.23.5.tar.gz` & `tmp/dagster-embedded-elt-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.5.tar", last modified: Thu May  9 17:55:27 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.6.tar", last modified: Thu May 16 20:12:27 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.5.tar` & `dagster-embedded-elt-0.23.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:26.992084 dagster-embedded-elt-0.23.5/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:26.996084 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5804 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    20594 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:26.992084 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.695878 dagster-embedded-elt-0.23.6/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5804 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    20594 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.695878 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/setup.py
```

### Comparing `dagster-embedded-elt-0.23.5/LICENSE` & `dagster-embedded-elt-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/PKG-INFO` & `dagster-embedded-elt-0.23.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.5
+Version: 0.23.6
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
             @dlt_assets(
                 dlt_source=hubspot(include_history=True),
                 dlt_pipeline=pipeline(
                     pipeline_name="hubspot",
                     dataset_name="hubspot",
                     destination="snowflake",
+                    progress="log",
                 ),
                 name="hubspot",
                 group_name="hubspot",
                 dlt_dagster_translator=HubspotDltDagsterTranslator(),
             )
             def hubspot_assets(context: AssetExecutionContext, dlt: DltDagsterResource):
                 yield from dlt.run(context=context)
@@ -65,14 +66,15 @@
                 dlt_source=github_reactions(
                     "dagster-io", "dagster", items_per_page=100, max_items=250
                 ),
                 dlt_pipeline=pipeline(
                     pipeline_name="github_issues",
                     dataset_name="github",
                     destination="snowflake",
+                    progress="log",
                 ),
                 name="github",
                 group_name="github",
             )
             def github_reactions_dagster_assets(context: AssetExecutionContext, dlt: DltDagsterResource):
                 yield from dlt.run(context=context)
```

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.5
+Version: 0.23.6
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.5/setup.py` & `dagster-embedded-elt-0.23.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.5", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.6", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

