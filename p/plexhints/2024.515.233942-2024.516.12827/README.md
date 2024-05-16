# Comparing `tmp/plexhints-2024.515.233942.tar.gz` & `tmp/plexhints-2024.516.12827.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plexhints-2024.515.233942.tar", last modified: Thu May 16 01:02:31 2024, max compression
+gzip compressed data, was "dist/plexhints-2024.516.12827.tar", last modified: Thu May 16 01:30:03 2024, max compression
```

## Comparing `plexhints-2024.515.233942.tar` & `plexhints-2024.516.12827.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/toc.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/global.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/docs/source/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/framework/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/docs/source/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/contributing/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/contributing/build_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/contributing/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/docs/source/code_docs/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/code_docs/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/docs/source/about/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/about/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/about/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/about/github_action.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/about/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/docs/source/about/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/plexhints/
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/resource_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/object_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/exception_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/util_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/model_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/network_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/core_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/prefs_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/agent_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/log_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/shortcut_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/constant_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/plugin_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    31368 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/template_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/locale_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/extras_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/decorator_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)    40824 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/parse_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/plexhints/proxy_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:02:31.000000 plexhints-2024.515.233942/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 01:01:48.000000 plexhints-2024.515.233942/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/toc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/global.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/docs/source/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/framework/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/docs/source/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/contributing/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/contributing/build_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/contributing/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/docs/source/code_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/code_docs/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/docs/source/about/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/about/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/about/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/about/github_action.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/about/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/docs/source/about/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/plexhints/
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/resource_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/object_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/exception_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/util_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/model_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/network_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/core_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/prefs_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/agent_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/log_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/shortcut_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/constant_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/plugin_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31368 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/template_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/locale_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/extras_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/decorator_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40824 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/parse_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/plexhints/proxy_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:30:03.000000 plexhints-2024.516.12827/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 01:29:15.000000 plexhints-2024.516.12827/README.rst
```

### Comparing `plexhints-2024.515.233942/plexhints.egg-info/SOURCES.txt` & `plexhints-2024.516.12827/plexhints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints.egg-info/PKG-INFO` & `plexhints-2024.516.12827/plexhints.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plexhints
-Version: 2024.515.233942
+Version: 2024.516.12827
 Summary: Type hinting library for Plex plugin development.
 Home-page: https://github.com/LizardByte/plexhints
 Author: LizardByte
 Author-email: LizardByte@github.com
 License: UNKNOWN
 Description: :github_url: https://github.com/LizardByte/plexhints/tree/nightly/README.rst
```

### Comparing `plexhints-2024.515.233942/docs/Makefile` & `plexhints-2024.516.12827/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/make.bat` & `plexhints-2024.516.12827/docs/make.bat`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/framework/index.rst` & `plexhints-2024.516.12827/docs/source/framework/index.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/contributing/build_plugin.rst` & `plexhints-2024.516.12827/docs/source/contributing/build_plugin.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/contributing/testing.rst` & `plexhints-2024.516.12827/docs/source/contributing/testing.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/conf.py` & `plexhints-2024.516.12827/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/about/installation.rst` & `plexhints-2024.516.12827/docs/source/about/installation.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/about/github_action.rst` & `plexhints-2024.516.12827/docs/source/about/github_action.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/docs/source/about/usage.rst` & `plexhints-2024.516.12827/docs/source/about/usage.rst`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/PKG-INFO` & `plexhints-2024.516.12827/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plexhints
-Version: 2024.515.233942
+Version: 2024.516.12827
 Summary: Type hinting library for Plex plugin development.
 Home-page: https://github.com/LizardByte/plexhints
 Author: LizardByte
 Author-email: LizardByte@github.com
 License: UNKNOWN
 Description: :github_url: https://github.com/LizardByte/plexhints/tree/nightly/README.rst
```

### Comparing `plexhints-2024.515.233942/plexhints/resource_kit.py` & `plexhints-2024.516.12827/plexhints/resource_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/object_kit.py` & `plexhints-2024.516.12827/plexhints/object_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/exception_kit.py` & `plexhints-2024.516.12827/plexhints/exception_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/_helpers.py` & `plexhints-2024.516.12827/plexhints/_helpers.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/__init__.py` & `plexhints-2024.516.12827/plexhints/__init__.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/util_kit.py` & `plexhints-2024.516.12827/plexhints/util_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/model_kit.py` & `plexhints-2024.516.12827/plexhints/model_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/network_kit.py` & `plexhints-2024.516.12827/plexhints/network_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/core_kit.py` & `plexhints-2024.516.12827/plexhints/core_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/prefs_kit.py` & `plexhints-2024.516.12827/plexhints/prefs_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/agent_kit.py` & `plexhints-2024.516.12827/plexhints/agent_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/log_kit.py` & `plexhints-2024.516.12827/plexhints/log_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/constant_kit.py` & `plexhints-2024.516.12827/plexhints/constant_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/plugin_kit.py` & `plexhints-2024.516.12827/plexhints/plugin_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/template_kit.py` & `plexhints-2024.516.12827/plexhints/template_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/locale_kit.py` & `plexhints-2024.516.12827/plexhints/locale_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/extras_kit.py` & `plexhints-2024.516.12827/plexhints/extras_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/decorator_kit.py` & `plexhints-2024.516.12827/plexhints/decorator_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/parse_kit.py` & `plexhints-2024.516.12827/plexhints/parse_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/plexhints/proxy_kit.py` & `plexhints-2024.516.12827/plexhints/proxy_kit.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/setup.py` & `plexhints-2024.516.12827/setup.py`

 * *Files identical despite different names*

### Comparing `plexhints-2024.515.233942/README.rst` & `plexhints-2024.516.12827/README.rst`

 * *Files identical despite different names*

