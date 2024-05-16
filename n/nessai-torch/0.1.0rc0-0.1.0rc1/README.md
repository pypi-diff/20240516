# Comparing `tmp/nessai_torch-0.1.0rc0.tar.gz` & `tmp/nessai_torch-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai_torch-0.1.0rc0.tar", last modified: Thu May 16 14:01:54 2024, max compression
+gzip compressed data, was "nessai_torch-0.1.0rc1.tar", last modified: Thu May 16 14:09:05 2024, max compression
```

## Comparing `nessai_torch-0.1.0rc0.tar` & `nessai_torch-0.1.0rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.431746 nessai_torch-0.1.0rc0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.419746 nessai_torch-0.1.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.423746 nessai_torch-0.1.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.423746 nessai_torch-0.1.0rc0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/examples/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:01:54.431746 nessai_torch-0.1.0rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.419746 nessai_torch-0.1.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.423746 nessai_torch-0.1.0rc0/src/nessai_torch/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/evidence.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/src/nessai_torch/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/proposal/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/proposal/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/proposal/spherical.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/tensorlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/src/nessai_torch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/gammaincinv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/src/nessai_torch/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-16 14:01:54.000000 nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-16 14:01:54.000000 nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:01:54.000000 nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 14:01:54.000000 nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 14:01:54.000000 nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/tests/integration_tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/tests/test_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:01:54.427746 nessai_torch-0.1.0rc0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/tests/test_utils/test_gammaincinv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/tests/test_utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-16 14:01:49.000000 nessai_torch-0.1.0rc0/tests/test_utils/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.104478 nessai_torch-0.1.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.092478 nessai_torch-0.1.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.096478 nessai_torch-0.1.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-16 14:09:05.104478 nessai_torch-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.096478 nessai_torch-0.1.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:09:05.104478 nessai_torch-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.092478 nessai_torch-0.1.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.096478 nessai_torch-0.1.0rc1/src/nessai_torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.100478 nessai_torch-0.1.0rc1/src/nessai_torch/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/proposal/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/proposal/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/proposal/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/tensorlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.100478 nessai_torch-0.1.0rc1/src/nessai_torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/gammaincinv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/src/nessai_torch/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.100478 nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-16 14:09:05.000000 nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-16 14:09:05.000000 nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:09:05.000000 nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 14:09:05.000000 nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 14:09:05.000000 nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.100478 nessai_torch-0.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.100478 nessai_torch-0.1.0rc1/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/tests/integration_tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:05.100478 nessai_torch-0.1.0rc1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/tests/test_utils/test_gammaincinv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/tests/test_utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-16 14:09:00.000000 nessai_torch-0.1.0rc1/tests/test_utils/test_sample.py
```

### Comparing `nessai_torch-0.1.0rc0/.github/workflows/publish.yml` & `nessai_torch-0.1.0rc1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/.github/workflows/tests.yml` & `nessai_torch-0.1.0rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/.gitignore` & `nessai_torch-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/LICENSE` & `nessai_torch-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/PKG-INFO` & `nessai_torch-0.1.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai-torch
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: nessai in pure PyTorch
 Author-email: "Michael J. Williams" <michaeljw1@googlemail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,28 +28,30 @@
 
 `nessai-torch` can be install using `pip`:
 
 ```
 pip install nessai-torch
 ```
 
-We recommend install PyTorch first to ensure the version is compatible with
+We recommend installing PyTorch first to ensure the version is compatible with
 your system.
 
 ## Basic usage
 
 `nessai-torch` has a different API to `nessai`, the user must define a
 log-likelihood function and a prior-transform function instead of a model
 object. It also has a reduced feature set compared to standard `nessai`.
 The basic usage is shown below, for a more complete example, see the
 `examples` directory.
 
 ```python
 from nessai_torch.sampler import Sampler
 
+# Define the log-likelihood and prior transform
+...
 
 sampler = Sampler(
 	log_likelihood=log_likelihood_fn,
 	prior_transform=prior_transform_fn,
 	dims=dims,  # Number of dimensions
 )
```

### Comparing `nessai_torch-0.1.0rc0/README.md` & `nessai_torch-0.1.0rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 
 `nessai-torch` can be install using `pip`:
 
 ```
 pip install nessai-torch
 ```
 
-We recommend install PyTorch first to ensure the version is compatible with
+We recommend installing PyTorch first to ensure the version is compatible with
 your system.
 
 ## Basic usage
 
 `nessai-torch` has a different API to `nessai`, the user must define a
 log-likelihood function and a prior-transform function instead of a model
 object. It also has a reduced feature set compared to standard `nessai`.
 The basic usage is shown below, for a more complete example, see the
 `examples` directory.
 
 ```python
 from nessai_torch.sampler import Sampler
 
+# Define the log-likelihood and prior transform
+...
 
 sampler = Sampler(
 	log_likelihood=log_likelihood_fn,
 	prior_transform=prior_transform_fn,
 	dims=dims,  # Number of dimensions
 )
```

### Comparing `nessai_torch-0.1.0rc0/examples/rosenbrock.py` & `nessai_torch-0.1.0rc1/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/pyproject.toml` & `nessai_torch-0.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/evidence.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/evidence.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/flows.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/flows.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/plot.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/plot.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/proposal/base.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/proposal/base.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/proposal/flow.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/proposal/flow.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/proposal/prior.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/proposal/prior.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/proposal/spherical.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/proposal/spherical.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/sampler.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/sampler.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/tensorlist.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/tensorlist.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/transforms.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/transforms.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/utils/gammaincinv.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/utils/gammaincinv.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/utils/io.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/utils/io.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/utils/maths.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/utils/maths.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/utils/sample.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/utils/sample.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch/utils/stats.py` & `nessai_torch-0.1.0rc1/src/nessai_torch/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/PKG-INFO` & `nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai-torch
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: nessai in pure PyTorch
 Author-email: "Michael J. Williams" <michaeljw1@googlemail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,28 +28,30 @@
 
 `nessai-torch` can be install using `pip`:
 
 ```
 pip install nessai-torch
 ```
 
-We recommend install PyTorch first to ensure the version is compatible with
+We recommend installing PyTorch first to ensure the version is compatible with
 your system.
 
 ## Basic usage
 
 `nessai-torch` has a different API to `nessai`, the user must define a
 log-likelihood function and a prior-transform function instead of a model
 object. It also has a reduced feature set compared to standard `nessai`.
 The basic usage is shown below, for a more complete example, see the
 `examples` directory.
 
 ```python
 from nessai_torch.sampler import Sampler
 
+# Define the log-likelihood and prior transform
+...
 
 sampler = Sampler(
 	log_likelihood=log_likelihood_fn,
 	prior_transform=prior_transform_fn,
 	dims=dims,  # Number of dimensions
 )
```

### Comparing `nessai_torch-0.1.0rc0/src/nessai_torch.egg-info/SOURCES.txt` & `nessai_torch-0.1.0rc1/src/nessai_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/tests/integration_tests/test_sampling.py` & `nessai_torch-0.1.0rc1/tests/integration_tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/tests/test_plot.py` & `nessai_torch-0.1.0rc1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/tests/test_utils/test_gammaincinv.py` & `nessai_torch-0.1.0rc1/tests/test_utils/test_gammaincinv.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/tests/test_utils/test_io.py` & `nessai_torch-0.1.0rc1/tests/test_utils/test_io.py`

 * *Files identical despite different names*

### Comparing `nessai_torch-0.1.0rc0/tests/test_utils/test_sample.py` & `nessai_torch-0.1.0rc1/tests/test_utils/test_sample.py`

 * *Files identical despite different names*

