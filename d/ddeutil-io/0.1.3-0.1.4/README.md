# Comparing `tmp/ddeutil_io-0.1.3.tar.gz` & `tmp/ddeutil_io-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_io-0.1.3.tar", last modified: Tue May 14 16:24:30 2024, max compression
+gzip compressed data, was "ddeutil_io-0.1.4.tar", last modified: Wed May 15 15:15:06 2024, max compression
```

## Comparing `ddeutil_io-0.1.3.tar` & `ddeutil_io-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.386695 ddeutil_io-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-14 16:24:30.386695 ddeutil_io-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:24:30.386695 ddeutil_io-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.378695 ddeutil_io-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.378695 ddeutil_io-0.1.3/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/src/ddeutil/io/__base/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/__regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 16:24:30.000000 ddeutil_io-0.1.3/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:24:30.382695 ddeutil_io-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_base_file_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-14 16:24:25.000000 ddeutil_io-0.1.3/tests/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.964480 ddeutil_io-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.964480 ddeutil_io-0.1.4/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.964480 ddeutil_io-0.1.4/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/src/ddeutil/io/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/__regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 15:15:06.000000 ddeutil_io-0.1.4/src/ddeutil_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:06.968480 ddeutil_io-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_base_file_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_config_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-15 15:15:00.000000 ddeutil_io-0.1.4/tests/test_register.py
```

### Comparing `ddeutil_io-0.1.3/LICENSE` & `ddeutil_io-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/PKG-INFO` & `ddeutil_io-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
@@ -22,16 +22,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ddeutil
 Requires-Dist: fmtutil
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: deepdiff==7.0.1
 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: sqlalchemy==2.0.20
-Requires-Dist: pandas==2.2.2
 
 # Data Utility Package: _IO_
 
 [![test](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml)
 [![python support version](https://img.shields.io/pypi/pyversions/ddeutil-io)](https://pypi.org/project/ddeutil-io/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/ddeutil-io)](https://github.com/korawica/ddeutil-io)
```

### Comparing `ddeutil_io-0.1.3/README.md` & `ddeutil_io-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/pyproject.toml` & `ddeutil_io-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 requires-python = ">=3.9.13"
 dependencies = [
     "ddeutil",
     "fmtutil",
     "pydantic==2.7.1",
     "deepdiff==7.0.1",
     "pyyaml==6.0.1",
-    "sqlalchemy==2.0.20",
-    "pandas==2.2.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/korawica/ddeutil-io/"
 "Source Code" = "https://github.com/korawica/ddeutil-io/"
```

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/__base/__init__.py` & `ddeutil_io-0.1.4/src/ddeutil/io/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/__base/__regex.py` & `ddeutil_io-0.1.4/src/ddeutil/io/__base/__regex.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/__base/files.py` & `ddeutil_io-0.1.4/src/ddeutil/io/__base/files.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/__base/utils.py` & `ddeutil_io-0.1.4/src/ddeutil/io/__base/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/config.py` & `ddeutil_io-0.1.4/src/ddeutil/io/config.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.4/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/models.py` & `ddeutil_io-0.1.4/src/ddeutil/io/models.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/register.py` & `ddeutil_io-0.1.4/src/ddeutil/io/register.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.4/src/ddeutil/io/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/src/ddeutil_io.egg-info/PKG-INFO` & `ddeutil_io-0.1.4/src/ddeutil_io.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
@@ -22,16 +22,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ddeutil
 Requires-Dist: fmtutil
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: deepdiff==7.0.1
 Requires-Dist: pyyaml==6.0.1
-Requires-Dist: sqlalchemy==2.0.20
-Requires-Dist: pandas==2.2.2
 
 # Data Utility Package: _IO_
 
 [![test](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/ddeutil-io/actions/workflows/tests.yml)
 [![python support version](https://img.shields.io/pypi/pyversions/ddeutil-io)](https://pypi.org/project/ddeutil-io/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/ddeutil-io)](https://github.com/korawica/ddeutil-io)
```

### Comparing `ddeutil_io-0.1.3/src/ddeutil_io.egg-info/SOURCES.txt` & `ddeutil_io-0.1.4/src/ddeutil_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_base_csv.py` & `ddeutil_io-0.1.4/tests/test_base_csv.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_base_dir.py` & `ddeutil_io-0.1.4/tests/test_base_dir.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_base_env.py` & `ddeutil_io-0.1.4/tests/test_base_env.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_base_file.py` & `ddeutil_io-0.1.4/tests/test_base_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_base_file_yaml.py` & `ddeutil_io-0.1.4/tests/test_base_file_yaml.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_config_file.py` & `ddeutil_io-0.1.4/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_config_sqlite.py` & `ddeutil_io-0.1.4/tests/test_config_sqlite.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_models.py` & `ddeutil_io-0.1.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.3/tests/test_register.py` & `ddeutil_io-0.1.4/tests/test_register.py`

 * *Files identical despite different names*

