# Comparing `tmp/brainglobe_workflows-1.1.5.tar.gz` & `tmp/brainglobe_workflows-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe_workflows-1.1.5.tar", last modified: Fri Apr 12 17:50:37 2024, max compression
+gzip compressed data, was "brainglobe_workflows-1.2.0.tar", last modified: Thu May 16 13:40:45 2024, max compression
```

## Comparing `brainglobe_workflows-1.1.5.tar` & `brainglobe_workflows-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.798472 brainglobe_workflows-1.1.5/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/benchmarks/cellfinder_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.798472 brainglobe_workflows-1.1.5/brainglobe_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/prep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/cellfinder_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/configs/cellfinder.json
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 17:50:37.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:50:35.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:45.412650 brainglobe_workflows-1.2.0/brainglobe_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8034 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/brainglobe_workflows/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/cellfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/cellfinder/cellfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/brainglobe_workflows/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/configs/cellfinder.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/brainglobe_workflows/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-05-16 13:40:44.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-16 13:40:45.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:40:44.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 13:40:44.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:40:43.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-16 13:40:44.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 13:40:44.000000 brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-16 13:40:36.000000 brainglobe_workflows-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:40:45.416650 brainglobe_workflows-1.2.0/setup.cfg
```

### Comparing `brainglobe_workflows-1.1.5/.gitignore` & `brainglobe_workflows-1.2.0/.gitignore`

 * *Files 22% similar despite different names*

```diff
@@ -124,11 +124,12 @@
 pip-wheel-metadata/
 
 # OS
 .DS_Store
 
 # written by setuptools_scm
 **/_version.py
-benchmarks/results/*
 
 # Benchmarking with ASV
-.asv/
+benchmarks/.asv/*
+benchmarks/results/*
+benchmarks/html/*
```

### Comparing `brainglobe_workflows-1.1.5/LICENSE` & `brainglobe_workflows-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe_workflows-1.1.5/PKG-INFO` & `brainglobe_workflows-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-workflows
-Version: 1.1.5
+Version: 1.2.0
 Summary: A collection of end-to-end data analysis workflows executed using BrainGlobe tools.
 Author: Christian Niedworok, Charly Rousseau
 Author-email: Adam Tyson <code@adamltyson.com>, BrainGlobe developers <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, BrainGlobe developers.
         All rights reserved.
@@ -52,15 +52,15 @@
 License-File: LICENSE
 Requires-Dist: brainglobe>=1.0.0
 Requires-Dist: brainreg>=1.0.0
 Requires-Dist: cellfinder>=1.1.0
 Requires-Dist: configobj
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: imio
-Requires-Dist: brainglobe-utils>=0.2.5
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: multiprocessing-logging>=0.3.4
 Requires-Dist: natsort
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: packaging
 Requires-Dist: pooch
 Requires-Dist: scikit-image
@@ -71,19 +71,14 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: coverage>=5.0.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: asv; extra == "dev"
-Requires-Dist: pooch; extra == "dev"
-Provides-Extra: asv-version
-Requires-Dist: asv; extra == "asv-version"
-Requires-Dist: pooch; extra == "asv-version"
-Requires-Dist: cellfinder-core; extra == "asv-version"
 Provides-Extra: napari
 Requires-Dist: napari[pyqt5]; extra == "napari"
 Requires-Dist: brainglobe-napari-io; extra == "napari"
 Requires-Dist: cellfinder[napari]>=1.0.0; extra == "napari"
 
 [![Python Version](https://img.shields.io/pypi/pyversions/brainglobe-workflows.svg)](https://pypi.org/project/brainglobe-workflows)
 [![PyPI](https://img.shields.io/pypi/v/brainglobe-workflows.svg)](https://pypi.org/project/brainglobe-workflows)
@@ -151,20 +146,23 @@
 Full documentation can be found [here](https://brainglobe.info/documentation/brainglobe-workflows/brainmapper/index.html).
 
 NOTE: The `brainmapper` workflow previously used the name "cellfinder", but this has been discontinued following the release of the [unified `cellfinder`](https://github.com/brainglobe/cellfinder) backend package to avoid conflation of terms.
 See our [blog post](https://brainglobe.info/blog/version1/cellfinder-core-and-plugin-merge.html) from the release for more information.
 
 ## Developer documentation
 
-This repository also includes workflow scripts that are benchmarked to support code development.
-These benchmarks are run regularly to ensure performance is stable, as the tools are developed and extended.
+This repository also includes code to benchmark typical workflows.
+These benchmarks are meant to be run regularly, to ensure performance is stable as the tools are developed and extended.
 
-- Developers can install these benchmarks locally via `pip install .[dev]`. By executing `asv run`, the benchmarks will run with default parameters on a small dataset that is downloaded from [GIN](https://gin.g-node.org/G-Node/info/wiki). See [the asv docs](https://asv.readthedocs.io/en/v0.6.1/using.html#running-benchmarks) for further details on how to run benchmarks.
-- Developers can also run these benchmarks on data they have stored locally, by specifying the relevant paths in an input (JSON) file.
-- We also maintain an internal runner that benchmarks the workflows over a large, exemplar dataset, of the scale we expect users to be handling. The result of these benchmarks are made publicly available.
+There are three main ways in which these benchmarks can be useful to developers:
+1. Developers can run the available benchmarks locally on a small test dataset.
+1. Developers can also run these benchmarks on data they have stored locally.
+1. We also plan to run the benchmarks on an internal runner using a larger dataset, of the scale we expect users to be handling. The result of these benchmarks will be made publicly available.
+
+For further details on how to run the benchmarks, see the [benchmarks README](benchmarks/README.md).
 
 Contributions to BrainGlobe are more than welcome.
 Please see the [developer guide](https://brainglobe.info/developers/index.html).
 
 ## Citing `brainglobe-workflows`
 
 **If you use any tools in the [brainglobe suite](https://brainglobe.info/documentation/index.html), please [let us know](mailto:code@adamltyson.com?subject=BrainGlobe), and we'd be happy to promote your paper/talk etc.**
```

### Comparing `brainglobe_workflows-1.1.5/README.md` & `brainglobe_workflows-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -64,20 +64,23 @@
 Full documentation can be found [here](https://brainglobe.info/documentation/brainglobe-workflows/brainmapper/index.html).
 
 NOTE: The `brainmapper` workflow previously used the name "cellfinder", but this has been discontinued following the release of the [unified `cellfinder`](https://github.com/brainglobe/cellfinder) backend package to avoid conflation of terms.
 See our [blog post](https://brainglobe.info/blog/version1/cellfinder-core-and-plugin-merge.html) from the release for more information.
 
 ## Developer documentation
 
-This repository also includes workflow scripts that are benchmarked to support code development.
-These benchmarks are run regularly to ensure performance is stable, as the tools are developed and extended.
+This repository also includes code to benchmark typical workflows.
+These benchmarks are meant to be run regularly, to ensure performance is stable as the tools are developed and extended.
 
-- Developers can install these benchmarks locally via `pip install .[dev]`. By executing `asv run`, the benchmarks will run with default parameters on a small dataset that is downloaded from [GIN](https://gin.g-node.org/G-Node/info/wiki). See [the asv docs](https://asv.readthedocs.io/en/v0.6.1/using.html#running-benchmarks) for further details on how to run benchmarks.
-- Developers can also run these benchmarks on data they have stored locally, by specifying the relevant paths in an input (JSON) file.
-- We also maintain an internal runner that benchmarks the workflows over a large, exemplar dataset, of the scale we expect users to be handling. The result of these benchmarks are made publicly available.
+There are three main ways in which these benchmarks can be useful to developers:
+1. Developers can run the available benchmarks locally on a small test dataset.
+1. Developers can also run these benchmarks on data they have stored locally.
+1. We also plan to run the benchmarks on an internal runner using a larger dataset, of the scale we expect users to be handling. The result of these benchmarks will be made publicly available.
+
+For further details on how to run the benchmarks, see the [benchmarks README](benchmarks/README.md).
 
 Contributions to BrainGlobe are more than welcome.
 Please see the [developer guide](https://brainglobe.info/developers/index.html).
 
 ## Citing `brainglobe-workflows`
 
 **If you use any tools in the [brainglobe suite](https://brainglobe.info/documentation/index.html), please [let us know](mailto:code@adamltyson.com?subject=BrainGlobe), and we'd be happy to promote your paper/talk etc.**
```

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/analyse.py` & `brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/analyse.py`

 * *Files identical despite different names*

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/main.py` & `brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import brainglobe_space as bgs
 import pandas as pd
 import tifffile
 from brainglobe_utils.cells.cells import MissingCellsError
 from brainglobe_utils.general.system import ensure_directory_exists
 from brainglobe_utils.image.heatmap import heatmap_from_points
 from brainglobe_utils.IO.cells import get_cells, save_cells
+from brainglobe_utils.IO.image.load import read_z_stack
 from cellfinder.core.main import suppress_tf_logging, tf_suppress_log_messages
 
 BRAINREG_PRE_PROCESSING_ARGS = None
 
 
 def get_downsampled_space(atlas, downsampled_image_path):
     target_shape = tifffile.imread(downsampled_image_path).shape
@@ -101,30 +102,29 @@
     )
 
 
 def run_all(args, what_to_run, atlas):
     from cellfinder.core.classify import classify
     from cellfinder.core.detect import detect
     from cellfinder.core.tools import prep
-    from cellfinder.core.tools.IO import read_with_dask
 
     from brainglobe_workflows.brainmapper import analyse
     from brainglobe_workflows.brainmapper.prep import (
         prep_candidate_detection,
         prep_channel_specific_general,
     )
 
     points = None
     signal_array = None
     args, what_to_run = prep_channel_specific_general(args, what_to_run)
 
     if what_to_run.detect:
         logging.info("Detecting cell candidates")
         args = prep_candidate_detection(args)
-        signal_array = read_with_dask(
+        signal_array = read_z_stack(
             args.signal_planes_paths[args.signal_channel]
         )
 
         points = detect.main(
             signal_array,
             args.start_plane,
             args.end_plane,
@@ -161,19 +161,19 @@
             args.model,
             args.n_free_cpus,
         )
         if what_to_run.classify:
             if points is None:
                 points = get_cells(args.paths.detected_points)
             if signal_array is None:
-                signal_array = read_with_dask(
+                signal_array = read_z_stack(
                     args.signal_planes_paths[args.signal_channel]
                 )
             logging.info("Running cell classification")
-            background_array = read_with_dask(args.background_planes_path[0])
+            background_array = read_z_stack(args.background_planes_path[0])
 
             points = classify.main(
                 points,
                 signal_array,
                 background_array,
                 args.n_free_cpus,
                 args.voxel_sizes,
```

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/parser.py` & `brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 
 from brainglobe_utils.general.numerical import (
     check_positive_float,
     check_positive_int,
 )
 from brainreg.core.cli import atlas_parse, geometry_parser, niftyreg_parse
 from brainreg.core.cli import backend_parse as brainreg_backend_parse
-from cellfinder.core.download.cli import (
-    download_directory_parser,
-    model_parser,
-)
+from cellfinder.core.download.cli import download_parser
 from cellfinder.core.tools.source_files import user_specific_configuration_path
 
 from brainglobe_workflows import __version__
 
 # TODO: Gradually move all paths as strings to Path objects
 
 models = {
@@ -61,17 +58,16 @@
     parser = pixel_parser(parser)
     parser = run_parse(parser)
     parser = io_parse(parser)
     parser = cell_detect_parse(parser)
     parser = classification_parse(parser)
     parser = cube_extract_parse(parser)
     parser = misc_parse(parser)
-    parser = model_parser(parser)
     parser = figures_parse(parser)
-    parser = download_directory_parser(parser)
+    parser = download_parser(parser)
 
     # brainreg options
     parser = atlas_parse(parser)
     parser = geometry_parser(parser)
     parser = brainreg_backend_parse(parser)
     # This needs to be abstracted away into brainreg for multiple backends
     parser = niftyreg_parse(parser)
```

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/prep.py` & `brainglobe_workflows-1.2.0/brainglobe_workflows/brainmapper/prep.py`

 * *Files identical despite different names*

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/cellfinder_core.py` & `brainglobe_workflows-1.2.0/brainglobe_workflows/cellfinder/cellfinder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """This script reproduces the most common cellfinder workflow
 
 It receives as an (optional) command line input the path to a configuration
 json file, that holds the values of the required parameters for the workflow.
 
+    python brainglobe_workflows/cellfinder.py --config path/to/config.json
+
 If no input json file is passed as a configuration, the default
 configuration defined at brainglobe_workflows/cellfinder/default_config.json
 is used.
 
-Example usage:
- - to pass a custom configuration, run (from the cellfinder_main.py
-   parent directory):
-    python cellfinder_core.py --config path/to/input/config.json
- - to use the default configuration, run
-    python cellfinder_core.py
-
+    python brainglobe_workflows/cellfinder.py
 
 """
 
 
 import datetime
 import json
 import logging
@@ -25,16 +21,16 @@
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Union
 
 import pooch
 from brainglobe_utils.IO.cells import save_cells
+from brainglobe_utils.IO.image.load import read_with_dask
 from cellfinder.core.main import main as cellfinder_run
-from cellfinder.core.tools.IO import read_with_dask
 from cellfinder.core.train.train_yml import depth_type
 
 from brainglobe_workflows.utils import (
     DEFAULT_JSON_CONFIG_PATH_CELLFINDER,
     config_parser,
     setup_logger,
 )
@@ -77,15 +73,15 @@
     cube_depth: int
     network_depth: depth_type
 
     # Optional parameters
 
     # install path: default path for downloaded and output data
     _install_path: Pathlike = (
-        Path.home() / ".brainglobe" / "workflows" / "cellfinder_core"
+        Path.home() / ".brainglobe" / "workflows" / "cellfinder"
     )
 
     # input data paths
     # Note: if not specified, the signal and background data
     # are assumed to be under "signal" and "background"
     # dirs under _install_path/cellfinder_test_data/
     # (see __post_init__ method)
@@ -433,31 +429,16 @@
 
     # run workflow
     run_workflow_from_cellfinder_run(cfg)  # only this will be benchmarked
 
     return cfg
 
 
-def main_app_wrapper():
-    """Parse command line arguments and
-    run cellfinder setup and workflow
-
-    This function is used to define an entry-point,
-    that allows the user to run the cellfinder workflow
-    for a given input config file as:
-    `cellfinder-workflow --config <path-to-input-config>`.
-
-    If no input config file is provided, the default is used.
-
-    """
+if __name__ == "__main__":
     # parse CLI arguments
     args = config_parser(
-        sys.argv[1:],  # sys.argv[0] is the script name
+        sys.argv[1:],
         str(DEFAULT_JSON_CONFIG_PATH_CELLFINDER),
     )
 
     # run setup and workflow
     _ = main(args.config)
-
-
-if __name__ == "__main__":
-    main_app_wrapper()
```

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/configs/cellfinder.json` & `brainglobe_workflows-1.2.0/brainglobe_workflows/configs/cellfinder.json`

 * *Files identical despite different names*

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows/utils.py` & `brainglobe_workflows-1.2.0/brainglobe_workflows/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # initialise argument parser
     parser = argparse.ArgumentParser(
         description=(
             """
             To launch the cellfinder workflow with default parameters, run:
                 `cellfinder-workflow`.
             The default parameters are those specifed in brainglobe_workflows/
-            cellfinder_core/configs/cellfinder.json.
+            cellfinder/configs/cellfinder.json.
 
 
             To launch the cellfinder workflow with a specific set of input
             parameters, run:
                 `cellfinder-workflow --config path/to/config.json`,
             where `path/to/input/config.json` is the json file with the
             desired parameters.
```

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/PKG-INFO` & `brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-workflows
-Version: 1.1.5
+Version: 1.2.0
 Summary: A collection of end-to-end data analysis workflows executed using BrainGlobe tools.
 Author: Christian Niedworok, Charly Rousseau
 Author-email: Adam Tyson <code@adamltyson.com>, BrainGlobe developers <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, BrainGlobe developers.
         All rights reserved.
@@ -52,15 +52,15 @@
 License-File: LICENSE
 Requires-Dist: brainglobe>=1.0.0
 Requires-Dist: brainreg>=1.0.0
 Requires-Dist: cellfinder>=1.1.0
 Requires-Dist: configobj
 Requires-Dist: fancylog>=0.0.7
 Requires-Dist: imio
-Requires-Dist: brainglobe-utils>=0.2.5
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: multiprocessing-logging>=0.3.4
 Requires-Dist: natsort
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: packaging
 Requires-Dist: pooch
 Requires-Dist: scikit-image
@@ -71,19 +71,14 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: coverage>=5.0.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: asv; extra == "dev"
-Requires-Dist: pooch; extra == "dev"
-Provides-Extra: asv-version
-Requires-Dist: asv; extra == "asv-version"
-Requires-Dist: pooch; extra == "asv-version"
-Requires-Dist: cellfinder-core; extra == "asv-version"
 Provides-Extra: napari
 Requires-Dist: napari[pyqt5]; extra == "napari"
 Requires-Dist: brainglobe-napari-io; extra == "napari"
 Requires-Dist: cellfinder[napari]>=1.0.0; extra == "napari"
 
 [![Python Version](https://img.shields.io/pypi/pyversions/brainglobe-workflows.svg)](https://pypi.org/project/brainglobe-workflows)
 [![PyPI](https://img.shields.io/pypi/v/brainglobe-workflows.svg)](https://pypi.org/project/brainglobe-workflows)
@@ -151,20 +146,23 @@
 Full documentation can be found [here](https://brainglobe.info/documentation/brainglobe-workflows/brainmapper/index.html).
 
 NOTE: The `brainmapper` workflow previously used the name "cellfinder", but this has been discontinued following the release of the [unified `cellfinder`](https://github.com/brainglobe/cellfinder) backend package to avoid conflation of terms.
 See our [blog post](https://brainglobe.info/blog/version1/cellfinder-core-and-plugin-merge.html) from the release for more information.
 
 ## Developer documentation
 
-This repository also includes workflow scripts that are benchmarked to support code development.
-These benchmarks are run regularly to ensure performance is stable, as the tools are developed and extended.
+This repository also includes code to benchmark typical workflows.
+These benchmarks are meant to be run regularly, to ensure performance is stable as the tools are developed and extended.
 
-- Developers can install these benchmarks locally via `pip install .[dev]`. By executing `asv run`, the benchmarks will run with default parameters on a small dataset that is downloaded from [GIN](https://gin.g-node.org/G-Node/info/wiki). See [the asv docs](https://asv.readthedocs.io/en/v0.6.1/using.html#running-benchmarks) for further details on how to run benchmarks.
-- Developers can also run these benchmarks on data they have stored locally, by specifying the relevant paths in an input (JSON) file.
-- We also maintain an internal runner that benchmarks the workflows over a large, exemplar dataset, of the scale we expect users to be handling. The result of these benchmarks are made publicly available.
+There are three main ways in which these benchmarks can be useful to developers:
+1. Developers can run the available benchmarks locally on a small test dataset.
+1. Developers can also run these benchmarks on data they have stored locally.
+1. We also plan to run the benchmarks on an internal runner using a larger dataset, of the scale we expect users to be handling. The result of these benchmarks will be made publicly available.
+
+For further details on how to run the benchmarks, see the [benchmarks README](benchmarks/README.md).
 
 Contributions to BrainGlobe are more than welcome.
 Please see the [developer guide](https://brainglobe.info/developers/index.html).
 
 ## Citing `brainglobe-workflows`
 
 **If you use any tools in the [brainglobe suite](https://brainglobe.info/documentation/index.html), please [let us know](mailto:code@adamltyson.com?subject=BrainGlobe), and we'd be happy to promote your paper/talk etc.**
```

### Comparing `brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/SOURCES.txt` & `brainglobe_workflows-1.2.0/brainglobe_workflows.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
-asv.conf.json
 pyproject.toml
-benchmarks/__init__.py
-benchmarks/cellfinder_core.py
 brainglobe_workflows/__init__.py
 brainglobe_workflows/utils.py
 brainglobe_workflows.egg-info/PKG-INFO
 brainglobe_workflows.egg-info/SOURCES.txt
 brainglobe_workflows.egg-info/dependency_links.txt
 brainglobe_workflows.egg-info/entry_points.txt
 brainglobe_workflows.egg-info/not-zip-safe
 brainglobe_workflows.egg-info/requires.txt
 brainglobe_workflows.egg-info/top_level.txt
 brainglobe_workflows/brainmapper/__init__.py
 brainglobe_workflows/brainmapper/analyse.py
 brainglobe_workflows/brainmapper/main.py
 brainglobe_workflows/brainmapper/parser.py
 brainglobe_workflows/brainmapper/prep.py
-brainglobe_workflows/cellfinder_core/__init__.py
-brainglobe_workflows/cellfinder_core/cellfinder_core.py
+brainglobe_workflows/cellfinder/__init__.py
+brainglobe_workflows/cellfinder/cellfinder.py
 brainglobe_workflows/configs/cellfinder.json
```

### Comparing `brainglobe_workflows-1.1.5/pyproject.toml` & `brainglobe_workflows-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 dependencies = [
     "brainglobe>=1.0.0",
     "brainreg>=1.0.0",
     "cellfinder>=1.1.0",
     "configobj",
     "fancylog>=0.0.7",
     "imio",
-    "brainglobe-utils>=0.2.5",
+    "brainglobe-utils>=0.5.0",
     "multiprocessing-logging>=0.3.4",
     "natsort",
     "numpy",
     "pandas",
     "packaging",
     "pooch",
     "scikit-image",
@@ -53,49 +53,39 @@
     "pytest-cov",
     "pytest",
     "gitpython",
     "coverage>=5.0.3",
     "pre-commit",
     "setuptools_scm",
     "asv",
-    "pooch",
 ]
-# Below, all the dependencies asv needs to run the benchmarks
-# (i.e., everything needed to install this package without the CLI tool)
-# Once the cellfinder CLI tool is deprecated, these will move to the
-# default dependencies.
-asv_version = ["asv", "pooch", "cellfinder-core"]
+
 
 napari = ["napari[pyqt5]", "brainglobe-napari-io", "cellfinder[napari]>=1.0.0"]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/brainglobe/brainglobe-workflows/issues"
 "Documentation" = "https://brainglobe.info/documentation/brainglobe-workflows"
 "Homepage" = "https://brainglobe.info"
 "Source Code" = "https://github.com/brainglobe/brainglobe-workflows"
 
 [project.scripts]
-cellfinder-workflow = "brainglobe_workflows.cellfinder_core.cellfinder_core:main_app_wrapper"
 brainmapper = "brainglobe_workflows.brainmapper.main:main"
 
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 
 [tool.setuptools.packages.find]
 include = ["brainglobe_workflows"]
-exclude = [
-    "tests",
-    "resources",
-    "benchmarks",
-]
+exclude = ["tests", "resources", "benchmarks"]
 
 [tool.black]
 target-version = ["py39", "py310"]
 skip-string-normalization = false
 line-length = 79
 ignore = ["*.yaml"]
 
@@ -109,14 +99,19 @@
 
 [tool.pytest.ini_options]
 addopts = "--cov=brainglobe-workflows"
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
 ]
+
+[tool.coverage.run]
+source = ["./*"]
+omit = ["benchmarks/*"]
+
 [tool.ruff]
 line-length = 79
 exclude = ["__init__.py", "build", ".eggs"]
 select = ["I", "E", "F"]
 fix = true
 
 [tool.setuptools_scm]
@@ -134,14 +129,18 @@
 
 [gh-actions:env]
 # This runs the coredev environment if the "coredev" github actions input
 # is set to "true"
 INPUT_COREDEV =
     true: coredev
 
+[coverage:run]
+source = ./*
+omit = benchmarks/*
+
 [testenv]
 extras =
     dev
 deps =
     coredev: git+https://github.com/brainglobe/cellfinder.git
 commands =
     pytest {toxinidir} -v --color=yes --cov=./ --cov-report=xml
```

