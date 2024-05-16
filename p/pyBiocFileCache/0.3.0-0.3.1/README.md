# Comparing `tmp/pybiocfilecache-0.3.0.tar.gz` & `tmp/pybiocfilecache-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiocfilecache-0.3.0.tar", last modified: Sun May  5 16:25:47 2024, max compression
+gzip compressed data, was "pybiocfilecache-0.3.1.tar", last modified: Thu May 16 19:28:05 2024, max compression
```

## Comparing `pybiocfilecache-0.3.0.tar` & `pybiocfilecache-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.043834 pybiocfilecache-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.047834 pybiocfilecache-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.051834 pybiocfilecache-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.051834 pybiocfilecache-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.043834 pybiocfilecache-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:25:12.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 16:25:47.000000 pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.051834 pybiocfilecache-0.3.0/src/pybiocfilecache/
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/BiocFileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/src/pybiocfilecache/db/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/db/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/src/pybiocfilecache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:25:47.055834 pybiocfilecache-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/data/test1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/data/test2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-05 16:25:04.000000 pybiocfilecache-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.603284 pybiocfilecache-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.603284 pybiocfilecache-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:27:27.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/src/pybiocfilecache/
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/BiocFileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/src/pybiocfilecache/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/db/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/data/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/data/test2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tox.ini
```

### Comparing `pybiocfilecache-0.3.0/.coveragerc` & `pybiocfilecache-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/.github/workflows/pypi-publish.yml` & `pybiocfilecache-0.3.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/.github/workflows/pypi-test.yml` & `pybiocfilecache-0.3.1/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/.gitignore` & `pybiocfilecache-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/.pre-commit-config.yaml` & `pybiocfilecache-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/CONTRIBUTING.rst` & `pybiocfilecache-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/LICENSE.txt` & `pybiocfilecache-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/PKG-INFO` & `pybiocfilecache-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.3.0
+Version: 0.3.1
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `pybiocfilecache-0.3.0/README.md` & `pybiocfilecache-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/docs/Makefile` & `pybiocfilecache-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/docs/conf.py` & `pybiocfilecache-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/docs/index.md` & `pybiocfilecache-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/docs/readme.md` & `pybiocfilecache-0.3.1/docs/readme.md`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/pyproject.toml` & `pybiocfilecache-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/setup.cfg` & `pybiocfilecache-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/setup.py` & `pybiocfilecache-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/PKG-INFO` & `pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.3.0
+Version: 0.3.1
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `pybiocfilecache-0.3.0/src/pyBiocFileCache.egg-info/SOURCES.txt` & `pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/src/pybiocfilecache/BiocFileCache.py` & `pybiocfilecache-0.3.1/src/pybiocfilecache/BiocFileCache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """Python Implementation of BiocFileCache."""
 
 import os
 from pathlib import Path
 from time import sleep, time
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 
+from ._exceptions import NoFpathError, RnameExistsError, RpathTimeoutError
 from .db import create_schema
 from .db.schema import Resource
 from .utils import copy_or_move, create_tmp_dir, generate_id
-from ._exceptions import NoFpathError, RnameExistsError, RpathTimeoutError
 
-__author__ = "jkanche"
+__author__ = "Jayaram Kancherla"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 class BiocFileCache:
     """Class to manage and cache files."""
 
     def __init__(self, cacheDirOrPath: Union[str, Path] = create_tmp_dir()):
         """Initialize BiocFileCache.
 
         Args:
-            cacheDirOrPath (Union[str, Path], optional): Path to cache.
-                directory. Defaults to tmp location, `create_tmp_dir()`.
+            cacheDirOrPath:
+                Path to cache directory.
+
+                Defaults to tmp location, :py:func:`~.utils.create_tmp_dir`.
 
         Raises:
             Exception: Failed to initialize cache.
         """
         if isinstance(cacheDirOrPath, str):
             cacheDirOrPath = Path(cacheDirOrPath)
 
@@ -47,46 +49,62 @@
         self.db_cache = f"{self.cache}/BiocFileCache.sqlite"
         (self.engine, self.sessionLocal) = create_schema(self.db_cache)
 
     def add(
         self,
         rname: str,
         fpath: Union[str, Path],
-        rtype: str = "local",
-        action: str = "copy",
+        rtype: Literal["local", "web", "relative"] = "local",
+        action: Literal["copy", "move", "asis"] = "copy",
         ext: bool = False,
     ) -> Resource:
         """Add a resource from the provided `fpath` to cache as `rname`.
 
         Args:
-            rname (str): Name of the resource to add to cache.
-            fpath (Union[str, Path]): Location of the resource.
-            rtype (str, optional): One of `"local"`, `"web"`, or `"relative"`.
-                Defaults to `"local"`.
-            action (str, optional): Either `"copy"`, `"move"` or `"asis"`.
-                Defaults to `"copy"`.
-            ext (bool, optional): Use filepath extension when storing in cache.
-                Defaults to `False`.
+            rname:
+                Name of the resource to add to cache.
 
-        Returns:
-            Resource: Database record of the new resource in cache.
+            fpath:
+                Location of the resource.
+
+            rtype:
+                One of ``local``, ``web``, or ``relative``.
+                Defaults to ``local``.
+
+            action:
+                Either ``copy``, ``move`` or ``asis``.
+                Defaults to ``copy``.
+
+            ext:
+                Whether to use filepath extension when storing in cache.
+                Defaults to `False`.
 
         Raises:
-            NoFpathError: When the `fpath` does not exist.
-            RnameExistsError: When the `rname` already exists in the cache.
-            sqlalchemy exceptions: When something is up with the cache.
+            NoFpathError:
+                When the `fpath` does not exist.
+
+            RnameExistsError:
+                When the `rname` already exists in the cache.
+                sqlalchemy exceptions: When something is up with the cache.
+
+        Returns:
+            Database record of the new resource in cache.
         """
         if isinstance(fpath, str):
             fpath = Path(fpath)
 
         if not fpath.exists():
-            raise NoFpathError(f"Resource at {fpath} does not exist.")
+            raise NoFpathError(f"Resource at '{fpath}' does not exist.")
 
         rid = generate_id()
-        rpath = f"{self.cache}/{rid}" + (f".{fpath.suffix}" if ext else "")
+        rpath = (
+            f"{self.cache}/{rid}" + (f".{fpath.suffix}" if ext else "")
+            if action != "asis"
+            else str(fpath)
+        )
 
         # create new record in the database
         res = Resource(
             **dict(
                 rid=rid,
                 rname=rname,
                 rpath=rpath,
@@ -119,36 +137,43 @@
 
         return res
 
     def query(self, query: str, field: str = "rname") -> List[Resource]:
         """Search cache for a resource.
 
         Args:
-            query (str): query or keywords to search.
-            field (str, optional): Field to search. Defaults to "rname".
+            query:
+                Query string or keywords to search.
+
+            field:
+                Field to search.
+                Defaults to "rname".
 
         Returns:
-            List[Resource]: list of matching resources from cache.
+            List of matching resources from cache.
         """
         with self.sessionLocal() as session:
             return (
                 session.query(Resource)
                 .filter(Resource[field].ilike("%{}%".format(query)))
                 .all()
             )
 
     def _get(self, session: Session, rname: str) -> Optional[Resource]:
         """Get a resource with `rname` from given `Session`.
 
         Args:
-            session (Session): The `Session` object to use.
-            rname (str): The `rname` of the `Resource` to get.
+            session:
+                The `Session` object to use.
+
+            rname:
+                The `rname` of the `Resource` to get.
 
         Returns:
-            (Resource, optional): The `Resource` for the `rname` if any.
+            The `Resource` for the `rname` if available.
         """
         resource: Optional[Resource] = (
             session.query(Resource).filter(Resource.rname == rname).first()
         )
 
         if resource is not None:
             # `Resource` may exist but `rpath` could still be being
@@ -165,26 +190,28 @@
 
         return resource
 
     def get(self, rname: str) -> Optional[Resource]:
         """Get resource by name from cache.
 
         Args:
-            rname (str): Name of the file to search.
+            rname:
+                Name of the file to search.
 
         Returns:
-            Optional[Resource]: matched resource from cache if exists.
+            Matched `Resource` from cache if exists.
         """
         return self._get(self.sessionLocal(), rname)
 
     def remove(self, rname: str) -> None:
         """Remove a resource from cache by name.
 
         Args:
-            rname (str): Name of the resource to remove.
+            rname:
+                Name of the resource to remove.
         """
         with self.sessionLocal() as session:
             res: Optional[Resource] = self._get(session, rname)
 
             if res is not None:
                 session.delete(res)
                 session.commit()
@@ -192,40 +219,56 @@
                 Path(res.rpath).unlink()
 
     def purge(self):
         """Remove all files from cache."""
         for file in os.scandir(self.cache):
             os.remove(file.path)
 
+        return True
+
     def update(
-        self, rname: str, fpath: Union[str, Path], action: str = "copy"
+        self,
+        rname: str,
+        fpath: Union[str, Path],
+        action: Literal["copy", "move", "asis"] = "copy",
     ) -> Resource:
         """Update a resource in cache.
 
         Args:
-            rname (str): name of the resource in cache.
-            fpath (Union[str, Path]): new resource to replace existing file in cache.
-            action (str, optional): either copy of move. defaults to copy.
+            rname:
+                Name of the resource in cache.
+
+            fpath:
+                New resource to replace existing file in cache.
+
+            action:
+                Either ``copy``, ``move`` or ``asis``.
+
+                Defaults to ``copy``.
 
         Returns:
-            Resource: Updated resource record in cache.
+            Updated resource record in cache.
         """
 
         if isinstance(fpath, str):
             fpath = Path(fpath)
 
         if not fpath.exists():
             raise Exception(f"File: '{fpath}' does not exist")
 
         with self.sessionLocal() as session:
             res = self._get(session, rname)
 
             if res is not None:
-                # copy the file to cache
-                copy_or_move(str(fpath), str(res.rpath), rname, action)
+                if action != "asis":
+                    # copy the file to cache
+                    copy_or_move(str(fpath), str(res.rpath), rname, action)
+                else:
+                    res.rpath = str(fpath)
+
                 res.access_time = res.last_modified_time = func.now()
                 session.merge(res)
                 session.commit()
                 session.refresh(res)
             else:
                 # technically an error since update shouldn't be called on
                 # non-existent resources in cache.
```

### Comparing `pybiocfilecache-0.3.0/src/pybiocfilecache/__init__.py` & `pybiocfilecache-0.3.1/src/pybiocfilecache/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/src/pybiocfilecache/db/Base.py` & `pybiocfilecache-0.3.1/src/pybiocfilecache/db/Base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from typing import Tuple
+
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 
 # from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import sessionmaker, declarative_base
-from typing import Tuple
+from sqlalchemy.orm import declarative_base, sessionmaker
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 Base = declarative_base()
 
 
 def create_schema(cache_dir: str) -> Tuple[Engine, sessionmaker]:
     """Create the schema in the sqlite database.
 
     Args:
-        cache_dir (str): Location where the cache directory
+        cache_dir:
+            Location where the cache directory.
 
     Returns:
-        a tuple of sqlalchemy engine and session maker
+        A tuple of sqlalchemy engine and session maker.
     """
     try:
         engine = create_engine(
             f"sqlite:///{cache_dir}", connect_args={"check_same_thread": False}
         )
 
         Base.metadata.create_all(bind=engine, checkfirst=True)
```

### Comparing `pybiocfilecache-0.3.0/src/pybiocfilecache/db/schema.py` & `pybiocfilecache-0.3.1/src/pybiocfilecache/db/schema.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.0/src/pybiocfilecache/utils.py` & `pybiocfilecache-0.3.1/src/pybiocfilecache/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,83 @@
+import logging
+import sys
 import tempfile
 import uuid
 from pathlib import Path
 from shutil import copy2, move
+from typing import Literal, Union
 
-from typing import Union
-import logging
-import sys
+__author__ = "Jayaram Kancherla"
+__copyright__ = "jkanche"
+__license__ = "MIT"
 
 
 def create_tmp_dir() -> str:
     """Create a temporary directory.
 
     Returns:
-        str: path to the directory
+        Temporary path to the directory.
     """
     return tempfile.mkdtemp()
 
 
 def generate_id() -> str:
     """Generate uuid.
 
     Returns:
-        str: unique string for use as id
+        Unique string for use as id.
     """
     return uuid.uuid4().hex
 
 
 def copy_or_move(
-    source: Union[str, Path], target: Union[str, Path], rname: str, action: str = "copy"
+    source: Union[str, Path],
+    target: Union[str, Path],
+    rname: str,
+    action: Literal["copy", "move", "asis"] = "copy",
 ) -> None:
-    """Copy or move a resource from `source` to `target`
+    """Copy or move a resource from ``source`` to ``target``.
 
     Args:
-        source (Union[str, Path]): source location of the resource to copy of move.
-        target (Union[str, Path]): destination to copy of move to.
-        rname (str): Name of resource to add to cache
-        action (str): copy of move file from source. Defaults to copy.
+        source:
+            Source location of the resource to copy of move.
+
+        target:
+            Destination to copy of move to.
+
+        rname:
+            Name of resource to add to cache.
+
+        action:
+            Copy of move file from source.
+            Defaults to copy.
 
     Raises:
-        ValueError: if action is not `copy` or `move`.
-        Exception: Error storing resource in the cache directory.
+        ValueError:
+            If action is not `copy`, `move` or `asis`.
+
+        Exception:
+            Error storing resource in the cache directory.
     """
 
-    if action not in ["copy", "move"]:
-        raise ValueError(f"Action must be either 'move' or 'copy', provided {action}")
+    if action not in ["copy", "move", "asis"]:
+        raise ValueError(
+            f"Action must be either 'move', 'copy' or 'asis', provided {action}."
+        )
 
     try:
         if action == "copy":
             copy2(source, target)
         elif action == "move":
             move(str(source), target)
+        elif action == "asis":
+            pass
     except Exception as e:
         raise Exception(
-            f"Error storing resource: '{rname}' from: '{source}' in '{target}'",
+            f"Error storing resource: '{rname}' from: '{source}' in '{target}'.",
         ) from e
 
 
 def setup_logging(loglevel):
     """Setup basic logging.
 
     Args:
```

### Comparing `pybiocfilecache-0.3.0/tests/test_cache.py` & `pybiocfilecache-0.3.1/tests/test_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
     frec1 = open(rec1.rpath, "r").read().strip()
     assert frec1 == "test1"
 
     frec2 = open(rec2.rpath, "r").read().strip()
     assert frec2 == "test2"
 
+    bfc.add("test3_asis", os.getcwd() + "/tests/data/test2.txt", action="asis")
+    rec3 = bfc.get("test3_asis")
+    assert rec3 is not None
+    assert rec3.rpath == os.getcwd() + "/tests/data/test2.txt"
+
+    frec3 = open(rec3.rpath, "r").read().strip()
+    assert frec3 == "test2"
+
     bfc.purge()
 
 
 def test_remove_operations():
     bfc = BiocFileCache(CACHE_DIR)
 
     bfc.add("test1", os.getcwd() + "/tests/data/test1.txt")
```

### Comparing `pybiocfilecache-0.3.0/tox.ini` & `pybiocfilecache-0.3.1/tox.ini`

 * *Files identical despite different names*

