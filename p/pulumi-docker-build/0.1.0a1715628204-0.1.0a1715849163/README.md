# Comparing `tmp/pulumi_docker_build-0.1.0a1715628204.tar.gz` & `tmp/pulumi_docker_build-0.1.0a1715849163.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker_build-0.1.0a1715628204.tar", last modified: Mon May 13 19:30:34 2024, max compression
+gzip compressed data, was "pulumi_docker_build-0.1.0a1715849163.tar", last modified: Thu May 16 08:52:52 2024, max compression
```

## Comparing `pulumi_docker_build-0.1.0a1715628204.tar` & `pulumi_docker_build-0.1.0a1715849163.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 19:30:34.196105 pulumi_docker_build-0.1.0a1715628204/
--rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-13 19:30:34.196105 pulumi_docker_build-0.1.0a1715628204/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2057 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 19:30:34.192105 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/
--rw-------   0 runner    (1000) runner    (1000)      983 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1928 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/_enums.py
--rw-------   0 runner    (1000) runner    (1000)    97964 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/_inputs.py
--rw-------   0 runner    (1000) runner    (1000)     9230 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 19:30:34.192105 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/config/
--rw-------   0 runner    (1000) runner    (1000)      267 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/config/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      441 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/config/__init__.pyi
--rw-------   0 runner    (1000) runner    (1000)      756 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/config/vars.py
--rw-------   0 runner    (1000) runner    (1000)    75687 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/image.py
--rw-------   0 runner    (1000) runner    (1000)    14598 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/index.py
--rw-------   0 runner    (1000) runner    (1000)    83253 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/outputs.py
--rw-------   0 runner    (1000) runner    (1000)     4780 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/provider.py
--rw-------   0 runner    (1000) runner    (1000)       49 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/pulumi-plugin.json
--rw-------   0 runner    (1000) runner    (1000)        0 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-13 19:30:34.192105 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-13 19:30:34.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-05-13 19:30:34.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-13 19:30:34.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-05-13 19:30:34.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-05-13 19:30:34.000000 pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      736 2024-05-13 19:30:23.000000 pulumi_docker_build-0.1.0a1715628204/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-13 19:30:34.196105 pulumi_docker_build-0.1.0a1715628204/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-16 08:52:52.985834 pulumi_docker_build-0.1.0a1715849163/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-16 08:52:52.985834 pulumi_docker_build-0.1.0a1715849163/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2057 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-16 08:52:52.985834 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/
+-rw-------   0 runner    (1000) runner    (1000)      983 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1928 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/_enums.py
+-rw-------   0 runner    (1000) runner    (1000)    97964 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/_inputs.py
+-rw-------   0 runner    (1000) runner    (1000)     9230 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-16 08:52:52.985834 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/config/
+-rw-------   0 runner    (1000) runner    (1000)      267 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/config/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      441 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/config/__init__.pyi
+-rw-------   0 runner    (1000) runner    (1000)      756 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/config/vars.py
+-rw-------   0 runner    (1000) runner    (1000)    75687 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/image.py
+-rw-------   0 runner    (1000) runner    (1000)    14598 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/index.py
+-rw-------   0 runner    (1000) runner    (1000)    83253 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/outputs.py
+-rw-------   0 runner    (1000) runner    (1000)     4780 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/provider.py
+-rw-------   0 runner    (1000) runner    (1000)       49 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/pulumi-plugin.json
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-16 08:52:52.985834 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2554 2024-05-16 08:52:52.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-05-16 08:52:52.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-16 08:52:52.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-05-16 08:52:52.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-05-16 08:52:52.000000 pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      736 2024-05-16 08:52:41.000000 pulumi_docker_build-0.1.0a1715849163/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-16 08:52:52.985834 pulumi_docker_build-0.1.0a1715849163/setup.cfg
```

### Comparing `pulumi_docker_build-0.1.0a1715628204/PKG-INFO` & `pulumi_docker_build-0.1.0a1715849163/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker_build
-Version: 0.1.0a1715628204
+Version: 0.1.0a1715849163
 Summary: A Pulumi provider for building modern Docker images with buildx and BuildKit.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker-build
 Keywords: docker,buildkit,buildx,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker_build-0.1.0a1715628204/README.md` & `pulumi_docker_build-0.1.0a1715849163/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/__init__.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/_enums.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/_inputs.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/_utilities.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/config/vars.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/image.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/index.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/outputs.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build/provider.py` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/PKG-INFO` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker_build
-Version: 0.1.0a1715628204
+Version: 0.1.0a1715849163
 Summary: A Pulumi provider for building modern Docker images with buildx and BuildKit.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker-build
 Keywords: docker,buildkit,buildx,kind/native
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker_build-0.1.0a1715628204/pulumi_docker_build.egg-info/SOURCES.txt` & `pulumi_docker_build-0.1.0a1715849163/pulumi_docker_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.1.0a1715628204/pyproject.toml` & `pulumi_docker_build-0.1.0a1715849163/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_docker_build"
   description = "A Pulumi provider for building modern Docker images with buildx and BuildKit."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["docker", "buildkit", "buildx", "kind/native"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715628204"
+  version = "0.1.0a1715849163"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-docker-build"
 
 [build-system]
```

