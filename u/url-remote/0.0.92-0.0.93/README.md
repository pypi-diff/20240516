# Comparing `tmp/url_remote-0.0.92.tar.gz` & `tmp/url_remote-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url_remote-0.0.92.tar", last modified: Sun May 12 22:47:50 2024, max compression
+gzip compressed data, was "url_remote-0.0.93.tar", last modified: Thu May 16 17:12:36 2024, max compression
```

## Comparing `url_remote-0.0.92.tar` & `url_remote-0.0.93.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.047888 url_remote-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-12 22:47:50.047888 url_remote-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-12 22:47:42.000000 url_remote-0.0.92/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-12 22:47:42.000000 url_remote-0.0.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 22:47:50.047888 url_remote-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-12 22:47:42.000000 url_remote-0.0.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.043888 url_remote-0.0.92/url_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.047888 url_remote-0.0.92/url_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/action_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/api_version_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/authentiction_api_version_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/brand_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/component_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/entity_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/environment_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/url_circlez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.047888 url_remote-0.0.92/url_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:12:36.027149 url_remote-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 17:12:36.027149 url_remote-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 17:12:26.000000 url_remote-0.0.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 17:12:26.000000 url_remote-0.0.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 17:12:36.027149 url_remote-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 17:12:26.000000 url_remote-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:12:36.023149 url_remote-0.0.93/url_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:12:36.027149 url_remote-0.0.93/url_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/action_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/api_version_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/authentiction_api_version_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/brand_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/component_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/entity_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/environment_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/our_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 17:12:26.000000 url_remote-0.0.93/url_remote/src/url_circlez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:12:36.027149 url_remote-0.0.93/url_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 17:12:36.000000 url_remote-0.0.93/url_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 17:12:36.000000 url_remote-0.0.93/url_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:12:36.000000 url_remote-0.0.93/url_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 17:12:36.000000 url_remote-0.0.93/url_remote.egg-info/top_level.txt
```

### Comparing `url_remote-0.0.92/README.md` & `url_remote-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.92/setup.py` & `url_remote-0.0.93/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "url-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.92',  # https://pypi.org/project/url-remote
+    version='0.0.93',  # https://pypi.org/project/url-remote
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="URL Local",
```

### Comparing `url_remote-0.0.92/url_remote/src/action_name_enum.py` & `url_remote-0.0.93/url_remote/src/action_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.92/url_remote/src/component_name_enum.py` & `url_remote-0.0.93/url_remote/src/component_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.92/url_remote/src/url_circlez.py` & `url_remote-0.0.93/url_remote/src/our_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'event.play1.circ.zone': '2iclscptqh.execute-api.us-east-1.amazonaws.com',
         'event.dvlp1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',
         'storage.play1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',  # TODO update
         'storage.dvlp1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',  # TODO update
         'smartlink.play1.circ.zone': 'wagdetw4hk.execute-api.us-east-1.amazonaws.com/dev',
         'smartlink.dvlp1.circ.zone': '6cqasxkwcl.execute-api.us-east-1.amazonaws.com/dev',
         'dialogWorkflow.play1.circ.zone': 'g91pb4afb1.execute-api.us-east-1.amazonaws.com/dev',
-        'dialogWorkflow.dvlp1.circ.zone': '989h6gwvmb.execute-api.us-east-1.amazonaws.com',
+        'dialogWorkflow.dvlp1.circ.zone': 'xoonx24zbg.execute-api.us-east-1.amazonaws.com/dev',
         # 'websocket.dvlp1.circ.zone': 'ws://23.22.217.199:8080',
         # 'websocket.play1.circ.zone': 'ws://23.22.217.199:8080',
     }
 
     @staticmethod
     def _base_domain(brand_name: str, environment_name: str) -> str:
         """
```

