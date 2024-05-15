# Comparing `tmp/ploomber-cloud-0.2.7.tar.gz` & `tmp/ploomber-cloud-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.7.tar", last modified: Wed May  8 23:02:09 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.8.tar", last modified: Wed May 15 22:37:25 2024, max compression
```

## Comparing `ploomber-cloud-0.2.7.tar` & `ploomber-cloud-0.2.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.142724 ploomber-cloud-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.146724 ploomber-cloud-0.2.7/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.062686 ploomber-cloud-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.7/CHANGELOG.md` & `ploomber-cloud-0.2.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.2.8 (2024-05-15)
+
+- [Feature] Add support for Flask applications
+
 ## 0.2.7 (2024-05-08)
 
 - [Feature] Add `--clear-cache` option to `ploomber-cloud examples`.
 
 ## 0.2.6 (2024-05-03)
 
 - [Feature] Allow switching the config file to use via `--config/-c` in `init`, `deploy`, `templates`, `resources`, and `labels` subcommands
```

### Comparing `ploomber-cloud-0.2.7/pyproject.toml` & `ploomber-cloud-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/setup.py` & `ploomber-cloud-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/abc.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/abc.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/api.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/config.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/constants.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
     "voila",
     "streamlit",
     "docker",
     "panel",
     "solara",
     "shiny-r",
     "dash",
+    "flask",
 }
 
 VALID_DOCKER_PROJECT_TYPES = {
-    "flask",
     "fastapi",
     "chainlit",
     "gradio",
     "shiny",
 }
 
 FORCE_INIT_MESSAGE = (
```

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/examples.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/init.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/io.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/io.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/labels.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/labels.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/templates.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/templates.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.8/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

