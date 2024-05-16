# Comparing `tmp/momapa-0.1.tar.gz` & `tmp/momapa-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momapa-0.1.tar", last modified: Sun May 12 13:51:03 2024, max compression
+gzip compressed data, was "momapa-0.2.tar", last modified: Thu May 16 19:42:10 2024, max compression
```

## Comparing `momapa-0.1.tar` & `momapa-0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-12 13:51:03.651049 momapa-0.1/
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     3877 2024-05-10 16:06:48.000000 momapa-0.1/.gitignore
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)    32421 2024-05-10 21:41:36.000000 momapa-0.1/LICENSE.md
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      184 2024-05-10 21:41:36.000000 momapa-0.1/Makefile
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      265 2024-05-12 13:51:03.651049 momapa-0.1/PKG-INFO
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     3444 2024-05-12 13:47:27.000000 momapa-0.1/README.md
-drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-12 13:51:03.647716 momapa-0.1/momapa/
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      495 2024-05-12 11:01:17.000000 momapa-0.1/momapa/__init__.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1435 2024-05-12 10:24:20.000000 momapa-0.1/momapa/argument.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      525 2024-05-10 21:41:36.000000 momapa-0.1/momapa/asset.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      689 2024-05-10 21:41:36.000000 momapa-0.1/momapa/file.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      365 2024-05-10 21:41:36.000000 momapa-0.1/momapa/java.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     4369 2024-05-12 13:46:12.000000 momapa-0.1/momapa/library.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      728 2024-05-12 11:04:56.000000 momapa-0.1/momapa/logging.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     3322 2024-05-12 10:58:14.000000 momapa-0.1/momapa/manifest.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     2321 2024-05-12 13:23:33.000000 momapa-0.1/momapa/os.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1222 2024-05-12 11:02:59.000000 momapa-0.1/momapa/rule.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1550 2024-05-12 11:03:12.000000 momapa-0.1/momapa/validator.py
-drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-12 13:51:03.647716 momapa-0.1/momapa.egg-info/
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      265 2024-05-12 13:51:03.000000 momapa-0.1/momapa.egg-info/PKG-INFO
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      651 2024-05-12 13:51:03.000000 momapa-0.1/momapa.egg-info/SOURCES.txt
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)        1 2024-05-12 13:51:03.000000 momapa-0.1/momapa.egg-info/dependency_links.txt
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)       13 2024-05-12 13:51:03.000000 momapa-0.1/momapa.egg-info/top_level.txt
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)       29 2024-05-10 21:41:36.000000 momapa-0.1/requirements-dev.txt
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      127 2024-05-12 13:51:03.651049 momapa-0.1/setup.cfg
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      479 2024-05-10 21:41:36.000000 momapa-0.1/setup.py
-drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-12 13:51:03.651049 momapa-0.1/tests/
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)        0 2024-05-10 21:41:36.000000 momapa-0.1/tests/__init__.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     4174 2024-05-12 10:26:46.000000 momapa-0.1/tests/argument_test.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      605 2024-05-10 21:41:36.000000 momapa-0.1/tests/assetindex_test.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1406 2024-05-10 21:41:36.000000 momapa-0.1/tests/file_test.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     2355 2024-05-10 21:41:36.000000 momapa-0.1/tests/gamedownloads_test.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      431 2024-05-10 21:41:36.000000 momapa-0.1/tests/java_version_test.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1199 2024-05-12 10:26:52.000000 momapa-0.1/tests/rule_test.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     8407 2024-05-12 13:45:57.000000 momapa-0.1/tests/test_library.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)      710 2024-05-12 11:06:04.000000 momapa-0.1/tests/test_logging.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     2872 2024-05-12 10:25:21.000000 momapa-0.1/tests/test_rule_validator.py
--rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1086 2024-05-12 10:36:35.000000 momapa-0.1/tests/test_ruleset_validator.py
+drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-16 19:42:10.120245 momapa-0.2/
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     3877 2024-05-10 16:06:48.000000 momapa-0.2/.gitignore
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)    32421 2024-05-10 21:41:36.000000 momapa-0.2/LICENSE.md
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      184 2024-05-10 21:41:36.000000 momapa-0.2/Makefile
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      265 2024-05-16 19:42:10.123579 momapa-0.2/PKG-INFO
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     3444 2024-05-12 13:47:27.000000 momapa-0.2/README.md
+drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-16 19:42:10.120245 momapa-0.2/momapa/
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      495 2024-05-12 11:01:17.000000 momapa-0.2/momapa/__init__.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1435 2024-05-12 10:24:20.000000 momapa-0.2/momapa/argument.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      525 2024-05-10 21:41:36.000000 momapa-0.2/momapa/asset.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      689 2024-05-10 21:41:36.000000 momapa-0.2/momapa/file.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      365 2024-05-10 21:41:36.000000 momapa-0.2/momapa/java.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     4312 2024-05-16 19:41:31.000000 momapa-0.2/momapa/library.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      728 2024-05-12 11:04:56.000000 momapa-0.2/momapa/logging.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     3322 2024-05-12 10:58:14.000000 momapa-0.2/momapa/manifest.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     2321 2024-05-12 13:23:33.000000 momapa-0.2/momapa/os.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1258 2024-05-16 19:41:15.000000 momapa-0.2/momapa/rule.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1550 2024-05-12 11:03:12.000000 momapa-0.2/momapa/validator.py
+drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-16 19:42:10.120245 momapa-0.2/momapa.egg-info/
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      265 2024-05-16 19:42:10.000000 momapa-0.2/momapa.egg-info/PKG-INFO
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      651 2024-05-16 19:42:10.000000 momapa-0.2/momapa.egg-info/SOURCES.txt
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)        1 2024-05-16 19:42:10.000000 momapa-0.2/momapa.egg-info/dependency_links.txt
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)       13 2024-05-16 19:42:10.000000 momapa-0.2/momapa.egg-info/top_level.txt
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)       29 2024-05-10 21:41:36.000000 momapa-0.2/requirements-dev.txt
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      127 2024-05-16 19:42:10.123579 momapa-0.2/setup.cfg
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      479 2024-05-16 19:39:50.000000 momapa-0.2/setup.py
+drwxr-xr-x   0 oxodao    (1000) oxodao    (1000)        0 2024-05-16 19:42:10.120245 momapa-0.2/tests/
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)        0 2024-05-10 21:41:36.000000 momapa-0.2/tests/__init__.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     4174 2024-05-12 10:26:46.000000 momapa-0.2/tests/argument_test.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      605 2024-05-10 21:41:36.000000 momapa-0.2/tests/assetindex_test.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1406 2024-05-10 21:41:36.000000 momapa-0.2/tests/file_test.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     2355 2024-05-10 21:41:36.000000 momapa-0.2/tests/gamedownloads_test.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      431 2024-05-10 21:41:36.000000 momapa-0.2/tests/java_version_test.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1199 2024-05-12 10:26:52.000000 momapa-0.2/tests/rule_test.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     8407 2024-05-12 13:45:57.000000 momapa-0.2/tests/test_library.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)      710 2024-05-12 11:06:04.000000 momapa-0.2/tests/test_logging.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     2872 2024-05-12 10:25:21.000000 momapa-0.2/tests/test_rule_validator.py
+-rw-r--r--   0 oxodao    (1000) oxodao    (1000)     1086 2024-05-12 10:36:35.000000 momapa-0.2/tests/test_ruleset_validator.py
```

### Comparing `momapa-0.1/.gitignore` & `momapa-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `momapa-0.1/LICENSE.md` & `momapa-0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `momapa-0.1/README.md` & `momapa-0.2/README.md`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/argument.py` & `momapa-0.2/momapa/argument.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/asset.py` & `momapa-0.2/momapa/asset.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/file.py` & `momapa-0.2/momapa/file.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/library.py` & `momapa-0.2/momapa/library.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 # org.lwjgl.lwjgl:lwjgl-platform:2.9.4-nightly-20150209
                 should_skip = False
                 if k == OS.OSX:
                     for r in data.get('rules', []):
                         if r.get('action') != 'disallow':
                             continue
 
-                        if r.get('os', {}).get('name') == OS.OSX:  # Not sure why its already parsed as enum here but heh
+                        if r.get('os', {}).get('name') == 'osx':
                             should_skip = True
 
                 if should_skip:
                     continue
                 #endregion
 
                 lib.rules = [
```

### Comparing `momapa-0.1/momapa/logging.py` & `momapa-0.2/momapa/logging.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/manifest.py` & `momapa-0.2/momapa/manifest.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/os.py` & `momapa-0.2/momapa/os.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa/rule.py` & `momapa-0.2/momapa/rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional, Self
+from copy import deepcopy
 
 from .os import map_to_generic_arch, map_to_generic_os, RuleAction
 
 
 # @TODO to validate:
 # os: name, version (regex), arch
 # features: is_demo_user, has_custom_resolution
@@ -17,15 +18,15 @@
         self.os = os
 
     @staticmethod
     def parse(data: Optional[dict]) -> Optional[Self]:
         if not data:
             return None
 
-        os = data.get('os')
+        os = deepcopy(data.get('os'))
         if os:
             name = os.get('name')
             if name:
                 os['name'] = map_to_generic_os(name)
 
             arch = os.get('arch')
             if arch:
```

### Comparing `momapa-0.1/momapa/validator.py` & `momapa-0.2/momapa/validator.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/momapa.egg-info/SOURCES.txt` & `momapa-0.2/momapa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/argument_test.py` & `momapa-0.2/tests/argument_test.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/assetindex_test.py` & `momapa-0.2/tests/assetindex_test.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/file_test.py` & `momapa-0.2/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/gamedownloads_test.py` & `momapa-0.2/tests/gamedownloads_test.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/rule_test.py` & `momapa-0.2/tests/rule_test.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/test_library.py` & `momapa-0.2/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/test_logging.py` & `momapa-0.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/test_rule_validator.py` & `momapa-0.2/tests/test_rule_validator.py`

 * *Files identical despite different names*

### Comparing `momapa-0.1/tests/test_ruleset_validator.py` & `momapa-0.2/tests/test_ruleset_validator.py`

 * *Files identical despite different names*

