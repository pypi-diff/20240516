# Comparing `tmp/aimsim-2.2.0.tar.gz` & `tmp/aimsim-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsim-2.2.0.tar", last modified: Mon Apr 15 16:35:26 2024, max compression
+gzip compressed data, was "aimsim-2.2.1.tar", last modified: Thu May 16 21:45:44 2024, max compression
```

## Comparing `aimsim-2.2.0.tar` & `aimsim-2.2.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.919880 aimsim-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-04-15 16:35:23.000000 aimsim-2.2.0/AIMSim-GUI.png
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 16:35:23.000000 aimsim-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 16:35:23.000000 aimsim-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-04-15 16:35:26.919880 aimsim-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-15 16:35:23.000000 aimsim-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.907880 aimsim-2.2.0/aimsim/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.907880 aimsim-2.2.0/aimsim/chemical_datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/chemical_datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/chemical_datastructures/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    48544 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/chemical_datastructures/molecule_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.907880 aimsim-2.2.0/aimsim/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    75466 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    63184 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/ops/similarity_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/aimsim/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/cluster_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/compare_target_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/extended_similarity_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/identify_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/measure_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/see_property_variation_with_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/tasks/visualize_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/aimsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/utils/ccbmlib_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-04-15 16:35:23.000000 aimsim-2.2.0/aimsim/utils/plotting_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.919880 aimsim-2.2.0/aimsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 16:35:26.000000 aimsim-2.2.0/aimsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:35:23.000000 aimsim-2.2.0/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.903880 aimsim-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_images/AIMSim-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_images/sulfonamide-substrate-scope.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/_static/plus.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.903880 aimsim-2.2.0/docs/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/interfaces/UI/
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/interfaces/UI/AIMSim-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.911881 aimsim-2.2.0/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim-2.2.0/docs/tests/sulfonamide-substrate-scope.png
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-15 16:35:23.000000 aimsim-2.2.0/implemented_metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/interfaces/UI/
--rw-r--r--   0 runner    (1001) docker     (127)    31374 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/AIMSim-GUI-corner-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/AIMSim-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/AIMSim_ui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/interfaces/UI/libraries/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/UI/libraries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-15 16:35:23.000000 aimsim-2.2.0/interfaces/config_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-15 16:35:23.000000 aimsim-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 16:35:23.000000 aimsim-2.2.0/requirements_core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:35:26.919880 aimsim-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-15 16:35:23.000000 aimsim-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.915881 aimsim-2.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:26.919880 aimsim-2.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/sulfonamide-substrate-scope-PDF.png
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/sulfonamide-substrate-scope.png
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_CompareTargetMolecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_Descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_LoadingErrorException.py
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_MeasureSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_Molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    52891 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_MoleculeSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_SimilarityMeasure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_SimilarityMeasureValueErrors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_ToolTip.py
--rw-r--r--   0 runner    (1001) docker     (127)    66192 2024-04-15 16:35:23.000000 aimsim-2.2.0/tests/test_multithreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.849737 aimsim-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-05-16 21:45:41.000000 aimsim-2.2.1/AIMSim-GUI.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 21:45:41.000000 aimsim-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 21:45:41.000000 aimsim-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-16 21:45:44.849737 aimsim-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-05-16 21:45:41.000000 aimsim-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.841737 aimsim-2.2.1/aimsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.841737 aimsim-2.2.1/aimsim/chemical_datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/chemical_datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/chemical_datastructures/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48544 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/chemical_datastructures/molecule_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.841737 aimsim-2.2.1/aimsim/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/ops/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75466 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/ops/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63184 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/ops/similarity_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/aimsim/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/cluster_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/compare_target_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/extended_similarity_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/identify_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/measure_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/see_property_variation_with_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/tasks/visualize_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/aimsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/utils/ccbmlib_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-05-16 21:45:41.000000 aimsim-2.2.1/aimsim/utils/plotting_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.849737 aimsim-2.2.1/aimsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-16 21:45:44.000000 aimsim-2.2.1/aimsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-16 21:45:44.000000 aimsim-2.2.1/aimsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:45:44.000000 aimsim-2.2.1/aimsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 21:45:44.000000 aimsim-2.2.1/aimsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 21:45:44.000000 aimsim-2.2.1/aimsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 21:45:44.000000 aimsim-2.2.1/aimsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-16 21:45:41.000000 aimsim-2.2.1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.837737 aimsim-2.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/_images/AIMSim-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/_images/sulfonamide-substrate-scope.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/_static/plus.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.837737 aimsim-2.2.1/docs/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/docs/interfaces/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/interfaces/UI/AIMSim-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-05-16 21:45:41.000000 aimsim-2.2.1/docs/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-16 21:45:41.000000 aimsim-2.2.1/implemented_metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.845737 aimsim-2.2.1/interfaces/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)    31374 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/UI/AIMSim-GUI-corner-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/UI/AIMSim-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/UI/AIMSim_ui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/UI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.849737 aimsim-2.2.1/interfaces/UI/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/UI/libraries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-16 21:45:41.000000 aimsim-2.2.1/interfaces/config_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-16 21:45:41.000000 aimsim-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 21:45:41.000000 aimsim-2.2.1/requirements_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:45:44.849737 aimsim-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-16 21:45:41.000000 aimsim-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.849737 aimsim-2.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:44.849737 aimsim-2.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/sulfonamide-substrate-scope-PDF.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_CompareTargetMolecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_Descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_LoadingErrorException.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_MeasureSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_Molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52891 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_MoleculeSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_SimilarityMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_SimilarityMeasureValueErrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_ToolTip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66192 2024-05-16 21:45:41.000000 aimsim-2.2.1/tests/test_multithreading.py
```

### Comparing `aimsim-2.2.0/AIMSim-GUI.png` & `aimsim-2.2.1/AIMSim-GUI.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/LICENSE` & `aimsim-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/PKG-INFO` & `aimsim-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsim
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python command line and GUI tool to analyze molecular similarity.
 Home-page: https://github.com/VlachosGroup/AIMSim
 Author: Himaghna Bhattacharjee, Jackson Burns
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `aimsim-2.2.0/README.md` & `aimsim-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/chemical_datastructures/molecule.py` & `aimsim-2.2.1/aimsim/chemical_datastructures/molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/chemical_datastructures/molecule_set.py` & `aimsim-2.2.1/aimsim/chemical_datastructures/molecule_set.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/exceptions.py` & `aimsim-2.2.1/aimsim/exceptions.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/ops/clustering.py` & `aimsim-2.2.1/aimsim/ops/clustering.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/ops/descriptor.py` & `aimsim-2.2.1/aimsim/ops/descriptor.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/ops/similarity_measures.py` & `aimsim-2.2.1/aimsim/ops/similarity_measures.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/cluster_data.py` & `aimsim-2.2.1/aimsim/tasks/cluster_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Data clustering task."""
 from os import makedirs
 from os.path import dirname
 
 import matplotlib.pyplot as plt
+try:
+    from matplotlib.cm import get_cmap
+except:  # noqa: E722
+    from matplotlib.pyplot import get_cmap
 from matplotlib.colors import rgb2hex
 import yaml
 
 from .task import Task
 from aimsim.exceptions import InvalidConfigurationError
 from aimsim.utils.plotting_scripts import plot_barchart, plot_density
 from aimsim.utils.plotting_scripts import plot_scatter_interactive
@@ -50,15 +54,15 @@
 
     def _extract_configs(self):
         self.n_clusters = self.configs["n_clusters"]
         self.clustering_method = self.configs.get("clustering_method", None)
         self.plot_settings = dict()
         self.plot_settings["cluster_plot"] = {
             "cluster_colors": [
-                rgb2hex(plt.cm.get_cmap("tab20", self.n_clusters)(cluster_id))
+                rgb2hex(get_cmap("tab20", self.n_clusters)(cluster_id))
                 for cluster_id in range(self.n_clusters)],
             "response": "Response",
         }
 
         self.plot_settings["cluster_plot"].update(
             self.configs.get("cluster_plot_settings", {}))
         self.plot_settings["embedding_plot"] = {
```

### Comparing `aimsim-2.2.0/aimsim/tasks/compare_target_molecule.py` & `aimsim-2.2.1/aimsim/tasks/compare_target_molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/extended_similarity_indices.py` & `aimsim-2.2.1/aimsim/tasks/extended_similarity_indices.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/identify_outliers.py` & `aimsim-2.2.1/aimsim/tasks/identify_outliers.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/measure_search.py` & `aimsim-2.2.1/aimsim/tasks/measure_search.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/see_property_variation_with_similarity.py` & `aimsim-2.2.1/aimsim/tasks/see_property_variation_with_similarity.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/task_manager.py` & `aimsim-2.2.1/aimsim/tasks/task_manager.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/tasks/visualize_dataset.py` & `aimsim-2.2.1/aimsim/tasks/visualize_dataset.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/utils/ccbmlib_fingerprints.py` & `aimsim-2.2.1/aimsim/utils/ccbmlib_fingerprints.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim/utils/plotting_scripts.py` & `aimsim-2.2.1/aimsim/utils/plotting_scripts.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/aimsim.egg-info/PKG-INFO` & `aimsim-2.2.1/aimsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsim
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python command line and GUI tool to analyze molecular similarity.
 Home-page: https://github.com/VlachosGroup/AIMSim
 Author: Himaghna Bhattacharjee, Jackson Burns
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `aimsim-2.2.0/aimsim.egg-info/SOURCES.txt` & `aimsim-2.2.1/aimsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/config.yaml` & `aimsim-2.2.1/config.yaml`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/docs/_images/AIMSim-logo.png` & `aimsim-2.2.1/docs/_images/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/docs/_images/sulfonamide-substrate-scope.png` & `aimsim-2.2.1/docs/_images/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/docs/interfaces/UI/AIMSim-logo.png` & `aimsim-2.2.1/docs/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/docs/tests/sulfonamide-substrate-scope.png` & `aimsim-2.2.1/docs/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/implemented_metrics.md` & `aimsim-2.2.1/implemented_metrics.md`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/interfaces/UI/AIMSim-GUI-corner-logo.png` & `aimsim-2.2.1/interfaces/UI/AIMSim-GUI-corner-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/interfaces/UI/AIMSim-logo.png` & `aimsim-2.2.1/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/interfaces/UI/AIMSim_ui_main.py` & `aimsim-2.2.1/interfaces/UI/AIMSim_ui_main.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/interfaces/config_reader.py` & `aimsim-2.2.1/interfaces/config_reader.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/setup.py` & `aimsim-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/sulfonamide-substrate-scope-PDF.png` & `aimsim-2.2.1/tests/sulfonamide-substrate-scope-PDF.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/sulfonamide-substrate-scope.png` & `aimsim-2.2.1/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_CompareTargetMolecule.py` & `aimsim-2.2.1/tests/test_CompareTargetMolecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_Descriptor.py` & `aimsim-2.2.1/tests/test_Descriptor.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_LoadingErrorException.py` & `aimsim-2.2.1/tests/test_LoadingErrorException.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_MeasureSearch.py` & `aimsim-2.2.1/tests/test_MeasureSearch.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_Molecule.py` & `aimsim-2.2.1/tests/test_Molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_MoleculeSet.py` & `aimsim-2.2.1/tests/test_MoleculeSet.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_SimilarityMeasure.py` & `aimsim-2.2.1/tests/test_SimilarityMeasure.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_SimilarityMeasureValueErrors.py` & `aimsim-2.2.1/tests/test_SimilarityMeasureValueErrors.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_TaskManager.py` & `aimsim-2.2.1/tests/test_TaskManager.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_ToolTip.py` & `aimsim-2.2.1/tests/test_ToolTip.py`

 * *Files identical despite different names*

### Comparing `aimsim-2.2.0/tests/test_multithreading.py` & `aimsim-2.2.1/tests/test_multithreading.py`

 * *Files identical despite different names*

