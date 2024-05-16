# Comparing `tmp/plexhints-2024.516.14140.tar.gz` & `tmp/plexhints-2024.516.21511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plexhints-2024.516.14140.tar", last modified: Thu May 16 01:44:11 2024, max compression
+gzip compressed data, was "dist/plexhints-2024.516.21511.tar", last modified: Thu May 16 02:17:50 2024, max compression
```

## Comparing `plexhints-2024.516.14140.tar` & `plexhints-2024.516.21511.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/toc.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/global.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/docs/source/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/framework/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/docs/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/contributing/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/contributing/build_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/contributing/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/docs/source/code_docs/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/code_docs/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/docs/source/about/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/about/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/about/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/about/github_action.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/about/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/docs/source/about/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/plexhints/
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/resource_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/object_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/exception_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/util_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/model_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/network_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/core_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/prefs_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/agent_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/log_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/shortcut_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/constant_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/plugin_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    31368 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/template_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/locale_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/extras_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/decorator_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    40824 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/parse_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/plexhints/proxy_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:44:11.000000 plexhints-2024.516.14140/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 01:42:23.000000 plexhints-2024.516.14140/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/toc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/global.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/docs/source/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/framework/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/docs/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/contributing/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/contributing/build_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/contributing/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/docs/source/code_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/code_docs/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/docs/source/about/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/about/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/about/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/about/github_action.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/about/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/docs/source/about/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/plexhints/
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/resource_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/object_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/exception_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/util_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/model_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/network_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/core_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/prefs_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/agent_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/log_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/shortcut_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/constant_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/plugin_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31368 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/template_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/locale_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/extras_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/decorator_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40824 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/parse_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/plexhints/proxy_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:17:50.000000 plexhints-2024.516.21511/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 02:15:55.000000 plexhints-2024.516.21511/README.rst
```

### Comparing `plexhints-2024.516.14140/plexhints.egg-info/SOURCES.txt` & `plexhints-2024.516.21511/plexhints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints.egg-info/PKG-INFO` & `plexhints-2024.516.21511/plexhints.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plexhints
-Version: 2024.516.14140
+Version: 2024.516.21511
 Summary: Type hinting library for Plex plugin development.
 Home-page: https://github.com/LizardByte/plexhints
 Author: LizardByte
 Author-email: LizardByte@github.com
 License: UNKNOWN
 Description: :github_url: https://github.com/LizardByte/plexhints/tree/nightly/README.rst
```

### Comparing `plexhints-2024.516.14140/docs/Makefile` & `plexhints-2024.516.21511/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/make.bat` & `plexhints-2024.516.21511/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/framework/index.rst` & `plexhints-2024.516.21511/docs/source/framework/index.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/contributing/build_plugin.rst` & `plexhints-2024.516.21511/docs/source/contributing/build_plugin.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/contributing/testing.rst` & `plexhints-2024.516.21511/docs/source/contributing/testing.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/conf.py` & `plexhints-2024.516.21511/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/about/installation.rst` & `plexhints-2024.516.21511/docs/source/about/installation.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/about/github_action.rst` & `plexhints-2024.516.21511/docs/source/about/github_action.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/docs/source/about/usage.rst` & `plexhints-2024.516.21511/docs/source/about/usage.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/PKG-INFO` & `plexhints-2024.516.21511/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plexhints
-Version: 2024.516.14140
+Version: 2024.516.21511
 Summary: Type hinting library for Plex plugin development.
 Home-page: https://github.com/LizardByte/plexhints
 Author: LizardByte
 Author-email: LizardByte@github.com
 License: UNKNOWN
 Description: :github_url: https://github.com/LizardByte/plexhints/tree/nightly/README.rst
```

### Comparing `plexhints-2024.516.14140/plexhints/resource_kit.py` & `plexhints-2024.516.21511/plexhints/resource_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/object_kit.py` & `plexhints-2024.516.21511/plexhints/object_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/exception_kit.py` & `plexhints-2024.516.21511/plexhints/exception_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/_helpers.py` & `plexhints-2024.516.21511/plexhints/_helpers.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/__init__.py` & `plexhints-2024.516.21511/plexhints/__init__.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/util_kit.py` & `plexhints-2024.516.21511/plexhints/util_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/model_kit.py` & `plexhints-2024.516.21511/plexhints/model_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/network_kit.py` & `plexhints-2024.516.21511/plexhints/network_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/core_kit.py` & `plexhints-2024.516.21511/plexhints/core_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/prefs_kit.py` & `plexhints-2024.516.21511/plexhints/prefs_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/agent_kit.py` & `plexhints-2024.516.21511/plexhints/agent_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/log_kit.py` & `plexhints-2024.516.21511/plexhints/log_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/constant_kit.py` & `plexhints-2024.516.21511/plexhints/constant_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/plugin_kit.py` & `plexhints-2024.516.21511/plexhints/plugin_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/template_kit.py` & `plexhints-2024.516.21511/plexhints/template_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/locale_kit.py` & `plexhints-2024.516.21511/plexhints/locale_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/extras_kit.py` & `plexhints-2024.516.21511/plexhints/extras_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/decorator_kit.py` & `plexhints-2024.516.21511/plexhints/decorator_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/parse_kit.py` & `plexhints-2024.516.21511/plexhints/parse_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/plexhints/proxy_kit.py` & `plexhints-2024.516.21511/plexhints/proxy_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/setup.py` & `plexhints-2024.516.21511/setup.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.516.14140/README.rst` & `plexhints-2024.516.21511/README.rst`

 * *Files identical despite different names*

