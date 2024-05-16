# Comparing `tmp/aimsim_core-2.2.0.tar.gz` & `tmp/aimsim_core-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsim_core-2.2.0.tar", last modified: Mon Apr 15 16:35:38 2024, max compression
+gzip compressed data, was "aimsim_core-2.2.1.tar", last modified: Thu May 16 21:45:55 2024, max compression
```

## Comparing `aimsim_core-2.2.0.tar` & `aimsim_core-2.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.475800 aimsim_core-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/AIMSim-GUI.png
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-15 16:35:38.475800 aimsim_core-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.463800 aimsim_core-2.2.0/aimsim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.467800 aimsim_core-2.2.0/aimsim/chemical_datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/chemical_datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/chemical_datastructures/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    48544 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/chemical_datastructures/molecule_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.467800 aimsim_core-2.2.0/aimsim/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/ops/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    75466 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/ops/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    63184 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/ops/similarity_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.467800 aimsim_core-2.2.0/aimsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/utils/ccbmlib_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/aimsim/utils/plotting_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.475800 aimsim_core-2.2.0/aimsim_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-15 16:35:38.000000 aimsim_core-2.2.0/aimsim_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-15 16:35:38.000000 aimsim_core-2.2.0/aimsim_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:35:38.000000 aimsim_core-2.2.0/aimsim_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 16:35:38.000000 aimsim_core-2.2.0/aimsim_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 16:35:38.000000 aimsim_core-2.2.0/aimsim_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.463800 aimsim_core-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.471800 aimsim_core-2.2.0/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/_images/AIMSim-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/_images/sulfonamide-substrate-scope.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.471800 aimsim_core-2.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/_static/plus.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.463800 aimsim_core-2.2.0/docs/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.471800 aimsim_core-2.2.0/docs/interfaces/UI/
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/interfaces/UI/AIMSim-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.471800 aimsim_core-2.2.0/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/docs/tests/sulfonamide-substrate-scope.png
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/implemented_metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.463800 aimsim_core-2.2.0/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.471800 aimsim_core-2.2.0/interfaces/UI/
--rw-r--r--   0 runner    (1001) docker     (127)    31374 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/interfaces/UI/AIMSim-GUI-corner-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/interfaces/UI/AIMSim-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/interfaces/UI/AIMSim_ui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/interfaces/UI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.471800 aimsim_core-2.2.0/interfaces/UI/libraries/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/interfaces/UI/libraries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/requirements_core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:35:38.475800 aimsim_core-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.475800 aimsim_core-2.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:35:38.475800 aimsim_core-2.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/sulfonamide-substrate-scope-PDF.png
--rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/sulfonamide-substrate-scope.png
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_CompareTargetMolecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_Descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_LoadingErrorException.py
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_MeasureSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_Molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)    52891 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_MoleculeSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_SimilarityMeasure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_SimilarityMeasureValueErrors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_ToolTip.py
--rw-r--r--   0 runner    (1001) docker     (127)    66192 2024-04-15 16:35:23.000000 aimsim_core-2.2.0/tests/test_multithreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.201767 aimsim_core-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/AIMSim-GUI.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-16 21:45:55.201767 aimsim_core-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.185767 aimsim_core-2.2.1/aimsim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.193767 aimsim_core-2.2.1/aimsim/chemical_datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/chemical_datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/chemical_datastructures/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48544 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/chemical_datastructures/molecule_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.193767 aimsim_core-2.2.1/aimsim/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/ops/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75466 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/ops/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63184 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/ops/similarity_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.193767 aimsim_core-2.2.1/aimsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/utils/ccbmlib_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/aimsim/utils/plotting_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.201767 aimsim_core-2.2.1/aimsim_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-16 21:45:55.000000 aimsim_core-2.2.1/aimsim_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-16 21:45:55.000000 aimsim_core-2.2.1/aimsim_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:45:55.000000 aimsim_core-2.2.1/aimsim_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 21:45:55.000000 aimsim_core-2.2.1/aimsim_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 21:45:55.000000 aimsim_core-2.2.1/aimsim_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.189767 aimsim_core-2.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.193767 aimsim_core-2.2.1/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/_images/AIMSim-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/_images/sulfonamide-substrate-scope.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.193767 aimsim_core-2.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/_static/plus.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.189767 aimsim_core-2.2.1/docs/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.193767 aimsim_core-2.2.1/docs/interfaces/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/interfaces/UI/AIMSim-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.197767 aimsim_core-2.2.1/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/docs/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/implemented_metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.189767 aimsim_core-2.2.1/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.197767 aimsim_core-2.2.1/interfaces/UI/
+-rw-r--r--   0 runner    (1001) docker     (127)    31374 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/interfaces/UI/AIMSim-GUI-corner-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90321 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/interfaces/UI/AIMSim-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/interfaces/UI/AIMSim_ui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/interfaces/UI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.197767 aimsim_core-2.2.1/interfaces/UI/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/interfaces/UI/libraries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/requirements_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:45:55.201767 aimsim_core-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.197767 aimsim_core-2.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:55.201767 aimsim_core-2.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/sulfonamide-substrate-scope-PDF.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147925 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_CompareTargetMolecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_Descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_LoadingErrorException.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_MeasureSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_Molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52891 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_MoleculeSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_SimilarityMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_SimilarityMeasureValueErrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_ToolTip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66192 2024-05-16 21:45:41.000000 aimsim_core-2.2.1/tests/test_multithreading.py
```

### Comparing `aimsim_core-2.2.0/AIMSim-GUI.png` & `aimsim_core-2.2.1/AIMSim-GUI.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/LICENSE` & `aimsim_core-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/PKG-INFO` & `aimsim_core-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsim_core
-Version: 2.2.0
+Version: 2.2.1
 Summary: Core AIMSim molecular featurization and comparison utilities.
 Home-page: https://github.com/VlachosGroup/AIMSim
 Author: Himaghna Bhattacharjee, Jackson Burns
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `aimsim_core-2.2.0/README.md` & `aimsim_core-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/chemical_datastructures/molecule.py` & `aimsim_core-2.2.1/aimsim/chemical_datastructures/molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/chemical_datastructures/molecule_set.py` & `aimsim_core-2.2.1/aimsim/chemical_datastructures/molecule_set.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/ops/clustering.py` & `aimsim_core-2.2.1/aimsim/ops/clustering.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/ops/descriptor.py` & `aimsim_core-2.2.1/aimsim/ops/descriptor.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/ops/similarity_measures.py` & `aimsim_core-2.2.1/aimsim/ops/similarity_measures.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/utils/ccbmlib_fingerprints.py` & `aimsim_core-2.2.1/aimsim/utils/ccbmlib_fingerprints.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim/utils/plotting_scripts.py` & `aimsim_core-2.2.1/aimsim/utils/plotting_scripts.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/aimsim_core.egg-info/PKG-INFO` & `aimsim_core-2.2.1/aimsim_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsim_core
-Version: 2.2.0
+Version: 2.2.1
 Summary: Core AIMSim molecular featurization and comparison utilities.
 Home-page: https://github.com/VlachosGroup/AIMSim
 Author: Himaghna Bhattacharjee, Jackson Burns
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `aimsim_core-2.2.0/aimsim_core.egg-info/SOURCES.txt` & `aimsim_core-2.2.1/aimsim_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/config.yaml` & `aimsim_core-2.2.1/config.yaml`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/docs/_images/AIMSim-logo.png` & `aimsim_core-2.2.1/docs/_images/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/docs/_images/sulfonamide-substrate-scope.png` & `aimsim_core-2.2.1/docs/_images/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/docs/interfaces/UI/AIMSim-logo.png` & `aimsim_core-2.2.1/docs/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/docs/tests/sulfonamide-substrate-scope.png` & `aimsim_core-2.2.1/docs/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/implemented_metrics.md` & `aimsim_core-2.2.1/implemented_metrics.md`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/interfaces/UI/AIMSim-GUI-corner-logo.png` & `aimsim_core-2.2.1/interfaces/UI/AIMSim-GUI-corner-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/interfaces/UI/AIMSim-logo.png` & `aimsim_core-2.2.1/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/interfaces/UI/AIMSim_ui_main.py` & `aimsim_core-2.2.1/interfaces/UI/AIMSim_ui_main.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/setup.py` & `aimsim_core-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/sulfonamide-substrate-scope-PDF.png` & `aimsim_core-2.2.1/tests/sulfonamide-substrate-scope-PDF.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/sulfonamide-substrate-scope.png` & `aimsim_core-2.2.1/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_CompareTargetMolecule.py` & `aimsim_core-2.2.1/tests/test_CompareTargetMolecule.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_Descriptor.py` & `aimsim_core-2.2.1/tests/test_Descriptor.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_LoadingErrorException.py` & `aimsim_core-2.2.1/tests/test_LoadingErrorException.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_MeasureSearch.py` & `aimsim_core-2.2.1/tests/test_MeasureSearch.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_Molecule.py` & `aimsim_core-2.2.1/tests/test_Molecule.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_MoleculeSet.py` & `aimsim_core-2.2.1/tests/test_MoleculeSet.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_SimilarityMeasure.py` & `aimsim_core-2.2.1/tests/test_SimilarityMeasure.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_SimilarityMeasureValueErrors.py` & `aimsim_core-2.2.1/tests/test_SimilarityMeasureValueErrors.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_TaskManager.py` & `aimsim_core-2.2.1/tests/test_TaskManager.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_ToolTip.py` & `aimsim_core-2.2.1/tests/test_ToolTip.py`

 * *Files identical despite different names*

### Comparing `aimsim_core-2.2.0/tests/test_multithreading.py` & `aimsim_core-2.2.1/tests/test_multithreading.py`

 * *Files identical despite different names*

