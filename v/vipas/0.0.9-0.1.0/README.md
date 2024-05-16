# Comparing `tmp/vipas-0.0.9.tar.gz` & `tmp/vipas-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.0.9.tar", last modified: Mon May 13 15:34:16 2024, max compression
+gzip compressed data, was "vipas-0.1.0.tar", last modified: Wed May 15 18:10:36 2024, max compression
```

## Comparing `vipas-0.0.9.tar` & `vipas-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 15:34:16.774093 vipas-0.0.9/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.9/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 15:34:16.774093 vipas-0.0.9/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.9/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.9/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-13 15:34:16.774093 vipas-0.0.9/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-13 15:33:54.000000 vipas-0.0.9/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 15:34:16.762093 vipas-0.0.9/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-12 09:48:23.000000 vipas-0.0.9/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 15:34:16.774093 vipas-0.0.9/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.9/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.9/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4122 2024-05-13 15:33:46.000000 vipas-0.0.9/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.9/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-12 09:47:51.000000 vipas-0.0.9/vipas/model.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 15:34:16.774093 vipas-0.0.9/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 15:34:16.000000 vipas-0.0.9/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-13 15:34:16.000000 vipas-0.0.9/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-13 15:34:16.000000 vipas-0.0.9/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-13 15:34:16.000000 vipas-0.0.9/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-13 15:34:16.000000 vipas-0.0.9/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.020362 vipas-0.1.0/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.0/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-15 18:10:36.020362 vipas-0.1.0/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.0/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.0/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-15 18:10:36.020362 vipas-0.1.0/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-15 16:38:12.000000 vipas-0.1.0/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.016362 vipas-0.1.0/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.0/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.020362 vipas-0.1.0/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.0/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.1.0/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.0/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.1.0/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-14 08:16:21.000000 vipas-0.1.0/vipas/model.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-15 18:10:36.020362 vipas-0.1.0/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-15 18:10:36.000000 vipas-0.1.0/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.0.9/LICENSE.md` & `vipas-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.9/README.md` & `vipas-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.9/setup.py` & `vipas-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.0.9"
+VERSION = "0.1.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.0.9/test/test_model_client.py` & `vipas-0.1.0/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.9/vipas/__init__.py` & `vipas-0.1.0/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.9/vipas/_rest.py` & `vipas-0.1.0/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.9/vipas/config.py` & `vipas-0.1.0/vipas/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if not self.vps_auth_token:
             self.setup_api_key()
 
     def setup_api_key(self):
         """Set up API key based on environment."""
         env_type = os.getenv("VPS_ENV_TYPE")
         if env_type == "vipas-streamlit":
-            self.host = "http://vps-proxy-service.vps-control.svc.cluster.local:443" 
+            self.host = "https://ix41nuuq3c-vpce-0c3dea8dfd371e6a1.execute-api.ap-south-1.amazonaws.com/v1" 
             self.vps_auth_token = self.extract_websocket_api_key()
         else:
             self.vps_auth_token = os.getenv("VPS_AUTH_TOKEN")
             if self.vps_auth_token is None or len(self.vps_auth_token) == 0:
                 raise ClientException(400, "VPS_AUTH_TOKEN is not set in the environment variables or it is empty")
 
     def extract_websocket_api_key(self):
```

### Comparing `vipas-0.0.9/vipas/exceptions.py` & `vipas-0.1.0/vipas/exceptions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.9/vipas/model.py` & `vipas-0.1.0/vipas/model.py`

 * *Files identical despite different names*

