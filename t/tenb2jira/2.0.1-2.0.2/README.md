# Comparing `tmp/tenb2jira-2.0.1.tar.gz` & `tmp/tenb2jira-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenb2jira-2.0.1.tar", last modified: Tue May  7 17:08:24 2024, max compression
+gzip compressed data, was "tenb2jira-2.0.2.tar", last modified: Thu May 16 16:09:21 2024, max compression
```

## Comparing `tenb2jira-2.0.1.tar` & `tenb2jira-2.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.984754 tenb2jira-2.0.1/tenb2jira/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.984754 tenb2jira-2.0.1/tenb2jira/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tenb2jira/jira/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/issuetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19287 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tenb2jira/tenable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/tenable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/tenable/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/tenable/tenable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tenb2jira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tests/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.344498 tenb2jira-2.0.2/tenb2jira/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/tenb2jira/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/tenb2jira/jira/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/issuetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/jira/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19287 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/tenb2jira/tenable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/tenable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/tenable/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/tenable/tenable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tenb2jira/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/tenb2jira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-16 16:09:21.000000 tenb2jira-2.0.2/tenb2jira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-16 16:09:21.000000 tenb2jira-2.0.2/tenb2jira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:09:21.000000 tenb2jira-2.0.2/tenb2jira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 16:09:21.000000 tenb2jira-2.0.2/tenb2jira.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 16:09:21.000000 tenb2jira-2.0.2/tenb2jira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 16:09:21.000000 tenb2jira-2.0.2/tenb2jira.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:09:21.348497 tenb2jira-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-16 16:09:17.000000 tenb2jira-2.0.2/tests/test_processor.py
```

### Comparing `tenb2jira-2.0.1/PKG-INFO` & `tenb2jira-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenb2jira
-Version: 2.0.1
+Version: 2.0.2
 Summary: Tenable Vulnerability Management to Jira Cloud issue manager
 Author-email: "Tenable, Inc." <smcgrath@tenable.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/tenable/integration-jira-cloud
 Project-URL: Repository, https://github.com/tenable/integration-jira-cloud
 Project-URL: Issues, https://github.com/tenable/integration-jira-cloud/issues
 Project-URL: Changelog, https://github.com/tenable/integration-jira-cloud/blob/master/CHANGELOG.md
```

### Comparing `tenb2jira-2.0.1/README.md` & `tenb2jira-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/pyproject.toml` & `tenb2jira-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/cli.py` & `tenb2jira-2.0.2/tenb2jira/cli.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/fields.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/fields.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/issues.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/issues.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/issuetypes.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/issuetypes.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/iterator.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/iterator.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/projects.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/projects.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/screens.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/screens.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/api/session.py` & `tenb2jira-2.0.2/tenb2jira/jira/api/session.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/field.py` & `tenb2jira-2.0.2/tenb2jira/jira/field.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/jira.py` & `tenb2jira-2.0.2/tenb2jira/jira/jira.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/jira/task.py` & `tenb2jira-2.0.2/tenb2jira/jira/task.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/models.py` & `tenb2jira-2.0.2/tenb2jira/models.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/processor.py` & `tenb2jira-2.0.2/tenb2jira/processor.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/tenable/generators.py` & `tenb2jira-2.0.2/tenb2jira/tenable/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,20 @@
             Returns the individual findings, flattened and merged with the
             asset data.
     """
     # Yes this is expensive on memory, however it's the only way to get the
     # other asset attributes available within the finding for the Jira ticket
     # without build a database to match everything up into.
     assets = {}
+    def spf(value: str) -> str:
+        return value.replace(' ', '_')
     for asset in assets_iter:
         assets[asset['id']] = {
-            'tags': [f'{t["key"]}:{t["value"]}' for t in asset['tags']],
+            'tags': [f'{spf(t["key"])}:{spf(t["value"])}'
+                     for t in asset['tags']],
             'ipv4': asset['ipv4s'],
             'ipv6': asset['ipv6s'],
         }
         if asset_fields:
             for field in asset_fields:
                 assets[asset['id']][field] = asset[field]
```

### Comparing `tenb2jira-2.0.1/tenb2jira/tenable/tenable.py` & `tenb2jira-2.0.2/tenb2jira/tenable/tenable.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira/validator.py` & `tenb2jira-2.0.2/tenb2jira/validator.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tenb2jira.egg-info/PKG-INFO` & `tenb2jira-2.0.2/tenb2jira.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenb2jira
-Version: 2.0.1
+Version: 2.0.2
 Summary: Tenable Vulnerability Management to Jira Cloud issue manager
 Author-email: "Tenable, Inc." <smcgrath@tenable.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/tenable/integration-jira-cloud
 Project-URL: Repository, https://github.com/tenable/integration-jira-cloud
 Project-URL: Issues, https://github.com/tenable/integration-jira-cloud/issues
 Project-URL: Changelog, https://github.com/tenable/integration-jira-cloud/blob/master/CHANGELOG.md
```

### Comparing `tenb2jira-2.0.1/tenb2jira.egg-info/SOURCES.txt` & `tenb2jira-2.0.2/tenb2jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tests/test_models.py` & `tenb2jira-2.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.1/tests/test_processor.py` & `tenb2jira-2.0.2/tests/test_processor.py`

 * *Files identical despite different names*

