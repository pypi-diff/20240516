# Comparing `tmp/ae_base-0.3.35.tar.gz` & `tmp/ae_base-0.3.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ae_base-0.3.35.tar", last modified: Mon Feb 26 17:33:39 2024, max compression
+gzip compressed data, was "ae_base-0.3.36.tar", last modified: Wed Mar 13 20:33:37 2024, max compression
```

## Comparing `ae_base-0.3.35.tar` & `ae_base-0.3.36.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 17:33:39.205365 ae_base-0.3.35/
--rw-rw-rw-   0 root         (0) root         (0)    35002 2024-02-26 17:33:27.000000 ae_base-0.3.35/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     5285 2024-02-26 17:33:39.204365 ae_base-0.3.35/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2997 2024-02-26 17:33:27.000000 ae_base-0.3.35/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 17:33:39.199365 ae_base-0.3.35/ae/
--rw-rw-rw-   0 root         (0) root         (0)    46681 2024-02-26 17:33:27.000000 ae_base-0.3.35/ae/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 17:33:39.201365 ae_base-0.3.35/ae_base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5285 2024-02-26 17:33:39.000000 ae_base-0.3.35/ae_base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2024-02-26 17:33:39.000000 ae_base-0.3.35/ae_base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 17:33:39.000000 ae_base-0.3.35/ae_base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      288 2024-02-26 17:33:39.000000 ae_base-0.3.35/ae_base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2024-02-26 17:33:39.000000 ae_base-0.3.35/ae_base.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 17:33:39.000000 ae_base-0.3.35/ae_base.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-26 17:33:39.205365 ae_base-0.3.35/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-02-26 17:33:27.000000 ae_base-0.3.35/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 17:33:39.201365 ae_base-0.3.35/tests/
--rw-rw-rw-   0 root         (0) root         (0)    31310 2024-02-26 17:33:27.000000 ae_base-0.3.35/tests/test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 20:33:37.813361 ae_base-0.3.36/
+-rw-rw-rw-   0 root         (0) root         (0)    35002 2024-03-13 20:33:26.000000 ae_base-0.3.36/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     5219 2024-03-13 20:33:37.813361 ae_base-0.3.36/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-03-13 20:33:26.000000 ae_base-0.3.36/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 20:33:37.808361 ae_base-0.3.36/ae/
+-rw-rw-rw-   0 root         (0) root         (0)    46681 2024-03-13 20:33:26.000000 ae_base-0.3.36/ae/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 20:33:37.810361 ae_base-0.3.36/ae_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5219 2024-03-13 20:33:37.000000 ae_base-0.3.36/ae_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2024-03-13 20:33:37.000000 ae_base-0.3.36/ae_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 20:33:37.000000 ae_base-0.3.36/ae_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      288 2024-03-13 20:33:37.000000 ae_base-0.3.36/ae_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        3 2024-03-13 20:33:37.000000 ae_base-0.3.36/ae_base.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 20:33:37.000000 ae_base-0.3.36/ae_base.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 20:33:37.813361 ae_base-0.3.36/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-13 20:33:26.000000 ae_base-0.3.36/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 20:33:37.809361 ae_base-0.3.36/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    31310 2024-03-13 20:33:26.000000 ae_base-0.3.36/tests/test_base.py
```

### Comparing `ae_base-0.3.35/LICENSE.md` & `ae_base-0.3.36/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.28 -->
+<!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.29 -->
 ### GNU GENERAL PUBLIC LICENSE
 
 Version 3, 29 June 2007
 
 Copyright (C) 2007 Free Software Foundation, Inc.
 <https://fsf.org/>
```

### Comparing `ae_base-0.3.35/PKG-INFO` & `ae_base-0.3.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ae_base
-Version: 0.3.35
+Version: 0.3.36
 Summary: ae namespace module portion base: basic constants, helper functions and context manager
 Home-page: https://gitlab.com/ae-group/ae_base
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://ae.readthedocs.io/en/latest/_autosummary/ae.base.html
 Project-URL: Repository, https://gitlab.com/ae-group/ae_base
@@ -49,25 +49,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project ae.ae V0.3.92 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.13 -->
-# base 0.3.35
+# base 0.3.36
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/ae-group/ae_base/develop?logo=python)](
     https://gitlab.com/ae-group/ae_base)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/ae-group/ae_base/release0.3.34?logo=python)](
-    https://gitlab.com/ae-group/ae_base/-/tree/release0.3.34)
+    https://img.shields.io/gitlab/pipeline/ae-group/ae_base/release0.3.35?logo=python)](
+    https://gitlab.com/ae-group/ae_base/-/tree/release0.3.35)
 [![PyPIVersions](https://img.shields.io/pypi/v/ae_base)](
     https://pypi.org/project/ae-base/#history)
 
->ae namespace module portion base: basic constants, helper functions and context manager.
+>ae_base module 0.3.36.
 
 [![Coverage](https://ae-group.gitlab.io/ae_base/coverage.svg)](
     https://ae-group.gitlab.io/ae_base/coverage/index.html)
 [![MyPyPrecision](https://ae-group.gitlab.io/ae_base/mypy.svg)](
     https://ae-group.gitlab.io/ae_base/lineprecision.txt)
 [![PyLintScore](https://ae-group.gitlab.io/ae_base/pylint.svg)](
     https://ae-group.gitlab.io/ae_base/pylint.log)
```

### Comparing `ae_base-0.3.35/README.md` & `ae_base-0.3.36/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project ae.ae V0.3.92 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.13 -->
-# base 0.3.35
+# base 0.3.36
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/ae-group/ae_base/develop?logo=python)](
     https://gitlab.com/ae-group/ae_base)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/ae-group/ae_base/release0.3.34?logo=python)](
-    https://gitlab.com/ae-group/ae_base/-/tree/release0.3.34)
+    https://img.shields.io/gitlab/pipeline/ae-group/ae_base/release0.3.35?logo=python)](
+    https://gitlab.com/ae-group/ae_base/-/tree/release0.3.35)
 [![PyPIVersions](https://img.shields.io/pypi/v/ae_base)](
     https://pypi.org/project/ae-base/#history)
 
->ae namespace module portion base: basic constants, helper functions and context manager.
+>ae_base module 0.3.36.
 
 [![Coverage](https://ae-group.gitlab.io/ae_base/coverage.svg)](
     https://ae-group.gitlab.io/ae_base/coverage/index.html)
 [![MyPyPrecision](https://ae-group.gitlab.io/ae_base/mypy.svg)](
     https://ae-group.gitlab.io/ae_base/lineprecision.txt)
 [![PyLintScore](https://ae-group.gitlab.io/ae_base/pylint.svg)](
     https://ae-group.gitlab.io/ae_base/pylint.log)
```

### Comparing `ae_base-0.3.35/ae/base.py` & `ae_base-0.3.36/ae/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 from contextlib import contextmanager
 from importlib.machinery import ModuleSpec
 from inspect import getinnerframes, getouterframes, getsourcefile
 from types import ModuleType
 from typing import Any, Callable, Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 
-__version__ = '0.3.35'
+__version__ = '0.3.36'
 
 
 DOCS_FOLDER = 'docs'                            #: project documentation root folder name
 TESTS_FOLDER = 'tests'                          #: name of project folder to store unit/integration tests
 TEMPLATES_FOLDER = 'templates'
 """ template folder name, used in template and namespace root projects to maintain and provide common file templates """
 
@@ -609,31 +609,31 @@
 
     :return:                    username string.
     """
     return getpass.getuser()
 
 
 def project_main_file(import_name: str, project_path: str = "") -> str:
-    """ determine the main module file path of a package project, containing the package __version__ module variable.
+    """ determine the main module file path of a project package, containing the project __version__ module variable.
 
     :param import_name:         import name of the module/package (including namespace prefixes for namespace packages).
     :param project_path:        optional path where the project of the package/module is situated. not needed if the
                                 current working directory is the root folder of either the import_name project or of a
                                 sister project (under the same project parent folder).
     :return:                    absolute file path/name of main module or empty string if no main/version file found.
     """
     join = os.path.join
     *namespace_dirs, portion_name = import_name.split('.')
-    package_name = ('_'.join(namespace_dirs) + '_' if namespace_dirs else "") + portion_name
+    project_name = ('_'.join(namespace_dirs) + '_' if namespace_dirs else "") + portion_name
     paths_parts = main_file_paths_parts(portion_name)
 
     project_path = norm_path(project_path)
     module_paths = []
-    if os.path.basename(project_path) != package_name:
-        module_paths.append(join(os.path.dirname(project_path), package_name, *namespace_dirs))
+    if os.path.basename(project_path) != project_name:
+        module_paths.append(join(os.path.dirname(project_path), project_name, *namespace_dirs))
     if namespace_dirs:
         module_paths.append(join(project_path, *namespace_dirs))
     module_paths.append(project_path)
 
     for module_path in module_paths:
         for path_parts in paths_parts:
             main_file = join(module_path, *path_parts)
```

### Comparing `ae_base-0.3.35/ae_base.egg-info/PKG-INFO` & `ae_base-0.3.36/ae_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ae_base
-Version: 0.3.35
+Version: 0.3.36
 Summary: ae namespace module portion base: basic constants, helper functions and context manager
 Home-page: https://gitlab.com/ae-group/ae_base
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://ae.readthedocs.io/en/latest/_autosummary/ae.base.html
 Project-URL: Repository, https://gitlab.com/ae-group/ae_base
@@ -49,25 +49,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project ae.ae V0.3.92 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.13 -->
-# base 0.3.35
+# base 0.3.36
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/ae-group/ae_base/develop?logo=python)](
     https://gitlab.com/ae-group/ae_base)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/ae-group/ae_base/release0.3.34?logo=python)](
-    https://gitlab.com/ae-group/ae_base/-/tree/release0.3.34)
+    https://img.shields.io/gitlab/pipeline/ae-group/ae_base/release0.3.35?logo=python)](
+    https://gitlab.com/ae-group/ae_base/-/tree/release0.3.35)
 [![PyPIVersions](https://img.shields.io/pypi/v/ae_base)](
     https://pypi.org/project/ae-base/#history)
 
->ae namespace module portion base: basic constants, helper functions and context manager.
+>ae_base module 0.3.36.
 
 [![Coverage](https://ae-group.gitlab.io/ae_base/coverage.svg)](
     https://ae-group.gitlab.io/ae_base/coverage/index.html)
 [![MyPyPrecision](https://ae-group.gitlab.io/ae_base/mypy.svg)](
     https://ae-group.gitlab.io/ae_base/lineprecision.txt)
 [![PyLintScore](https://ae-group.gitlab.io/ae_base/pylint.svg)](
     https://ae-group.gitlab.io/ae_base/pylint.log)
```

### Comparing `ae_base-0.3.35/setup.py` & `ae_base-0.3.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.28
+# THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_project V0.3.29
 """ setup this project with setuptools and aedev.setup_project. """
 import pprint
 import sys
 
 import setuptools
 
 from aedev.setup_project import project_env_vars    # type: ignore
```

### Comparing `ae_base-0.3.35/tests/test_base.py` & `ae_base-0.3.36/tests/test_base.py`

 * *Files identical despite different names*

