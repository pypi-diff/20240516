# Comparing `tmp/pympipool-0.8.1.tar.gz` & `tmp/pympipool-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.8.1.tar", last modified: Mon Apr 22 17:38:46 2024, max compression
+gzip compressed data, was "pympipool-0.8.2.tar", last modified: Mon May  6 20:49:56 2024, max compression
```

## Comparing `pympipool-0.8.1.tar` & `pympipool-0.8.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.491462 pympipool-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-22 17:38:06.000000 pympipool-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 17:38:06.000000 pympipool-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-04-22 17:38:46.491462 pympipool-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-22 17:38:06.000000 pympipool-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.483462 pympipool-0.8.1/pympipool/
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-22 17:38:46.491462 pympipool-0.8.1/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.487462 pympipool-0.8.1/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/backend/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/backend/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.487462 pympipool-0.8.1/pympipool/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/scheduler/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/scheduler/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.487462 pympipool-0.8.1/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    23991 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/executorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/inputcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.487462 pympipool-0.8.1/pympipool/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shell/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-22 17:38:06.000000 pympipool-0.8.1/pympipool/shell/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.491462 pympipool-0.8.1/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-04-22 17:38:46.000000 pympipool-0.8.1/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-22 17:38:46.000000 pympipool-0.8.1/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:38:46.000000 pympipool-0.8.1/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 17:38:46.000000 pympipool-0.8.1/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 17:38:46.000000 pympipool-0.8.1/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-22 17:38:45.000000 pympipool-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 17:38:46.491462 pympipool-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 17:38:06.000000 pympipool-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:38:46.491462 pympipool-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_backend_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_dependencies_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_executor_backend_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_executor_backend_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_executor_backend_mpi_noblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_flux_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_integration_pyiron_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_mpi_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_mpi_executor_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_shared_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_shared_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_shared_executorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_shared_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-22 17:38:06.000000 pympipool-0.8.1/tests/test_shell_interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.424580 pympipool-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-06 20:49:15.000000 pympipool-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 20:49:15.000000 pympipool-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-06 20:49:56.424580 pympipool-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-06 20:49:15.000000 pympipool-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.416581 pympipool-0.8.2/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-06 20:49:56.424580 pympipool-0.8.2/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.416581 pympipool-0.8.2/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/backend/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/backend/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.420580 pympipool-0.8.2/pympipool/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/scheduler/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/scheduler/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.420580 pympipool-0.8.2/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23991 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/inputcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.420580 pympipool-0.8.2/pympipool/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shell/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-06 20:49:15.000000 pympipool-0.8.2/pympipool/shell/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.424580 pympipool-0.8.2/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-06 20:49:56.000000 pympipool-0.8.2/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-06 20:49:56.000000 pympipool-0.8.2/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:49:56.000000 pympipool-0.8.2/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 20:49:56.000000 pympipool-0.8.2/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 20:49:56.000000 pympipool-0.8.2/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-06 20:49:55.000000 pympipool-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:49:56.424580 pympipool-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-06 20:49:15.000000 pympipool-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:49:56.424580 pympipool-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_backend_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_dependencies_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_executor_backend_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_executor_backend_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_executor_backend_mpi_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_flux_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_integration_pyiron_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_mpi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_mpi_executor_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shared_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shared_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shared_executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shared_input_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shared_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-06 20:49:15.000000 pympipool-0.8.2/tests/test_shell_interactive.py
```

### Comparing `pympipool-0.8.1/LICENSE` & `pympipool-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/PKG-INFO` & `pympipool-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.8.1
+Version: 0.8.2
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
         
@@ -47,18 +47,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
 Requires-Dist: mpi4py<=3.1.6,>=3.1.4
-Requires-Dist: pyzmq<=26.0.2,>=25.0.0
-Requires-Dist: tqdm<=4.66.2,>=4.44.0
+Requires-Dist: pyzmq<=26.0.3,>=25.0.0
+Requires-Dist: tqdm<=4.66.4,>=4.44.0
 
-# pympipool - up-scale python functions for high performance computing
+# pympipool
 [![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pympipool/HEAD?labpath=notebooks%2Fexamples.ipynb)
 
 ## Challenges
 In high performance computing (HPC) the Python programming language is commonly used as high-level language to
 orchestrate the coupling of scientific applications. Still the efficient usage of highly parallel HPC clusters remains
@@ -177,8 +177,7 @@
   * [Coupled Functions](https://pympipool.readthedocs.io/en/latest/examples.html#coupled-functions)
   * [SLURM Job Scheduler](https://pympipool.readthedocs.io/en/latest/examples.html#slurm-job-scheduler) 
   * [Workstation Support](https://pympipool.readthedocs.io/en/latest/examples.html#workstation-support)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html)
   * [Contributions](https://pympipool.readthedocs.io/en/latest/development.html#contributions)
   * [License](https://pympipool.readthedocs.io/en/latest/development.html#license)
   * [Integration](https://pympipool.readthedocs.io/en/latest/development.html#integration)
-* [Module Index](https://pympipool.readthedocs.io/en/latest/py-modindex.html)
```

### Comparing `pympipool-0.8.1/README.md` & `pympipool-0.8.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pympipool - up-scale python functions for high performance computing
+# pympipool
 [![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pympipool/HEAD?labpath=notebooks%2Fexamples.ipynb)
 
 ## Challenges
 In high performance computing (HPC) the Python programming language is commonly used as high-level language to
 orchestrate the coupling of scientific applications. Still the efficient usage of highly parallel HPC clusters remains
@@ -121,8 +121,7 @@
   * [Coupled Functions](https://pympipool.readthedocs.io/en/latest/examples.html#coupled-functions)
   * [SLURM Job Scheduler](https://pympipool.readthedocs.io/en/latest/examples.html#slurm-job-scheduler) 
   * [Workstation Support](https://pympipool.readthedocs.io/en/latest/examples.html#workstation-support)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html)
   * [Contributions](https://pympipool.readthedocs.io/en/latest/development.html#contributions)
   * [License](https://pympipool.readthedocs.io/en/latest/development.html#license)
   * [Integration](https://pympipool.readthedocs.io/en/latest/development.html#integration)
-* [Module Index](https://pympipool.readthedocs.io/en/latest/py-modindex.html)
```

### Comparing `pympipool-0.8.1/pympipool/__init__.py` & `pympipool-0.8.2/pympipool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 from ._version import get_versions
 from pympipool.scheduler import create_executor
 from pympipool.shell.executor import SubprocessExecutor
 from pympipool.shell.interactive import ShellExecutor
 from pympipool.shared.dependencies import ExecutorWithDependencies
+from pympipool.shared.inputcheck import check_refresh_rate as _check_refresh_rate
 
 
 __version__ = get_versions()["version"]
 
 
 class Executor:
     """
@@ -145,18 +146,15 @@
                 backend=backend,
                 block_allocation=block_allocation,
                 init_function=init_function,
                 command_line_argument_lst=command_line_argument_lst,
                 refresh_rate=refresh_rate,
             )
         else:
-            if refresh_rate != 0.01:
-                raise ValueError(
-                    "The sleep_interval parameter is only used when disable_dependencies=False."
-                )
+            _check_refresh_rate(refresh_rate=refresh_rate)
             return create_executor(
                 max_cores=max_cores,
                 cores_per_worker=cores_per_worker,
                 threads_per_core=threads_per_core,
                 gpus_per_worker=gpus_per_worker,
                 oversubscribe=oversubscribe,
                 cwd=cwd,
```

### Comparing `pympipool-0.8.1/pympipool/backend/mpiexec.py` & `pympipool-0.8.2/pympipool/backend/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/backend/serial.py` & `pympipool-0.8.2/pympipool/backend/serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/scheduler/__init__.py` & `pympipool-0.8.2/pympipool/scheduler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from pympipool.shared.interface import SLURM_COMMAND
 from pympipool.shared.inputcheck import (
     check_command_line_argument_lst,
     check_gpus_per_worker,
     check_threads_per_core,
     check_oversubscribe,
     check_executor,
+    check_backend,
+    check_init_function,
 )
 from pympipool.scheduler.slurm import (
     PySlurmExecutor,
     PySlurmStepExecutor,
 )
 
 try:  # The PyFluxExecutor requires flux-core to be installed.
@@ -75,24 +77,17 @@
                                     resource requirements, pympipool supports block allocation. In this case all
                                     resources have to be defined on the executor, rather than during the submission
                                     of the individual function.
         init_function (None): optional function to preset arguments for functions which are submitted later
         command_line_argument_lst (list): Additional command line arguments for the srun call (SLURM only)
 
     """
-    if not block_allocation and init_function is not None:
-        raise ValueError("")
-    if backend not in ["auto", "mpi", "slurm", "flux"]:
-        raise ValueError(
-            'The currently implemented backends are ["flux", "mpi", "slurm"]. '
-            'Alternatively, you can select "auto", the default option, to automatically determine the backend. But '
-            + backend
-            + " is not a valid choice."
-        )
-    elif backend == "flux" or (backend == "auto" and flux_installed):
+    check_init_function(block_allocation=block_allocation, init_function=init_function)
+    check_backend(backend=backend)
+    if backend == "flux" or (backend == "auto" and flux_installed):
         check_oversubscribe(oversubscribe=oversubscribe)
         check_command_line_argument_lst(
             command_line_argument_lst=command_line_argument_lst
         )
         if block_allocation:
             return PyFluxExecutor(
                 max_workers=int(max_cores / cores_per_worker),
```

### Comparing `pympipool-0.8.1/pympipool/scheduler/flux.py` & `pympipool-0.8.2/pympipool/scheduler/flux.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/scheduler/mpi.py` & `pympipool-0.8.2/pympipool/scheduler/mpi.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/scheduler/slurm.py` & `pympipool-0.8.2/pympipool/scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shared/backend.py` & `pympipool-0.8.2/pympipool/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shared/communication.py` & `pympipool-0.8.2/pympipool/shared/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shared/dependencies.py` & `pympipool-0.8.2/pympipool/shared/dependencies.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shared/executorbase.py` & `pympipool-0.8.2/pympipool/shared/executorbase.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shared/interface.py` & `pympipool-0.8.2/pympipool/shared/interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shared/thread.py` & `pympipool-0.8.2/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shell/executor.py` & `pympipool-0.8.2/pympipool/shell/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool/shell/interactive.py` & `pympipool-0.8.2/pympipool/shell/interactive.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/pympipool.egg-info/PKG-INFO` & `pympipool-0.8.2/pympipool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.8.1
+Version: 0.8.2
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
         
@@ -47,18 +47,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudpickle<=3.0.0,>=2.0.0
 Requires-Dist: mpi4py<=3.1.6,>=3.1.4
-Requires-Dist: pyzmq<=26.0.2,>=25.0.0
-Requires-Dist: tqdm<=4.66.2,>=4.44.0
+Requires-Dist: pyzmq<=26.0.3,>=25.0.0
+Requires-Dist: tqdm<=4.66.4,>=4.44.0
 
-# pympipool - up-scale python functions for high performance computing
+# pympipool
 [![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/pympipool/HEAD?labpath=notebooks%2Fexamples.ipynb)
 
 ## Challenges
 In high performance computing (HPC) the Python programming language is commonly used as high-level language to
 orchestrate the coupling of scientific applications. Still the efficient usage of highly parallel HPC clusters remains
@@ -177,8 +177,7 @@
   * [Coupled Functions](https://pympipool.readthedocs.io/en/latest/examples.html#coupled-functions)
   * [SLURM Job Scheduler](https://pympipool.readthedocs.io/en/latest/examples.html#slurm-job-scheduler) 
   * [Workstation Support](https://pympipool.readthedocs.io/en/latest/examples.html#workstation-support)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html)
   * [Contributions](https://pympipool.readthedocs.io/en/latest/development.html#contributions)
   * [License](https://pympipool.readthedocs.io/en/latest/development.html#license)
   * [Integration](https://pympipool.readthedocs.io/en/latest/development.html#integration)
-* [Module Index](https://pympipool.readthedocs.io/en/latest/py-modindex.html)
```

### Comparing `pympipool-0.8.1/pympipool.egg-info/SOURCES.txt` & `pympipool-0.8.2/pympipool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,10 +36,11 @@
 tests/test_flux_executor.py
 tests/test_integration_pyiron_workflow.py
 tests/test_mpi_executor.py
 tests/test_mpi_executor_future.py
 tests/test_shared_backend.py
 tests/test_shared_communication.py
 tests/test_shared_executorbase.py
+tests/test_shared_input_check.py
 tests/test_shared_thread.py
 tests/test_shell_executor.py
 tests/test_shell_interactive.py
```

### Comparing `pympipool-0.8.1/pyproject.toml` & `pympipool-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "cloudpickle>=2.0.0,<=3.0.0",
     "mpi4py>=3.1.4,<=3.1.6",
-    "pyzmq>=25.0.0,<=26.0.2",
-    "tqdm>=4.44.0,<=4.66.2",
+    "pyzmq>=25.0.0,<=26.0.3",
+    "tqdm>=4.44.0,<=4.66.4",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pyiron/pympipool"
 Documentation = "https://pympipool.readthedocs.io"
 Repository = "https://github.com/pyiron/pympipool"
```

### Comparing `pympipool-0.8.1/tests/test_backend_serial.py` & `pympipool-0.8.2/tests/test_backend_serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_dependencies_executor.py` & `pympipool-0.8.2/tests/test_dependencies_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_executor_backend_flux.py` & `pympipool-0.8.2/tests/test_executor_backend_flux.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_executor_backend_mpi.py` & `pympipool-0.8.2/tests/test_executor_backend_mpi.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_executor_backend_mpi_noblock.py` & `pympipool-0.8.2/tests/test_executor_backend_mpi_noblock.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_flux_executor.py` & `pympipool-0.8.2/tests/test_flux_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_integration_pyiron_workflow.py` & `pympipool-0.8.2/tests/test_integration_pyiron_workflow.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_mpi_executor.py` & `pympipool-0.8.2/tests/test_mpi_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_mpi_executor_future.py` & `pympipool-0.8.2/tests/test_mpi_executor_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_shared_backend.py` & `pympipool-0.8.2/tests/test_shared_backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_shared_communication.py` & `pympipool-0.8.2/tests/test_shared_communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_shared_executorbase.py` & `pympipool-0.8.2/tests/test_shared_executorbase.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_shell_executor.py` & `pympipool-0.8.2/tests/test_shell_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.1/tests/test_shell_interactive.py` & `pympipool-0.8.2/tests/test_shell_interactive.py`

 * *Files identical despite different names*

