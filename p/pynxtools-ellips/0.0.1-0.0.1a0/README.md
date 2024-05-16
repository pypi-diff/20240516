# Comparing `tmp/pynxtools_ellips-0.0.1.tar.gz` & `tmp/pynxtools_ellips-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools_ellips-0.0.1.tar", last modified: Fri May  3 12:21:20 2024, max compression
+gzip compressed data, was "pynxtools_ellips-0.0.1a0.tar", last modified: Thu May 16 09:39:42 2024, max compression
```

## Comparing `pynxtools_ellips-0.0.1.tar` & `pynxtools_ellips-0.0.1a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.470749 pynxtools_ellips-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.458750 pynxtools_ellips-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.462750 pynxtools_ellips-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.462750 pynxtools_ellips-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2024-05-03 12:21:20.470749 pynxtools_ellips-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.462750 pynxtools_ellips-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.462750 pynxtools_ellips-0.0.1/docs/explanation/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/explanation/appdefs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.462750 pynxtools_ellips-0.0.1/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/how-tos/dummy.md
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/macros.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.462750 pynxtools_ellips-0.0.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/reference/vase.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.466750 pynxtools_ellips-0.0.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.466750 pynxtools_ellips-0.0.1/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/docs/tutorial/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.466750 pynxtools_ellips-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   192360 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/examples/SiO2onSi.nxs
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/examples/eln_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   482497 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/examples/test-data.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/mkdocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.466750 pynxtools_ellips-0.0.1/pynxtools_ellips/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/pynxtools_ellips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/pynxtools_ellips/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/pynxtools_ellips/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.470749 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2024-05-03 12:21:20.000000 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 12:21:20.000000 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:21:20.000000 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 12:21:20.000000 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 12:21:20.000000 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 12:21:20.000000 pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:21:20.470749 pynxtools_ellips-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.466750 pynxtools_ellips-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:21:20.470749 pynxtools_ellips-0.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/tests/data/config_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/tests/data/eln_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   482497 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/tests/data/test-data.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-03 12:20:59.000000 pynxtools_ellips-0.0.1/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.192813 pynxtools_ellips-0.0.1a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.180813 pynxtools_ellips-0.0.1a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-16 09:39:42.192813 pynxtools_ellips-0.0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/docs/explanation/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/explanation/appdefs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/how-tos/dummy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/macros.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/reference/vase.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.184813 pynxtools_ellips-0.0.1a0/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/docs/tutorial/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.188813 pynxtools_ellips-0.0.1a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   192360 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/examples/SiO2onSi.nxs
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/examples/eln_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   482497 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/examples/test-data.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/mkdocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.188813 pynxtools_ellips-0.0.1a0/pynxtools_ellips/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.188813 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-16 09:39:42.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 09:39:42.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:39:42.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 09:39:42.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 09:39:42.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:39:42.000000 pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:39:42.192813 pynxtools_ellips-0.0.1a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.188813 pynxtools_ellips-0.0.1a0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:42.188813 pynxtools_ellips-0.0.1a0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/tests/data/config_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/tests/data/eln_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   482497 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/tests/data/test-data.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-16 09:39:36.000000 pynxtools_ellips-0.0.1a0/tests/test_reader.py
```

### Comparing `pynxtools_ellips-0.0.1/.github/workflows/build_docs.yml` & `pynxtools_ellips-0.0.1a0/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/.github/workflows/publish.yml` & `pynxtools_ellips-0.0.1a0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/.github/workflows/pylint.yml` & `pynxtools_ellips-0.0.1a0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/.github/workflows/pytest.yml` & `pynxtools_ellips-0.0.1a0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/.gitignore` & `pynxtools_ellips-0.0.1a0/.gitignore`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/LICENSE` & `pynxtools_ellips-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/PKG-INFO` & `pynxtools_ellips-0.0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-ellips
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: A reader for transferring ellipsometry data from vendor formats to NeXus and NOMAD.
 Author: The NOMAD Authors
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pynxtools_ellips-0.0.1/README.md` & `pynxtools_ellips-0.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/dev-requirements.txt` & `pynxtools_ellips-0.0.1a0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/docs/index.md` & `pynxtools_ellips-0.0.1a0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/docs/macros.py` & `pynxtools_ellips-0.0.1a0/docs/macros.py`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/docs/stylesheets/extra.css` & `pynxtools_ellips-0.0.1a0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/docs/tutorial/installation.md` & `pynxtools_ellips-0.0.1a0/docs/tutorial/installation.md`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/examples/README.md` & `pynxtools_ellips-0.0.1a0/examples/README.md`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/examples/SiO2onSi.nxs` & `pynxtools_ellips-0.0.1a0/examples/SiO2onSi.nxs`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/examples/eln_data.yaml` & `pynxtools_ellips-0.0.1a0/examples/eln_data.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,52 +3,54 @@
   data_software: WVASE
   data_software/@url: https://www.jawoollam.com/ellipsometry-software/wvase
   data_software/version: '3.882'
   data_type: Psi/Delta
   spectrum_type: wavelength
   spectrum_unit: angstrom
 Instrument:
-  Beam_path:
-    Detector:
-      count_time:
-        unit: s
-        value: 1.0
-      detector_type: CCD spectrometer
-    focussing_probes:
-      angular_spread:
-        unit: rad
-        value: 0.2
-      data_correction: false
-    light_source:
-      source_type: arc lamp
-    rotating_element:
-      revolutions: 50.0
+  Detector:
+    count_time:
+      unit: s
+      value: 1.0
+    detector_type: CCD spectrometer
+  focussing_probes:
+    angular_spread:
+      unit: rad
+      value: 0.2
+    data_correction: false
+  light_source:
+    source_type: arc lamp
+  rotating_element:
+    revolutions: 50.0
   Sample_stage:
     environment_conditions:
-      medium: air
     stage_type: manual stage
-  angle_of_incidence/@unit: degrees
-  calibration_status: no calibration
-  company: J. A. Woollam Co.
+#  angle_of_incidence/@unit: degrees
+  device_information:
+    vendor: J. A. Woollam Co.
+    model: RC2 (Vers. 0.0.1)
   ellipsometer_type: dual compensator
-  model: RC2
-  model/@version: 0.0.1
   rotating_element_type: compensator (source side)
-  software: CompleteEASE
-  software/@url: https://www.jawoollam.com/ellipsometry-software/completeease
-  software/version: '6.37'
+  software_RC2: CompleteEASE
+  software_RC2/@url: https://www.jawoollam.com/ellipsometry-software/completeease
+  software_RC2/@version: '6.37'
+  instrument_calibration_RC2:
+    calibration_status: no calibration
 Sample:
   atom_types: Si, O
   backside_roughness: false
   chemical_formula: SiO2
   layer_structure: 2nm SiO2 on Si
-  sample_history: Commercially purchased sample
   sample_name: 2nm SiO2 on Si
-  sample_type: multi layer
+  physical_form: multi layer
   substrate: Si
+  environment:
+    sample_medium: air
+  history:
+    notes: Commercially purchased sample
 User:
   address: Zum Großen Windkanal 2, 12489 Berlin, Germany
   affiliation: Humboldt-Universität zu Berlin
   email: surname.name@physik.hu-berlin.de
   name: Name Surname
 colnames:
 - type
@@ -56,14 +58,18 @@
 - angle_of_incidence
 - Psi
 - Delta
 - err.Psi
 - err.Delta
 derived_parameter_type: depolarization
 experiment_description: RC2 scan on 2nm SiO2 on Si in air
-experiment_identifier: exp-ID
-experiment_type: NIR-Vis-UV spectroscopic ellipsometry
+experiment_identifier:
+  identifier: exp-ID
+  is_persistent: "false"
+experiment_type: ellipsometry
+ellipsometry_experiment_type: NIR-Vis-UV spectroscopic ellipsometry
 filename: test-data.dat
 plot_name: Psi and Delta
+title: RC2 Ellipsometry of 2nm SiO2 on Si
 sep: \t
 skip: 3
-start_time: '2022-01-27T03:35:00+00:00'
+start_time: '2022-01-27T03:35:00+00:00'
```

### Comparing `pynxtools_ellips-0.0.1/examples/test-data.dat` & `pynxtools_ellips-0.0.1a0/examples/test-data.dat`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/mkdocs.yaml` & `pynxtools_ellips-0.0.1a0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/pynxtools_ellips/mock.py` & `pynxtools_ellips-0.0.1a0/pynxtools_ellips/mock.py`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/pynxtools_ellips/reader.py` & `pynxtools_ellips-0.0.1a0/pynxtools_ellips/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,31 +33,40 @@
 from pynxtools_ellips.mock import MockEllips
 
 DEFAULT_HEADER = {"sep": "\t", "skip": 0}
 
 
 CONVERT_DICT = {
     "unit": "@units",
-    "Beam_path": "BEAM_PATH[beam_path]",
     "Detector": "DETECTOR[detector]",
     "Data": "data_collection",
     "Derived_parameters": "derived_parameters",
     "Environment": "environment_conditions",
     "Instrument": "INSTRUMENT[instrument]",
     "Sample": "SAMPLE[sample]",
     "Sample_stage": "sample_stage",
     "User": "USER[user]",
     "Instrument/angle_of_incidence": "INSTRUMENT[instrument]/angle_of_incidence",
     "Instrument/angle_of_incidence/unit": "INSTRUMENT[instrument]/angle_of_incidence/@units",
     "column_names": "data_collection/column_names",
     "data_error": "data_collection/data_error",
     "depolarization": "derived_parameters/depolarization",
     "measured_data": "data_collection/measured_data",
-    "software": "software/program",
-    "data_software": "data_software/program",
+    "data_software": "software_TYPE[data_software]/program",
+    "experiment_identifier/identifier": "IDENTIFIER[experiment_identifier]/IDENTIFIER[identifier]",
+    "experiment_identifier/is_persistent": "IDENTIFIER[experiment_identifier]/IS_PERSISTENT[is_persistent]",
+    "software_RC2": "software_TYPE[software_RC2]/program",
+    "software_RC2/@url": "software_TYPE[software_RC2]/program/@url",
+    "software_RC2/@version": "software_TYPE[software_RC2]/program/@version",
+    "instrument_calibration_RC2": "instrument_calibration_DEVICE[instrument_calibration_RC2]/calibration_status",
+    "instrument_calibration_RC2/calibration_status": "instrument_calibration_DEVICE[instrument_calibration_RC2]/calibration_status",
+    "environment": "ENVIRONMENT[environment_sample]",
+    "history/notes": "HISTORY[history]/notes",
+    "light_source": "source_TYPE[source_light]",
+    "source_type": "type",
 }
 
 CONFIG_KEYS = [
     "colnames",
     "derived_parameter_type",
     "err-var",
     "filename",
@@ -66,16 +75,15 @@
     "sep",
     "skip",
     "spectrum_type",
     "spectrum_unit",
 ]
 
 REPLACE_NESTED = {
-    "Instrument/Beam_path": "INSTRUMENT[instrument]/BEAM_PATH[beam_path]",
-    "Env_Conditions": "INSTRUMENT[instrument]/sample_stage/environment_conditions",
+    "Inc_Det_Angles": "INSTRUMENT[instrument]",
     "Instrument": "INSTRUMENT[instrument]",
 }
 
 
 def load_header(filename, default):
     """load the yaml description file, and apply defaults from
     the defalut dict for all keys not found from the file.
@@ -343,23 +351,19 @@
         if spectrum_type not in header["colnames"]:
             print("ERROR: spectrum type not found in 'colnames'")
         header[f"data_collection/NAME_spectrum[{spectrum_type}_spectrum]"] = (
             whole_data[spectrum_type].to_numpy()[0 : counts[0]].astype("float64")
         )
 
         def write_scan_axis(name: str, values: list, units: str):
-            base_path = f"Env_Conditions/PARAMETER[{name}]"
-            header[f"{base_path}/values"] = values
-            header[f"{base_path}/values/@units"] = units
-            header[f"{base_path}/number_of_parameters"] = len(values)
-            header[f"{base_path}/number_of_parameters/@units"] = ""
-            header[f"{base_path}/parameter_type"] = name
+            base_path = f"Inc_Det_Angles/PARAMETER[{name}]"
+            header[f"{base_path}"] = values
+            header[f"{base_path}/@units"] = units
 
-        header["Instrument/angle_of_incidence"] = unique_angles
-        for axis in ["detection_angle", "incident_angle"]:
+        for axis in ["angle_of_detection", "angle_of_incidence"]:
             write_scan_axis(axis, unique_angles, "degree")
 
         # Create mocked ellipsometry data template:
         if is_mock:
             header, labels = mock_function(header)
 
         if "atom_types" not in header["Sample"]:
@@ -405,69 +409,75 @@
         else:
             spectrum_unit = header["Data"]["spectrum_unit"]
         # MK:: Carola, Ron, Flo, Tamas, Sandor refactor the above-mentioned construct
         # there has to be a unit parsing control logic already at the level of this reader
         # because test-data.data has improper units like Angstroms or degrees
         # the fix above prevents that these incorrect units are get just blindly carried
         # over into the nxs file and thus causing nomas to fail
-        template[f"/ENTRY[entry]/plot/AXISNAME[{spectrum_type}]"] = {
+        template[f"/ENTRY[entry]/data_collection/AXISNAME[{spectrum_type}]"] = {
             "link": f"/entry/data_collection/{spectrum_type}_spectrum"
         }
         template[
             f"/ENTRY[entry]/data_collection/NAME_spectrum[{spectrum_type}_spectrum]/@units"
         ] = spectrum_unit
         template[
             f"/ENTRY[entry]/data_collection/NAME_spectrum[{spectrum_type}_spectrum]/@long_name"
         ] = f"{spectrum_type} ({spectrum_unit})"
         plot_name = header["plot_name"]
         for dindx in range(0, len(labels.keys())):
             for index, key in enumerate(data_list[dindx]):
-                template[f"/ENTRY[entry]/plot/DATA[{key}]"] = {
+                template[f"/ENTRY[entry]/data_collection/DATA[{key}]"] = {
                     "link": "/entry/data_collection/measured_data",
                     "shape": np.index_exp[index, dindx, :],
                 }
                 # MK:: Carola, Ron, Flo, Tamas, Sandor refactor the following line
                 # using a proper unit parsing logic
-                template[f"/ENTRY[entry]/plot/DATA[{key}]/@units"] = "degree"
+                template[f"/ENTRY[entry]/data_collection/DATA[{key}]/@units"] = "degree"
                 if dindx == 0 and index == 0:
-                    template[f"/ENTRY[entry]/plot/DATA[{key}]/@long_name"] = (
-                        f"{plot_name} (degree)"
-                    )
-                template[f"/ENTRY[entry]/plot/DATA[{key}_errors]"] = {
+                    template[
+                        f"/ENTRY[entry]/data_collection/DATA[{key}]/@long_name"
+                    ] = f"{plot_name} (degree)"
+                template[f"/ENTRY[entry]/data_collection/DATA[{key}_errors]"] = {
                     "link": "/entry/data_collection/data_error",
                     "shape": np.index_exp[index, dindx, :],
                 }
                 # MK:: Carola, Ron, Flo, Tamas, Sandor refactor the following line
                 template[f"/ENTRY[entry]/plot/DATA[{key}_errors]/@units"] = "degree"
 
         # Define default plot showing Psi and Delta at all angles:
         template["/@default"] = "entry"
-        template["/ENTRY[entry]/@default"] = "plot"
-        template["/ENTRY[entry]/plot/@signal"] = f"{data_list[0][0]}"
-        template["/ENTRY[entry]/plot/@axes"] = spectrum_type
-        template["/ENTRY[entry]/plot/title"] = plot_name
+        template["/ENTRY[entry]/@default"] = "data_collection"
+        template["/ENTRY[entry]/data_collection/@signal"] = f"{data_list[0][0]}"
+        template["/ENTRY[entry]/data_collection/@axes"] = spectrum_type
+        template["/ENTRY[entry]/data_collection/title"] = plot_name
 
         # if len(data_list[0]) > 1:
-        template["/ENTRY[entry]/plot/@auxiliary_signals"] = data_list[0][1:]
+        template["/ENTRY[entry]/data_collection/@auxiliary_signals"] = data_list[0][1:]
         for index in range(1, len(data_list)):
-            template["/ENTRY[entry]/plot/@auxiliary_signals"] += data_list[index]
+            template["/ENTRY[entry]/data_collection/@auxiliary_signals"] += data_list[
+                index
+            ]
 
         template["/ENTRY[entry]/definition"] = "NXellipsometry"
         template["/ENTRY[entry]/definition/@url"] = (
             "https://github.com/FAIRmat-NFDI/nexus_definitions/"
             f"blob/{get_nexus_version_hash()}/contributed_definitions/NXellipsometry.nxdl.xml"
         )
         template["/ENTRY[entry]/definition/@version"] = get_nexus_version()
-        template["/ENTRY[entry]/program_name"] = "pynxtools"
+        template[
+            "/ENTRY[entry]/INSTRUMENT[instrument]/software_TYPE[software_NeXuS]/program"
+        ] = "pynxtools"
         try:
-            template["/ENTRY[entry]/program_name/@version"] = version("pynxtools")
+            template[
+                "/ENTRY[entry]/INSTRUMENT[instrument]/software_TYPE[software_NeXuS]/program/@version"
+            ] = version("pynxtools")
         except PackageNotFoundError:
             pass
-        template["/ENTRY[entry]/program_name/@url"] = (
-            "https://github.com/FAIRmat-NFDI/pynxtools"
-        )
+        template[
+            "/ENTRY[entry]/INSTRUMENT[instrument]/software_TYPE[software_NeXuS]/program/@url"
+        ] = "https://github.com/FAIRmat-NFDI/pynxtools"
 
         return template
 
 
 # This has to be set to allow the convert script to use this reader. Set it to "MyDataReader".
 READER = EllipsometryReader
```

### Comparing `pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/PKG-INFO` & `pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-ellips
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: A reader for transferring ellipsometry data from vendor formats to NeXus and NOMAD.
 Author: The NOMAD Authors
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pynxtools_ellips-0.0.1/pynxtools_ellips.egg-info/SOURCES.txt` & `pynxtools_ellips-0.0.1a0/pynxtools_ellips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/pyproject.toml` & `pynxtools_ellips-0.0.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pynxtools>=0.2.1"
 ]
 
 [project.entry-points."pynxtools.reader"]
-ellips = "pynxtools_ellips.reader:ELLIPSReader"
+ellips = "pynxtools_ellips.reader:EllipsometryReader"
 
 [project.urls]
 "Homepage" = "https://github.com/FAIRmat-NFDI/pynxtools-ellips"
 "Bug Tracker" = "https://github.com/FAIRmat-NFDI/pynxtools-ellips/issues"
 [project.optional-dependencies]
 dev = [
     "mypy",
```

### Comparing `pynxtools_ellips-0.0.1/tests/data/eln_data.yaml` & `pynxtools_ellips-0.0.1a0/tests/data/eln_data.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -3,52 +3,54 @@
   data_software: WVASE
   data_software/@url: https://www.jawoollam.com/ellipsometry-software/wvase
   data_software/version: '3.882'
   data_type: Psi/Delta
   spectrum_type: wavelength
   spectrum_unit: angstrom
 Instrument:
-  Beam_path:
-    Detector:
-      count_time:
-        unit: s
-        value: 1.0
-      detector_type: CCD spectrometer
-    focussing_probes:
-      angular_spread:
-        unit: rad
-        value: 0.2
-      data_correction: false
-    light_source:
-      source_type: arc lamp
-    rotating_element:
-      revolutions: 50.0
+  Detector:
+    count_time:
+      unit: s
+      value: 1.0
+    detector_type: CCD spectrometer
+  focussing_probes:
+    angular_spread:
+      unit: rad
+      value: 0.2
+    data_correction: false
+  light_source:
+    source_type: arc lamp
+  rotating_element:
+    revolutions: 50.0
   Sample_stage:
     environment_conditions:
-      medium: air
     stage_type: manual stage
-  angle_of_incidence/@unit: degrees
-  calibration_status: no calibration
-  company: J. A. Woollam Co.
+#  angle_of_incidence/@unit: degrees
+  device_information:
+    vendor: J. A. Woollam Co.
+    model: RC2 (Vers. 0.0.1)
   ellipsometer_type: dual compensator
-  model: RC2
-  model/@version: 0.0.1
   rotating_element_type: compensator (source side)
-  software: CompleteEASE
-  software/@url: https://www.jawoollam.com/ellipsometry-software/completeease
-  software/version: '6.37'
+  software_RC2: CompleteEASE
+  software_RC2/@url: https://www.jawoollam.com/ellipsometry-software/completeease
+  software_RC2/@version: '6.37'
+  instrument_calibration_RC2:
+    calibration_status: no calibration
 Sample:
   atom_types: Si, O
   backside_roughness: false
   chemical_formula: SiO2
   layer_structure: 2nm SiO2 on Si
-  sample_history: Commercially purchased sample
   sample_name: 2nm SiO2 on Si
-  sample_type: multi layer
+  physical_form: multi layer
   substrate: Si
+  environment:
+    sample_medium: air
+  history:
+    notes: Commercially purchased sample
 User:
   address: Zum Großen Windkanal 2, 12489 Berlin, Germany
   affiliation: Humboldt-Universität zu Berlin
   email: surname.name@physik.hu-berlin.de
   name: Name Surname
 colnames:
 - type
@@ -56,14 +58,18 @@
 - angle_of_incidence
 - Psi
 - Delta
 - err.Psi
 - err.Delta
 derived_parameter_type: depolarization
 experiment_description: RC2 scan on 2nm SiO2 on Si in air
-experiment_identifier: exp-ID
-experiment_type: NIR-Vis-UV spectroscopic ellipsometry
+experiment_identifier:
+  identifier: exp-ID
+  is_persistent: "false"
+experiment_type: ellipsometry
+ellipsometry_experiment_type: NIR-Vis-UV spectroscopic ellipsometry
 filename: test-data.dat
 plot_name: Psi and Delta
+title: RC2 Ellipsometry of 2nm SiO2 on Si
 sep: \t
 skip: 3
-start_time: '2022-01-27T03:35:00+00:00'
+start_time: '2022-01-27T03:35:00+00:00'
```

### Comparing `pynxtools_ellips-0.0.1/tests/data/test-data.dat` & `pynxtools_ellips-0.0.1a0/tests/data/test-data.dat`

 * *Files identical despite different names*

### Comparing `pynxtools_ellips-0.0.1/tests/test_reader.py` & `pynxtools_ellips-0.0.1a0/tests/test_reader.py`

 * *Files identical despite different names*

