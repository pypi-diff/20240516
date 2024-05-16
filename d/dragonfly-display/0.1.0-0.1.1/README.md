# Comparing `tmp/dragonfly-display-0.1.0.tar.gz` & `tmp/dragonfly-display-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-display-0.1.0.tar", last modified: Wed Mar 20 18:49:34 2024, max compression
+gzip compressed data, was "dist/dragonfly-display-0.1.1.tar", last modified: Thu May 16 17:00:42 2024, max compression
```

## Comparing `dragonfly-display-0.1.0.tar` & `dragonfly-display-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/dragonfly_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/dragonfly_display/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/dragonfly_display/_extend_dragonfly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/dragonfly_display/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/dragonfly_display/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/dragonfly_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/extras-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:49:34.000000 dragonfly-display-0.1.0/tests/json/
--rw-r--r--   0 runner    (1001) docker     (127)   112149 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/tests/json/model_with_doors_skylights.dfjson
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-20 18:48:39.000000 dragonfly-display-0.1.0/tests/model_extend_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/dragonfly_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/dragonfly_display/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/dragonfly_display/_extend_dragonfly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/dragonfly_display/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/dragonfly_display/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/dragonfly_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/extras-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:00:42.000000 dragonfly-display-0.1.1/tests/json/
+-rw-r--r--   0 runner    (1001) docker     (127)   112149 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/tests/json/model_with_doors_skylights.dfjson
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-16 16:59:37.000000 dragonfly-display-0.1.1/tests/model_extend_test.py
```

### Comparing `dragonfly-display-0.1.0/.github/workflows/ci.yaml` & `dragonfly-display-0.1.1/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 jobs:
 
   test:
     name: Unit tests
     strategy:
       matrix:
-        python-version: ['3.7', '3.10']
+        python-version: ['3.10']
         os: [macos-latest, ubuntu-latest, windows-latest]
 
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v2
       - name: set up Python
         uses: actions/setup-python@v2
```

### Comparing `dragonfly-display-0.1.0/Dockerfile` & `dragonfly-display-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/LICENSE` & `dragonfly-display-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/PKG-INFO` & `dragonfly-display-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-display
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds methods to translate dragonfly objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/dragonfly-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dragonfly-display-0.1.0/README.md` & `dragonfly-display-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/deploy.sh` & `dragonfly-display-0.1.1/deploy.sh`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/dev-requirements.txt` & `dragonfly-display-0.1.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/docs/_static/custom.css` & `dragonfly-display-0.1.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/docs/_templates/layout.html` & `dragonfly-display-0.1.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/docs/conf.py` & `dragonfly-display-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/docs/index.rst` & `dragonfly-display-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/dragonfly_display/cli/__init__.py` & `dragonfly-display-0.1.1/dragonfly_display/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """dragonfly-display commands."""
 import click
 import sys
 import os
 import logging
 import json
 import pickle
+import tempfile
+import uuid
 
 from honeybee_display.attr import FaceAttribute, RoomAttribute
 
 from dragonfly.model import Model
 from dragonfly.cli import main
 
 
@@ -100,16 +102,15 @@
 @click.option(
     '--output-format', '-of', help='Text for the output format of the resulting '
     'VisualizationSet File (.vsf). Choose from: vsf, json, pkl, vtkjs, html. Note '
     'that both vsf and json refer to the the JSON version of the VisualizationSet '
     'file and the distinction between the two is only for help in coordinating file '
     'extensions (since both .vsf and .json can be acceptable). Also note that '
     'ladybug-vtk must be installed in order for the vtkjs or html options to be usable '
-    'and the html format refers to a web page with the vtkjs file embedded within it. '
-    'The vtkjs and html options also require an explicit --output-file to be specified.',
+    'and the html format refers to a web page with the vtkjs file embedded within it.',
     type=str, default='vsf', show_default=True)
 @click.option(
     '--output-file', help='Optional file to output the JSON string of '
     'the config object. By default, it will be printed out to stdout',
     type=click.File('w'), default='-', show_default=True)
 def model_to_vis_set(
         model_file, multiplier, no_ceil_adjacency,
@@ -154,30 +155,42 @@
         elif output_format == 'pkl':
             if output_file.name != '<stdout>':
                 out_folder, out_file = os.path.split(output_file.name)
                 vis_set.to_pkl(out_file, out_folder)
             else:
                 output_file.write(pickle.dumps(vis_set.to_dict()))
         elif output_format in ('vtkjs', 'html'):
-            assert output_file.name != '<stdout>', \
-                'Must specify an --output-file to use --output-format vtkjs.'
-            out_folder, out_file = os.path.split(output_file.name)
-            try:
+            if output_file.name == '<stdout>':  # get a temporary file
+                out_file = str(uuid.uuid4())[:6]
+                out_folder = tempfile.gettempdir()
+            else:
+                out_folder, out_file = os.path.split(output_file.name)
                 if out_file.endswith('.vtkjs'):
                     out_file = out_file[:-6]
                 elif out_file.endswith('.html'):
                     out_file = out_file[:-5]
+            try:
                 if output_format == 'vtkjs':
                     vis_set.to_vtkjs(output_folder=out_folder, file_name=out_file)
                 if output_format == 'html':
                     vis_set.to_html(output_folder=out_folder, file_name=out_file)
             except AttributeError as ae:
                 raise AttributeError(
                     'Ladybug-vtk must be installed in order to use --output-format '
                     'vtkjs.\n{}'.format(ae))
+            if output_file.name == '<stdout>':  # load file contents to stdout
+                out_file_ext = out_file + '.' + output_format
+                out_file_path = os.path.join(out_folder, out_file_ext)
+                if output_format == 'html':
+                    with open(out_file_path, encoding='utf-8') as of:
+                        f_contents = of.read()
+                else:  # vtkjs can only be read as binary
+                    with open(out_file_path, 'rb') as of:
+                        f_contents = of.read()
+                output_file.write(f_contents)
         else:
             raise ValueError('Unrecognized output-format "{}".'.format(output_format))
     except Exception as e:
         _logger.exception('Failed to translate Model to VisualizationSet.\n{}'.format(e))
         sys.exit(1)
     else:
         sys.exit(0)
```

### Comparing `dragonfly-display-0.1.0/dragonfly_display/model.py` & `dragonfly-display-0.1.1/dragonfly_display/model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/dragonfly_display.egg-info/PKG-INFO` & `dragonfly-display-0.1.1/dragonfly_display.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-display
-Version: 0.1.0
+Version: 0.1.1
 Summary: Adds methods to translate dragonfly objects to VisualizationSets.
 Home-page: https://github.com/ladybug-tools/dragonfly-display
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dragonfly-display-0.1.0/dragonfly_display.egg-info/SOURCES.txt` & `dragonfly-display-0.1.1/dragonfly_display.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/setup.py` & `dragonfly-display-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/tests/json/model_with_doors_skylights.dfjson` & `dragonfly-display-0.1.1/tests/json/model_with_doors_skylights.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-display-0.1.0/tests/model_extend_test.py` & `dragonfly-display-0.1.1/tests/model_extend_test.py`

 * *Files identical despite different names*

