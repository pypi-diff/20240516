# Comparing `tmp/graph-scheduler-1.1.2.tar.gz` & `tmp/graph-scheduler-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-scheduler-1.1.2.tar", last modified: Wed Apr 19 00:41:46 2023, max compression
+gzip compressed data, was "graph-scheduler-1.2.0.tar", last modified: Fri Dec 15 01:06:19 2023, max compression
```

## Comparing `graph-scheduler-1.1.2.tar` & `graph-scheduler-1.2.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/
--rw-------   0 katherine  (1000) katherine  (1000)    11358 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/LICENSE.txt
--rw-------   0 katherine  (1000) katherine  (1000)      290 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/MANIFEST.in
--rw-------   0 katherine  (1000) katherine  (1000)     2660 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/PKG-INFO
--rw-------   0 katherine  (1000) katherine  (1000)     1828 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/README.md
--rw-------   0 katherine  (1000) katherine  (1000)     2623 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/conftest.py
--rw-------   0 katherine  (1000) katherine  (1000)      140 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/dev_requirements.txt
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/docs/
--rw-------   0 katherine  (1000) katherine  (1000)      133 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Condition.rst
--rw-------   0 katherine  (1000) katherine  (1000)      634 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Makefile
--rw-------   0 katherine  (1000) katherine  (1000)      133 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Scheduler.rst
--rw-------   0 katherine  (1000) katherine  (1000)      118 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Time.rst
--rw-------   0 katherine  (1000) katherine  (1000)     2672 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/conf.py
--rw-------   0 katherine  (1000) katherine  (1000)      442 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/index.rst
--rw-------   0 katherine  (1000) katherine  (1000)      760 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/make.bat
--rw-------   0 katherine  (1000) katherine  (1000)       54 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs_requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)      127 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/pyproject.toml
--rw-------   0 katherine  (1000) katherine  (1000)       29 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)     2550 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/setup.cfg
--rw-------   0 katherine  (1000) katherine  (1000)      591 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/setup.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/src/
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/src/graph_scheduler/
--rw-------   0 katherine  (1000) katherine  (1000)     1244 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)      497 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/src/graph_scheduler/_version.py
--rw-------   0 katherine  (1000) katherine  (1000)    76898 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/condition.py
--rw-------   0 katherine  (1000) katherine  (1000)    42008 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)    26192 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/time.py
--rw-------   0 katherine  (1000) katherine  (1000)     2704 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/utilities.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/
--rw-------   0 katherine  (1000) katherine  (1000)     2660 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/PKG-INFO
--rw-------   0 katherine  (1000) katherine  (1000)      835 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/SOURCES.txt
--rw-------   0 katherine  (1000) katherine  (1000)        1 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/dependency_links.txt
--rw-------   0 katherine  (1000) katherine  (1000)      236 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/requires.txt
--rw-------   0 katherine  (1000) katherine  (1000)       16 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/top_level.txt
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/tests/
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/tests/documentation/
--rw-------   0 katherine  (1000) katherine  (1000)      506 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/documentation/test_module_docs.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/tests/scheduling/
--rw-------   0 katherine  (1000) katherine  (1000)     1635 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/conftest.py
--rw-------   0 katherine  (1000) katherine  (1000)    57241 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/test_condition.py
--rw-------   0 katherine  (1000) katherine  (1000)    95802 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/test_scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)     8785 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/test_time.py
--rw-------   0 katherine  (1000) katherine  (1000)    78254 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/versioneer.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.337518 graph-scheduler-1.2.0/
+-rw-------   0 katherine  (1000) katherine  (1000)    11358 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/LICENSE.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      290 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/MANIFEST.in
+-rw-------   0 katherine  (1000) katherine  (1000)     2762 2023-12-15 01:06:19.337518 graph-scheduler-1.2.0/PKG-INFO
+-rw-------   0 katherine  (1000) katherine  (1000)     1828 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/README.md
+-rw-------   0 katherine  (1000) katherine  (1000)      535 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/conftest.py
+-rw-------   0 katherine  (1000) katherine  (1000)       99 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/dev_requirements.txt
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/docs/
+-rw-------   0 katherine  (1000) katherine  (1000)      135 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/docs/Condition.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      634 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/docs/Makefile
+-rw-------   0 katherine  (1000) katherine  (1000)      112 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/docs/Scheduler.rst
+-rw-------   0 katherine  (1000) katherine  (1000)       97 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/docs/Time.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     2672 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/docs/conf.py
+-rw-------   0 katherine  (1000) katherine  (1000)      442 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/docs/index.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      760 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/docs/make.bat
+-rw-------   0 katherine  (1000) katherine  (1000)       57 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/docs_requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)       21 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/psyneulink_requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      127 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/pyproject.toml
+-rw-------   0 katherine  (1000) katherine  (1000)       51 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)     2410 2023-12-15 01:06:19.337518 graph-scheduler-1.2.0/setup.cfg
+-rw-------   0 katherine  (1000) katherine  (1000)      591 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/setup.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/src/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.337518 graph-scheduler-1.2.0/src/graph_scheduler/
+-rw-------   0 katherine  (1000) katherine  (1000)     1727 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/src/graph_scheduler/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)      497 2023-12-15 01:06:19.337518 graph-scheduler-1.2.0/src/graph_scheduler/_version.py
+-rw-------   0 katherine  (1000) katherine  (1000)   125966 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/src/graph_scheduler/condition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    50798 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/src/graph_scheduler/scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)    26195 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/src/graph_scheduler/time.py
+-rw-------   0 katherine  (1000) katherine  (1000)     9902 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/src/graph_scheduler/utilities.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/src/graph_scheduler.egg-info/
+-rw-------   0 katherine  (1000) katherine  (1000)     2762 2023-12-15 01:06:19.000000 graph-scheduler-1.2.0/src/graph_scheduler.egg-info/PKG-INFO
+-rw-------   0 katherine  (1000) katherine  (1000)     1097 2023-12-15 01:06:19.000000 graph-scheduler-1.2.0/src/graph_scheduler.egg-info/SOURCES.txt
+-rw-------   0 katherine  (1000) katherine  (1000)        1 2023-12-15 01:06:19.000000 graph-scheduler-1.2.0/src/graph_scheduler.egg-info/dependency_links.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      220 2023-12-15 01:06:19.000000 graph-scheduler-1.2.0/src/graph_scheduler.egg-info/requires.txt
+-rw-------   0 katherine  (1000) katherine  (1000)       16 2023-12-15 01:06:19.000000 graph-scheduler-1.2.0/src/graph_scheduler.egg-info/top_level.txt
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/tests/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/tests/documentation/
+-rw-------   0 katherine  (1000) katherine  (1000)      473 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/documentation/test_module_docs.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/tests/integration/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.333518 graph-scheduler-1.2.0/tests/integration/psyneulink/
+-rw-------   0 katherine  (1000) katherine  (1000)     1514 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/integration/psyneulink/conftest.py
+-rw-------   0 katherine  (1000) katherine  (1000)     1241 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/integration/psyneulink/test_condition_psyneulink.py
+-rw-------   0 katherine  (1000) katherine  (1000)    34848 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/integration/psyneulink/test_scheduler_psyneulink.py
+-rw-------   0 katherine  (1000) katherine  (1000)      529 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/integration/psyneulink/test_time_psyneulink.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-12-15 01:06:19.337518 graph-scheduler-1.2.0/tests/scheduling/
+-rw-------   0 katherine  (1000) katherine  (1000)     1962 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/scheduling/conftest.py
+-rw-------   0 katherine  (1000) katherine  (1000)    87459 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/scheduling/test_condition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    42015 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/scheduling/test_scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8903 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/scheduling/test_time.py
+-rw-------   0 katherine  (1000) katherine  (1000)     4489 2023-12-15 00:44:35.000000 graph-scheduler-1.2.0/tests/test_utilities.py
+-rw-------   0 katherine  (1000) katherine  (1000)    78254 2023-04-18 23:03:00.000000 graph-scheduler-1.2.0/versioneer.py
```

### Comparing `graph-scheduler-1.1.2/LICENSE.txt` & `graph-scheduler-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.2/PKG-INFO` & `graph-scheduler-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: graph-scheduler
-Version: 1.1.2
+Version: 1.2.0
 Summary: A graph-based scheduler of nodes based on structure and conditions
 Home-page: https://github.com/kmantel/graph-scheduler
 Author: Katherine Mantel, Princeton University
 Author-email: kmantel@princeton.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kmantel/graph-scheduler/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # Graph Scheduler
```

### Comparing `graph-scheduler-1.1.2/README.md` & `graph-scheduler-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.2/conftest.py` & `graph-scheduler-1.2.0/tests/integration/psyneulink/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,47 @@
-import doctest
 import pytest
-
-from psyneulink import clear_registry, primary_registries
 from psyneulink.core import llvm as pnlvm
 
 
 def pytest_runtest_setup(item):
     if 'cuda' in item.keywords and not pnlvm.ptx_enabled:
-            pytest.skip('PTX engine not enabled/available')
+        pytest.skip('PTX engine not enabled/available')
 
-    doctest.ELLIPSIS_MARKER = "[...]"
 
 def pytest_generate_tests(metafunc):
-    mech_and_func_modes = ['Python',
-                           pytest.param('LLVM', marks=pytest.mark.llvm),
-                           pytest.param('PTX', marks=[pytest.mark.llvm,
-                                                      pytest.mark.cuda])
-                          ]
-
-    if "func_mode" in metafunc.fixturenames:
-        metafunc.parametrize("func_mode", mech_and_func_modes)
-
-    if "mech_mode" in metafunc.fixturenames:
-        metafunc.parametrize("mech_mode", mech_and_func_modes)
-
     if "comp_mode_no_llvm" in metafunc.fixturenames:
         modes = [m for m in get_comp_execution_modes()
                  if m.values[0] is not pnlvm.ExecutionMode.LLVM]
         metafunc.parametrize("comp_mode", modes)
 
     elif "comp_mode" in metafunc.fixturenames:
         metafunc.parametrize("comp_mode", get_comp_execution_modes())
 
-    if "autodiff_mode" in metafunc.fixturenames:
-        auto_modes = [pnlvm.ExecutionMode.Python,
-                      pytest.param(pnlvm.ExecutionMode.LLVMRun, marks=pytest.mark.llvm)]
-        metafunc.parametrize("autodiff_mode", auto_modes)
-
 
 def pytest_runtest_teardown(item):
-    for registry in primary_registries:
-        # Clear Registry to have a stable reference for indexed suffixes of default names
-        clear_registry(registry)
-
     pnlvm.cleanup()
 
+
 @pytest.fixture
 def comp_mode_no_llvm():
     # dummy fixture to allow 'comp_mode' filtering
     pass
 
+
 @pytest.helpers.register
 def get_comp_execution_modes():
-    return [pytest.param(pnlvm.ExecutionMode.Python),
-            pytest.param(pnlvm.ExecutionMode.LLVM, marks=pytest.mark.llvm),
-            pytest.param(pnlvm.ExecutionMode.LLVMExec, marks=pytest.mark.llvm),
-            pytest.param(pnlvm.ExecutionMode.LLVMRun, marks=pytest.mark.llvm),
-            pytest.param(pnlvm.ExecutionMode.PTXExec, marks=[pytest.mark.llvm, pytest.mark.cuda]),
-            pytest.param(pnlvm.ExecutionMode.PTXRun, marks=[pytest.mark.llvm,  pytest.mark.cuda])
-           ]
+    return [
+        pytest.param(pnlvm.ExecutionMode.Python),
+        pytest.param(pnlvm.ExecutionMode.LLVM, marks=pytest.mark.llvm),
+        pytest.param(pnlvm.ExecutionMode.LLVMExec, marks=pytest.mark.llvm),
+        pytest.param(pnlvm.ExecutionMode.LLVMRun, marks=pytest.mark.llvm),
+        pytest.param(pnlvm.ExecutionMode.PTXExec, marks=[pytest.mark.llvm, pytest.mark.cuda]),
+        pytest.param(pnlvm.ExecutionMode.PTXRun, marks=[pytest.mark.llvm, pytest.mark.cuda])
+    ]
 
 
-# TODO: remove this helper when tests no longer use psyneulink
 @pytest.helpers.register
 def composition_to_scheduler_args(composition):
     return {
         'graph': composition.graph_processing.prune_feedback_edges()[0],
         'default_execution_id': composition.default_execution_id
     }
```

### Comparing `graph-scheduler-1.1.2/docs/Makefile` & `graph-scheduler-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.2/docs/conf.py` & `graph-scheduler-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.2/docs/make.bat` & `graph-scheduler-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.2/setup.cfg` & `graph-scheduler-1.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 
@@ -30,32 +32,25 @@
 python-tag = py3
 
 [tool:pytest]
 addopts = 
 	-s
 	-vv
 	-n auto
-	--benchmark-disable
-	--benchmark-disable-gc
-	--benchmark-warmup=on
-	--benchmark-warmup-iterations=2
 	--cov
 	--cov-config setup.cfg
 	--pydocstyle
 	--pycodestyle
 	--strict-markers
 	--strict-config
 markers = 
-	composition: PsyNeuLink Composition tests
 	llvm: Tests using LLVM runtime compiler
 	cuda: Tests using LLVM runtime compiler and CUDA GPGPU backend
-	mechanism: Tests of Mechanism classes
-	transfer_mechanism
 	psyneulink: Tests requiring PsyNeuLink
-required_plugins = pytest-benchmark pytest-cov pytest-helpers-namespace pytest-pycodestyle pytest-pydocstyle pytest-xdist
+required_plugins = pytest-cov pytest-helpers-namespace pytest-pycodestyle pytest-pydocstyle pytest-xdist
 xfail_strict = True
 filterwarnings = 
 	error:Creating an ndarray from ragged nested sequences \(which is a list-or-tuple of lists-or-tuples-or ndarrays with different lengths or shapes\) is deprecated.*:numpy.VisibleDeprecationWarning
 	ignore:Multiple ParameterPorts:UserWarning
 
 [pycodestyle]
 ignore = E117,E124,E126,E127,E128,E231,E241,E261,E265,E302,E303,E501,W503
```

### Comparing `graph-scheduler-1.1.2/setup.py` & `graph-scheduler-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.2/src/graph_scheduler/__init__.py` & `graph-scheduler-1.2.0/src/graph_scheduler/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,32 +7,51 @@
 the user. Patterns of execution are linked to abstract units of time and
 may optionally be mapped to real time units using pint.
 
 Source: https://github.com/kmantel/graph-scheduler
 Documentation: https://kmantel.github.io/graph-scheduler/
 """
 
+import inspect
 import pint
 
 _unit_registry = pint.get_application_registry()
 pint.set_application_registry(_unit_registry)
 _unit_registry.precision = 8  # TODO: remove when floating point issues resolved
 
 from . import condition  # noqa: E402
 from . import scheduler  # noqa: E402
 from . import time  # noqa: E402
+from . import utilities  # noqa: E402
 
-from .condition import *  # noqa: E402
-from .scheduler import *  # noqa: E402
-from .time import *  # noqa: E402
+
+condition.__all__ = []
+for k, v in condition.__dict__.items():
+    if (
+        (
+            k[0] != '_'
+            and inspect.isclass(v)
+            and issubclass(v, condition.ConditionBase)
+        )
+        or k in condition._additional__all__
+    ):
+        condition.__all__.append(k)
+
+
+from .condition import *  # noqa: E402, F401, F403
+from .scheduler import *  # noqa: E402, F401, F403
+from .time import *  # noqa: E402, F401, F403
+from .utilities import *  # noqa: E402, F401, F403
 
 __all__ = list(condition.__all__)
 __all__.extend(scheduler.__all__)
 __all__.extend(time.__all__)
+__all__.extend(utilities.__all__)
 __all__.extend([
     '_unit_registry'
 ])
 
 from . import _version  # noqa: E402
 __version__ = _version.get_versions()['version']
 
+del inspect
 del pint
```

### Comparing `graph-scheduler-1.1.2/src/graph_scheduler/scheduler.py` & `graph-scheduler-1.2.0/src/graph_scheduler/scheduler.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,24 +29,33 @@
   (see `below <Scheduler_Algorithm>`).
 
 Conditions can be added to a Scheduler when it is created by specifying a `ConditionSet` (a set of
 `Conditions <Condition>`) in the **conditions** argument of its constructor.  Individual Conditions and/or
 ConditionSets can also be added after the Scheduler has been created, using its `add_condition` and
 `add_condition_set` methods, respectively.
 
+`Graph structure Conditions <Condition_Graph_Structure_Intro>` are
+applied to the Scheduler's graph in the order in which they are `added
+<Scheduler.add_condition>`.
+
+
 .. _Scheduler_Algorithm:
 
 Algorithm
 ---------
 
 .. _Consideration_Set:
 
 When a Scheduler is created, it constructs a `consideration_queue`:  a list of ``consideration sets``
-that defines the order in which nodes are eligible to be executed.  This is based on the dependencies specified in the graph
-specification provided in the Scheduler's constructor.  Each ``consideration_set``
+that defines the order in which nodes are eligible to be executed. This
+is determined by the topological ordering of the `graph
+<Scheduler.graph>` provided to the `Scheduler's constructor
+<Scheduler>`, which is then modified by any `graph structure conditions
+<Condition_Graph_Structure_Intro>` that are `added
+<Scheduler.add_condition>` to the Scheduler. Each ``consideration_set``
 is a set of nodes that are eligible to execute at the same time/`CONSIDERATION_SET_EXECUTION` (i.e.,
 that appear at the same "depth" in a sequence of dependencies, and among which there are no dependencies).  The first
 ``consideration_set`` consists of only origin nodes. The second consists of all nodes
 that receive edges from the nodes in the first ``consideration_set``.
 The third consists of nodes that receive edges from nodes in the first two ``consideration sets``,
 and so forth.  When the Scheduler is run, it uses the `consideration_queue` to determine which
 nodes are eligible to execute in each `CONSIDERATION_SET_EXECUTION` of a `PASS`, and then evaluates the `Condition <Condition>`
@@ -149,19 +158,21 @@
 for a particular node or set of nodes is met).
 
 .. _Scheduler_Termination_Conditions:
 
 *Termination Conditions*
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
-Termination conditions are `Conditions <Condition>` that specify when the open-ended units of time - `ENVIRONMENT_STATE_UPDATE
+Termination conditions are basic `Conditions <Condition>` that specify
+when the open-ended units of time - `ENVIRONMENT_STATE_UPDATE
 <TimeScale.ENVIRONMENT_STATE_UPDATE>` and `ENVIRONMENT_SEQUENCE` - have ended.  By default, the termination condition for an `ENVIRONMENT_STATE_UPDATE <TimeScale.ENVIRONMENT_STATE_UPDATE>` is
 `AllHaveRun`, which is satisfied when all nodes have run at least once within the environment state update, and the termination
 condition for an `ENVIRONMENT_SEQUENCE` is when all of its constituent environment state updates have terminated.
-
+`Graph structure conditions <Condition_Graph_Structure_Intro>` cannot
+be used as termination conditions.
 
 .. _Scheduler_Absolute_Time:
 
 Absolute Time
 -------------
 
 The scheduler supports scheduling of models of real-time systems in
@@ -298,26 +309,33 @@
 """
 
 import copy
 import datetime
 import enum
 import fractions
 import logging
-import typing
+import warnings
+from typing import Dict, Hashable, Iterable, List, Set, Union
 
+import networkx as nx
 import numpy as np
 import pint
-from toposort import toposort
+from toposort import CircularDependencyError, toposort
 
 from graph_scheduler import _unit_registry
 from graph_scheduler.condition import (
-    All, AllHaveRun, Always, Condition, ConditionSet, EveryNCalls, Never,
-    _parse_absolute_unit, _quantity_as_integer,
+    AddEdgeTo, All, AllHaveRun, Always, Condition, ConditionSet, EveryNCalls,
+    Never, RemoveEdgeFrom, _parse_absolute_unit,
+    _quantity_as_integer, typing_condition_base,
 )
 from graph_scheduler.time import _get_pint_unit, Clock, TimeScale
+from graph_scheduler.utilities import (
+    cached_graph_function, clone_graph, networkx_digraph_to_dependency_dict,
+    typing_graph_dependency_dict,
+)
 
 __all__ = [
     'Scheduler', 'SchedulerError', 'SchedulingMode',
 ]
 
 logger = logging.getLogger(__name__)
 
@@ -336,14 +354,37 @@
             EXACT_TIME
                 `Exact time Mode <Scheduler_Exact_Time>`
     """
     STANDARD = enum.auto()
     EXACT_TIME = enum.auto()
 
 
+@cached_graph_function
+def _build_consideration_queue(
+    graph: typing_graph_dependency_dict
+) -> List[Set[Hashable]]:
+    return list(toposort(graph))
+
+
+def _generate_consideration_queue_indices(
+    consideration_queue: Iterable[Set[Hashable]]
+) -> Dict[Hashable, int]:
+    """
+    Returns:
+        A dictionary mapping nodes to their indices in
+        **consideration_queue**
+    """
+    consideration_queue_indices = {}
+    for i, cs in enumerate(consideration_queue):
+        consideration_queue_indices.update({
+            n: i for n in cs
+        })
+    return consideration_queue_indices
+
+
 class SchedulerError(Exception):
 
     def __init__(self, error_value):
         self.error_value = error_value
 
     def __str__(self):
         return repr(self.error_value)
@@ -353,16 +394,20 @@
     """Generates an order of execution for nodes in a graph or graph
     specification dictionary, possibly determined by a set of `Conditions <Condition>`.
 
     Arguments
     ---------
 
     graph : Dict[object: set(object)], `networkx.DiGraph`
-        a graph specification dictionary - each entry of the dictionary must be an object,
-        and the value of each entry must be a set of zero or more objects that project directly to the key.
+        a directed acyclic graph (DAG). Specified as either:
+            - a graph specification dictionary: each entry of the
+            dictionary must be an object, and the value of each entry
+            must be a set of zero or more objects that project directly
+            to the key.
+            - a `networkx.DiGraph`
 
     conditions  : ConditionSet
         set of `Conditions <Condition>` that specify when individual nodes in **graph**
         execute and any dependencies among them.
 
     mode : SchedulingMode[STANDARD|EXACT_TIME] : SchedulingMode.STANDARD
         sets the mode of scheduling: `standard <Scheduler_Execution>` or
@@ -388,16 +433,18 @@
 
     consideration_queue : list
         a list form of the Scheduler's toposort ordering of its nodes
 
     consideration_queue_indices : dict
         a dict mapping **nodes** to their position in the `consideration_queue`
 
-    termination_conds : Dict[TimeScale: Condition]
-        a mapping from `TimeScales <TimeScale>` to `Conditions <Condition>` that, when met, terminate the execution
+    termination_conds : Dict[TimeScale: `Condition <graph_scheduler.condition.Condition>`]
+        a mapping from `TimeScales <TimeScale>` to `Conditions
+        <graph_scheduler.condition.Condition>` that, when met, terminate
+        the execution
         of the specified `TimeScale`. On set, update only for the
         `TimeScale`\\ s specified in the argument.
 
     mode
         sets the mode of scheduling: `standard <Scheduler_Execution>` or
         `exact time <Scheduler_Exact_Time>`
 
@@ -415,76 +462,70 @@
     def __init__(
         self,
         graph,
         conditions=None,
         termination_conds=None,
         default_execution_id=None,
         mode: SchedulingMode = SchedulingMode.STANDARD,
-        default_absolute_time_unit: typing.Union[str, pint.Quantity] = _get_pint_unit(1, 'ms'),
-        **kwargs
+        default_absolute_time_unit: Union[str, pint.Quantity] = _get_pint_unit(1, 'ms'),
     ):
         """
         :param self:
         :param conditions: (ConditionSet) - a :keyword:`ConditionSet` to be scheduled
         """
-        self.conditions = ConditionSet(conditions)
+        self.conditions = ConditionSet()
+        self._last_handled_structural_condition_order = None
+
+        self._graphs = []
+        self._consideration_queues = []
+        self._consideration_queue_indices = []
 
-        # the consideration queue is the ordered list of sets of nodes in the graph, by the
-        # order in which they should be checked to ensure that all parents have a chance to run before their children
-        self.consideration_queue = []
         if termination_conds is None:
             termination_conds = default_termination_conds.copy()
         else:
             termination_conds = {**default_termination_conds, **termination_conds}
         self.default_termination_conds = Scheduler._parse_termination_conditions(termination_conds)
         self._termination_conds = self.default_termination_conds.copy()
 
         self.cycle_nodes = set()
         self.mode = mode
         self.default_absolute_time_unit = _parse_absolute_unit(default_absolute_time_unit)
 
-        if graph is not None:
-            try:
-                # networkx graph
-                self.dependency_dict = {
-                    child: set(parents.keys())
-                    for child, parents in graph.succ.items()
-                }
-            except AttributeError:
-                self.dependency_dict = graph
-            self.consideration_queue = list(toposort(self.dependency_dict))
-            self.nodes = []
-            for consideration_set in self.consideration_queue:
-                for node in consideration_set:
-                    self.nodes.append(node)
-        else:
+        if isinstance(graph, nx.DiGraph):
+            base_graph = networkx_digraph_to_dependency_dict(graph)
+        elif graph is None or isinstance(graph, nx.Graph):
             raise SchedulerError(
                 'Must instantiate a Scheduler with a graph dependency dict or a networkx.DiGraph'
             )
+        else:
+            # add empty dependency set for senders that aren't present
+            base_graph = {
+                **{n: set() for n in set().union(*graph.values())},
+                **clone_graph(graph)
+            }
+
+        self._push_graph(base_graph)
 
-        self._generate_consideration_queue_indices()
+        self.nodes = list(base_graph.keys())
+
+        # add conditions after initial graph to deal with structural
+        if conditions is not None:
+            self.add_condition_set(conditions)
 
         self.default_execution_id = default_execution_id
         # stores the in order list of self.run's yielded outputs
         self.execution_list = {self.default_execution_id: []}
         self.execution_timestamps = {self.default_execution_id: []}
         self.clocks = {self.default_execution_id: Clock()}
         self.counts_total = {}
         self.counts_useable = {}
         self._init_counts(execution_id=self.default_execution_id)
         self.date_creation = datetime.datetime.now()
         self.date_last_run_end = None
 
-    def _generate_consideration_queue_indices(self):
-        self.consideration_queue_indices = {}
-        for i, cs in enumerate(self.consideration_queue):
-            self.consideration_queue_indices.update({
-                n: i for n in cs
-            })
-
     def _init_counts(self, execution_id, base_execution_id=NotImplemented):
         """
             Attributes
             ----------
 
                 execution_id
                     the execution_id to initialize counts for
@@ -583,124 +624,236 @@
         new_conds = self.termination_conds.copy()
         new_conds.update(termination_conds)
 
         return new_conds
 
     @staticmethod
     def _parse_termination_conditions(termination_conds):
+        err_msg = (
+            "Termination conditions must be a dictionary of the form"
+            " {TimeScale: Condition, ...} and cannot include"
+            " GraphStructureCondition."
+        )
+
         # parse string representation of TimeScale
-        parsed_conds = {}
+        parsed_conds = termination_conds
         delkeys = set()
         for scale in termination_conds:
             try:
                 parsed_conds[getattr(TimeScale, scale.upper())] = termination_conds[scale]
                 delkeys.add(scale)
             except (AttributeError, TypeError):
                 pass
 
-        termination_conds.update(parsed_conds)
-
         try:
-            termination_conds = {
-                k: termination_conds[k] for k in termination_conds
+            parsed_conds = {
+                k: parsed_conds[k]
+                for k in parsed_conds
                 if (
                     isinstance(k, TimeScale)
-                    and isinstance(termination_conds[k], Condition)
+                    and isinstance(parsed_conds[k], Condition)
                     and k not in delkeys
                 )
             }
         except TypeError:
-            raise TypeError('termination_conditions must be a dictionary of the form {TimeScale: Condition, ...}')
+            raise TypeError(err_msg)
         else:
-            return termination_conds
+            invalid_conds = {
+                k: termination_conds[k]
+                for k in termination_conds.keys() - parsed_conds.keys() - delkeys
+            }
+            if len(invalid_conds) > 0:
+                raise SchedulerError(f"{err_msg} Invalid: {invalid_conds}")
+            return parsed_conds
 
     def end_environment_sequence(self, execution_id=NotImplemented):
         """Signals that an `ENVIRONMENT_SEQUENCE` has completed
 
         Args:
             execution_id (optional): Defaults to `Scheduler.default_execution_id`
         """
         if execution_id is NotImplemented:
             execution_id = self.default_execution_id
 
         self._increment_time(TimeScale.ENVIRONMENT_SEQUENCE, execution_id)
 
+    def add_graph_edge(self, sender: Hashable, receiver: Hashable) -> AddEdgeTo:
+        """
+        Adds an edge to the `graph <Scheduler.graph>` from **sender** to
+        **receiver**. Equivalent to ``add_condition(sender,
+        AddEdgeTo(receiver))``.
+
+        Args:
+            sender (Hashable): sender of the new edge
+            receiver (Hashable): receiver of the new edge
+
+        Returns:
+            AddEdgeTo: the new condition added to implement the edge
+        """
+        cond = AddEdgeTo(receiver)
+        self.add_condition(sender, cond)
+        return cond
+
+    def remove_graph_edge(self, sender: Hashable, receiver: Hashable) -> RemoveEdgeFrom:
+        """
+        Removes an edge from the `graph <Scheduler.graph>` from
+        **sender** to **receiver** if it exists. Equivalent to
+        ``add_condition(receiver, RemoveEdgeFrom(sender))``.
+
+        Args:
+            sender (Hashable): sender of the edge to be removed
+            receiver (Hashable): receiver of the edge to be removed
+
+        Returns:
+            RemoveEdgeFrom: the new condition added to implement the edge
+        """
+        cond = RemoveEdgeFrom(sender)
+        self.add_condition(receiver, cond)
+        return cond
+
     ################################################################################
     # Wrapper methods
     #   to allow the user to ignore the ConditionSet internals
     ################################################################################
     def __contains__(self, item):
         return self.conditions.__contains__(item)
 
-    def add_condition(self, owner, condition):
+    def add_condition(
+        self, owner: Hashable, condition: typing_condition_base
+    ):
         """
-        Adds a `Condition` to the Scheduler. If **owner** already has a Condition, it is overwritten
-        with the new one. If you want to add multiple conditions to a single owner, use the
-        `composite Conditions <Conditions_Composite>` to accurately specify the desired behavior.
+        Adds a `basic <Condition>` or `graph structure
+        <GraphStructureCondition>` Condition to the Scheduler.
+
+        If **condition** is basic, it will overwrite the current basic
+        Condition for **owner**, if present. If you want to add multiple
+        basic Conditions to a single owner, instead add a single
+        `Composite Condition <Conditions_Composite>` to accurately
+        specify the desired behavior.
+
+        If **condition** is structural, it will be applied on top of
+        `Scheduler.graph` in the order it is added.
 
         Arguments
         ---------
 
         owner : ``node``
             specifies the node with which the **condition** should be associated. **condition**
             will govern the execution behavior of **owner**
 
-        condition : Condition
+        condition : ConditionBase
             specifies the Condition, associated with the **owner** to be added to the ConditionSet.
         """
         self.conditions.add_condition(owner, condition)
+        self._handle_modified_structural_conditions()
 
     def add_condition_set(self, conditions):
         """
-        Adds a set of `Conditions <Condition>` (in the form of a dict or another ConditionSet) to the Scheduler.
-        Any Condition added here will overwrite an existing Condition for a given owner.
-        If you want to add multiple conditions to a single owner, add a single `Composite Condition <Conditions_Composite>`
-        to accurately specify the desired behavior.
+        Adds a set of `basic <Condition>` or `graph structure
+        <GraphStructureCondition>` Conditions (in the form of a dict or
+        another ConditionSet) to the Scheduler.
+
+        Any basic Condition added here will overwrite the current basic
+        Condition for a given owner, if present. If you want to add
+        multiple basic Conditions to a single owner, instead add a
+        single `Composite Condition <Conditions_Composite>` to
+        accurately specify the desired behavior.
+
+        Any structural Condition added here will be applied on top of
+        `Scheduler.graph` in the order they are returned by iteration
+        over **conditions**.
 
         Arguments
         ---------
 
         conditions : dict[``node``: `Condition`], `ConditionSet`
             specifies collection of Conditions to be added to this ConditionSet,
 
             if a dict is provided:
                 each entry should map an owner node (the node whose execution behavior will be
                 governed) to a `Condition <Condition>`
 
         """
         self.conditions.add_condition_set(conditions)
+        self._handle_modified_structural_conditions()
+
+    def remove_condition(
+        self, owner_or_condition: Union[Hashable, typing_condition_base]
+    ) -> Union[typing_condition_base, None]:
+        """
+        Removes the condition specified as or owned by
+        **owner_or_condition**.
+
+        Args:
+            owner_or_condition (Union[Hashable, `ConditionBase`]):
+                Either a condition or the owner of a condition
+
+        Returns:
+            The condition removed, or None if no condition removed
+
+        Raises:
+            ConditionError:
+                - when **owner_or_condition** is an owner and it owns
+                  multiple conditions
+                - when **owner_or_condition** is a condition and its
+                  owner is None
+        """
+        return self.conditions.remove_condition(owner_or_condition)
 
     ################################################################################
     # Validation methods
     #   to provide the user with info if they do something odd
     ################################################################################
     def _validate_run_state(self):
+        try:
+            _build_consideration_queue(self.graph)
+        except CircularDependencyError as e:
+            raise SchedulerError(
+                f'Cannot run on a graph that contains a cycle: {e}'
+            ) from e
+
+        if (
+            self.consideration_queue == 1
+            and self.consideration_queue[0] == set()
+            and len(self.graph) != 0
+        ):
+            raise SchedulerError('Unexpected empty consideration queue')
+
         self._validate_conditions()
 
     def _validate_conditions(self):
         unspecified_nodes = []
         for node in self.nodes:
-            if node not in self.conditions:
-                dependencies = list(self.dependency_dict[node])
+            if node not in self.conditions.conditions_basic:
+                dependencies = list(self.graph[node])
                 if len(dependencies) == 0:
                     cond = Always()
                 elif len(dependencies) == 1:
                     cond = EveryNCalls(dependencies[0], 1)
                 else:
                     cond = All(*[EveryNCalls(x, 1) for x in dependencies])
 
                 self.add_condition(node, cond)
                 unspecified_nodes.append(node)
         if len(unspecified_nodes) > 0:
             logger.info(
                 'These nodes have no Conditions specified, and will be scheduled with conditions: {0}'.format(
-                    {node: self.conditions[node] for node in unspecified_nodes}
+                    {node: self.conditions.conditions_basic[node] for node in unspecified_nodes}
                 )
             )
 
+        if (
+            self.mode is SchedulingMode.EXACT_TIME
+            and len(self.conditions.conditions_structural) > 0
+        ):
+            warnings.warn(
+                'In exact time mode, graph structure conditions will have no'
+                f' effect: {self.conditions.conditions_structural}'
+            )
+
     ################################################################################
     # Run methods
     ################################################################################
     def run(
         self,
         termination_conds=None,
         execution_id=None,
@@ -713,19 +866,14 @@
         executions at each iteration
 
         :param termination_conds: (dict) - a mapping from `TimeScale`\\s to `Condition`\\s that when met
                terminate the execution of the specified `TimeScale`
         """
         self._validate_run_state()
 
-        if self.mode is SchedulingMode.EXACT_TIME:
-            effective_consideration_queue = [set(self.nodes)]
-        else:
-            effective_consideration_queue = self.consideration_queue
-
         if termination_conds is None:
             termination_conds = self.termination_conds
         else:
             termination_conds = self._combine_termination_conditions(termination_conds)
 
         current_time = self.get_clock(execution_id).time
         is_satisfied_kwargs = {
@@ -767,22 +915,22 @@
         ):
             self._reset_counts_total(TimeScale.PASS, execution_id)
 
             execution_list_has_changed = False
             cur_index_consideration_queue = 0
 
             while (
-                cur_index_consideration_queue < len(effective_consideration_queue)
+                cur_index_consideration_queue < len(self.consideration_queue)
                 and not termination_conds[TimeScale.ENVIRONMENT_STATE_UPDATE].is_satisfied(**is_satisfied_kwargs)
                 and not termination_conds[TimeScale.ENVIRONMENT_SEQUENCE].is_satisfied(**is_satisfied_kwargs)
             ):
                 # all nodes to be added during this consideration set execution
                 cur_consideration_set_execution_exec = set()
                 # the current "layer/group" of nodes that MIGHT be added during this consideration set execution
-                cur_consideration_set = effective_consideration_queue[cur_index_consideration_queue]
+                cur_consideration_set = self.consideration_queue[cur_index_consideration_queue]
 
                 try:
                     iter(cur_consideration_set)
                 except TypeError as e:
                     raise SchedulerError('cur_consideration_set is not iterable, did you ensure that this Scheduler was instantiated with an actual toposort output for param toposort_ordering? err: {0}'.format(e))
 
                 # do-while, on cur_consideration_set_has_changed
@@ -790,15 +938,15 @@
                 # and nodes can cause cascading adds within this set
                 while True:
                     cur_consideration_set_has_changed = False
                     for current_node in cur_consideration_set:
                         # only add each node once during a single consideration set execution, this also serves
                         # to prevent infinitely cascading adds
                         if current_node not in cur_consideration_set_execution_exec:
-                            if self.conditions.conditions[current_node].is_satisfied(**is_satisfied_kwargs):
+                            if self.conditions.conditions_basic[current_node].is_satisfied(**is_satisfied_kwargs):
                                 cur_consideration_set_execution_exec.add(current_node)
                                 execution_list_has_changed = True
                                 cur_consideration_set_has_changed = True
 
                                 for ts in TimeScale:
                                     self.counts_total[execution_id][ts][current_node] += 1
                                 # current_node's node is added to the execution queue, so we now need to
@@ -886,19 +1034,22 @@
     def get_absolute_conditions(self, termination_conds=None):
         if termination_conds is None:
             termination_conds = self.termination_conds
 
         return {
             owner: cond
             for owner, cond
-            in [*self.conditions.conditions.items(), *termination_conds.items()]
+            in [*self.conditions.conditions_basic.items(), *termination_conds.items()]
             if cond.is_absolute
         }
 
-    def get_clock(self, execution_id):
+    def get_clock(self, execution_id=NotImplemented):
+        if execution_id is NotImplemented:
+            execution_id = self.default_execution_id
+
         try:
             return self.clocks[execution_id.default_execution_id]
         except AttributeError:
             if execution_id not in self.clocks:
                 self._init_clock(execution_id)
             return self.clocks[execution_id]
         except KeyError:
@@ -928,7 +1079,102 @@
             self._termination_conds = self._combine_termination_conditions(
                 termination_conds
             )
 
     @property
     def _in_exact_time_mode(self):
         return self.mode is SchedulingMode.EXACT_TIME or len(self.consideration_queue) == 1
+
+    def _handle_modified_structural_conditions(self):
+        if self._last_handled_structural_condition_order != self.conditions.structural_condition_order:
+            common_index = -1
+            for i, cond in enumerate(self.conditions.structural_condition_order):
+                try:
+                    if self._last_handled_structural_condition_order[i] == cond:
+                        common_index = i
+                    else:
+                        break
+                except (IndexError, TypeError):
+                    break
+
+            # remove scheduler dependency dicts down to the common
+            # structural condition
+            if self._last_handled_structural_condition_order is not None:
+                # if anything must be done with the popped structures
+                # and cond, the iteration order should be reversed
+                for cond in self._last_handled_structural_condition_order[common_index + 1:]:
+                    self._pop_graph()
+
+            # add dependency dicts for new structural conditions
+            cur_graph = self._graphs[-1]
+            for cond in self.conditions.structural_condition_order[common_index + 1:]:
+                cur_graph = cond.modify_graph(cur_graph)
+                self._push_graph(cur_graph)
+
+            self._last_handled_structural_condition_order = copy.copy(
+                self.conditions.structural_condition_order
+            )
+
+    def _push_graph(self, graph):
+        try:
+            consideration_queue = _build_consideration_queue(graph)
+        except CircularDependencyError as e:
+            consideration_queue = [set()]
+            try:
+                cond = self.conditions.structural_condition_order[-1]
+            except IndexError:
+                cond_str = 'Base graph'
+            else:
+                cond_str = f'Condition {cond} for {cond.owner} creates a cycle: {e}'
+            warnings.warn(cond_str)
+
+        self._graphs.append(graph)
+        self._consideration_queues.append(consideration_queue)
+        self._consideration_queue_indices.append(
+            _generate_consideration_queue_indices(consideration_queue)
+        )
+
+    def _pop_graph(self):
+        return (
+            self._graphs.pop(),
+            self._consideration_queues.pop(),
+            self._consideration_queue_indices.pop(),
+        )
+
+    @property
+    def graph(self) -> typing_graph_dependency_dict:
+        """
+        The current graph used by this Scheduler, which is modified by
+        any `graph structure conditions
+        <Condition_Graph_Structure_Intro>` added
+        """
+        self._handle_modified_structural_conditions()
+        return self._graphs[-1]
+
+    # Maintain backwards compatibility for v1.x
+    @property
+    def dependency_dict(self) -> typing_graph_dependency_dict:
+        return self.graph
+
+    @property
+    def consideration_queue(self) -> List[Set[Hashable]]:
+        """
+        The ordered list of sets of nodes in the graph, by the order in
+        which they will be checked to ensure that all senders have a
+        chance to run before their receivers
+        """
+        self._handle_modified_structural_conditions()
+
+        if self.mode is SchedulingMode.EXACT_TIME:
+            return [set(self.graph.keys())]
+        else:
+            return self._consideration_queues[-1]
+
+    @property
+    def consideration_queue_indices(self) -> Dict[Hashable, int]:
+        """
+        A dictionary mapping the graph's nodes to their position in the
+        original consideration queue. This is the same as the
+        consideration queue when not using SchedulingMode.EXACT_TIME.
+        """
+        self._handle_modified_structural_conditions()
+        return self._consideration_queue_indices[-1]
```

### Comparing `graph-scheduler-1.1.2/src/graph_scheduler/time.py` & `graph-scheduler-1.2.0/src/graph_scheduler/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import copy
 import enum
 import functools
 import keyword
 import re
 import types
-import typing
+from typing import Dict, Union
 
 from graph_scheduler import _unit_registry
 
 __all__ = [
     'Clock', 'TimeScale', 'Time', 'SimpleTime', 'TimeHistoryTree', 'TimeScaleError', 'set_time_scale_alias', 'remove_time_scale_alias'
 ]
 
@@ -618,28 +618,28 @@
     if keyword.iskeyword(attr):
         return f'{attr}_'
     else:
         return attr
 
 
 @functools.lru_cache(maxsize=None)
-def _time_scale_to_class_str(time_scale: typing.Union[TimeScale, str]) -> str:
+def _time_scale_to_class_str(time_scale: Union[TimeScale, str]) -> str:
     try:
         name = time_scale.name
     except AttributeError:
         name = time_scale
 
     return ''.join([f'{x[0].upper()}{x[1:].lower()}' for x in name.split('_')])
 
 
 def _attr_str_to_time_scale(attr_str):
     return getattr(TimeScale, attr_str.rstrip('_'))
 
 
-def _multi_substitute_docstring(cls, subs: typing.Dict[str, str]):
+def _multi_substitute_docstring(cls, subs: Dict[str, str]):
     new_docstring = cls.__doc__
     try:
         for prev, new in subs.items():
             new_docstring = re.sub(prev, new, new_docstring)
     except TypeError:
         pass
     else:
```

### Comparing `graph-scheduler-1.1.2/src/graph_scheduler.egg-info/PKG-INFO` & `graph-scheduler-1.2.0/src/graph_scheduler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: graph-scheduler
-Version: 1.1.2
+Version: 1.2.0
 Summary: A graph-based scheduler of nodes based on structure and conditions
 Home-page: https://github.com/kmantel/graph-scheduler
 Author: Katherine Mantel, Princeton University
 Author-email: kmantel@princeton.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kmantel/graph-scheduler/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # Graph Scheduler
```

### Comparing `graph-scheduler-1.1.2/tests/scheduling/test_time.py` & `graph-scheduler-1.2.0/tests/scheduling/test_time.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-import psyneulink as pnl
 import pytest
 
-import graph_scheduler
-from graph_scheduler.time import (
-    SimpleTime, Time, TimeHistoryTree, TimeScale, _time_scale_aliases,
-    remove_time_scale_alias, set_time_scale_alias,
-)
+import graph_scheduler as gs
+
+SimpleTestNode = pytest.helpers.get_test_node()
 
 
 class TestTime:
     @pytest.mark.parametrize(
         'base, increment_time_scale, expected',
         [
             (
-                Time(environment_sequence=0, environment_state_update=0, pass_=0, consideration_set_execution=0),
-                TimeScale.ENVIRONMENT_STATE_UPDATE,
-                Time(environment_sequence=0, environment_state_update=1, pass_=0, consideration_set_execution=0),
+                gs.Time(environment_sequence=0, environment_state_update=0, pass_=0, consideration_set_execution=0),
+                gs.TimeScale.ENVIRONMENT_STATE_UPDATE,
+                gs.Time(environment_sequence=0, environment_state_update=1, pass_=0, consideration_set_execution=0),
             ),
             (
-                Time(environment_sequence=0, environment_state_update=0, pass_=5, consideration_set_execution=9),
-                TimeScale.ENVIRONMENT_STATE_UPDATE,
-                Time(environment_sequence=0, environment_state_update=1, pass_=0, consideration_set_execution=0),
+                gs.Time(environment_sequence=0, environment_state_update=0, pass_=5, consideration_set_execution=9),
+                gs.TimeScale.ENVIRONMENT_STATE_UPDATE,
+                gs.Time(environment_sequence=0, environment_state_update=1, pass_=0, consideration_set_execution=0),
             ),
             (
-                Time(environment_sequence=1, environment_state_update=0, pass_=5, consideration_set_execution=9),
-                TimeScale.ENVIRONMENT_STATE_UPDATE,
-                Time(environment_sequence=1, environment_state_update=1, pass_=0, consideration_set_execution=0),
+                gs.Time(environment_sequence=1, environment_state_update=0, pass_=5, consideration_set_execution=9),
+                gs.TimeScale.ENVIRONMENT_STATE_UPDATE,
+                gs.Time(environment_sequence=1, environment_state_update=1, pass_=0, consideration_set_execution=0),
             ),
             (
-                Time(environment_sequence=1, environment_state_update=0, pass_=5, consideration_set_execution=9),
-                TimeScale.CONSIDERATION_SET_EXECUTION,
-                Time(environment_sequence=1, environment_state_update=0, pass_=5, consideration_set_execution=10),
+                gs.Time(environment_sequence=1, environment_state_update=0, pass_=5, consideration_set_execution=9),
+                gs.TimeScale.CONSIDERATION_SET_EXECUTION,
+                gs.Time(environment_sequence=1, environment_state_update=0, pass_=5, consideration_set_execution=10),
             ),
         ],
     )
     def test_increment(self, base, increment_time_scale, expected):
         base._increment_by_time_scale(increment_time_scale)
         assert base == expected
 
-    @pytest.mark.psyneulink
     def test_multiple_runs(self):
-        t1 = pnl.TransferMechanism()
-        t2 = pnl.TransferMechanism()
-
-        C = pnl.Composition(pathways=[t1, t2])
+        t1 = SimpleTestNode('t1')
+        t2 = SimpleTestNode('t2')
 
-        C.run(inputs={t1: [[1.0], [2.0], [3.0]]})
-        assert C.scheduler.get_clock(C).time == pnl.Time(run=1, trial=0, pass_=0, time_step=0)
+        sched = gs.Scheduler(graph={t1: set(), t2: {t1}})
 
-        C.run(inputs={t1: [[4.0], [5.0], [6.0]]})
-        assert C.scheduler.get_clock(C).time == pnl.Time(run=2, trial=0, pass_=0, time_step=0)
+        sched.run()
+        sched.end_environment_sequence()
+        assert sched.get_clock().time == gs.Time(environment_sequence=1, environment_state_update=0, pass_=0, consideration_set_execution=0)
+
+        sched.run()
+        sched.end_environment_sequence()
+        assert sched.get_clock().time == gs.Time(environment_sequence=2, environment_state_update=0, pass_=0, consideration_set_execution=0)
 
     def test_get_set_item_time(self):
-        t = Time(run=1, trial=2, pass_=3, time_step=4)
-        st = SimpleTime(t)
+        t = gs.Time(environment_sequence=1, environment_state_update=2, pass_=3, consideration_set_execution=4)
+        st = gs.SimpleTime(t)
 
         assert t[0] == 4
         assert t[1] == 3
         assert t[2] == 2
         assert t[3] == 1
         assert t[4] == 0
 
@@ -86,151 +84,151 @@
         assert st[0] == 6
         assert st[2] == 2
         assert st[3] == 5
 
 
 class TestTimeHistoryTree:
     def test_defaults(self):
-        h = TimeHistoryTree()
+        h = gs.TimeHistoryTree()
 
         for node in [h, h.children[0]]:
             assert len(node.children) == 1
             assert all([node.total_times[ts] == 0 for ts in node.total_times])
-            assert node.time_scale == TimeScale.get_parent(node.children[0].time_scale)
-            assert node.time_scale >= TimeScale.ENVIRONMENT_STATE_UPDATE
+            assert node.time_scale == gs.TimeScale.get_parent(node.children[0].time_scale)
+            assert node.time_scale >= gs.TimeScale.ENVIRONMENT_STATE_UPDATE
 
     @pytest.mark.parametrize(
         'max_depth',
         [
-            (TimeScale.ENVIRONMENT_SEQUENCE),
-            (TimeScale.ENVIRONMENT_STATE_UPDATE)
+            (gs.TimeScale.ENVIRONMENT_SEQUENCE),
+            (gs.TimeScale.ENVIRONMENT_STATE_UPDATE)
         ])
     def test_max_depth(self, max_depth):
-        h = TimeHistoryTree(max_depth=max_depth)
+        h = gs.TimeHistoryTree(max_depth=max_depth)
 
         node = h
         found_max_depth = h.time_scale == max_depth
         while len(node.children) > 0:
             node = node.children[0]
             found_max_depth = found_max_depth or node.time_scale == max_depth
             assert node.time_scale >= max_depth
 
         assert found_max_depth
 
 
 class TestAliasTimeScale:
     @pytest.fixture(scope='class', autouse=True)
     def setup_alias(cls):
-        # must save and replace psyneulink aliases as long as tests still
-        # depend on psyneulink
-        existing_aliases = _time_scale_aliases.copy()
+        # save and replace other aliases in case integration packages
+        # apply them (psyneulink does)
+        existing_aliases = gs.time._time_scale_aliases.copy()
         for ts, alias in existing_aliases.items():
-            remove_time_scale_alias(alias)
+            gs.remove_time_scale_alias(alias)
 
-        set_time_scale_alias('MY_ENVIRONMENT_STATE_UPDATE_ALIAS', TimeScale.ENVIRONMENT_STATE_UPDATE)
+        gs.set_time_scale_alias('MY_ENVIRONMENT_STATE_UPDATE_ALIAS', gs.TimeScale.ENVIRONMENT_STATE_UPDATE)
 
         yield
 
-        remove_time_scale_alias('MY_ENVIRONMENT_STATE_UPDATE_ALIAS')
+        gs.remove_time_scale_alias('MY_ENVIRONMENT_STATE_UPDATE_ALIAS')
         for ts, alias in existing_aliases.items():
-            set_time_scale_alias(alias, ts)
+            gs.set_time_scale_alias(alias, ts)
 
     @staticmethod
     def assert_environment_state_update_and_alias_equals(time_obj, value):
         assert time_obj.my_environment_state_update_alias == value
         assert time_obj.environment_state_update == value
 
-        if isinstance(time_obj, Time):
-            assert time_obj._get_by_time_scale(TimeScale.ENVIRONMENT_STATE_UPDATE) == value
-            assert time_obj._get_by_time_scale(TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS) == value
+        if isinstance(time_obj, gs.Time):
+            assert time_obj._get_by_time_scale(gs.TimeScale.ENVIRONMENT_STATE_UPDATE) == value
+            assert time_obj._get_by_time_scale(gs.TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS) == value
 
     def test_alias_references_timescale(self):
-        assert TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS is TimeScale.ENVIRONMENT_STATE_UPDATE
-        assert TimeScale.get_parent(TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS) is TimeScale.get_parent(TimeScale.ENVIRONMENT_STATE_UPDATE)
-        assert TimeScale.get_child(TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS) is TimeScale.get_child(TimeScale.ENVIRONMENT_STATE_UPDATE)
+        assert gs.TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS is gs.TimeScale.ENVIRONMENT_STATE_UPDATE
+        assert gs.TimeScale.get_parent(gs.TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS) is gs.TimeScale.get_parent(gs.TimeScale.ENVIRONMENT_STATE_UPDATE)
+        assert gs.TimeScale.get_child(gs.TimeScale.MY_ENVIRONMENT_STATE_UPDATE_ALIAS) is gs.TimeScale.get_child(gs.TimeScale.ENVIRONMENT_STATE_UPDATE)
 
     @pytest.mark.parametrize(
         'kwargs, value',
         [
             ({'environment_state_update': 1}, 1),
             ({'my_environment_state_update_alias': 1}, 1)
         ]
     )
     def test_time_change_in_init(self, kwargs, value):
-        t = Time(**kwargs)
-        st = SimpleTime(t)
+        t = gs.Time(**kwargs)
+        st = gs.SimpleTime(t)
 
         self.assert_environment_state_update_and_alias_equals(t, value)
         self.assert_environment_state_update_and_alias_equals(st, value)
 
     def test_time_change_by_original_attr(self):
-        t = Time()
-        st = SimpleTime(t)
+        t = gs.Time()
+        st = gs.SimpleTime(t)
 
         t.environment_state_update = 1
 
         self.assert_environment_state_update_and_alias_equals(t, 1)
         self.assert_environment_state_update_and_alias_equals(st, 1)
 
     def test_time_change_by_alias_attr(self):
-        t = Time()
-        st = SimpleTime(t)
+        t = gs.Time()
+        st = gs.SimpleTime(t)
 
         t.my_environment_state_update_alias = 1
 
         self.assert_environment_state_update_and_alias_equals(t, 1)
         self.assert_environment_state_update_and_alias_equals(st, 1)
 
-    @pytest.mark.parametrize('time_scale', [TimeScale.ENVIRONMENT_STATE_UPDATE, 'MY_ENVIRONMENT_STATE_UPDATE_ALIAS'])
+    @pytest.mark.parametrize('time_scale', [gs.TimeScale.ENVIRONMENT_STATE_UPDATE, 'MY_ENVIRONMENT_STATE_UPDATE_ALIAS'])
     def test_time_change_by_method_set(self, time_scale):
         # alias does not exist at parametrization time
         try:
-            time_scale = getattr(TimeScale, time_scale)
+            time_scale = getattr(gs.TimeScale, time_scale)
         except TypeError:
             pass
 
-        t = Time()
-        st = SimpleTime(t)
+        t = gs.Time()
+        st = gs.SimpleTime(t)
         t._set_by_time_scale(time_scale, 1)
 
         self.assert_environment_state_update_and_alias_equals(t, 1)
         self.assert_environment_state_update_and_alias_equals(st, 1)
 
-    @pytest.mark.parametrize('time_scale', [TimeScale.ENVIRONMENT_STATE_UPDATE, 'MY_ENVIRONMENT_STATE_UPDATE_ALIAS'])
+    @pytest.mark.parametrize('time_scale', [gs.TimeScale.ENVIRONMENT_STATE_UPDATE, 'MY_ENVIRONMENT_STATE_UPDATE_ALIAS'])
     def test_time_change_by_method_increment(self, time_scale):
         # alias does not exist at parametrization time
         try:
-            time_scale = getattr(TimeScale, time_scale)
+            time_scale = getattr(gs.TimeScale, time_scale)
         except TypeError:
             pass
 
-        t = Time()
-        st = SimpleTime(t)
+        t = gs.Time()
+        st = gs.SimpleTime(t)
         t._increment_by_time_scale(time_scale)
 
         self.assert_environment_state_update_and_alias_equals(t, 1)
         self.assert_environment_state_update_and_alias_equals(st, 1)
 
     def test_time_repr(self):
-        t = Time(my_environment_state_update_alias=1)
-        st = SimpleTime(t)
+        t = gs.Time(my_environment_state_update_alias=1)
+        st = gs.SimpleTime(t)
 
         assert repr(t) == 'Time(environment_sequence: 0, my_environment_state_update_alias: 1, pass: 0, consideration_set_execution: 0)'
         assert repr(st) == 'Time(environment_sequence: 0, my_environment_state_update_alias: 1, consideration_set_execution: 0)'
 
     def test_aliased_conditions(self):
         graph = {'A': set()}
-        sched_orig = graph_scheduler.Scheduler(
+        sched_orig = gs.Scheduler(
             graph=graph,
-            termination_conds={TimeScale.ENVIRONMENT_STATE_UPDATE: graph_scheduler.AtPass(2)}
+            termination_conds={gs.TimeScale.ENVIRONMENT_STATE_UPDATE: gs.AtPass(2)}
         )
-        sched_alias = graph_scheduler.Scheduler(
+        sched_alias = gs.Scheduler(
             graph=graph,
-            termination_conds={TimeScale.ENVIRONMENT_STATE_UPDATE: graph_scheduler.AtPass(2)}
+            termination_conds={gs.TimeScale.ENVIRONMENT_STATE_UPDATE: gs.AtPass(2)}
         )
 
-        sched_orig.add_condition('A', graph_scheduler.BeforeEnvironmentStateUpdate(3))
-        sched_alias.add_condition('A', graph_scheduler.BeforeMyEnvironmentStateUpdateAlias(3))
+        sched_orig.add_condition('A', gs.BeforeEnvironmentStateUpdate(3))
+        sched_alias.add_condition('A', gs.BeforeMyEnvironmentStateUpdateAlias(3))
 
         # should run in environment state updates 0-2 and not in 3
         for _ in range(4):
             assert list(sched_orig.run()) == list(sched_alias.run())
```

### Comparing `graph-scheduler-1.1.2/versioneer.py` & `graph-scheduler-1.2.0/versioneer.py`

 * *Files identical despite different names*

