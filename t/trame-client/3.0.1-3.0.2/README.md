# Comparing `tmp/trame-client-3.0.1.tar.gz` & `tmp/trame-client-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-3.0.1.tar", last modified: Fri Apr 12 22:23:23 2024, max compression
+gzip compressed data, was "trame-client-3.0.2.tar", last modified: Wed Apr 17 20:44:08 2024, max compression
```

## Comparing `trame-client-3.0.1.tar` & `trame-client-3.0.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-12 22:22:53.000000 trame-client-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-12 22:22:53.000000 trame-client-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3539 2024-04-12 22:23:23.328211 trame-client-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2024-04-12 22:22:53.000000 trame-client-3.0.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      935 2024-04-12 22:23:23.332212 trame-client-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 22:22:53.000000 trame-client-3.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    26004 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/js/app.7c11979c.js
--rw-r--r--   0 root         (0) root         (0)   156057 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
--rw-r--r--   0 root         (0) root         (0)     2890 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/loading.tpl
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2024-04-12 22:23:13.000000 trame-client-3.0.1/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.324211 trame-client-3.0.1/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   102078 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/assets/index-26129a2a.js
--rw-r--r--   0 root         (0) root         (0)     1359 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/assets/index-e80c1ba5.css
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     2890 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/loading.tpl
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   147534 2024-04-12 22:23:19.000000 trame-client-3.0.1/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9364 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1134 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/formatter.py
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     3816 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/testing.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/version.py
--rw-r--r--   0 root         (0) root         (0)     3190 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/utils/web_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.328211 trame-client-3.0.1/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22879 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     9071 2024-04-12 22:22:53.000000 trame-client-3.0.1/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:23:23.320211 trame-client-3.0.1/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3539 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-12 22:23:23.000000 trame-client-3.0.1/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.679409 trame-client-3.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-17 20:43:37.000000 trame-client-3.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-17 20:43:37.000000 trame-client-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-04-17 20:44:08.679409 trame-client-3.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-17 20:43:37.000000 trame-client-3.0.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      935 2024-04-17 20:44:08.679409 trame-client-3.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:43:37.000000 trame-client-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.675409 trame-client-3.0.2/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.675409 trame-client-3.0.2/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.675409 trame-client-3.0.2/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.675409 trame-client-3.0.2/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    26057 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/js/app.7d0e64a7.js
+-rw-r--r--   0 root         (0) root         (0)   156057 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/loading.tpl
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2024-04-17 20:43:57.000000 trame-client-3.0.2/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.675409 trame-client-3.0.2/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.675409 trame-client-3.0.2/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   102131 2024-04-17 20:44:05.000000 trame-client-3.0.2/trame_client/module/vue3-www/assets/index-75032529.js
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-17 20:44:05.000000 trame-client-3.0.2/trame_client/module/vue3-www/assets/index-e80c1ba5.css
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-17 20:44:05.000000 trame-client-3.0.2/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-04-17 20:44:05.000000 trame-client-3.0.2/trame_client/module/vue3-www/loading.tpl
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-17 20:44:05.000000 trame-client-3.0.2/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   147534 2024-04-17 20:44:05.000000 trame-client-3.0.2/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.679409 trame-client-3.0.2/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.679409 trame-client-3.0.2/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9364 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.679409 trame-client-3.0.2/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/formatter.py
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/testing.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/version.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/utils/web_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.679409 trame-client-3.0.2/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22879 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     9071 2024-04-17 20:43:37.000000 trame-client-3.0.2/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:44:08.671409 trame-client-3.0.2/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3539 2024-04-17 20:44:08.000000 trame-client-3.0.2/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-17 20:44:08.000000 trame-client-3.0.2/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:44:08.000000 trame-client-3.0.2/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-17 20:44:08.000000 trame-client-3.0.2/trame_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-17 20:44:08.000000 trame-client-3.0.2/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-3.0.1/LICENSE` & `trame-client-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/PKG-INFO` & `trame-client-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-3.0.1/README.rst` & `trame-client-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/setup.cfg` & `trame-client-3.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 3.0.1
+version = 3.0.2
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-client-3.0.1/trame_client/LICENSE` & `trame-client-3.0.2/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/encoders/numpy.py` & `trame-client-3.0.2/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-3.0.2/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/index.html` & `trame-client-3.0.2/trame_client/module/vue2-www/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="" data-app-name="trame"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,minimum-scale=1"><meta name="description" content="Application built with trame, a product from Kitware"><meta name="keywords" content="trame, OpenSource, Stateful Python Application, Kitware"><meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate"/><meta http-equiv="Pragma" content="no-cache"/><meta http-equiv="Expires" content="0"/><link rel="icon" href="logo.png"><script src="vue.global.js"></script><title>trame is built by Kitware</title><script defer="defer" src="js/chunk-vendors.3aa0189c.js"></script><script defer="defer" src="js/app.7c11979c.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script>fetch("./loading.tpl").then((r) => r.text()).then((c) => document.querySelector("#app").innerHTML = c)</script></body></html>
+<!doctype html><html lang="" data-app-name="trame"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,minimum-scale=1"><meta name="description" content="Application built with trame, a product from Kitware"><meta name="keywords" content="trame, OpenSource, Stateful Python Application, Kitware"><meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate"/><meta http-equiv="Pragma" content="no-cache"/><meta http-equiv="Expires" content="0"/><link rel="icon" href="logo.png"><script src="vue.global.js"></script><title>trame is built by Kitware</title><script defer="defer" src="js/chunk-vendors.3aa0189c.js"></script><script defer="defer" src="js/app.7d0e64a7.js"></script><link href="css/app.0b077e70.css" rel="stylesheet"></head><body style="margin: 0; padding: 0;"><noscript><strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script>fetch("./loading.tpl").then((r) => r.text()).then((c) => document.querySelector("#app").innerHTML = c)</script></body></html>
```

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/js/app.7c11979c.js` & `trame-client-3.0.2/trame_client/module/vue2-www/js/app.7d0e64a7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -163,24 +163,24 @@
                 var S = {
                         getClient: T,
                         resetClient: _,
                         getStatus: C,
                         configDecorator: b
                     },
                     $ = (n(8324), n(9274)),
-                    R = n(7117);
+                    x = n(7117);
                 n(5137);
-                const x = {};
+                const R = {};
 
                 function O(e, t) {
                     return e.priority - t.priority
                 }
 
                 function L(e) {
-                    x.addAttachement = e
+                    R.addAttachement = e
                 }
                 const U = {
                         priority: 0,
                         async decorate(e) {
                             if (null === e || void 0 === e) return e;
                             if (e.constructor && e.constructor === File) {
                                 const {
@@ -486,15 +486,15 @@
                             props: {
                                 templateName: {
                                     type: String,
                                     default: "main"
                                 }
                             },
                             components: {
-                                VRuntimeTemplate: R.Z
+                                VRuntimeTemplate: x.Z
                             },
                             computed: (0, s.Z)((0, s.Z)({}, r), {}, {
                                 contentTemplate() {
                                     const e = `trame__template_${this.templateName}`;
                                     return this[e] || `<div>No state variable for ${e} with the following state.<br><pre>${JSON.stringify(this.trame.state.get(),null,2)}</pre></div>`
                                 },
                                 tts() {
@@ -837,19 +837,19 @@
                     $e = {
                         container: "style_container_VCsHx",
                         loader: "style_loader_CNsNi",
                         spin: "style_spin_BAaPb",
                         message: "style_message_rmggO"
                     };
 
-                function Re(e) {
+                function xe(e) {
                     this["$style"] = $e.locals || $e
                 }
-                var xe = (0, le.Z)(Se, Te, _e, !1, Re, null, null),
-                    Oe = xe.exports,
+                var Re = (0, le.Z)(Se, Te, _e, !1, xe, null, null),
+                    Oe = Re.exports,
                     Le = function() {
                         var e = this,
                             t = e._self._c;
                         return t("div", {
                             class: e.$style.container
                         }, [t("div", {
                             class: e.$style.center
@@ -1202,55 +1202,62 @@
                         setup(e, {
                             emit: t
                         }) {
                             const n = Tt("trame"),
                                 s = _t(null);
 
                             function r() {
-                                const r = s.value.getBoundingClientRect(),
-                                    i = window.devicePixelRatio,
-                                    a = 96 * i,
-                                    o = {
-                                        size: r,
-                                        pixelRatio: i,
-                                        dpi: a
-                                    };
-                                e.name && (o.name = e.name), n && n.state.set(e.name, o), t("change", o)
+                                const {
+                                    x: r,
+                                    y: i,
+                                    width: a,
+                                    height: o
+                                } = s.value.getBoundingClientRect(), l = {
+                                    x: r,
+                                    y: i,
+                                    width: a,
+                                    height: o
+                                }, c = window.devicePixelRatio, u = 96 * c, h = {
+                                    size: l,
+                                    pixelRatio: c,
+                                    dpi: u
+                                };
+                                e.name && (h.name = e.name), n && n.state.set(e.name, h), t("change", h)
                             }
                             const i = new ResizeObserver(r);
                             return Ct((() => {
                                 i.observe(s.value)
                             })), St((() => {
                                 i.unobserve(s.value)
                             })), {
                                 elem: s,
                                 resize: r
                             }
                         },
                         template: '<div ref="elem" style="overflow: hidden; position: relative; width: 100%; height: 100%; margin: 0; padding: 0;"><slot></slot></div>'
                     },
-                    Rt = {
+                    xt = {
                         TrameApp: we,
                         TrameConnect: ue,
                         TrameLoading: Oe,
                         TrameReconnect: Ee,
                         TrameTemplate: ye,
                         TrameStateResolver: Ke,
                         TrameStyle: Ye,
                         TrameExec: Qe,
                         TrameGetter: it,
                         TrameClientStateChange: lt,
                         TrameClientTriggers: ht,
                         TrameLifeCycleMonitor: wt,
                         TrameSizeObserver: $t
                     },
-                    xt = {
+                    Rt = {
                         install(e) {
-                            Object.keys(Rt).forEach((t => {
-                                e.component(t, Rt[t])
+                            Object.keys(xt).forEach((t => {
+                                e.component(t, xt[t])
                             }))
                         }
                     };
                 const Ot = "TrameConnect";
 
                 function Lt() {
                     const e = S.getStatus(Ot),
@@ -1258,15 +1265,15 @@
                     t ? t.innerHTML = e.message || e.type : console.error("WsError", e.message || e.type)
                 }
                 async function Ut(e) {
                     try {
                         var t, n, r;
                         null !== (t = window) && void 0 !== t && null !== (n = t.parent) && void 0 !== n && null !== (r = n.trameJupyter) && void 0 !== r && r.init && (window.WSLINK = window.parent.trameJupyter.init(window))
                     } catch (o) {}
-                    e.use(xt);
+                    e.use(Rt);
                     const i = S.getClient(Ot);
                     try {
                         await i.connect(S.configDecorator({
                             application: "trame",
                             useUrl: !0
                         }))
                     } catch (o) {
@@ -1377,8 +1384,8 @@
             s.forEach(t.bind(null, 0)), s.push = t.bind(null, s.push.bind(s))
         }();
     var s = n.O(void 0, [998], (function() {
         return n(7660)
     }));
     s = n.O(s)
 })();
-//# sourceMappingURL=app.7c11979c.js.map
+//# sourceMappingURL=app.7d0e64a7.js.map
```

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js` & `trame-client-3.0.2/trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/loading.tpl` & `trame-client-3.0.2/trame_client/module/vue2-www/loading.tpl`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/logo.png` & `trame-client-3.0.2/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue2-www/vue.global.js` & `trame-client-3.0.2/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue3-www/assets/index-26129a2a.js` & `trame-client-3.0.2/trame_client/module/vue3-www/assets/index-75032529.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -877,44 +877,44 @@
         if (!Symbol.asyncIterator) throw new TypeError("Symbol.asyncIterator is not defined.");
         var r = n.apply(t, e || []),
             i, o = [];
         return i = {}, s("next"), s("throw"), s("return"), i[Symbol.asyncIterator] = function() {
             return this
         }, i;
 
-        function s(l) {
-            r[l] && (i[l] = function(p) {
+        function s(p) {
+            r[p] && (i[p] = function(l) {
                 return new Promise(function(y, g) {
-                    o.push([l, p, y, g]) > 1 || a(l, p)
+                    o.push([p, l, y, g]) > 1 || a(p, l)
                 })
             })
         }
 
-        function a(l, p) {
+        function a(p, l) {
             try {
-                u(r[l](p))
+                u(r[p](l))
             } catch (y) {
                 h(o[0][3], y)
             }
         }
 
-        function u(l) {
-            l.value instanceof G ? Promise.resolve(l.value.v).then(c, f) : h(o[0][2], l)
+        function u(p) {
+            p.value instanceof G ? Promise.resolve(p.value.v).then(c, f) : h(o[0][2], p)
         }
 
-        function c(l) {
-            a("next", l)
+        function c(p) {
+            a("next", p)
         }
 
-        function f(l) {
-            a("throw", l)
+        function f(p) {
+            a("throw", p)
         }
 
-        function h(l, p) {
-            l(p), o.shift(), o.length && a(o[0][0], o[0][1])
+        function h(p, l) {
+            p(l), o.shift(), o.length && a(o[0][0], o[0][1])
         }
     },
     sr = function(t) {
         var e = typeof t;
         return e === "string" || e === "number"
     },
     J = -1,
@@ -970,15 +970,15 @@
                     case 3:
                         return [2]
                 }
             })
         }, t.prototype.decodeAsync = function(e) {
             var n, r, i, o;
             return ir(this, void 0, void 0, function() {
-                var s, a, u, c, f, h, l, p;
+                var s, a, u, c, f, h, p, l;
                 return we(this, function(y) {
                     switch (y.label) {
                         case 0:
                             s = !1, y.label = 1;
                         case 1:
                             y.trys.push([1, 6, 7, 12]), n = We(e), y.label = 2;
                         case 2:
@@ -1013,64 +1013,64 @@
                         case 11:
                             return [7];
                         case 12:
                             if (s) {
                                 if (this.hasRemaining(1)) throw this.createExtraByteError(this.totalPos);
                                 return [2, a]
                             }
-                            throw f = this, h = f.headByte, l = f.pos, p = f.totalPos, new RangeError("Insufficient data in parsing ".concat(de(h), " at ").concat(p, " (").concat(l, " in the current buffer)"))
+                            throw f = this, h = f.headByte, p = f.pos, l = f.totalPos, new RangeError("Insufficient data in parsing ".concat(de(h), " at ").concat(l, " (").concat(p, " in the current buffer)"))
                     }
                 })
             })
         }, t.prototype.decodeArrayStream = function(e) {
             return this.decodeMultiAsync(e, !0)
         }, t.prototype.decodeStream = function(e) {
             return this.decodeMultiAsync(e, !1)
         }, t.prototype.decodeMultiAsync = function(e, n) {
             return or(this, arguments, function() {
-                var i, o, s, a, u, c, f, h, l;
-                return we(this, function(p) {
-                    switch (p.label) {
+                var i, o, s, a, u, c, f, h, p;
+                return we(this, function(l) {
+                    switch (l.label) {
                         case 0:
-                            i = n, o = -1, p.label = 1;
+                            i = n, o = -1, l.label = 1;
                         case 1:
-                            p.trys.push([1, 13, 14, 19]), s = We(e), p.label = 2;
+                            l.trys.push([1, 13, 14, 19]), s = We(e), l.label = 2;
                         case 2:
                             return [4, G(s.next())];
                         case 3:
-                            if (a = p.sent(), !!a.done) return [3, 12];
+                            if (a = l.sent(), !!a.done) return [3, 12];
                             if (u = a.value, n && o === 0) throw this.createExtraByteError(this.totalPos);
-                            this.appendBuffer(u), i && (o = this.readArraySize(), i = !1, this.complete()), p.label = 4;
+                            this.appendBuffer(u), i && (o = this.readArraySize(), i = !1, this.complete()), l.label = 4;
                         case 4:
-                            p.trys.push([4, 9, , 10]), p.label = 5;
+                            l.trys.push([4, 9, , 10]), l.label = 5;
                         case 5:
                             return [4, G(this.doDecodeSync())];
                         case 6:
-                            return [4, p.sent()];
+                            return [4, l.sent()];
                         case 7:
-                            return p.sent(), --o === 0 ? [3, 8] : [3, 5];
+                            return l.sent(), --o === 0 ? [3, 8] : [3, 5];
                         case 8:
                             return [3, 10];
                         case 9:
-                            if (c = p.sent(), !(c instanceof Oe)) throw c;
+                            if (c = l.sent(), !(c instanceof Oe)) throw c;
                             return [3, 10];
                         case 10:
-                            this.totalPos += this.pos, p.label = 11;
+                            this.totalPos += this.pos, l.label = 11;
                         case 11:
                             return [3, 2];
                         case 12:
                             return [3, 19];
                         case 13:
-                            return f = p.sent(), h = {
+                            return f = l.sent(), h = {
                                 error: f
                             }, [3, 19];
                         case 14:
-                            return p.trys.push([14, , 17, 18]), a && !a.done && (l = s.return) ? [4, G(l.call(s))] : [3, 16];
+                            return l.trys.push([14, , 17, 18]), a && !a.done && (p = s.return) ? [4, G(p.call(s))] : [3, 16];
                         case 15:
-                            p.sent(), p.label = 16;
+                            l.sent(), l.label = 16;
                         case 16:
                             return [3, 18];
                         case 17:
                             if (h) throw h.error;
                             return [7];
                         case 18:
                             return [7];
@@ -1298,130 +1298,130 @@
     const i = {},
         o = /^(rpc|publish|system):(\w+(?:\.\w+)*):(?:\d+)$/,
         s = {};
     let a = null,
         u = 512 * 1024;
     const c = new $n;
 
-    function f(l) {
-        if (l && l.id) {
-            if (l.error) {
-                const p = i[l.id];
-                p ? p.reject(l.error) : console.error("Server error:", l.error)
+    function f(p) {
+        if (p && p.id) {
+            if (p.error) {
+                const l = i[p.id];
+                l ? l.reject(p.error) : console.error("Server error:", p.error)
             } else {
-                const p = o.exec(l.id);
-                if (p) {
-                    const y = p[1];
+                const l = o.exec(p.id);
+                if (l) {
+                    const y = l[1];
                     if (y === "rpc") {
-                        const g = i[l.id];
+                        const g = i[p.id];
                         if (!g) {
-                            console.log("session message id without matching call, dropped", l);
+                            console.log("session message id without matching call, dropped", p);
                             return
                         }
-                        g.resolve(l.result)
+                        g.resolve(p.result)
                     } else if (y == "publish") {
-                        console.assert(i[l.id] === void 0, "publish message received matching in-flight rpc call");
-                        const g = p[2];
+                        console.assert(i[p.id] === void 0, "publish message received matching in-flight rpc call");
+                        const g = l[2];
                         if (!s[g]) return;
-                        s[g].forEach(S => S([l.result]))
+                        s[g].forEach(S => S([p.result]))
                     } else if (y == "system") {
-                        const g = i[l.id];
-                        l.id === "system:c0:0" ? (a = l.result.clientID, u = l.result.maxMsgSize || u, g && g.resolve(a)) : (console.error("Unknown system message", l.id), g && g.reject({
+                        const g = i[p.id];
+                        p.id === "system:c0:0" ? (a = p.result.clientID, u = p.result.maxMsgSize || u, g && g.resolve(a)) : (console.error("Unknown system message", p.id), g && g.reject({
                             code: -32099,
-                            message: `Unknown system message ${l.id}`
+                            message: `Unknown system message ${p.id}`
                         }))
-                    } else console.error("Unknown rpc id format", l.id)
+                    } else console.error("Unknown rpc id format", p.id)
                 }
             }
-            delete i[l.id]
+            delete i[p.id]
         }
     }
-    t.onconnect = l => {
-        const p = Y(),
+    t.onconnect = p => {
+        const l = Y(),
             y = "system:c0:0";
-        i[y] = p;
+        i[y] = l;
         const g = {
                 wslink: "1.0",
                 id: y,
                 method: "wslink.hello",
                 args: [{
                     secret: e.secret
                 }],
                 kwargs: {}
             },
             w = new Xe().encode(g);
         for (let v of Ge(w, u)) e.ws.send(v, {
             binary: !0
         });
-        return p.promise
-    }, t.call = (l, p = [], y = {}) => {
+        return l.promise
+    }, t.call = (p, l = [], y = {}) => {
         const g = Y();
         if (e.ws && a && e.ws.readyState === 1) {
             const S = `rpc:${a}:${r++}`;
             i[S] = g;
             const w = {
                     wslink: "1.0",
                     id: S,
-                    method: l,
-                    args: p,
+                    method: p,
+                    args: l,
                     kwargs: y
                 },
                 U = new Xe().encode(w);
             for (let E of Ge(U, u)) e.ws.send(E, {
                 binary: !0
             })
         } else g.reject({
             code: -32099,
-            message: `RPC call ${l} unsuccessful: connection not open`
+            message: `RPC call ${p} unsuccessful: connection not open`
         });
         return g.promise
-    }, t.subscribe = (l, p) => {
+    }, t.subscribe = (p, l) => {
         const y = Y();
-        return e.ws && a ? (s[l] || (s[l] = []), s[l].push(p), y.resolve({
-            topic: l,
-            callback: p
+        return e.ws && a ? (s[p] || (s[p] = []), s[p].push(l), y.resolve({
+            topic: p,
+            callback: l
         })) : y.reject({
             code: -32099,
-            message: `Subscribe call ${l} unsuccessful: connection not open`
+            message: `Subscribe call ${p} unsuccessful: connection not open`
         }), {
-            topic: l,
-            callback: p,
+            topic: p,
+            callback: l,
             promise: y.promise,
             unsubscribe: () => t.unsubscribe({
-                topic: l,
-                callback: p
+                topic: p,
+                callback: l
             })
         }
-    }, t.unsubscribe = l => {
-        const p = Y(),
+    }, t.unsubscribe = p => {
+        const l = Y(),
             {
                 topic: y,
                 callback: g
-            } = l;
-        if (!s[y]) return p.reject({
+            } = p;
+        if (!s[y]) return l.reject({
             code: -32099,
             message: `Unsubscribe call ${y} unsuccessful: not subscribed`
-        }), p.promise;
+        }), l.promise;
         const S = s[y].indexOf(g);
-        return S !== -1 ? (s[y].splice(S, 1), p.resolve()) : p.reject({
+        return S !== -1 ? (s[y].splice(S, 1), l.resolve()) : l.reject({
             code: -32099,
             message: `Unsubscribe call ${y} unsuccessful: callback not found`
-        }), p.promise
+        }), l.promise
     }, t.close = () => {
-        const l = Y();
-        return e.ws.close(), c.releasePendingMessages(), l.resolve(), l.promise
+        const p = Y();
+        return e.ws.close(), c.releasePendingMessages(), p.resolve(), p.promise
     };
 
     function h() {
         return new ur
     }
-    t.onmessage = async l => {
-        const p = await c.processChunk(l.data, h);
-        p && f(p)
-    }, t.addAttachment = l => l instanceof ArrayBuffer ? new DataView(l) : l
+    t.onmessage = async p => {
+        const l = await c.processChunk(p.data, h);
+        l && f(l)
+    }, t.addAttachment = p => p instanceof ArrayBuffer ? new DataView(p) : p
 }
 const lr = {
     secret: "wslink-secret",
     ws: null
 };
 
 function Et(t, e, n = {}) {
@@ -1621,17 +1621,17 @@
             r = bt,
             i = Object.prototype.propertyIsEnumerable,
             o = !i.call({
                 toString: null
             }, "toString"),
             s = i.call(function() {}, "prototype"),
             a = ["toString", "toLocaleString", "valueOf", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "constructor"],
-            u = function(l) {
-                var p = l.constructor;
-                return p && p.prototype === l
+            u = function(p) {
+                var l = p.constructor;
+                return l && l.prototype === p
             },
             c = {
                 $applicationCache: !0,
                 $console: !0,
                 $external: !0,
                 $frame: !0,
                 $frameElement: !0,
@@ -1652,49 +1652,49 @@
                 $self: !0,
                 $webkitIndexedDB: !0,
                 $webkitStorageInfo: !0,
                 $window: !0
             },
             f = function() {
                 if (typeof window > "u") return !1;
-                for (var l in window) try {
-                    if (!c["$" + l] && e.call(window, l) && window[l] !== null && typeof window[l] == "object") try {
-                        u(window[l])
+                for (var p in window) try {
+                    if (!c["$" + p] && e.call(window, p) && window[p] !== null && typeof window[p] == "object") try {
+                        u(window[p])
                     } catch {
                         return !0
                     }
                 } catch {
                     return !0
                 }
                 return !1
             }(),
-            h = function(l) {
-                if (typeof window > "u" || !f) return u(l);
+            h = function(p) {
+                if (typeof window > "u" || !f) return u(p);
                 try {
-                    return u(l)
+                    return u(p)
                 } catch {
                     return !1
                 }
             };
-        t = function(p) {
-            var y = p !== null && typeof p == "object",
-                g = n.call(p) === "[object Function]",
-                S = r(p),
-                w = y && n.call(p) === "[object String]",
+        t = function(l) {
+            var y = l !== null && typeof l == "object",
+                g = n.call(l) === "[object Function]",
+                S = r(l),
+                w = y && n.call(l) === "[object String]",
                 v = [];
             if (!y && !g && !S) throw new TypeError("Object.keys called on a non-object");
             var U = s && g;
-            if (w && p.length > 0 && !e.call(p, 0))
-                for (var E = 0; E < p.length; ++E) v.push(String(E));
-            if (S && p.length > 0)
-                for (var b = 0; b < p.length; ++b) v.push(String(b));
+            if (w && l.length > 0 && !e.call(l, 0))
+                for (var E = 0; E < l.length; ++E) v.push(String(E));
+            if (S && l.length > 0)
+                for (var b = 0; b < l.length; ++b) v.push(String(b));
             else
-                for (var O in p) !(U && O === "prototype") && e.call(p, O) && v.push(String(O));
+                for (var O in l) !(U && O === "prototype") && e.call(l, O) && v.push(String(O));
             if (o)
-                for (var R = h(p), $ = 0; $ < a.length; ++$) !(R && a[$] === "constructor") && e.call(p, a[$]) && v.push(a[$]);
+                for (var R = h(l), $ = 0; $ < a.length; ++$) !(R && a[$] === "constructor") && e.call(l, a[$]) && v.push(a[$]);
             return v
         }
     }
     return me = t, me
 }
 var br = Array.prototype.slice,
     Lr = bt,
@@ -1980,28 +1980,28 @@
             o = Yr("%" + i + "%", n),
             s = o.name,
             a = o.value,
             u = !1,
             c = o.alias;
         c && (i = c[0], Kr(r, Gr([0, 1], c)));
         for (var f = 1, h = !0; f < r.length; f += 1) {
-            var l = r[f],
-                p = ce(l, 0, 1),
-                y = ce(l, -1);
-            if ((p === '"' || p === "'" || p === "`" || y === '"' || y === "'" || y === "`") && p !== y) throw new P("property names with quotes must have matching quotes");
-            if ((l === "constructor" || !h) && (u = !0), i += "." + l, s = "%" + i + "%", ae(N, s)) a = N[s];
+            var p = r[f],
+                l = ce(p, 0, 1),
+                y = ce(p, -1);
+            if ((l === '"' || l === "'" || l === "`" || y === '"' || y === "'" || y === "`") && l !== y) throw new P("property names with quotes must have matching quotes");
+            if ((p === "constructor" || !h) && (u = !0), i += "." + p, s = "%" + i + "%", ae(N, s)) a = N[s];
             else if (a != null) {
-                if (!(l in a)) {
+                if (!(p in a)) {
                     if (!n) throw new K("base intrinsic for " + e + " exists, but the property is not available.");
                     return
                 }
                 if (I && f + 1 >= r.length) {
-                    var g = I(a, l);
-                    h = !!g, h && "get" in g && !("originalValue" in g.get) ? a = g.get : a = a[l]
-                } else h = ae(a, l), a = a[l];
+                    var g = I(a, p);
+                    h = !!g, h && "get" in g && !("originalValue" in g.get) ? a = g.get : a = a[p]
+                } else h = ae(a, p), a = a[p];
                 h && !u && (N[s] = a)
             }
         }
         return a
     },
     Qr = qr,
     be = Qr("%Object.defineProperty%", !0),
@@ -2447,32 +2447,32 @@
 
 function Wt(t, e, n, r) {
     let i = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
     n.forEach(o => {
         if (e[o] && r && e[o].length !== r) throw new RangeError(`Invalid initial number of values for array (${o})`);
         const s = `_on${x(o)}Changed`;
         t[`set${x(o)}`] = function() {
-            var p;
+            var l;
             if (e.deleted) return T("instance deleted - cannot call any method"), !1;
             for (var a = arguments.length, u = new Array(a), c = 0; c < a; c++) u[c] = arguments[c];
             let f = u,
-                h, l = !1;
-            if (f.length === 1 && (f[0] == null || f[0].length >= 0) && (f = f[0], l = !0), f == null) h = e[o] !== f;
+                h, p = !1;
+            if (f.length === 1 && (f[0] == null || f[0].length >= 0) && (f = f[0], p = !0), f == null) h = e[o] !== f;
             else {
                 if (r && f.length !== r)
                     if (f.length < r && i !== void 0)
-                        for (f = Array.from(f), l = !1; f.length < r;) f.push(i);
+                        for (f = Array.from(f), p = !1; f.length < r;) f.push(i);
                     else throw new RangeError(`Invalid number of values for array setter (${o})`);
                 h = e[o] == null || e[o].length !== f.length;
                 for (let y = 0; !h && y < f.length; ++y) h = e[o][y] !== f[y];
-                h && l && (f = Array.from(f))
+                h && p && (f = Array.from(f))
             }
             if (h) {
                 const y = e[o.name];
-                e[o] = f, (p = e[s]) == null || p.call(e, t, e, f, y), t.modified()
+                e[o] = f, (l = e[s]) == null || l.call(e, t, e, f, y), t.modified()
             }
             return h
         }, t[`set${x(o)}From`] = a => {
             const u = e[o];
             a.forEach((c, f) => {
                 u[f] = c
             })
@@ -2491,117 +2491,117 @@
         e[i] !== void 0 && (e[`_${i}`] = e[i], delete e[i])
     }
 }
 
 function Ii(t, e, n, r) {
     e.inputData ? e.inputData = e.inputData.map(F) : e.inputData = [], e.inputConnection ? e.inputConnection = e.inputConnection.map(F) : e.inputConnection = [], e.output ? e.output = e.output.map(F) : e.output = [], e.inputArrayToProcess ? e.inputArrayToProcess = e.inputArrayToProcess.map(F) : e.inputArrayToProcess = [], e.numberOfInputs = n;
 
-    function i(p) {
+    function i(l) {
         let y = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         if (e.deleted) {
             T("instance deleted - cannot call any method");
             return
         }
         if (y >= e.numberOfInputs) {
             T(`algorithm ${t.getClassName()} only has ${e.numberOfInputs} input ports. To add more input ports, use addInputData()`);
             return
-        }(e.inputData[y] !== p || e.inputConnection[y]) && (e.inputData[y] = p, e.inputConnection[y] = null, t.modified && t.modified())
+        }(e.inputData[y] !== l || e.inputConnection[y]) && (e.inputData[y] = l, e.inputConnection[y] = null, t.modified && t.modified())
     }
 
     function o() {
-        let p = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        return e.inputConnection[p] && (e.inputData[p] = e.inputConnection[p]()), e.inputData[p]
+        let l = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        return e.inputConnection[l] && (e.inputData[l] = e.inputConnection[l]()), e.inputData[l]
     }
 
-    function s(p) {
+    function s(l) {
         let y = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         if (e.deleted) {
             T("instance deleted - cannot call any method");
             return
         }
         if (y >= e.numberOfInputs) {
             let g = `algorithm ${t.getClassName()} only has `;
             g += `${e.numberOfInputs}`, g += " input ports. To add more input ports, use addInputConnection()", T(g);
             return
         }
-        e.inputData[y] = null, e.inputConnection[y] = p
+        e.inputData[y] = null, e.inputConnection[y] = l
     }
 
     function a() {
-        let p = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        return e.inputConnection[p]
+        let l = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        return e.inputConnection[l]
     }
 
     function u() {
-        let p = e.numberOfInputs;
-        for (; p && !e.inputData[p - 1] && !e.inputConnection[p - 1];) p--;
-        return p === e.numberOfInputs && e.numberOfInputs++, p
+        let l = e.numberOfInputs;
+        for (; l && !e.inputData[l - 1] && !e.inputConnection[l - 1];) l--;
+        return l === e.numberOfInputs && e.numberOfInputs++, l
     }
 
-    function c(p) {
+    function c(l) {
         if (e.deleted) {
             T("instance deleted - cannot call any method");
             return
         }
-        s(p, u())
+        s(l, u())
     }
 
-    function f(p) {
+    function f(l) {
         if (e.deleted) {
             T("instance deleted - cannot call any method");
             return
         }
-        i(p, u())
+        i(l, u())
     }
 
     function h() {
-        let p = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        return e.deleted ? (T("instance deleted - cannot call any method"), null) : (t.shouldUpdate() && t.update(), e.output[p])
+        let l = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        return e.deleted ? (T("instance deleted - cannot call any method"), null) : (t.shouldUpdate() && t.update(), e.output[l])
     }
     t.shouldUpdate = () => {
         var S, w;
-        const p = t.getMTime();
+        const l = t.getMTime();
         let y = 1 / 0,
             g = r;
         for (; g--;) {
             if (!e.output[g] || e.output[g].isDeleted()) return !0;
             const v = e.output[g].getMTime();
-            if (v < p) return !0;
+            if (v < l) return !0;
             v < y && (y = v)
         }
         for (g = e.numberOfInputs; g--;)
             if ((S = e.inputConnection[g]) != null && S.filter.shouldUpdate() || ((w = t.getInputData(g)) == null ? void 0 : w.getMTime()) > y) return !0;
         return !1
     };
 
-    function l() {
-        let p = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-        const y = () => h(p);
+    function p() {
+        let l = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
+        const y = () => h(l);
         return y.filter = t, y
     }
     if (e.numberOfInputs) {
-        let p = e.numberOfInputs;
-        for (; p--;) e.inputData.push(null), e.inputConnection.push(null);
+        let l = e.numberOfInputs;
+        for (; l--;) e.inputData.push(null), e.inputConnection.push(null);
         t.setInputData = i, t.setInputConnection = s, t.addInputData = f, t.addInputConnection = c, t.getInputData = o, t.getInputConnection = a
     }
-    r && (t.getOutputData = h, t.getOutputPort = l), t.update = () => {
-        const p = [];
+    r && (t.getOutputData = h, t.getOutputPort = p), t.update = () => {
+        const l = [];
         if (e.numberOfInputs) {
             let y = 0;
-            for (; y < e.numberOfInputs;) p[y] = t.getInputData(y), y++
+            for (; y < e.numberOfInputs;) l[y] = t.getInputData(y), y++
         }
-        t.shouldUpdate() && t.requestData && t.requestData(p, e.output)
-    }, t.getNumberOfInputPorts = () => e.numberOfInputs, t.getNumberOfOutputPorts = () => r || e.output.length, t.getInputArrayToProcess = p => {
-        const y = e.inputArrayToProcess[p],
-            g = e.inputData[p];
+        t.shouldUpdate() && t.requestData && t.requestData(l, e.output)
+    }, t.getNumberOfInputPorts = () => e.numberOfInputs, t.getNumberOfOutputPorts = () => r || e.output.length, t.getInputArrayToProcess = l => {
+        const y = e.inputArrayToProcess[l],
+            g = e.inputData[l];
         return y && g ? g[`get${y.fieldAssociation}`]().getArray(y.arrayName) : null
-    }, t.setInputArrayToProcess = function(p, y, g) {
+    }, t.setInputArrayToProcess = function(l, y, g) {
         let S = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : "Scalars";
-        for (; e.inputArrayToProcess.length < p;) e.inputArrayToProcess.push(null);
-        e.inputArrayToProcess[p] = {
+        for (; e.inputArrayToProcess.length < l;) e.inputArrayToProcess.push(null);
+        e.inputArrayToProcess[l] = {
             arrayName: y,
             fieldAssociation: g,
             attributeType: S
         }
     }
 }
 const Pt = Symbol("Event abort");
@@ -2633,27 +2633,27 @@
     function u() {
         if (e.deleted) {
             T("instance deleted - cannot call any method");
             return
         }
         const c = r.slice();
         for (let f = 0; f < c.length; ++f) {
-            const [, h, l] = c[f];
+            const [, h, p] = c[f];
             if (h) {
-                if (l < 0) setTimeout(() => h.apply(t, arguments), 1 - l);
+                if (p < 0) setTimeout(() => h.apply(t, arguments), 1 - p);
                 else if (h.apply(t, arguments) === Pt) break
             }
         }
     }
     t[`invoke${x(n)}`] = u, t[`on${x(n)}`] = function(c) {
         let f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
         if (!c.apply) return console.error(`Invalid callback for event ${n}`), null;
         if (e.deleted) return T("instance deleted - cannot call any method"), null;
         const h = o++;
-        return r.push([h, c, f]), r.sort((l, p) => p[2] - l[2]), a(h)
+        return r.push([h, c, f]), r.sort((p, l) => l[2] - p[2]), a(h)
     }, t.delete = () => {
         i(), r.forEach(c => {
             let [f] = c;
             return s(f)
         })
     }
 }
@@ -2748,15 +2748,15 @@
     e.proxyId = `${Gi++}`, e.ui = JSON.parse(JSON.stringify(e.ui || [])), pe(t, e, ["proxyId", "proxyGroup", "proxyName"]), Gt(t, e, ["proxyManager"]);
     const r = {},
         i = {};
 
     function o(c, f) {
         i[f] || (i[f] = []);
         const h = i[f];
-        for (let l = 0; l < c.length; l++) h.push(c[l].name), r[c[l].name] = c[l], c[l].children && c[l].children.length && o(c[l].children, c[l].name)
+        for (let p = 0; p < c.length; p++) h.push(c[p].name), r[c[p].name] = c[p], c[p].children && c[p].children.length && o(c[p].children, c[p].name)
     }
     o(e.ui, ne), t.updateUI = c => {
         e.ui = JSON.parse(JSON.stringify(c || [])), Object.keys(r).forEach(f => delete r[f]), Object.keys(i).forEach(f => delete i[f]), o(e.ui, ne), t.modified()
     };
 
     function s() {
         let c = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : ne;
@@ -2777,25 +2777,25 @@
     }, t.gcPropertyLinks = c => {
         const f = e.propertyLinkSubscribers[c] || [];
         for (; f.length;) f.pop().unbind(t)
     }, e.propertyLinkMap = {}, t.getPropertyLink = function(c) {
         let f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
         if (e.propertyLinkMap[c]) return e.propertyLinkMap[c];
         let h = null;
-        const l = [];
-        let p = 0,
+        const p = [];
+        let l = 0,
             y = !1;
 
         function g(E) {
             let b = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
             if (y) return null;
             const O = [];
             let R = null;
-            for (p = l.length; p--;) {
-                const V = l[p];
+            for (l = p.length; l--;) {
+                const V = p[l];
                 V.instance === E ? R = V : O.push(V)
             }
             if (!R) return null;
             const $ = R.instance[`get${x(R.propertyName)}`]();
             if (!Ri($, h) || b) {
                 for (h = $, y = !0; O.length;) {
                     const V = O.pop();
@@ -2806,55 +2806,55 @@
                 y = !1
             }
             return e.propertyLinkMap[c].persistent && (e.propertyLinkMap[c].value = $), $
         }
 
         function S(E, b) {
             const O = [];
-            for (p = l.length; p--;) {
-                const R = l[p];
-                R.instance === E && (R.propertyName === b || b === void 0) && (R.subscription.unsubscribe(), O.push(p))
+            for (l = p.length; l--;) {
+                const R = p[l];
+                R.instance === E && (R.propertyName === b || b === void 0) && (R.subscription.unsubscribe(), O.push(l))
             }
-            for (; O.length;) l.splice(O.pop(), 1)
+            for (; O.length;) p.splice(O.pop(), 1)
         }
 
         function w(E, b) {
             let O = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1;
             const R = E.onModified(g),
-                $ = l[0];
-            return l.push({
+                $ = p[0];
+            return p.push({
                 instance: E,
                 propertyName: b,
                 subscription: R
             }), O && (e.propertyLinkMap[c].persistent && e.propertyLinkMap[c].value !== void 0 ? E.set({
                 [b]: e.propertyLinkMap[c].value
             }) : $ && g($.instance, !0)), {
                 unsubscribe: () => S(E, b)
             }
         }
 
         function v() {
-            for (; l.length;) l.pop().subscription.unsubscribe()
+            for (; p.length;) p.pop().subscription.unsubscribe()
         }
         const U = {
             bind: w,
             unbind: S,
             unsubscribe: v,
             persistent: f
         };
         return e.propertyLinkMap[c] = U, U
     };
 
     function a() {
         let c = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : ne;
         const f = [],
             h = e.proxyId,
-            l = s(c) || [];
-        for (let p = 0; p < l.length; p++) {
-            const y = l[p],
+            p = s(c) || [];
+        for (let l = 0; l < p.length; l++) {
+            const y = p[l],
                 g = t[`get${x(y)}`],
                 S = g ? g() : void 0,
                 w = {
                     id: h,
                     name: y,
                     value: S
                 },
@@ -2877,21 +2877,21 @@
 
     function u() {
         if (e.links)
             for (let c = 0; c < e.links.length; c++) {
                 const {
                     link: f,
                     property: h,
-                    persistent: l,
-                    updateOnBind: p,
+                    persistent: p,
+                    updateOnBind: l,
                     type: y
                 } = e.links[c];
                 if (y === "application") {
-                    const g = e.proxyManager.getPropertyLink(f, l);
-                    t.registerPropertyLinkForGC(g, "application"), g.bind(t, h, p)
+                    const g = e.proxyManager.getPropertyLink(f, p);
+                    t.registerPropertyLinkForGC(g, "application"), g.bind(t, h, l)
                 }
             }
     }
     jt(u)
 }
 
 function Wi(t, e, n) {
@@ -2903,16 +2903,16 @@
         const a = o[s],
             {
                 modelKey: u,
                 property: c,
                 modified: f = !0
             } = n[a],
             h = x(c),
-            l = x(a);
-        t[`get${l}`] = e[u][`get${h}`], t[`set${l}`] = e[u][`set${h}`], f && i.push(e[u].onModified(t.modified))
+            p = x(a);
+        t[`get${p}`] = e[u][`get${h}`], t[`set${p}`] = e[u][`set${h}`], f && i.push(e[u].onModified(t.modified))
     }
     t.delete = () => {
         for (; i.length;) i.pop().unsubscribe();
         r()
     }
 }
 
@@ -3554,19 +3554,19 @@
                 o = Object.keys(r);
             for (let u = 0; u < o.length; u++) {
                 let c = !0;
                 const f = o[u],
                     h = r[f];
                 if ((a = h == null ? void 0 : h._filter) != null && a.length) {
                     c = !1;
-                    const l = this.state[f],
-                        p = Object.keys(h);
-                    for (let y = 0; !c && y < p.length; y++) {
-                        const g = p[y];
-                        g[0] !== "_" && (l === void 0 || l[g] !== h[g]) && (c = !0)
+                    const p = this.state[f],
+                        l = Object.keys(h);
+                    for (let y = 0; !c && y < l.length; y++) {
+                        const g = l[y];
+                        g[0] !== "_" && (p === void 0 || p[g] !== h[g]) && (c = !0)
                     }
                 }
                 c && (i.push(f), this.state[f] = h)
             }
             this.mtime += 1;
             const s = [];
             for (let u = 0; u < i.length; u++) {
@@ -3785,25 +3785,25 @@
         n = n.filter(u => u !== a)
     }, e.connect = async function(a) {
         return e.client || (e.client = Ae.createClient()), e.state && (e.state.delete(), e.client = Ae.createClient()), e.client.isConnected() || await e.client.connect(a), e.client.getConnection().getSession().addAttachment, e.state = new To(e.client), e.config = e.client.getConfig(), await e.state.loadState(), r = !0, o(), e.config
     }, e.trigger = async function(a, u = [], c = {}) {
         let f = [];
         const h = {};
         if (u) {
-            const l = u.map(p => De(p));
-            f = await Promise.all(l)
+            const p = u.map(l => De(l));
+            f = await Promise.all(p)
         }
         if (c) {
-            const l = [],
-                p = [];
+            const p = [],
+                l = [];
             Object.entries(c).forEach(g => {
-                l.push(g[0]), p.push(De(g[1]))
+                p.push(g[0]), l.push(De(g[1]))
             });
-            const y = await Promise.all(p);
-            for (let g = 0; g < l.length; g++) h[l[g]] = y[g]
+            const y = await Promise.all(l);
+            for (let g = 0; g < p.length; g++) h[p[g]] = y[g]
         }
         return await e.client.getRemote().Trame.trigger(a, f, h)
     }, window.trame = e, e
 }
 const {
     inject: an,
     ref: cn,
@@ -3920,29 +3920,29 @@
                 n = re(!1),
                 r = re(1),
                 i = re(1),
                 o = [];
 
             function s(f) {
                 const h = `trame-template-${f.toLowerCase().substring(16)}`.replaceAll("_", "-").replaceAll("--", "-"),
-                    l = t.state.get(f);
+                    p = t.state.get(f);
                 t.app.component(h, {
                     props: ["name"],
                     setup: Fo,
-                    template: l
+                    template: p
                 })
             }
             const a = ({
                 type: f,
                 keys: h
             }) => {
                 if (f === "dirty-state")
-                    for (let l = 0; l < h.length; l++) {
-                        const p = h[l];
-                        p.startsWith("trame__template_") && s(p)
+                    for (let p = 0; p < h.length; p++) {
+                        const l = h[p];
+                        l.startsWith("trame__template_") && s(l)
                     } else f === "refresh" ? i.value++ : f === "ready" && (n.value = !0, i.value++)
             };
 
             function u(f) {
                 r.value = f, t.state && t.state.set("trame__busy", f), f === 0 && t.state.flush()
             }
 
@@ -3982,25 +3982,25 @@
                 o.push(() => {
                     var w, v, U;
                     return (U = (v = (w = t == null ? void 0 : t.client) == null ? void 0 : w.getRemote()) == null ? void 0 : v.Trame) == null ? void 0 : U.unsubscribe(h)
                 }), (S = (g = (y = t.client) == null ? void 0 : y.getRemote()) == null ? void 0 : g.Trame) == null || S.lifeCycleUpdate("client_connected"), window.addEventListener("beforeunload", () => {
                     var w, v, U;
                     return (U = (v = (w = t.client) == null ? void 0 : w.getRemote()) == null ? void 0 : v.Trame) == null ? void 0 : U.lifeCycleUpdate("client_exited")
                 });
-                const l = window.trame.utils.router,
-                    p = t.state.get("trame__routes");
-                p != null && p.length && l && p.forEach(w => {
-                    l.addRoute(w)
+                const p = window.trame.utils.router,
+                    l = t.state.get("trame__routes");
+                l != null && l.length && p && l.forEach(w => {
+                    p.addRoute(w)
                 })
             }
             return Vo(() => {
                 t.addConnectListener(c)
             }), zo(() => {
-                var f, h, l;
-                for (t.removeConnectListener(c), (l = (h = (f = t.client) == null ? void 0 : f.getRemote()) == null ? void 0 : h.Trame) == null || l.lifeCycleUpdate("client_unmounted"); o.length;) o.pop()()
+                var f, h, p;
+                for (t.removeConnectListener(c), (p = (h = (f = t.client) == null ? void 0 : f.getRemote()) == null ? void 0 : h.Trame) == null || p.lifeCycleUpdate("client_unmounted"); o.length;) o.pop()()
             }), {
                 connected: e,
                 ready: n,
                 busy: r,
                 refreshTS: i
             }
         },
@@ -4037,15 +4037,15 @@
                 n = lt(null),
                 r = lt(null);
 
             function i(a, u) {
                 const c = JSON.parse(JSON.stringify(e.state.get(t.name)));
                 let f = c;
                 const h = String(a).split(".");
-                for (let l = 0; l < h.length - 1; l++) f = f[h[l]];
+                for (let p = 0; p < h.length - 1; p++) f = f[h[p]];
                 f[h.at(-1)] = u, e.state.set(t.name, c)
             }
 
             function o(a) {
                 e.state.set(t.name, a)
             }
 
@@ -4306,23 +4306,30 @@
         setup(t, {
             emit: e
         }) {
             const n = ms("trame"),
                 r = Ss(null);
 
             function i() {
-                const s = r.value.getBoundingClientRect(),
-                    a = window.devicePixelRatio,
-                    u = 96 * a,
-                    c = {
-                        size: s,
-                        pixelRatio: a,
-                        dpi: u
-                    };
-                t.name && (c.name = t.name), n && n.state.set(t.name, c), e("change", c)
+                const {
+                    x: s,
+                    y: a,
+                    width: u,
+                    height: c
+                } = r.value.getBoundingClientRect(), f = {
+                    x: s,
+                    y: a,
+                    width: u,
+                    height: c
+                }, h = window.devicePixelRatio, p = 96 * h, l = {
+                    size: f,
+                    pixelRatio: h,
+                    dpi: p
+                };
+                t.name && (l.name = t.name), n && n.state.set(t.name, l), e("change", l)
             }
             const o = new ResizeObserver(i);
             return xs(() => {
                 o.observe(r.value)
             }), Es(() => {
                 o.unobserve(r.value)
             }), {
```

### Comparing `trame-client-3.0.1/trame_client/module/vue3-www/assets/index-e80c1ba5.css` & `trame-client-3.0.2/trame_client/module/vue3-www/assets/index-e80c1ba5.css`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue3-www/index.html` & `trame-client-3.0.2/trame_client/module/vue3-www/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <meta name="keywords" content="trame, OpenSource, Stateful Python Application, Kitware">
     <meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate" />
     <meta http-equiv="Pragma" content="no-cache" />
     <meta http-equiv="Expires" content="0" />
     <link rel="icon" href="logo.png">
     <title>trame is built by Kitware</title>
     <script src="vue.global.js"></script>
-    <script type="module" crossorigin src="./assets/index-26129a2a.js"></script>
+    <script type="module" crossorigin src="./assets/index-75032529.js"></script>
     <link rel="stylesheet" href="./assets/index-e80c1ba5.css">
   </head>
   <body>
     <noscript>
       <strong>We're sorry but trame built by Kitware doesn't work properly without JavaScript enabled. Please enable it to continue.</strong>
     </noscript>
     <div id="app"></div>
```

### Comparing `trame-client-3.0.1/trame_client/module/vue3-www/loading.tpl` & `trame-client-3.0.2/trame_client/module/vue3-www/loading.tpl`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue3-www/logo.png` & `trame-client-3.0.2/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/module/vue3-www/vue.global.js` & `trame-client-3.0.2/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/resources/attributes.json` & `trame-client-3.0.2/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/resources/vue.json` & `trame-client-3.0.2/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/ui/core.py` & `trame-client-3.0.2/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/ui/html.py` & `trame-client-3.0.2/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/utils/formatter.py` & `trame-client-3.0.2/trame_client/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/utils/testing.py` & `trame-client-3.0.2/trame_client/utils/testing.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/utils/version.py` & `trame-client-3.0.2/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/utils/web_module.py` & `trame-client-3.0.2/trame_client/utils/web_module.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/widgets/core.py` & `trame-client-3.0.2/trame_client/widgets/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/widgets/generator.py` & `trame-client-3.0.2/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/widgets/html.py` & `trame-client-3.0.2/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client/widgets/trame.py` & `trame-client-3.0.2/trame_client/widgets/trame.py`

 * *Files identical despite different names*

### Comparing `trame-client-3.0.1/trame_client.egg-info/PKG-INFO` & `trame-client-3.0.2/trame_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-client-3.0.1/trame_client.egg-info/SOURCES.txt` & `trame-client-3.0.2/trame_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 trame_client/module/vue2.py
 trame_client/module/vue3.py
 trame_client/module/vue2-www/index.html
 trame_client/module/vue2-www/loading.tpl
 trame_client/module/vue2-www/logo.png
 trame_client/module/vue2-www/vue.global.js
 trame_client/module/vue2-www/css/app.0b077e70.css
-trame_client/module/vue2-www/js/app.7c11979c.js
+trame_client/module/vue2-www/js/app.7d0e64a7.js
 trame_client/module/vue2-www/js/chunk-vendors.3aa0189c.js
 trame_client/module/vue3-www/index.html
 trame_client/module/vue3-www/loading.tpl
 trame_client/module/vue3-www/logo.png
 trame_client/module/vue3-www/vue.global.js
-trame_client/module/vue3-www/assets/index-26129a2a.js
+trame_client/module/vue3-www/assets/index-75032529.js
 trame_client/module/vue3-www/assets/index-e80c1ba5.css
 trame_client/resources/attributes.json
 trame_client/resources/events.json
 trame_client/resources/vue.json
 trame_client/ui/__init__.py
 trame_client/ui/core.py
 trame_client/ui/html.py
```

