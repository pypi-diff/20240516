# Comparing `tmp/prefect_kubernetes-0.3.8.tar.gz` & `tmp/prefect_kubernetes-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_kubernetes-0.3.8.tar", last modified: Thu Apr 25 19:20:16 2024, max compression
+gzip compressed data, was "prefect_kubernetes-0.3.9.tar", last modified: Fri Apr 26 15:03:56 2024, max compression
```

## Comparing `prefect_kubernetes-0.3.8.tar` & `prefect_kubernetes-0.3.9.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.421620 prefect_kubernetes-0.3.8/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:15.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    47720 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.425620 prefect_kubernetes-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/kube_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/multiple_resource_defintion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_complex_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_pod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_events_replicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   117678 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.028932 prefect_kubernetes-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-26 15:03:56.028932 prefect_kubernetes-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.020932 prefect_kubernetes-0.3.9/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47720 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.028932 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-26 15:03:55.000000 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-26 15:03:56.000000 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:55.000000 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 15:03:55.000000 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-26 15:03:55.000000 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 15:03:55.000000 prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:56.028932 prefect_kubernetes-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.024932 prefect_kubernetes-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/kube_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:56.028932 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/multiple_resource_defintion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/sample_complex_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/sample_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/sample_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/sample_pod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/sample_k8s_resources/sample_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_events_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117678 2024-04-26 15:03:43.000000 prefect_kubernetes-0.3.9/tests/test_worker.py
```

### Comparing `prefect_kubernetes-0.3.8/PKG-INFO` & `prefect_kubernetes-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prefect integrations for interacting with Kubernetes.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-kubernetes
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: kubernetes>=24.2.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

### Comparing `prefect_kubernetes-0.3.8/README.md` & `prefect_kubernetes-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/credentials.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/custom_objects.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/deployments.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/events.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/events.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/exceptions.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/flows.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/flows.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/jobs.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/pods.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/services.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/utilities.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes/worker.py` & `prefect_kubernetes-0.3.9/prefect_kubernetes/worker.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/PKG-INFO` & `prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prefect integrations for interacting with Kubernetes.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-kubernetes
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: kubernetes>=24.2.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
```

### Comparing `prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect_kubernetes-0.3.9/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 prefect_kubernetes/__init__.py
 prefect_kubernetes/_version.py
 prefect_kubernetes/credentials.py
 prefect_kubernetes/custom_objects.py
 prefect_kubernetes/deployments.py
```

### Comparing `prefect_kubernetes-0.3.8/pyproject.toml` & `prefect_kubernetes-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/conftest.py` & `prefect_kubernetes-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_complex_deployment.yaml` & `prefect_kubernetes-0.3.9/tests/sample_k8s_resources/sample_complex_deployment.yaml`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_block_standards.py` & `prefect_kubernetes-0.3.9/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_credentials.py` & `prefect_kubernetes-0.3.9/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_custom_objects.py` & `prefect_kubernetes-0.3.9/tests/test_custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_deployments.py` & `prefect_kubernetes-0.3.9/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_events_replicator.py` & `prefect_kubernetes-0.3.9/tests/test_events_replicator.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_flows.py` & `prefect_kubernetes-0.3.9/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_jobs.py` & `prefect_kubernetes-0.3.9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_pods.py` & `prefect_kubernetes-0.3.9/tests/test_pods.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_services.py` & `prefect_kubernetes-0.3.9/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_utilities.py` & `prefect_kubernetes-0.3.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prefect_kubernetes-0.3.8/tests/test_worker.py` & `prefect_kubernetes-0.3.9/tests/test_worker.py`

 * *Files identical despite different names*

