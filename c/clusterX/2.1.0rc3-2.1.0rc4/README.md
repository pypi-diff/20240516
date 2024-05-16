# Comparing `tmp/clusterX-2.1.0rc3.tar.gz` & `tmp/clusterX-2.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterX-2.1.0rc3.tar", last modified: Thu Dec  7 15:21:13 2023, max compression
+gzip compressed data, was "clusterX-2.1.0rc4.tar", last modified: Mon Apr 22 14:09:32 2024, max compression
```

## Comparing `clusterX-2.1.0rc3.tar` & `clusterX-2.1.0rc4.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.198833 clusterX-2.1.0rc3/
--rw-------   0 srigamonti  (6002) sol       (6001)    11477 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/COPYING
--rw-------   0 srigamonti  (6002) sol       (6001)    11477 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/LICENSE.txt
--rw-------   0 srigamonti  (6002) sol       (6001)       60 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/MANIFEST.in
--rw-r--r--   0 srigamonti  (6002) sol       (6001)      738 2023-12-07 15:21:13.198833 clusterX-2.1.0rc3/PKG-INFO
--rw-------   0 srigamonti  (6002) sol       (6001)      219 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/README.rst
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterX.egg-info/
--rw-r--r--   0 srigamonti  (6002) sol       (6001)      738 2023-12-07 15:21:13.000000 clusterX-2.1.0rc3/clusterX.egg-info/PKG-INFO
--rw-------   0 srigamonti  (6002) sol       (6001)     1938 2023-12-07 15:21:13.000000 clusterX-2.1.0rc3/clusterX.egg-info/SOURCES.txt
--rw-------   0 srigamonti  (6002) sol       (6001)        1 2023-12-07 15:21:13.000000 clusterX-2.1.0rc3/clusterX.egg-info/dependency_links.txt
--rw-------   0 srigamonti  (6002) sol       (6001)       48 2023-12-07 15:21:13.000000 clusterX-2.1.0rc3/clusterX.egg-info/entry_points.txt
--rw-------   0 srigamonti  (6002) sol       (6001)      101 2023-12-07 15:21:13.000000 clusterX-2.1.0rc3/clusterX.egg-info/requires.txt
--rw-------   0 srigamonti  (6002) sol       (6001)        9 2023-12-07 15:21:13.000000 clusterX-2.1.0rc3/clusterX.egg-info/top_level.txt
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/
--rw-------   0 srigamonti  (6002) sol       (6001)      626 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/__init__.py
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/calculators/
--rw-------   0 srigamonti  (6002) sol       (6001)      294 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/calculators/__init__.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2270 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/calculators/emt.py
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/cli/
--rw-------   0 srigamonti  (6002) sol       (6001)      208 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/cli/__init__.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1648 2023-05-17 17:23:39.000000 clusterX-2.1.0rc3/clusterx/cli/commands.py
--rw-------   0 srigamonti  (6002) sol       (6001)      670 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/cli/main.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1303 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/cli/plot_clusters.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1251 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/cli/spacegroup.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1068 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/cli/test.py
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/clusters/
--rw-------   0 srigamonti  (6002) sol       (6001)        0 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/clusters/__init__.py
--rw-------   0 srigamonti  (6002) sol       (6001)     9798 2023-08-02 17:06:09.000000 clusterX-2.1.0rc3/clusterx/clusters/cluster.py
--rw-------   0 srigamonti  (6002) sol       (6001)    62833 2023-08-02 16:45:14.000000 clusterX-2.1.0rc3/clusterx/clusters/clusters_pool.py
--rw-------   0 srigamonti  (6002) sol       (6001)    25723 2023-08-02 16:27:57.000000 clusterX-2.1.0rc3/clusterx/clusters_selector.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1360 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/config.py
--rw-------   0 srigamonti  (6002) sol       (6001)    19100 2023-08-02 16:27:57.000000 clusterX-2.1.0rc3/clusterx/correlations.py
--rw-------   0 srigamonti  (6002) sol       (6001)      352 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/cross_validation.py
--rw-------   0 srigamonti  (6002) sol       (6001)    13889 2023-07-20 22:00:43.000000 clusterX-2.1.0rc3/clusterx/derivative_structures.py
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/estimators/
--rw-------   0 srigamonti  (6002) sol       (6001)        0 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/estimators/__init__.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2984 2023-05-08 09:57:44.000000 clusterX-2.1.0rc3/clusterx/estimators/estimator_factory.py
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/io/
--rw-------   0 srigamonti  (6002) sol       (6001)      208 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/io/__init__.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1393 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/io/atat.py
--rw-------   0 srigamonti  (6002) sol       (6001)      484 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/io/formats.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2283 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/lattices.py
--rw-------   0 srigamonti  (6002) sol       (6001)    27785 2023-08-02 16:27:57.000000 clusterX-2.1.0rc3/clusterx/model.py
--rw-------   0 srigamonti  (6002) sol       (6001)    25400 2023-06-05 11:08:41.000000 clusterX-2.1.0rc3/clusterx/parent_lattice.py
--rw-------   0 srigamonti  (6002) sol       (6001)    14639 2023-05-10 17:03:30.000000 clusterX-2.1.0rc3/clusterx/structure.py
--rw-------   0 srigamonti  (6002) sol       (6001)    11069 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/structure_selector.py
--rw-------   0 srigamonti  (6002) sol       (6001)    35850 2023-12-07 13:50:32.000000 clusterX-2.1.0rc3/clusterx/structures_set.py
--rw-------   0 srigamonti  (6002) sol       (6001)    21924 2023-05-08 09:57:44.000000 clusterX-2.1.0rc3/clusterx/super_cell.py
--rw-------   0 srigamonti  (6002) sol       (6001)     3653 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/symmetry.py
-drwx------   0 srigamonti  (6002) sol       (6001)        0 2023-12-07 15:21:13.194833 clusterX-2.1.0rc3/clusterx/test/
--rw-------   0 srigamonti  (6002) sol       (6001)      434 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/__init__.py
--rw-------   0 srigamonti  (6002) sol       (6001)     3071 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_clathrate_mc.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2315 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_cluster.py
--rw-------   0 srigamonti  (6002) sol       (6001)     5390 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_cluster_correlations.py
--rw-------   0 srigamonti  (6002) sol       (6001)     7527 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_cluster_expansion.py
--rw-------   0 srigamonti  (6002) sol       (6001)    14654 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_cluster_orbit.py
--rw-------   0 srigamonti  (6002) sol       (6001)    12876 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_cluster_orbit2.py
--rw-------   0 srigamonti  (6002) sol       (6001)    13813 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_clusters_generation.py
--rw-------   0 srigamonti  (6002) sol       (6001)     7628 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_clusters_selector.py
--rw-------   0 srigamonti  (6002) sol       (6001)     7744 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_clusters_selector_lasso.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2132 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_concentration.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2926 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_emt2_calculator.py
--rw-------   0 srigamonti  (6002) sol       (6001)     2346 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_folders.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1491 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_get_all_hnf.py
--rw-------   0 srigamonti  (6002) sol       (6001)     3954 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_get_unique_supercells.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1418 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_is_nary.py
--rw-------   0 srigamonti  (6002) sol       (6001)     3994 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_lattice_representation.py
--rw-------   0 srigamonti  (6002) sol       (6001)    23113 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_metropolis.py
--rw-------   0 srigamonti  (6002) sol       (6001)     8623 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_parent_lattice_creation.py
--rw-------   0 srigamonti  (6002) sol       (6001)     4577 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_predict_swap.py
--rw-------   0 srigamonti  (6002) sol       (6001)     7625 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_structure_selector.py
--rw-------   0 srigamonti  (6002) sol       (6001)     1834 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_structures_set.py
--rw-------   0 srigamonti  (6002) sol       (6001)     5713 2023-05-08 09:50:06.000000 clusterX-2.1.0rc3/clusterx/test/test_wanglandau.py
--rw-------   0 srigamonti  (6002) sol       (6001)    40776 2023-07-20 22:00:43.000000 clusterX-2.1.0rc3/clusterx/utils.py
--rw-------   0 srigamonti  (6002) sol       (6001)    24903 2023-12-07 13:50:32.000000 clusterX-2.1.0rc3/clusterx/visualization.py
--rw-------   0 srigamonti  (6002) sol       (6001)       38 2023-12-07 15:21:13.198833 clusterX-2.1.0rc3/setup.cfg
--rw-------   0 srigamonti  (6002) sol       (6001)      735 2023-12-07 15:12:41.000000 clusterX-2.1.0rc3/setup.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.563360 clusterX-2.1.0rc4/
+-rw-------   0 srigamonti  (6002) sol       (6001)    11477 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/COPYING
+-rw-------   0 srigamonti  (6002) sol       (6001)    11477 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/LICENSE.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)       60 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/MANIFEST.in
+-rw-------   0 srigamonti  (6002) sol       (6001)      442 2024-04-22 14:09:32.563360 clusterX-2.1.0rc4/PKG-INFO
+-rw-------   0 srigamonti  (6002) sol       (6001)      219 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/README.rst
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.443359 clusterX-2.1.0rc4/clusterX.egg-info/
+-rw-r--r--   0 srigamonti  (6002) sol       (6001)      442 2024-04-22 14:09:31.000000 clusterX-2.1.0rc4/clusterX.egg-info/PKG-INFO
+-rw-------   0 srigamonti  (6002) sol       (6001)     2052 2024-04-22 14:09:31.000000 clusterX-2.1.0rc4/clusterX.egg-info/SOURCES.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)        1 2024-04-22 14:09:31.000000 clusterX-2.1.0rc4/clusterX.egg-info/dependency_links.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)       48 2024-04-22 14:09:31.000000 clusterX-2.1.0rc4/clusterX.egg-info/entry_points.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)      101 2024-04-22 14:09:31.000000 clusterX-2.1.0rc4/clusterX.egg-info/requires.txt
+-rw-------   0 srigamonti  (6002) sol       (6001)        9 2024-04-22 14:09:31.000000 clusterX-2.1.0rc4/clusterX.egg-info/top_level.txt
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.491360 clusterX-2.1.0rc4/clusterx/
+-rw-------   0 srigamonti  (6002) sol       (6001)      626 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/__init__.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.495360 clusterX-2.1.0rc4/clusterx/calculators/
+-rw-------   0 srigamonti  (6002) sol       (6001)      294 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/calculators/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2270 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/calculators/emt.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.499360 clusterX-2.1.0rc4/clusterx/cli/
+-rw-------   0 srigamonti  (6002) sol       (6001)      208 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/cli/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1648 2023-05-17 17:23:39.000000 clusterX-2.1.0rc4/clusterx/cli/commands.py
+-rw-------   0 srigamonti  (6002) sol       (6001)      670 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/cli/main.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1303 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/cli/plot_clusters.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1251 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/cli/spacegroup.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1068 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/cli/test.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.515360 clusterX-2.1.0rc4/clusterx/clusters/
+-rw-------   0 srigamonti  (6002) sol       (6001)        0 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/clusters/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     9798 2023-08-02 17:06:09.000000 clusterX-2.1.0rc4/clusterx/clusters/cluster.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    62833 2023-08-02 16:45:14.000000 clusterX-2.1.0rc4/clusterx/clusters/clusters_pool.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    25723 2023-08-02 16:27:57.000000 clusterX-2.1.0rc4/clusterx/clusters_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1360 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/config.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    19100 2023-08-02 16:27:57.000000 clusterX-2.1.0rc4/clusterx/correlations.py
+-rw-------   0 srigamonti  (6002) sol       (6001)      352 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/cross_validation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    13889 2023-07-20 22:00:43.000000 clusterX-2.1.0rc4/clusterx/derivative_structures.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.519360 clusterX-2.1.0rc4/clusterx/estimators/
+-rw-------   0 srigamonti  (6002) sol       (6001)        0 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/estimators/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2984 2023-05-08 09:57:44.000000 clusterX-2.1.0rc4/clusterx/estimators/estimator_factory.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.523360 clusterX-2.1.0rc4/clusterx/io/
+-rw-------   0 srigamonti  (6002) sol       (6001)      208 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/io/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1393 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/io/atat.py
+-rw-------   0 srigamonti  (6002) sol       (6001)      484 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/io/formats.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2283 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/lattices.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    27785 2023-08-02 16:27:57.000000 clusterX-2.1.0rc4/clusterx/model.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    25400 2023-06-05 11:08:41.000000 clusterX-2.1.0rc4/clusterx/parent_lattice.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    14639 2023-05-10 17:03:30.000000 clusterX-2.1.0rc4/clusterx/structure.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    11069 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/structure_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    35850 2023-12-07 13:50:32.000000 clusterX-2.1.0rc4/clusterx/structures_set.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    21924 2023-05-08 09:57:44.000000 clusterX-2.1.0rc4/clusterx/super_cell.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3653 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/symmetry.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.539360 clusterX-2.1.0rc4/clusterx/test/
+-rw-------   0 srigamonti  (6002) sol       (6001)      434 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3071 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_clathrate_mc.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2315 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_cluster.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     5390 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_cluster_correlations.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7527 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_cluster_expansion.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    14654 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_cluster_orbit.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    12876 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_cluster_orbit2.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    13813 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_clusters_generation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7628 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_clusters_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7744 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_clusters_selector_lasso.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2132 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_concentration.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2926 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_emt2_calculator.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     2346 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_folders.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1491 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_get_all_hnf.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3954 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_get_unique_supercells.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1418 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_is_nary.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     3994 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_lattice_representation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    23113 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_metropolis.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     8623 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_parent_lattice_creation.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     4577 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_predict_swap.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     7625 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_structure_selector.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     1834 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_structures_set.py
+-rw-------   0 srigamonti  (6002) sol       (6001)     5713 2023-05-08 09:50:06.000000 clusterX-2.1.0rc4/clusterx/test/test_wanglandau.py
+drwx------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:09:32.543360 clusterX-2.1.0rc4/clusterx/thermodynamics/
+-rw-------   0 srigamonti  (6002) sol       (6001)        0 2024-04-22 14:04:40.000000 clusterX-2.1.0rc4/clusterx/thermodynamics/__init__.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    33994 2023-05-09 14:08:49.000000 clusterX-2.1.0rc4/clusterx/thermodynamics/monte_carlo.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    58551 2023-08-02 16:27:57.000000 clusterX-2.1.0rc4/clusterx/thermodynamics/wang_landau.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    40776 2023-07-20 22:00:43.000000 clusterX-2.1.0rc4/clusterx/utils.py
+-rw-------   0 srigamonti  (6002) sol       (6001)    24903 2023-12-07 13:50:32.000000 clusterX-2.1.0rc4/clusterx/visualization.py
+-rw-------   0 srigamonti  (6002) sol       (6001)       38 2024-04-22 14:09:32.563360 clusterX-2.1.0rc4/setup.cfg
+-rw-------   0 srigamonti  (6002) sol       (6001)      735 2024-04-22 14:09:03.000000 clusterX-2.1.0rc4/setup.py
```

### Comparing `clusterX-2.1.0rc3/COPYING` & `clusterX-2.1.0rc4/COPYING`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/LICENSE.txt` & `clusterX-2.1.0rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterX.egg-info/SOURCES.txt` & `clusterX-2.1.0rc4/clusterX.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -59,8 +59,11 @@
 clusterx/test/test_is_nary.py
 clusterx/test/test_lattice_representation.py
 clusterx/test/test_metropolis.py
 clusterx/test/test_parent_lattice_creation.py
 clusterx/test/test_predict_swap.py
 clusterx/test/test_structure_selector.py
 clusterx/test/test_structures_set.py
-clusterx/test/test_wanglandau.py
+clusterx/test/test_wanglandau.py
+clusterx/thermodynamics/__init__.py
+clusterx/thermodynamics/monte_carlo.py
+clusterx/thermodynamics/wang_landau.py
```

### Comparing `clusterX-2.1.0rc3/clusterx/__init__.py` & `clusterX-2.1.0rc4/clusterx/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/calculators/emt.py` & `clusterX-2.1.0rc4/clusterx/calculators/emt.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/cli/commands.py` & `clusterX-2.1.0rc4/clusterx/cli/commands.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/cli/main.py` & `clusterX-2.1.0rc4/clusterx/cli/main.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/cli/plot_clusters.py` & `clusterX-2.1.0rc4/clusterx/cli/plot_clusters.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/cli/spacegroup.py` & `clusterX-2.1.0rc4/clusterx/cli/spacegroup.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/cli/test.py` & `clusterX-2.1.0rc4/clusterx/cli/test.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/clusters/cluster.py` & `clusterX-2.1.0rc4/clusterx/clusters/cluster.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/clusters/clusters_pool.py` & `clusterX-2.1.0rc4/clusterx/clusters/clusters_pool.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/clusters_selector.py` & `clusterX-2.1.0rc4/clusterx/clusters_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/config.py` & `clusterX-2.1.0rc4/clusterx/config.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/correlations.py` & `clusterX-2.1.0rc4/clusterx/correlations.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/derivative_structures.py` & `clusterX-2.1.0rc4/clusterx/derivative_structures.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/estimators/estimator_factory.py` & `clusterX-2.1.0rc4/clusterx/estimators/estimator_factory.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/io/atat.py` & `clusterX-2.1.0rc4/clusterx/io/atat.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/lattices.py` & `clusterX-2.1.0rc4/clusterx/lattices.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/model.py` & `clusterX-2.1.0rc4/clusterx/model.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/parent_lattice.py` & `clusterX-2.1.0rc4/clusterx/parent_lattice.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/structure.py` & `clusterX-2.1.0rc4/clusterx/structure.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/structure_selector.py` & `clusterX-2.1.0rc4/clusterx/structure_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/structures_set.py` & `clusterX-2.1.0rc4/clusterx/structures_set.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/super_cell.py` & `clusterX-2.1.0rc4/clusterx/super_cell.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/symmetry.py` & `clusterX-2.1.0rc4/clusterx/symmetry.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_clathrate_mc.py` & `clusterX-2.1.0rc4/clusterx/test/test_clathrate_mc.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_cluster.py` & `clusterX-2.1.0rc4/clusterx/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_cluster_correlations.py` & `clusterX-2.1.0rc4/clusterx/test/test_cluster_correlations.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_cluster_expansion.py` & `clusterX-2.1.0rc4/clusterx/test/test_cluster_expansion.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_cluster_orbit.py` & `clusterX-2.1.0rc4/clusterx/test/test_cluster_orbit.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_cluster_orbit2.py` & `clusterX-2.1.0rc4/clusterx/test/test_cluster_orbit2.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_clusters_generation.py` & `clusterX-2.1.0rc4/clusterx/test/test_clusters_generation.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_clusters_selector.py` & `clusterX-2.1.0rc4/clusterx/test/test_clusters_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_clusters_selector_lasso.py` & `clusterX-2.1.0rc4/clusterx/test/test_clusters_selector_lasso.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_concentration.py` & `clusterX-2.1.0rc4/clusterx/test/test_concentration.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_emt2_calculator.py` & `clusterX-2.1.0rc4/clusterx/test/test_emt2_calculator.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_folders.py` & `clusterX-2.1.0rc4/clusterx/test/test_folders.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_get_all_hnf.py` & `clusterX-2.1.0rc4/clusterx/test/test_get_all_hnf.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_get_unique_supercells.py` & `clusterX-2.1.0rc4/clusterx/test/test_get_unique_supercells.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_is_nary.py` & `clusterX-2.1.0rc4/clusterx/test/test_is_nary.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_lattice_representation.py` & `clusterX-2.1.0rc4/clusterx/test/test_lattice_representation.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_metropolis.py` & `clusterX-2.1.0rc4/clusterx/test/test_metropolis.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_parent_lattice_creation.py` & `clusterX-2.1.0rc4/clusterx/test/test_parent_lattice_creation.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_predict_swap.py` & `clusterX-2.1.0rc4/clusterx/test/test_predict_swap.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_structure_selector.py` & `clusterX-2.1.0rc4/clusterx/test/test_structure_selector.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_structures_set.py` & `clusterX-2.1.0rc4/clusterx/test/test_structures_set.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/test/test_wanglandau.py` & `clusterX-2.1.0rc4/clusterx/test/test_wanglandau.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/utils.py` & `clusterX-2.1.0rc4/clusterx/utils.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/clusterx/visualization.py` & `clusterX-2.1.0rc4/clusterx/visualization.py`

 * *Files identical despite different names*

### Comparing `clusterX-2.1.0rc3/setup.py` & `clusterX-2.1.0rc4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='clusterX',
-      version='2.1.0.rc3',
+      version='2.1.0.rc4',
       description='CELL (aka clusterX) is a python package for building Cluster Expansion models of simple and complex alloys and performing thermodynamical analyses of materials.',
       url='http://sol.physik.hu-berlin.de/cell/',
       author='CELL Developers',
       author_email='srigamonti@physik.hu-berlin.de',
       license='http://www.apache.org/licenses/LICENSE-2.0',
       packages=find_packages(),
       install_requires=['numpy', 'scipy', 'scikit-learn', 'matplotlib','ase','plac','pytest','spglib','sympy','nglview','ipywidgets','pytest-html', 'tqdm'],
```

