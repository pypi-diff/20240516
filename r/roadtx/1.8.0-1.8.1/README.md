# Comparing `tmp/roadtx-1.8.0.tar.gz` & `tmp/roadtx-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.8.0.tar", last modified: Wed May  1 14:39:32 2024, max compression
+gzip compressed data, was "roadtx-1.8.1.tar", last modified: Thu May  2 11:01:46 2024, max compression
```

## Comparing `roadtx-1.8.0.tar` & `roadtx-1.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.463863 roadtx-1.8.0/
--rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-05-01 14:39:32.463863 roadtx-1.8.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.459863 roadtx-1.8.0/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.463863 roadtx-1.8.0/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (127)    17458 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/federation.py
--rw-r--r--   0 vsts      (1001) docker     (127)   208284 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/firstpartyscopes.json
--rw-r--r--   0 vsts      (1001) docker     (127)     7865 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81212 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23357 2024-05-01 14:37:27.000000 roadtx-1.8.0/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 14:39:32.463863 roadtx-1.8.0/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-01 14:39:28.000000 roadtx-1.8.0/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-05-01 14:39:32.000000 roadtx-1.8.0/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-01 14:39:32.463863 roadtx-1.8.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1157 2024-05-01 14:37:27.000000 roadtx-1.8.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 11:01:46.836073 roadtx-1.8.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-05-02 11:01:46.836073 roadtx-1.8.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 11:01:46.832073 roadtx-1.8.1/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 11:01:46.836073 roadtx-1.8.1/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17458 2024-05-02 11:00:10.000000 roadtx-1.8.1/roadtools/roadtx/federation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   208284 2024-05-02 11:00:10.000000 roadtx-1.8.1/roadtools/roadtx/firstpartyscopes.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     7865 2024-05-02 11:00:10.000000 roadtx-1.8.1/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81271 2024-05-02 11:00:10.000000 roadtx-1.8.1/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23357 2024-05-02 11:00:10.000000 roadtx-1.8.1/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-02 11:01:46.836073 roadtx-1.8.1/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-05-02 11:01:46.000000 roadtx-1.8.1/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-05-02 11:01:46.000000 roadtx-1.8.1/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-02 11:01:46.000000 roadtx-1.8.1/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-02 11:01:46.000000 roadtx-1.8.1/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-02 11:01:43.000000 roadtx-1.8.1/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-02 11:01:46.000000 roadtx-1.8.1/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-05-02 11:01:46.000000 roadtx-1.8.1/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-02 11:01:46.836073 roadtx-1.8.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1157 2024-05-02 11:00:10.000000 roadtx-1.8.1/setup.py
```

### Comparing `roadtx-1.8.0/PKG-INFO` & `roadtx-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.8.0
+Version: 1.8.1
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.8.0/roadtools/roadtx/federation.py` & `roadtx-1.8.1/roadtools/roadtx/federation.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.8.0/roadtools/roadtx/firstpartyscopes.json` & `roadtx-1.8.1/roadtools/roadtx/firstpartyscopes.json`

 * *Files identical despite different names*

### Comparing `roadtx-1.8.0/roadtools/roadtx/keepass.py` & `roadtx-1.8.1/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.8.0/roadtools/roadtx/main.py` & `roadtx-1.8.1/roadtools/roadtx/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,14 +891,16 @@
             print(f"{alias:<15} - {useragent}")
     elif args.command == 'interactiveauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
         auth.use_cae = args.cae
+        if args.scope:
+            auth.scope = args.scope
         # Intercept if custom UA is set
         custom_ua = args.user_agent is not None
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
```

### Comparing `roadtx-1.8.0/roadtools/roadtx/selenium.py` & `roadtx-1.8.1/roadtools/roadtx/selenium.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.8.0/roadtx.egg-info/PKG-INFO` & `roadtx-1.8.1/roadtx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.8.0
+Version: 1.8.1
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.8.0/setup.py` & `roadtx-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.8.0',
+      version='1.8.1',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
```

