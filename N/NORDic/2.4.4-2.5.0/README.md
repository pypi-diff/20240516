# Comparing `tmp/NORDic-2.4.4.tar.gz` & `tmp/nordic-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NORDic-2.4.4.tar", last modified: Mon Sep 18 13:48:29 2023, max compression
+gzip compressed data, was "nordic-2.5.0.tar", last modified: Thu May 16 10:20:16 2024, max compression
```

## Comparing `NORDic-2.4.4.tar` & `nordic-2.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.951847 NORDic-2.4.4/
--rw-r--r--   0 kali      (1000) kali      (1000)     7650 2023-09-18 13:48:29.951847 NORDic-2.4.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     7048 2023-08-30 19:54:11.000000 NORDic-2.4.4/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-07-10 04:44:57.000000 NORDic-2.4.4/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-09-18 13:48:29.951847 NORDic-2.4.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1355 2023-09-18 13:48:19.000000 NORDic-2.4.4/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.943847 NORDic-2.4.4/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.947847 NORDic-2.4.4/src/NORDic/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.947847 NORDic-2.4.4/src/NORDic/NORDic_DR/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/NORDic_DR/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    16835 2023-08-30 05:16:04.000000 NORDic-2.4.4/src/NORDic/NORDic_DR/bandits.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     6065 2023-08-30 05:48:10.000000 NORDic-2.4.4/src/NORDic/NORDic_DR/functions.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    14603 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/NORDic_DR/utils.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.947847 NORDic-2.4.4/src/NORDic/NORDic_DS/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/NORDic_DS/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    13963 2023-08-30 05:53:53.000000 NORDic-2.4.4/src/NORDic/NORDic_DS/functions.py
--rw-r--r--   0 kali      (1000) kali      (1000)     9027 2023-08-30 05:53:12.000000 NORDic-2.4.4/src/NORDic/NORDic_DS/get_drug_signatures.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19269 2023-08-30 05:52:59.000000 NORDic-2.4.4/src/NORDic/NORDic_DS/get_drug_targets.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.951847 NORDic-2.4.4/src/NORDic/NORDic_NI/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/NORDic_NI/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     8840 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/NORDic_NI/cytoscape_style.py
--rw-r--r--   0 kali      (1000) kali      (1000)    40424 2023-08-30 06:01:24.000000 NORDic-2.4.4/src/NORDic/NORDic_NI/functions.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.951847 NORDic-2.4.4/src/NORDic/NORDic_PMR/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/NORDic_PMR/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15331 2023-08-30 06:07:53.000000 NORDic-2.4.4/src/NORDic/NORDic_PMR/functions.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.951847 NORDic-2.4.4/src/NORDic/UTILS/
--rwxr-xr-x   0 kali      (1000) kali      (1000)     7371 2023-08-30 06:13:17.000000 NORDic-2.4.4/src/NORDic/UTILS/DISGENET_utils.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    29571 2023-08-30 06:29:35.000000 NORDic-2.4.4/src/NORDic/UTILS/LINCS_utils.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    18438 2023-08-30 06:37:53.000000 NORDic-2.4.4/src/NORDic/UTILS/STRING_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/UTILS/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     9545 2023-08-30 06:41:33.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_data.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    15110 2023-08-30 06:45:42.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_exp.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35835 2023-08-30 07:06:09.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_grn.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15337 2023-08-30 07:13:57.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_network.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19184 2023-08-30 07:26:13.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_plot.py
--rw-r--r--   0 kali      (1000) kali      (1000)    22538 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_sim.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     8313 2023-08-30 07:35:29.000000 NORDic-2.4.4/src/NORDic/UTILS/utils_state.py
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-10 04:44:57.000000 NORDic-2.4.4/src/NORDic/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.947847 NORDic-2.4.4/src/NORDic.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     7650 2023-09-18 13:48:29.000000 NORDic-2.4.4/src/NORDic.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1140 2023-09-18 13:48:29.000000 NORDic-2.4.4/src/NORDic.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-09-18 13:48:29.000000 NORDic-2.4.4/src/NORDic.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      256 2023-09-18 13:48:29.000000 NORDic-2.4.4/src/NORDic.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2023-09-18 13:48:29.000000 NORDic-2.4.4/src/NORDic.egg-info/top_level.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-09-18 13:48:29.951847 NORDic-2.4.4/tests/
--rw-r--r--   0 kali      (1000) kali      (1000)     2898 2023-08-12 08:09:14.000000 NORDic-2.4.4/tests/tests_DR.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2729 2023-08-12 08:08:53.000000 NORDic-2.4.4/tests/tests_DS.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4910 2023-08-12 08:08:56.000000 NORDic-2.4.4/tests/tests_NI.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4959 2023-08-19 16:04:06.000000 NORDic-2.4.4/tests/tests_PKN.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2903 2023-08-12 08:09:02.000000 NORDic-2.4.4/tests/tests_PMR.py
--rw-r--r--   0 kali      (1000) kali      (1000)    12867 2023-08-19 16:57:08.000000 NORDic-2.4.4/tests/tests_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.681368 nordic-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-16 10:20:16.681368 nordic-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-16 10:20:08.000000 nordic-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 10:20:08.000000 nordic-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:20:16.681368 nordic-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 10:20:08.000000 nordic-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.673368 nordic-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.673368 nordic-2.5.0/src/NORDic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.673368 nordic-2.5.0/src/NORDic/NORDic_DR/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DR/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16835 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DR/bandits.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6065 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DR/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14603 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DR/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.677368 nordic-2.5.0/src/NORDic/NORDic_DS/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13963 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DS/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DS/get_drug_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19269 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_DS/get_drug_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.677368 nordic-2.5.0/src/NORDic/NORDic_NI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_NI/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8840 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_NI/cytoscape_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40429 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_NI/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.677368 nordic-2.5.0/src/NORDic/NORDic_PMR/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_PMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/NORDic_PMR/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.677368 nordic-2.5.0/src/NORDic/UTILS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7371 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/DISGENET_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29571 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/LINCS_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18439 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/STRING_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9545 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15110 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_exp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35841 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_grn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19184 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22538 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_sim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8313 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/UTILS/utils_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:08.000000 nordic-2.5.0/src/NORDic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.681368 nordic-2.5.0/src/NORDic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-16 10:20:16.000000 nordic-2.5.0/src/NORDic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-16 10:20:16.000000 nordic-2.5.0/src/NORDic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:20:16.000000 nordic-2.5.0/src/NORDic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-16 10:20:16.000000 nordic-2.5.0/src/NORDic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 10:20:16.000000 nordic-2.5.0/src/NORDic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:20:16.681368 nordic-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-16 10:20:08.000000 nordic-2.5.0/tests/tests_DR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-16 10:20:08.000000 nordic-2.5.0/tests/tests_DS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-16 10:20:08.000000 nordic-2.5.0/tests/tests_NI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-16 10:20:08.000000 nordic-2.5.0/tests/tests_PKN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-16 10:20:08.000000 nordic-2.5.0/tests/tests_PMR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-05-16 10:20:08.000000 nordic-2.5.0/tests/tests_sim.py
```

### Comparing `NORDic-2.4.4/PKG-INFO` & `nordic-2.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-Metadata-Version: 2.1
-Name: NORDic
-Version: 2.4.4
-Summary: Network Oriented Repurposing of Drugs (NORDic): network identification / master regulator detection / drug effect simulator / drug repurposing
-Home-page: https://github.com/clreda/NORDic
-Author: Clémence Réda
-Author-email: clemence.reda@inserm.fr
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.8.5
-Description-Content-Type: text/markdown
-
 # Network Oriented Repurposing of Drugs (NORDic)
-[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
+[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047) [![publication](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d/status.svg)](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d)
 
 ## Statement of need
 
 Being able to build in an automated and reproducible way a model of gene interactions and their influences on gene activity will allow to consider more complex diseases and biological phenomena, on a larger set of genes. These models might speed up the understanding of the gene regulation hierarchy by bioinformaticians and biologists, allow to predict novel drugs or gene targets which might be investigated later for healthcare purposes. In particular, the network-oriented approach allow to predict off-targets, which are non-specific drug targets which might lead to otherwise unexpected toxic side effects.
 
 [NORDic](https://github.com/clreda/NORDic) is an open-source package which allows to focus on a network-oriented approach to identify regulatory mechanisms linked to a disease, to detect master regulators in a diseased transcriptomic context, to simulate drug effects on a patient through a network, and adaptively test drugs to perform sample-efficient, error-bound drug repurposing. As such, it is comprised of four distinct submodules:
 - **NORDic NI** identifies a disease-associated gene regulatory network (as a *Boolean network*) with its dynamics combining several biological sources and methods. The main contribution is that this inference can be performed even in the absence of previously curated experiments and prior knowledge networks.
@@ -50,18 +36,21 @@
 apt-get install graphviz # for Debian distributions, check the correct command for your own distribution
 conda install -c colomoto -y -q maboss
 pip install NORDic 
 ```
 
 ### Using conda (package hosted on Anaconda.org)
 
-All dependencies are retrievable from Anaconda:
+All dependencies (except for clingo) are retrievable from Anaconda:
 
 ```bash
+conda install -c potassco clingo
+
 conda install -c creda -y -q nordic
+conda install -c bioconda -y -q nordic
 ```
 
 ### Using [CoLoMoTo-Docker](https://github.com/colomoto/colomoto-docker) (since March 1st, 2023)
 
 ```bash
 pip install -U colomoto-docker
 colomoto-docker
@@ -102,31 +91,37 @@
 help(func)
 ```
 
 The documentation website is up at [this page](https://clreda.github.io/NORDic).
 
 ## Cite
 
-If you use **NORDic** in academic research, please cite the following preliminary work (which relied on the same type of pipeline as **NORDic NI** and **NORDic PMR**, but with different implementations):
+If you use **NORDic** in academic research, please cite the following JOSS paper:
+
+[![publication](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d/status.svg)](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d)
 
 + Formatted citation:
 
-> Réda, C., & Delahaye-Duriez, A. (2022, August). Prioritization of Candidate Genes Through Boolean Networks. In Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14–16, 2022, Proceedings (pp. 89-121). Cham: Springer International Publishing.
+> Réda et al., (2023). NORDic: a Network-Oriented package for the Repurposing of Drugs. Journal of Open Source Software, 8(90), 5532, https://doi.org/10.21105/joss.05532
 
 + BibTeX citation:
 
 ```bash
-@inproceedings{reda2022prioritization,
-  title={Prioritization of Candidate Genes Through Boolean Networks},
-  author={R{\'e}da, Cl{\'e}mence and Delahaye-Duriez, Andr{\'e}e},
-  booktitle={Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14--16, 2022, Proceedings},
-  pages={89--121},
-  year={2022},
-  organization={Springer}
-}
+@article{Réda2023, 
+    doi = {10.21105/joss.05532}, 
+    url = {https://doi.org/10.21105/joss.05532}, 
+    year = {2023}, 
+    publisher = {The Open Journal}, 
+    volume = {8}, 
+    number = {90}, 
+    pages = {5532}, 
+    author = {Clémence Réda and Andrée Delahaye-Duriez}, 
+    title = {NORDic: a Network-Oriented package for the Repurposing of Drugs}, 
+    journal = {Journal of Open Source Software} 
+} 
 ```
 
 ## License
 
 This code is under [OSI-approved](https://opensource.org/licenses/) [MIT license](https://raw.githubusercontent.com/clreda/NORDic/main/LICENSE).
 
 ## Community guidelines with respect to contributions, issue reporting, and support
```

### Comparing `NORDic-2.4.4/setup.py` & `nordic-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "NORDic"
-VERSION = "2.4.4"
+VERSION = "2.5.0"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="clemence.reda@inserm.fr",
     url="https://github.com/clreda/NORDic",
     license_files = ('LICENSE'),
```

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_DR/bandits.py` & `nordic-2.5.0/src/NORDic/NORDic_DR/bandits.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_DR/functions.py` & `nordic-2.5.0/src/NORDic/NORDic_DR/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_DR/utils.py` & `nordic-2.5.0/src/NORDic/NORDic_DR/utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_DS/functions.py` & `nordic-2.5.0/src/NORDic/NORDic_DS/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_DS/get_drug_signatures.py` & `nordic-2.5.0/src/NORDic/NORDic_DS/get_drug_signatures.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_DS/get_drug_targets.py` & `nordic-2.5.0/src/NORDic/NORDic_DS/get_drug_targets.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_NI/cytoscape_style.py` & `nordic-2.5.0/src/NORDic/NORDic_NI/cytoscape_style.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_NI/functions.py` & `nordic-2.5.0/src/NORDic/NORDic_NI/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
             assert all([v in ["0","1",np.nan] for v in list(profiles.loc[[g for g in model_genes if (g in profiles.index)]].values.flatten())])
             profiles = profiles[[c for c in profiles.columns if ((profiles.loc["perturbed"][c] in model_genes+["None"]) and (profiles.loc["cell_line"][c] in cell_lines))]]
             profiles = profiles.loc[[g for g in list(profiles.index) if (g in model_genes+add_rows_profiles)]]
         profiles.to_csv(profiles_fname)
 
     profiles = pd.read_csv(profiles_fname, index_col=0, low_memory=False)
     if (not pd.isnull(profiles.values).all()):
-        nconds = len(set(["_".join([profiles.loc[v][c] for v in ["perturbed","perturbation","cell_line"]]) for c in profiles.columns]))
+        nconds = len(set(["_".join([str(profiles.loc[v][c]) for v in ["perturbed","perturbation","cell_line"]]) for c in profiles.columns]))
     else:
         nconds = 0
     ngenes = len([p for p in profiles.index if (p not in add_rows_profiles)])
     print("... %d genes in %d profiles (%d experiments)" % (0 if (profiles is None) else ngenes, 0 if (profiles is None) else profiles.shape[1], 0 if (profiles is None) else nconds))
     if (profiles is None and force_experiments):
         raise ValueError("No experimental profile could be found.")
         assert (not force_experiments) or ((profiles is not None) and profiles.shape[1]>0)
```

### Comparing `NORDic-2.4.4/src/NORDic/NORDic_PMR/functions.py` & `nordic-2.5.0/src/NORDic/NORDic_PMR/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/DISGENET_utils.py` & `nordic-2.5.0/src/NORDic/UTILS/DISGENET_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/LINCS_utils.py` & `nordic-2.5.0/src/NORDic/UTILS/LINCS_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/STRING_utils.py` & `nordic-2.5.0/src/NORDic/UTILS/STRING_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -408,8 +408,8 @@
         values[list(network.columns).index("directed")] = int(values[list(network.columns).index("directed")])
         values[list(network.columns).index("score")] = float(values[list(network.columns).index("score")])
         network.loc[x] = values
     if (not quiet):
         print("... Aggregate info once again")
     network.index = range(network.shape[0])
     network.sort_values(by="score", ascending=False)
-    return network
+    return network
```

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_data.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_data.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_exp.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_exp.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_grn.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_grn.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,29 +484,29 @@
     for exp_nb in exps_ids:
         cell = exps[exp_nb].split("_")[-1]
         cols = ["Exp%d_"%(exp_nb+1)+x for x in ["init", "final"]]
         data_df = signatures[["initial_"+cell, exps[exp_nb-1]]]
 
         ## Compatible with perturbation experiment
         data_df = data_df.T
-        pert, sign = exps[exp_nb].split("_")[0], 0 if (exps[exp_nb].split("_")[1]=="KD") else 1
+        pert, sign = exps[exp_nb-1].split("_")[0], 0 if (exps[exp_nb-1].split("_")[1]=="KD") else 1
         data_df[pert] = sign 
         data_df = data_df.T
 
         data_df.columns = cols
         for col in cols:
             data_exps.update(data_df[[col]].dropna().astype(int).to_dict())
     if (not quiet):
         print_exps = pd.DataFrame.from_dict(data_exps, orient="index").fillna(-1).astype(int)
         print_exps[print_exps==-1] = ""
         print("\n<UTILS_GRN> %d experiments\n%s" % (len(exps_ids), str(print_exps)))
     BO = bonesis.BoNesis(grn, data_exps)
     ## 2. Instantiate reachability & fixed point constraints
     for exp_nb in exps_ids:
-        exp = exps[exp_nb]
+        exp = exps[exp_nb-1]
         pert, sign = exp.split("_")[:2]
         cell = exp.split("_")[-1]
         sign = int(sign!="KD")
         with BO.mutant({pert: sign}) as m:
             final_FP = m.fixed(~m.obs("Exp%d_final" % (exp_nb+1)))
             ## 2a. There exists a trajectory : init -> trapspace
             ~m.obs("Exp%d_init" % (exp_nb+1)) >= final_FP #~m.obs("Exp%d_final" % (exp_nb+1)) ##
```

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_network.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_network.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_plot.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_plot.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_sim.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_sim.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic/UTILS/utils_state.py` & `nordic-2.5.0/src/NORDic/UTILS/utils_state.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/src/NORDic.egg-info/PKG-INFO` & `nordic-2.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 Metadata-Version: 2.1
 Name: NORDic
-Version: 2.4.4
+Version: 2.5.0
 Summary: Network Oriented Repurposing of Drugs (NORDic): network identification / master regulator detection / drug effect simulator / drug repurposing
 Home-page: https://github.com/clreda/NORDic
 Author: Clémence Réda
 Author-email: clemence.reda@inserm.fr
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
+Requires-Dist: pandas>=1.5.1
+Requires-Dist: numpy>=1.22.4
+Requires-Dist: clingo>=5.6.1
+Requires-Dist: graphviz>=0.20.1
+Requires-Dist: bonesis>=0.4.91
+Requires-Dist: mpbn>=2.0
+Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: scikit_learn>=1.1.2
+Requires-Dist: scipy>=1.6.2
+Requires-Dist: qnorm>=0.5.1
+Requires-Dist: tqdm>=4.62.3
+Requires-Dist: cmapPy>=4.0.1
+Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: quadprog>=0.1.11
+Requires-Dist: seaborn>=0.12.1
+Requires-Dist: omnipath>=1.0.6
+Requires-Dist: maboss>=0.8.4
 
 # Network Oriented Repurposing of Drugs (NORDic)
-[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
+[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047) [![publication](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d/status.svg)](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d)
 
 ## Statement of need
 
 Being able to build in an automated and reproducible way a model of gene interactions and their influences on gene activity will allow to consider more complex diseases and biological phenomena, on a larger set of genes. These models might speed up the understanding of the gene regulation hierarchy by bioinformaticians and biologists, allow to predict novel drugs or gene targets which might be investigated later for healthcare purposes. In particular, the network-oriented approach allow to predict off-targets, which are non-specific drug targets which might lead to otherwise unexpected toxic side effects.
 
 [NORDic](https://github.com/clreda/NORDic) is an open-source package which allows to focus on a network-oriented approach to identify regulatory mechanisms linked to a disease, to detect master regulators in a diseased transcriptomic context, to simulate drug effects on a patient through a network, and adaptively test drugs to perform sample-efficient, error-bound drug repurposing. As such, it is comprised of four distinct submodules:
 - **NORDic NI** identifies a disease-associated gene regulatory network (as a *Boolean network*) with its dynamics combining several biological sources and methods. The main contribution is that this inference can be performed even in the absence of previously curated experiments and prior knowledge networks.
@@ -50,18 +67,21 @@
 apt-get install graphviz # for Debian distributions, check the correct command for your own distribution
 conda install -c colomoto -y -q maboss
 pip install NORDic 
 ```
 
 ### Using conda (package hosted on Anaconda.org)
 
-All dependencies are retrievable from Anaconda:
+All dependencies (except for clingo) are retrievable from Anaconda:
 
 ```bash
+conda install -c potassco clingo
+
 conda install -c creda -y -q nordic
+conda install -c bioconda -y -q nordic
 ```
 
 ### Using [CoLoMoTo-Docker](https://github.com/colomoto/colomoto-docker) (since March 1st, 2023)
 
 ```bash
 pip install -U colomoto-docker
 colomoto-docker
@@ -102,31 +122,37 @@
 help(func)
 ```
 
 The documentation website is up at [this page](https://clreda.github.io/NORDic).
 
 ## Cite
 
-If you use **NORDic** in academic research, please cite the following preliminary work (which relied on the same type of pipeline as **NORDic NI** and **NORDic PMR**, but with different implementations):
+If you use **NORDic** in academic research, please cite the following JOSS paper:
+
+[![publication](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d/status.svg)](https://joss.theoj.org/papers/a8173d7864bf1bc8dd074c7ce80d6d7d)
 
 + Formatted citation:
 
-> Réda, C., & Delahaye-Duriez, A. (2022, August). Prioritization of Candidate Genes Through Boolean Networks. In Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14–16, 2022, Proceedings (pp. 89-121). Cham: Springer International Publishing.
+> Réda et al., (2023). NORDic: a Network-Oriented package for the Repurposing of Drugs. Journal of Open Source Software, 8(90), 5532, https://doi.org/10.21105/joss.05532
 
 + BibTeX citation:
 
 ```bash
-@inproceedings{reda2022prioritization,
-  title={Prioritization of Candidate Genes Through Boolean Networks},
-  author={R{\'e}da, Cl{\'e}mence and Delahaye-Duriez, Andr{\'e}e},
-  booktitle={Computational Methods in Systems Biology: 20th International Conference, CMSB 2022, Bucharest, Romania, September 14--16, 2022, Proceedings},
-  pages={89--121},
-  year={2022},
-  organization={Springer}
-}
+@article{Réda2023, 
+    doi = {10.21105/joss.05532}, 
+    url = {https://doi.org/10.21105/joss.05532}, 
+    year = {2023}, 
+    publisher = {The Open Journal}, 
+    volume = {8}, 
+    number = {90}, 
+    pages = {5532}, 
+    author = {Clémence Réda and Andrée Delahaye-Duriez}, 
+    title = {NORDic: a Network-Oriented package for the Repurposing of Drugs}, 
+    journal = {Journal of Open Source Software} 
+} 
 ```
 
 ## License
 
 This code is under [OSI-approved](https://opensource.org/licenses/) [MIT license](https://raw.githubusercontent.com/clreda/NORDic/main/LICENSE).
 
 ## Community guidelines with respect to contributions, issue reporting, and support
```

### Comparing `NORDic-2.4.4/src/NORDic.egg-info/SOURCES.txt` & `nordic-2.5.0/src/NORDic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/tests/tests_DR.py` & `nordic-2.5.0/tests/tests_DR.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/tests/tests_DS.py` & `nordic-2.5.0/tests/tests_DS.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/tests/tests_NI.py` & `nordic-2.5.0/tests/tests_NI.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/tests/tests_PKN.py` & `nordic-2.5.0/tests/tests_PKN.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/tests/tests_PMR.py` & `nordic-2.5.0/tests/tests_PMR.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.4/tests/tests_sim.py` & `nordic-2.5.0/tests/tests_sim.py`

 * *Files identical despite different names*

