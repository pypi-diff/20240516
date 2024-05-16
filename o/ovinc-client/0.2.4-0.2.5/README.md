# Comparing `tmp/ovinc_client-0.2.4.tar.gz` & `tmp/ovinc_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovinc_client-0.2.4.tar", last modified: Mon May 13 11:31:51 2024, max compression
+gzip compressed data, was "ovinc_client-0.2.5.tar", last modified: Thu May 16 02:55:58 2024, max compression
```

## Comparing `ovinc_client-0.2.4.tar` & `ovinc_client-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.940554 ovinc_client-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 11:31:51.940554 ovinc_client-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.932554 ovinc_client-0.2.4/ovinc_client/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.936554 ovinc_client-0.2.4/ovinc_client/account/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.936554 ovinc_client-0.2.4/ovinc_client/account/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/account/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.936554 ovinc_client-0.2.4/ovinc_client/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/components/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/components/notice.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/components/tcaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.936554 ovinc_client-0.2.4/ovinc_client/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/paginations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/core/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.940554 ovinc_client-0.2.4/ovinc_client/trace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/instrumentors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/ovinc_client/trace/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:31:51.940554 ovinc_client-0.2.4/ovinc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 11:31:51.000000 ovinc_client-0.2.4/ovinc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-13 11:31:51.000000 ovinc_client-0.2.4/ovinc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:31:51.000000 ovinc_client-0.2.4/ovinc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 11:31:51.000000 ovinc_client-0.2.4/ovinc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 11:31:51.000000 ovinc_client-0.2.4/ovinc_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:31:51.940554 ovinc_client-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-13 11:31:47.000000 ovinc_client-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.152659 ovinc_client-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 02:55:58.148659 ovinc_client-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.144659 ovinc_client-0.2.5/ovinc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.144659 ovinc_client-0.2.5/ovinc_client/account/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.144659 ovinc_client-0.2.5/ovinc_client/account/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/account/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.144659 ovinc_client-0.2.5/ovinc_client/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/components/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/components/notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/components/tcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.148659 ovinc_client-0.2.5/ovinc_client/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/paginations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/core/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.148659 ovinc_client-0.2.5/ovinc_client/trace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/instrumentors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/ovinc_client/trace/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:55:58.148659 ovinc_client-0.2.5/ovinc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 02:55:58.000000 ovinc_client-0.2.5/ovinc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-16 02:55:58.000000 ovinc_client-0.2.5/ovinc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:55:58.000000 ovinc_client-0.2.5/ovinc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-16 02:55:58.000000 ovinc_client-0.2.5/ovinc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 02:55:58.000000 ovinc_client-0.2.5/ovinc_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:55:58.152659 ovinc_client-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-16 02:55:50.000000 ovinc_client-0.2.5/setup.py
```

### Comparing `ovinc_client-0.2.4/LICENSE` & `ovinc_client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/PKG-INFO` & `ovinc_client-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovinc_client
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Tool for OVINC Union API
 Home-page: https://www.ovinc.cn/
 Author: OVINC
 Author-email: contact@ovinc.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django<5,>=4
@@ -30,14 +30,15 @@
 Requires-Dist: opentelemetry-instrumentation-django==0.45b0
 Requires-Dist: opentelemetry-instrumentation-dbapi==0.45b0
 Requires-Dist: opentelemetry-instrumentation-redis==0.45b0
 Requires-Dist: opentelemetry-instrumentation-requests==0.45b0
 Requires-Dist: opentelemetry-instrumentation-celery==0.45b0
 Requires-Dist: opentelemetry-instrumentation-logging==0.45b0
 Requires-Dist: opentelemetry-instrumentation-httpx==0.45b0
+Requires-Dist: ipython<9,>=8.10.0
 
 ## OVINC Union Api Client
 
 ### Init
 
 Init: `APP_CODE` `APP_SECRET` `OVINC_API_URL`
```

### Comparing `ovinc_client-0.2.4/ovinc_client/account/constants.py` & `ovinc_client-0.2.5/ovinc_client/account/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/account/migrations/0001_initial.py` & `ovinc_client-0.2.5/ovinc_client/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/account/models.py` & `ovinc_client-0.2.5/ovinc_client/account/models.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/account/serializers.py` & `ovinc_client-0.2.5/ovinc_client/account/serializers.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/account/views.py` & `ovinc_client-0.2.5/ovinc_client/account/views.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/client.py` & `ovinc_client-0.2.5/ovinc_client/client.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/components/base.py` & `ovinc_client-0.2.5/ovinc_client/components/base.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/components/notice.py` & `ovinc_client-0.2.5/ovinc_client/components/notice.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/auth.py` & `ovinc_client-0.2.5/ovinc_client/core/auth.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/cache.py` & `ovinc_client-0.2.5/ovinc_client/core/cache.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/constants.py` & `ovinc_client-0.2.5/ovinc_client/core/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/exceptions.py` & `ovinc_client-0.2.5/ovinc_client/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/lock.py` & `ovinc_client-0.2.5/ovinc_client/core/lock.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/logger.py` & `ovinc_client-0.2.5/ovinc_client/core/logger.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/middlewares.py` & `ovinc_client-0.2.5/ovinc_client/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/models.py` & `ovinc_client-0.2.5/ovinc_client/core/models.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/paginations.py` & `ovinc_client-0.2.5/ovinc_client/core/paginations.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/renderers.py` & `ovinc_client-0.2.5/ovinc_client/core/renderers.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/utils.py` & `ovinc_client-0.2.5/ovinc_client/core/utils.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/core/viewsets.py` & `ovinc_client-0.2.5/ovinc_client/core/viewsets.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/trace/constants.py` & `ovinc_client-0.2.5/ovinc_client/trace/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/trace/exporters.py` & `ovinc_client-0.2.5/ovinc_client/trace/exporters.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/trace/instrumentors.py` & `ovinc_client-0.2.5/ovinc_client/trace/instrumentors.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/trace/setup.py` & `ovinc_client-0.2.5/ovinc_client/trace/setup.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/trace/utils.py` & `ovinc_client-0.2.5/ovinc_client/trace/utils.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client/trace/views.py` & `ovinc_client-0.2.5/ovinc_client/trace/views.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client.egg-info/PKG-INFO` & `ovinc_client-0.2.5/ovinc_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovinc_client
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Tool for OVINC Union API
 Home-page: https://www.ovinc.cn/
 Author: OVINC
 Author-email: contact@ovinc.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django<5,>=4
@@ -30,14 +30,15 @@
 Requires-Dist: opentelemetry-instrumentation-django==0.45b0
 Requires-Dist: opentelemetry-instrumentation-dbapi==0.45b0
 Requires-Dist: opentelemetry-instrumentation-redis==0.45b0
 Requires-Dist: opentelemetry-instrumentation-requests==0.45b0
 Requires-Dist: opentelemetry-instrumentation-celery==0.45b0
 Requires-Dist: opentelemetry-instrumentation-logging==0.45b0
 Requires-Dist: opentelemetry-instrumentation-httpx==0.45b0
+Requires-Dist: ipython<9,>=8.10.0
 
 ## OVINC Union Api Client
 
 ### Init
 
 Init: `APP_CODE` `APP_SECRET` `OVINC_API_URL`
```

### Comparing `ovinc_client-0.2.4/ovinc_client.egg-info/SOURCES.txt` & `ovinc_client-0.2.5/ovinc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.4/ovinc_client.egg-info/requires.txt` & `ovinc_client-0.2.5/ovinc_client.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,7 +21,8 @@
 opentelemetry-instrumentation-django==0.45b0
 opentelemetry-instrumentation-dbapi==0.45b0
 opentelemetry-instrumentation-redis==0.45b0
 opentelemetry-instrumentation-requests==0.45b0
 opentelemetry-instrumentation-celery==0.45b0
 opentelemetry-instrumentation-logging==0.45b0
 opentelemetry-instrumentation-httpx==0.45b0
+ipython<9,>=8.10.0
```

### Comparing `ovinc_client-0.2.4/setup.py` & `ovinc_client-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ovinc_client",
-    version="0.2.4",
+    version="0.2.5",
     author="OVINC",
     url="https://www.ovinc.cn/",
     author_email="contact@ovinc.cn",
     description="A Tool for OVINC Union API",
     packages=[
         "ovinc_client",
         "ovinc_client.account",
@@ -44,11 +44,12 @@
         "opentelemetry-instrumentation-django==0.45b0",
         "opentelemetry-instrumentation-dbapi==0.45b0",
         "opentelemetry-instrumentation-redis==0.45b0",
         "opentelemetry-instrumentation-requests==0.45b0",
         "opentelemetry-instrumentation-celery==0.45b0",
         "opentelemetry-instrumentation-logging==0.45b0",
         "opentelemetry-instrumentation-httpx==0.45b0",
+        "ipython>=8.10.0,<9",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

