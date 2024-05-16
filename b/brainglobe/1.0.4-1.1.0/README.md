# Comparing `tmp/brainglobe-1.0.4.tar.gz` & `tmp/brainglobe-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-1.0.4.tar", last modified: Tue Mar 26 12:01:11 2024, max compression
+gzip compressed data, was "brainglobe-1.1.0.tar", last modified: Thu May 16 13:04:16 2024, max compression
```

## Comparing `brainglobe-1.0.4.tar` & `brainglobe-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.355213 brainglobe-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.347213 brainglobe-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.351213 brainglobe-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-26 12:01:06.000000 brainglobe-1.0.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-26 12:01:06.000000 brainglobe-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-26 12:01:06.000000 brainglobe-1.0.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-26 12:01:06.000000 brainglobe-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-26 12:01:06.000000 brainglobe-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-03-26 12:01:11.355213 brainglobe-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-26 12:01:06.000000 brainglobe-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.351213 brainglobe-1.0.4/brainglobe/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-26 12:01:06.000000 brainglobe-1.0.4/brainglobe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.351213 brainglobe-1.0.4/brainglobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-03-26 12:01:11.000000 brainglobe-1.0.4/brainglobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-26 12:01:11.000000 brainglobe-1.0.4/brainglobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:01:11.000000 brainglobe-1.0.4/brainglobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-26 12:01:11.000000 brainglobe-1.0.4/brainglobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 12:01:11.000000 brainglobe-1.0.4/brainglobe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-26 12:01:06.000000 brainglobe-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 12:01:11.355213 brainglobe-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.351213 brainglobe-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:06.000000 brainglobe-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.351213 brainglobe-1.0.4/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:06.000000 brainglobe-1.0.4/tests/test_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:11.351213 brainglobe-1.0.4/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:01:06.000000 brainglobe-1.0.4/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-26 12:01:06.000000 brainglobe-1.0.4/tests/test_unit/test__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.357892 brainglobe-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.349892 brainglobe-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.353892 brainglobe-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-16 13:04:12.000000 brainglobe-1.1.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-16 13:04:12.000000 brainglobe-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 13:04:12.000000 brainglobe-1.1.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-16 13:04:12.000000 brainglobe-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-16 13:04:12.000000 brainglobe-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-16 13:04:16.357892 brainglobe-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-16 13:04:12.000000 brainglobe-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.353892 brainglobe-1.1.0/brainglobe/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 13:04:12.000000 brainglobe-1.1.0/brainglobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.353892 brainglobe-1.1.0/brainglobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-16 13:04:16.000000 brainglobe-1.1.0/brainglobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-16 13:04:16.000000 brainglobe-1.1.0/brainglobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:04:16.000000 brainglobe-1.1.0/brainglobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 13:04:16.000000 brainglobe-1.1.0/brainglobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 13:04:16.000000 brainglobe-1.1.0/brainglobe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-16 13:04:12.000000 brainglobe-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:04:16.357892 brainglobe-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.353892 brainglobe-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:12.000000 brainglobe-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.353892 brainglobe-1.1.0/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:12.000000 brainglobe-1.1.0/tests/test_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:16.353892 brainglobe-1.1.0/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:04:12.000000 brainglobe-1.1.0/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 13:04:12.000000 brainglobe-1.1.0/tests/test_unit/test__version__.py
```

### Comparing `brainglobe-1.0.4/.github/workflows/test_and_deploy.yml` & `brainglobe-1.1.0/.github/workflows/test_and_deploy.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,24 +38,30 @@
     strategy:
       matrix:
         # Run all supported Python versions on linux
         python-version: ["3.9", "3.10"]
         os: [ubuntu-latest]
         # Include one windows and macos run
         include:
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
+          python-version: "3.10"
+        - os: macos-latest # ARM Mac
           python-version: "3.10"
         - os: windows-latest
           python-version: "3.10"
 
     steps:
       # Run tests
+      - name: install HDF5 libs on ARM Mac
+        if: matrix.os == 'macos-latest'
+        run: brew install hdf5
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
 
   build_sdist_wheels:
     name: Build source distribution
     needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
```

### Comparing `brainglobe-1.0.4/.gitignore` & `brainglobe-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-1.0.4/CITATION.cff` & `brainglobe-1.1.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainglobe-1.0.4/LICENSE` & `brainglobe-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-1.0.4/PKG-INFO` & `brainglobe-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe
-Version: 1.0.4
+Version: 1.1.0
 Summary: Python-based tools for computational neuroanatomy.
 Author-email: BrainGlobe Developers <hello@brainglobe.info>
 License: BSD-3-Clause
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-meta/issues
 Project-URL: documentation, https://docs.brainglobe.info
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-meta
@@ -16,24 +16,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: brainglobe-atlasapi<3,>=2.0.1
+Requires-Dist: brainglobe-atlasapi<3,>=2.0.6
 Requires-Dist: brainglobe-heatmap<1,>=0.5.2
 Requires-Dist: brainglobe-napari-io<1,>=0.3.4
 Requires-Dist: brainglobe-segmentation<2,>=1.2.3
-Requires-Dist: brainglobe-space<2,>=1.0.0
-Requires-Dist: brainglobe-utils<1,>=0.4.2
-Requires-Dist: brainreg[napari]<2,>=1.0.7
+Requires-Dist: brainglobe-space<2,>=1.0.2
+Requires-Dist: brainglobe-utils<1,>=0.5.0
+Requires-Dist: brainreg[napari]<2,>=1.0.9
 Requires-Dist: brainrender-napari<1,>=0.0.3
-Requires-Dist: brainrender<3,>=2.1.6
-Requires-Dist: cellfinder[napari]<2,>=1.1.1
+Requires-Dist: brainrender<3,>=2.1.9
+Requires-Dist: cellfinder[napari]<2,>=1.2.0
 Requires-Dist: napari[all]
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: black; extra == "dev"
```

### Comparing `brainglobe-1.0.4/README.md` & `brainglobe-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-1.0.4/brainglobe.egg-info/PKG-INFO` & `brainglobe-1.1.0/brainglobe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe
-Version: 1.0.4
+Version: 1.1.0
 Summary: Python-based tools for computational neuroanatomy.
 Author-email: BrainGlobe Developers <hello@brainglobe.info>
 License: BSD-3-Clause
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-meta/issues
 Project-URL: documentation, https://docs.brainglobe.info
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-meta
@@ -16,24 +16,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: brainglobe-atlasapi<3,>=2.0.1
+Requires-Dist: brainglobe-atlasapi<3,>=2.0.6
 Requires-Dist: brainglobe-heatmap<1,>=0.5.2
 Requires-Dist: brainglobe-napari-io<1,>=0.3.4
 Requires-Dist: brainglobe-segmentation<2,>=1.2.3
-Requires-Dist: brainglobe-space<2,>=1.0.0
-Requires-Dist: brainglobe-utils<1,>=0.4.2
-Requires-Dist: brainreg[napari]<2,>=1.0.7
+Requires-Dist: brainglobe-space<2,>=1.0.2
+Requires-Dist: brainglobe-utils<1,>=0.5.0
+Requires-Dist: brainreg[napari]<2,>=1.0.9
 Requires-Dist: brainrender-napari<1,>=0.0.3
-Requires-Dist: brainrender<3,>=2.1.6
-Requires-Dist: cellfinder[napari]<2,>=1.1.1
+Requires-Dist: brainrender<3,>=2.1.9
+Requires-Dist: cellfinder[napari]<2,>=1.2.0
 Requires-Dist: napari[all]
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: black; extra == "dev"
```

### Comparing `brainglobe-1.0.4/pyproject.toml` & `brainglobe-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Operating System :: OS Independent",
   "License :: OSI Approved :: BSD License",
 ]
 
 dependencies = [
-  "brainglobe-atlasapi>=2.0.1,<3",
+  "brainglobe-atlasapi>=2.0.6,<3",
   "brainglobe-heatmap>=0.5.2,<1",
   "brainglobe-napari-io>=0.3.4,<1",
   "brainglobe-segmentation>=1.2.3,<2",
-  "brainglobe-space>=1.0.0,<2",
-  "brainglobe-utils>=0.4.2,<1",
-  "brainreg[napari]>=1.0.7,<2",
+  "brainglobe-space>=1.0.2,<2",
+  "brainglobe-utils>=0.5.0,<1",
+  "brainreg[napari]>=1.0.9,<2",
   "brainrender-napari>=0.0.3,<1",
-  "brainrender>=2.1.6,<3",
-  "cellfinder[napari]>=1.1.1,<2",
+  "brainrender>=2.1.9,<3",
+  "cellfinder[napari]>=1.2.0,<2",
   "napari[all]",
   # brainglobe-napari [WIP],
 ]
 
 [project.optional-dependencies]
 dev = [
   "pytest",
```

