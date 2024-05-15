# Comparing `tmp/mapel-elections-2.1.8.tar.gz` & `tmp/mapel_elections-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-elections-2.1.8.tar", last modified: Sat Mar 23 13:42:15 2024, max compression
+gzip compressed data, was "mapel_elections-2.1.9.tar", last modified: Mon Apr 15 08:50:18 2024, max compression
```

## Comparing `mapel-elections-2.1.8.tar` & `mapel_elections-2.1.9.tar`

### file list

```diff
@@ -1,96 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.825371 mapel-elections-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-23 13:42:15.825371 mapel-elections-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 13:42:15.825371 mapel-elections-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.809371 mapel-elections-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.809371 mapel-elections-2.1.8/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.809371 mapel-elections-2.1.8/src/mapel/elections/
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.813371 mapel-elections-2.1.8/src/mapel/elections/cultures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/guardians.py
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/guardians_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/mallows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.813371 mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/group_separable_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/single_crossing_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/single_peaked_matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.813371 mapel-elections-2.1.8/src/mapel/elections/cultures/nonstandard/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/nonstandard/alliances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/nonstandard/field_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/nonstandard/parties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/preflib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.813371 mapel-elections-2.1.8/src/mapel/elections/cultures/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/sampling/samplemat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.813371 mapel-elections-2.1.8/src/mapel/elections/cultures/to_be_removed/
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/to_be_removed/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/to_be_removed/mallows_urn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.817371 mapel-elections-2.1.8/src/mapel/elections/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/committee_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/cppdistances.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23680 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/ilp_isomorphic.py
--rw-r--r--   0 runner    (1001) docker     (127)    45354 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/main_approval_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances/main_ordinal_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.817371 mapel-elections-2.1.8/src/mapel/elections/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/approx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/banzhaf_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/cohesive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/dependent_rounding.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/diversity.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/justified_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/partylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/power_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/proportionality_degree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/ranging_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features/vc_diversity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.821371 mapel-elections-2.1.8/src/mapel/elections/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/ApprovalElection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/ApprovalElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/Election.py
--rw-r--r--   0 runner    (1001) docker     (127)    29809 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/ElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/ElectionFamily.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/OrdinalElection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/OrdinalElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.821371 mapel-elections-2.1.8/src/mapel/elections/other/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/matrix2png.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/pabulib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/other/winners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.821371 mapel-elections-2.1.8/src/mapel/elections/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/persistence/election_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)    15357 2024-03-23 13:42:07.000000 mapel-elections-2.1.8/src/mapel/elections/persistence/election_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:15.825371 mapel-elections-2.1.8/src/mapel_elections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-23 13:42:15.000000 mapel-elections-2.1.8/src/mapel_elections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-03-23 13:42:15.000000 mapel-elections-2.1.8/src/mapel_elections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:42:15.000000 mapel-elections-2.1.8/src/mapel_elections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-23 13:42:15.000000 mapel-elections-2.1.8/src/mapel_elections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-23 13:42:15.000000 mapel-elections-2.1.8/src/mapel_elections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.117065 mapel_elections-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-15 08:50:18.117065 mapel_elections-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:50:18.117065 mapel_elections-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.101065 mapel_elections-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.101065 mapel_elections-2.1.9/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.101065 mapel_elections-2.1.9/src/mapel/elections/
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.105065 mapel_elections-2.1.9/src/mapel/elections/cultures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/guardians.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/guardians_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/mallows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.105065 mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/group_separable_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/single_crossing_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/single_peaked_matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.105065 mapel_elections-2.1.9/src/mapel/elections/cultures/nonstandard/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/nonstandard/alliances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/nonstandard/field_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/nonstandard/parties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/preflib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.105065 mapel_elections-2.1.9/src/mapel/elections/cultures/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/sampling/samplemat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.105065 mapel_elections-2.1.9/src/mapel/elections/cultures/to_be_removed/
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/to_be_removed/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/to_be_removed/mallows_urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.109065 mapel_elections-2.1.9/src/mapel/elections/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/committee_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/cppdistances.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/feature_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23680 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/ilp_isomorphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45354 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/main_approval_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/main_ordinal_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances/positionwise_infty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.109065 mapel_elections-2.1.9/src/mapel/elections/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/banzhaf_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/cohesive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/dap_approximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/dependent_rounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/justified_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/partylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/power_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/proportionality_degree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/ranging_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features/vc_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.113065 mapel_elections-2.1.9/src/mapel/elections/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/ApprovalElection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/ApprovalElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15343 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/Election.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/ElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/ElectionFamily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/ElectionFeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/OrdinalElection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/OrdinalElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.113065 mapel_elections-2.1.9/src/mapel/elections/other/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/matrix2png.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/pabulib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12737 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/other/winners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.113065 mapel_elections-2.1.9/src/mapel/elections/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/persistence/election_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15357 2024-04-15 08:50:09.000000 mapel_elections-2.1.9/src/mapel/elections/persistence/election_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:18.113065 mapel_elections-2.1.9/src/mapel_elections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-15 08:50:18.000000 mapel_elections-2.1.9/src/mapel_elections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-15 08:50:18.000000 mapel_elections-2.1.9/src/mapel_elections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:50:18.000000 mapel_elections-2.1.9/src/mapel_elections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 08:50:18.000000 mapel_elections-2.1.9/src/mapel_elections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 08:50:18.000000 mapel_elections-2.1.9/src/mapel_elections.egg-info/top_level.txt
```

### Comparing `mapel-elections-2.1.8/LICENSE.txt` & `mapel_elections-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/PKG-INFO` & `mapel_elections-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-elections
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Elections
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-elections-2.1.8/README.md` & `mapel_elections-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/pyproject.toml` & `mapel_elections-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-elections"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Piotr Faliszewski", email = "faliszew@agh.edu.pl"},
  {name = "Lukasz Janeczko", email = "lukij1997@gmail.com"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/__init__.py` & `mapel_elections-2.1.9/src/mapel/elections/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/fake.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/fake.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/group_separable.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/guardians.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/guardians.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/guardians_plus.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/guardians_plus.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/mallows.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/group_separable_matrices.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/group_separable_matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/single_crossing_matrices.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/single_crossing_matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/matrices/single_peaked_matrices.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/matrices/single_peaked_matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/nonstandard/alliances.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/nonstandard/alliances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/nonstandard/field_experiment.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/nonstandard/field_experiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/params.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/params.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/preflib.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/preflib.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/sampling/samplemat.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/sampling/samplemat.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/to_be_removed/euclidean.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/to_be_removed/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/to_be_removed/mallows_urn.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/to_be_removed/mallows_urn.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/unused.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/unused.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures/urn.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures/urn.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,10 +5,11 @@
 def truncated_urn_mask(num_voters=None,
                        num_candidates=None,
                        p=None,
                        alpha=None,
                        **kwargs):
     return pref_approval.truncated_ordinal(num_voters=num_voters,
                                            num_candidates=num_candidates,
-                                           p=p,
+                                           rel_num_approvals=p,
                                            ordinal_sampler=pref_ordinal.urn,
-                                           ordinal_sampler_parameters={'alpha': alpha})
+                                           ordinal_sampler_parameters={'alpha': alpha},
+                                           **kwargs)
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/cultures_.py` & `mapel_elections-2.1.9/src/mapel/elections/cultures_.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 from mapel.elections.cultures.nonstandard.alliances import *
 import mapel.elections.cultures.nonstandard.field_experiment as fe
 from mapel.elections.cultures.preflib import generate_preflib_votes
 
 import mapel.elections.cultures.group_separable as group_separable
 import mapel.elections.cultures.euclidean as euclidean
 import mapel.elections.cultures.urn as urn
+import mapel.elections.cultures.identity as identity
 
 import prefsampling.ordinal as pref_ordinal
 import prefsampling.approval as pref_approval
 
 registered_approval_cultures = {
     'impartial': pref_approval.impartial,
     'impartial_culture': pref_approval.impartial,
     'ic': pref_approval.impartial,
-    'id': pref_approval.identity,
+    'id': identity.identity_mask,
+
     'resampling': pref_approval.resampling,
     'disjoint_resampling': pref_approval.disjoint_resampling,
     'moving_resampling': pref_approval.moving_resampling,
     'noise': pref_approval.noise,
-    'euclidean': pref_approval.euclidean,
+    'euclidean': euclidean.euclidean_app_mask,
     'full': pref_approval.full,
     'empty': pref_approval.empty,
     'truncated_urn': urn.truncated_urn_mask,
     'urn_partylist': pref_approval.urn_partylist,
 
     'field': fe.generate_approval_field_votes,  # unsupported culture
     'truncated_mallows': mallows.generate_approval_truncated_mallows_votes,  # unsupported culture
@@ -63,15 +65,15 @@
     'walsh': pref_ordinal.single_peaked_walsh,
     'spoc': pref_ordinal.single_peaked_circle,
     'stratification': pref_ordinal.stratification,
     'mallows': pref_ordinal.mallows,
     'didi': pref_ordinal.didi,
 
     'group-separable': group_separable.gs_mask,
-    'euclidean': euclidean.euclidean_mask,
+    'euclidean': euclidean.euclidean_ord_mask,
 
     'norm-mallows': mallows.generate_mallows_votes,
     'real_identity': guardians.generate_real_identity_votes,
 
     'plackett-luce': pref_ordinal.plackett_luce,
 
     'mallows_urn': mallows_urn.generate_mallows_urn_votes,
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances/committee_distances.py` & `mapel_elections-2.1.9/src/mapel/elections/distances/committee_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances/cppdistances.cpp` & `mapel_elections-2.1.9/src/mapel/elections/distances/cppdistances.cpp`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances/ilp_isomorphic.py` & `mapel_elections-2.1.9/src/mapel/elections/distances/ilp_isomorphic.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances/lp.py` & `mapel_elections-2.1.9/src/mapel/elections/distances/lp.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances/main_approval_distances.py` & `mapel_elections-2.1.9/src/mapel/elections/distances/main_approval_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances/main_ordinal_distances.py` & `mapel_elections-2.1.9/src/mapel/elections/distances/main_ordinal_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/distances_.py` & `mapel_elections-2.1.9/src/mapel/elections/distances_.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 from tqdm import tqdm
 
 import mapel.core.persistence.experiment_exports as exports
 from mapel.core.inner_distances import map_str_to_func
 from mapel.core.objects.Experiment import Experiment
 from mapel.elections.distances import main_approval_distances as mad
 from mapel.elections.distances import main_ordinal_distances as mod
+from mapel.elections.distances import positionwise_infty
+from mapel.elections.distances import feature_distance
 from mapel.elections.objects.ApprovalElection import ApprovalElection
 from mapel.elections.objects.OrdinalElection import OrdinalElection
 
 registered_approval_distances = {
     'approvalwise': mad.compute_approvalwise,
 
     'hamming': mad.compute_hamming,  # unsupported distance
 }
 
 registered_ordinal_distances = {
+    'positionwise_infty': positionwise_infty.positionwise_size_independent,
+    'feature_l1': feature_distance.features_vector_l1,
+    'feature_l2': feature_distance.features_vector_l2,
     'positionwise': mod.compute_positionwise_distance,
     'bordawise': mod.compute_bordawise_distance,
     'pairwise': mod.compute_pairwise_distance,
     'discrete': mod.compute_discrete_distance,
 
     'swap': mod.compute_swap_distance,
     'spearman': mod.compute_spearman_distance,
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/approx.py` & `mapel_elections-2.1.9/src/mapel/elections/features/approx.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/banzhaf_cc.py` & `mapel_elections-2.1.9/src/mapel/elections/features/banzhaf_cc.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/clustering.py` & `mapel_elections-2.1.9/src/mapel/elections/features/clustering.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/cohesive.py` & `mapel_elections-2.1.9/src/mapel/elections/features/cohesive.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/dependent_rounding.py` & `mapel_elections-2.1.9/src/mapel/elections/features/dependent_rounding.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/dimensionality.py` & `mapel_elections-2.1.9/src/mapel/elections/features/dimensionality.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/distortion.py` & `mapel_elections-2.1.9/src/mapel/elections/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/diversity.py` & `mapel_elections-2.1.9/src/mapel/elections/features/diversity.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/justified_representation.py` & `mapel_elections-2.1.9/src/mapel/elections/features/justified_representation.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/other.py` & `mapel_elections-2.1.9/src/mapel/elections/features/other.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/partylist.py` & `mapel_elections-2.1.9/src/mapel/elections/features/partylist.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/power_index.py` & `mapel_elections-2.1.9/src/mapel/elections/features/power_index.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/proportionality_degree.py` & `mapel_elections-2.1.9/src/mapel/elections/features/proportionality_degree.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/ranging_cc.py` & `mapel_elections-2.1.9/src/mapel/elections/features/ranging_cc.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/scores.py` & `mapel_elections-2.1.9/src/mapel/elections/features/scores.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features/vc_diversity.py` & `mapel_elections-2.1.9/src/mapel/elections/features/vc_diversity.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/features_.py` & `mapel_elections-2.1.9/src/mapel/elections/features_.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import mapel.elections.features.approx as approx
 import mapel.elections.features.banzhaf_cc as banzhaf_cc
 import mapel.elections.features.clustering as clustering
 import mapel.elections.features.cohesive as cohesive
 import mapel.elections.features.dimensionality as dimensionality
 import mapel.elections.features.distortion as distortion
 import mapel.elections.features.diversity as diversity
+import mapel.elections.features.entropy as entropy
+import mapel.elections.features.dap_approximate as dap_approx
 import mapel.elections.features.justified_representation as jr
 import mapel.elections.features.other as other
 import mapel.elections.features.partylist as partylist
 import mapel.elections.features.proportionality_degree as prop_deg
 import mapel.elections.features.ranging_cc as ranging_cc
 import mapel.elections.features.scores as scores
 import mapel.elections.features.vc_diversity as vcd
@@ -78,18 +80,21 @@
     'support_diversity_summed': diversity.support_diversity_summed,
     'support_diversity_normed_summed': diversity.support_diversity_normed_summed,
     'support_diversity_normed2_summed': diversity.support_diversity_normed2_summed,
     'support_diversity_normed3_summed': diversity.support_diversity_normed3_summed,
     'dist_to_Borda_mean': diversity.dist_to_Borda_mean,
     'dist_to_Kemeny_mean': diversity.dist_to_Kemeny_mean,
     'borda_spread': scores.borda_spread,
+    'Entropy': entropy.entropy,
     'Agreement': diversity.agreement_index,
     'Diversity': diversity.diversity_index,
     'Polarization': diversity.polarization_index,
-
+    'AgreementApprox': dap_approx.agreement_index,
+    'DiversityApprox': dap_approx.diversity_index,
+    'PolarizationApprox': dap_approx.polarization_index,
     'avg_distortion_from_guardians': distortion.avg_distortion_from_guardians,
     # unsupported feature
     'worst_distortion_from_guardians': distortion.worst_distortion_from_guardians,
     # unsupported feature
     'abstract': other.abstract,  # unsupported feature
     'distortion': distortion,  # unsupported feature
     'monotonicity_triplets': distortion.monotonicity_triplets,  # unsupported feature
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/ApprovalElection.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/ApprovalElection.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/ApprovalElectionExperiment.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/ApprovalElectionExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/Election.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/Election.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from abc import abstractmethod
 
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.linalg as la
 from sklearn.manifold import MDS
 
+from mapel.elections.objects.ElectionFeatures import ElectionFeatures
 import mapel.elections.persistence.election_exports as exports
 import mapel.elections.persistence.election_imports as imports
 from mapel.core.glossary import *
 from mapel.core.inner_distances import l2
 from mapel.core.objects.Instance import Instance
 from mapel.elections.features_ import get_local_feature
 from mapel.elections.other.winners import compute_sntv_winners, compute_borda_winners, \
@@ -60,14 +61,15 @@
         self.potes = None
         self.features = {}
         self.object_type = 'vote'
         self.points = {}
         self.is_shifted = is_shifted
         self.is_imported = is_imported
         self.fast_import = fast_import
+        self.election_features = ElectionFeatures(election_id)
 
         self.import_distances()
         self.import_coordinates()
 
     def import_distances(self):
         """
         Import distances from a .csv file.
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/ElectionExperiment.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/ElectionExperiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from abc import ABCMeta, abstractmethod
 from multiprocessing import Process
 from time import sleep
 import ast
 import time
 from tqdm import tqdm
 
+from mapel.elections.objects.ElectionFeatures import ST_KEY, AN_KEY, ID_KEY, UN_KEY
 from mapel.elections.objects.ElectionFamily import ElectionFamily
 from mapel.elections.objects.OrdinalElection import OrdinalElection
 from mapel.elections.objects.ApprovalElection import ApprovalElection
 import mapel.elections.distances_ as metr
 import mapel.elections.other.rules as rules
 import mapel.elections.features_ as features
 from mapel.core.objects.Experiment import Experiment
@@ -728,16 +729,75 @@
                 experiment_id=self.experiment_id, rule_name=rule_name)
 
     def add_election_to_family(self, election=None, family_id=None):
         election.instance_id = f'{self.families[family_id]}_{self.families[family_id].size}'
         self.instances[election.instance_id] = election
         self.families[family_id].add_election(election)
 
+    def prepare_election_features(self):
+        for election in self.instances.items():
+            election[1].election_features.votes = election[1].votes
+            election[1].election_features.num_candidates = election[1].num_candidates
+            election[1].election_features.num_voters = election[1].num_voters
+            election[1].election_features.calculate_all()
+
+    def prepare_compass_dictionary(self):
+        for election in self.instances.items():
+            election[1].election_features.votes = election[1].votes
+            election[1].election_features.num_candidates = election[1].num_candidates
+            election[1].election_features.num_voters = election[1].num_voters
+            election[1].election_features.compass_points['ST'] = self.instances[
+                ST_KEY + str(election[1].num_candidates)]
+            election[1].election_features.compass_points['AN'] = self.instances[
+                AN_KEY + str(election[1].num_candidates)]
+            election[1].election_features.compass_points['ID'] = self.instances[
+                ID_KEY + str(election[1].num_candidates)]
+            election[1].election_features.compass_points['UN'] = self.instances[
+                UN_KEY + str(election[1].num_candidates)]
+
+    def calculate_dap(self, id):
+        dap = list()
+        dap.append(self.features['Diversity'][id])
+        dap.append(self.features['Agreement'][id])
+        dap.append(self.features['Polarization'][id])
+        return dap
+
+    def calculate_features_vector(self, id, features_list: list):
+        vector = list()
+        if 'd' in features_list:
+            vector.append(self.features['Diversity'][id])
+        if 'a' in features_list:
+            vector.append(self.features['Agreement'][id])
+        if 'p' in features_list:
+            vector.append(self.features['Polarization'][id])
+        if 'e' in features_list:
+            vector.append(self.features['Entropy'][id])
+        if 'e2' in features_list:
+            vector.append(self.features['Entropy'][id] * self.features['Entropy'][id])
+        if 'cds' in features_list:
+            vector.append(self.features['CandidateDistanceStd'][id])
+        return vector
+
+    def prepare_election_sizes(self):
+        for election in self.instances.items():
+            self.election_sizes.add(election[1].num_candidates)
+
+    def prepare_feature_vectors(self, features: list):
+        for election in self.instances.items():
+            election[1].election_features.votes = election[1].votes
+            election[1].election_features.num_candidates = election[1].num_candidates
+            election[1].election_features.num_voters = election[1].num_voters
+            election[1].election_features.features_vector = self.calculate_features_vector(election[1].election_id,
+                                                                                           features)
+
 
 def check_if_all_equal(values, subject):
     if any(x != values[0] for x in values):
         text = f'Not all {subject} values are equal!'
         warnings.warn(text)
 
+
+
+
 # # # # # # # # # # # # # # # #
 # LAST CLEANUP ON: 22.10.2021 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/ElectionFamily.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/ElectionFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/OrdinalElection.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/OrdinalElection.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/objects/OrdinalElectionExperiment.py` & `mapel_elections-2.1.9/src/mapel/elections/objects/OrdinalElectionExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/matrices.py` & `mapel_elections-2.1.9/src/mapel/elections/other/matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/matrix2png.py` & `mapel_elections-2.1.9/src/mapel/elections/other/matrix2png.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/pabulib.py` & `mapel_elections-2.1.9/src/mapel/elections/other/pabulib.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/parser.py` & `mapel_elections-2.1.9/src/mapel/elections/other/parser.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/rules.py` & `mapel_elections-2.1.9/src/mapel/elections/other/rules.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/utilities.py` & `mapel_elections-2.1.9/src/mapel/elections/other/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,35 +18,37 @@
     mallows_params_phi: custom phis that will be added into the csv file
     mallows_params_colors: colors of corresponding custom phis for Mallows elections
     incl_euclidean: bool whether euclidean cultures should be included
     incl_extremes: bool whether UN, AN, ID and IDAN should be included
 
 """
 
+
 def generate_mapcsv_contents(*args, **kwargs):
     candidates = [8, 9, 10, 11, 12]
     alphas = [0.2, 0.4, 0.6, 0.8, 1]
     family_size = 10
     urn_family_size = 10
     mallows_family_size = 10
     num_voters = 100
-    file_name = "map.txt"
+    file_name = "map.csv"
     incl_ic = True
     incl_iac = False
     incl_urn = True
     incl_conitzer = True
     incl_walsh = True
     incl_sc = True
     incl_spoc = True
     incl_mallows_default = True
     incl_mallows_custom = False
     mallows_params_phi = None
     mallows_params_colors = None
     incl_euclidean = True
     incl_extremes = True
+    incl_group_separable = True
 
     for key, val in kwargs.items():
         if key == "candidates":
             candidates = val
         elif key == "alphas":
             alphas = val
         elif key == "family_size":
@@ -76,14 +78,16 @@
             mallows_params_phi = val
         elif key == "mallows_params_colors":
             mallows_params_colors = val
         elif key == "incl_euclidean":
             incl_euclidean = val
         elif key == "incl_extremes":
             incl_extremes = val
+        elif key == "incl_group_separable":
+            incl_group_separable = val
         else:
             print("Optional argument \"", key, "\" does not exist.")
 
     if incl_mallows_custom is True and (mallows_params_phi is None or mallows_params_colors is None):
         incl_mallows_custom = False
         print("Missing parameter values for custom mallows, so no custom mallows will be added.")
 
@@ -104,16 +108,18 @@
             file.write(iac_string)
 
         if incl_urn:
             urn_alpha = [0.01, 0.02, 0.05, 0.1, 0.5]
             urn_alpha_color = ['palegoldenrod', 'yellow', 'gold', 'orange', 'red']
             for j in range(0, len(urn_alpha)):
                 urn_string = str(urn_family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "urn" + ";" + "{'alpha': " + str(urn_alpha[j]) + "}" + ";" + str(urn_alpha_color[j]) + ";" + str(
-                alphas[i]) + ";" + "urn" + str(candidates[i]) + '-' + str(urn_alpha[j]) + ";" + "o" + ";" + "{}" + ";" + "Urn-" + str(urn_alpha[j]) + "\n"
+                    num_voters) + ";" + "urn" + ";" + "{'alpha': " + str(urn_alpha[j]) + "}" + ";" + str(
+                    urn_alpha_color[j]) + ";" + str(
+                    alphas[i]) + ";" + "urn" + str(candidates[i]) + '-' + str(
+                    urn_alpha[j]) + ";" + "o" + ";" + "{}" + ";" + "Urn-" + str(urn_alpha[j]) + "\n"
                 file.write(urn_string)
 
         if incl_conitzer:
             conitzer_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
                 num_voters) + ";" + "conitzer" + ";" + "{}" + ";" + "saddlebrown" + ";" + str(
                 alphas[i]) + ";" + "conitzer" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "SP-Conitzer \n"
@@ -134,81 +140,97 @@
             file.write(singlecrossing_string)
 
         if incl_mallows_default:
             phis = [0.001, 0.01, 0.1, 0.5, 0.75, 0.99]
             phis_colors = ['paleturquoise', 'skyblue', 'dodgerblue', 'cornflowerblue', 'blue', 'navy']
             for j in range(0, len(phis)):
                 mallows_string = str(mallows_family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "norm-mallows" + ";" + "{'normphi':" + str(phis[j]) + "}" + ";" + phis_colors[j] + ";" + str(
-                alphas[i]) + ";" + "norm-mallows-" + str(candidates[i]) + '-' + str(phis[j]) + ";" + "o" + ";" + "{}" + ";" + "Norm-Mallows-" + str(phis[j]) + "\n"
+                    num_voters) + ";" + "norm-mallows" + ";" + "{'normphi':" + str(phis[j]) + "}" + ";" + phis_colors[
+                                     j] + ";" + str(
+                    alphas[i]) + ";" + "norm-mallows-" + str(candidates[i]) + '-' + str(
+                    phis[j]) + ";" + "o" + ";" + "{}" + ";" + "Norm-Mallows-" + str(phis[j]) + "\n"
                 file.write(mallows_string)
 
         if incl_mallows_custom:
             for j in range(0, len(mallows_params_phi)):
                 mallows_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                    num_voters) + ";" + "norm-mallows" + ";" + "{'normphi': " + str(mallows_params_phi[j]) +"}" + ";" + mallows_params_colors[j] + ";" + str(
+                    num_voters) + ";" + "norm-mallows" + ";" + "{'normphi': " + str(mallows_params_phi[j]) + "}" + ";" + \
+                                 mallows_params_colors[j] + ";" + str(
                     alphas[i]) + ";" + "norm-mallows" + str(candidates[i]) + str(
-                    mallows_params_phi[j]) + ";" + "x" + ";" + "{}" + ";" + "Norm-Mallows-" +str(mallows_params_phi[j]) +"\n"
+                    mallows_params_phi[j]) + ";" + "x" + ";" + "{}" + ";" + "Norm-Mallows-" + str(
+                    mallows_params_phi[j]) + "\n"
                 file.write(mallows_string)
 
         if incl_spoc:
             spoc_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "spoc_conitzer" + ";" + "{}" + ";" + "firebrick" + ";" + str(
-                alphas[i]) + ";" + "spoc_conitzer" + str(
+                num_voters) + ";" + "spoc" + ";" + "{}" + ";" + "firebrick" + ";" + str(
+                alphas[i]) + ";" + "spoc" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "SPOC \n"
             file.write(spoc_string)
 
-
         if incl_euclidean:
             euclidean_1_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 1, 'space': 'uniform'}" + ";" + "lime" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 1, 'space': 'uniform'}" + ";" + "lime" + ";" + str(
                 alphas[i]) + ";" + "Interval" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "1D Interval \n"
             euclidean_2_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 2, 'space': 'uniform'}" + ";" + "green" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 2, 'space': 'uniform'}" + ";" + "green" + ";" + str(
                 alphas[i]) + ";" + "Square" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "Square \n"
             euclidean_3_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 3, 'space': 'uniform'}" + ";" + "forestgreen" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 3, 'space': 'uniform'}" + ";" + "forestgreen" + ";" + str(
                 alphas[i]) + ";" + "Cube" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "3-Cube \n"
             euclidean_5_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 5, 'space': 'uniform'}" + ";" + "palegreen" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 5, 'space': 'uniform'}" + ";" + "palegreen" + ";" + str(
                 alphas[i]) + ";" + "5-Cube" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "5-Cube \n"
             euclidean_10_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 10, 'space': 'uniform'}" + ";" + "yellowgreen" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 10, 'space': 'uniform'}" + ";" + "yellowgreen" + ";" + str(
                 alphas[i]) + ";" + "10-Cube" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "10-Cube \n"
             euclidean_2_sphere_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 2, 'space': 'sphere'}" + ";" + "deeppink" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 2, 'space': 'sphere'}" + ";" + "deeppink" + ";" + str(
                 alphas[i]) + ";" + "Circle" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "Circle \n"
             euclidean_3_sphere_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
-                num_voters) + ";" + "euclidean" + ";" + "{'dim': 3, 'space': 'sphere'}" + ";" + "lightpink" + ";" + str(
+                num_voters) + ";" + "euclidean" + ";" + "{'dimension': 3, 'space': 'sphere'}" + ";" + "lightpink" + ";" + str(
                 alphas[i]) + ";" + "Sphere" + str(
                 candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "Sphere \n"
             file.write(euclidean_1_string)
             file.write(euclidean_2_string)
             file.write(euclidean_3_string)
             file.write(euclidean_5_string)
             file.write(euclidean_10_string)
             file.write(euclidean_2_sphere_string)
             file.write(euclidean_3_sphere_string)
 
+        if incl_group_separable:
+            balanced_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
+                num_voters) + ";" + "group-separable" + ";" + "{\'tree_sampler\' : \'balanced\'}" + ";" + "purple" + ";" + str(
+                alphas[i]) + ";" + "group-separable" + str(
+                candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "GS-Balanced \n"
+            caterpillar_string = str(family_size) + ";" + str(candidates[i]) + ";" + str(
+                num_voters) + ";" + "group-separable" + ";" + "{\'tree_sampler\' : \'caterpillar\'}" + ";" + "violet" + ";" + str(
+                alphas[i]) + ";" + "group-separable" + str(
+                candidates[i]) + ";" + "o" + ";" + "{}" + ";" + "GS-Caterpillar \n"
+            file.write(balanced_string)
+            file.write(caterpillar_string)
+
     if incl_extremes:
         st_string = '1' + ';' + str(15) + ';' + '50' + ';real_stratification;{};black;' + str(1) + ';ST;x;{};ST \n'
         un_string = '1' + ';' + str(15) + ';' + '50' + ';un_from_matrix;{};black;' + str(1) + ';UN;x;{};UN \n'
         id_string = '1' + ';' + str(15) + ';' + '50' + ';real_identity;{};rosybrown;' + str(1) + ';ID;x;{};ID \n'
         an_string = '1' + ';' + str(15) + ';' + '50' + ';real_antagonism;{};royalblue;' + str(1) + ';AN;x;{};AN \n'
-        idan_string = '4' + ';' + str(15) + ';' + '50' + ';idan_part;{};midnightblue;' + str(1) + ';IDAN;x;{\'variable\' : \'part_share\'};IDAN \n'
+        idan_string = '4' + ';' + str(15) + ';' + '50' + ';idan_part;{};midnightblue;' + str(
+            1) + ';IDAN;x;{\'variable\' : \'part_share\'};IDAN \n'
         file.write(st_string)
         file.write(un_string)
         file.write(id_string)
         file.write(an_string)
-        file.write(idan_string)
+        # file.write(idan_string)
 
     file.close()
 
 
 if __name__ == "__main__":
-    generate_mapcsv_contents()
+    generate_mapcsv_contents(file_name="mymap.csv")
```

### Comparing `mapel-elections-2.1.8/src/mapel/elections/other/winners.py` & `mapel_elections-2.1.9/src/mapel/elections/other/winners.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/persistence/election_exports.py` & `mapel_elections-2.1.9/src/mapel/elections/persistence/election_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel/elections/persistence/election_imports.py` & `mapel_elections-2.1.9/src/mapel/elections/persistence/election_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.1.8/src/mapel_elections.egg-info/PKG-INFO` & `mapel_elections-2.1.9/src/mapel_elections.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-elections
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Elections
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-elections-2.1.8/src/mapel_elections.egg-info/SOURCES.txt` & `mapel_elections-2.1.9/src/mapel_elections.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/mapel/elections/cultures/__init__.py
 src/mapel/elections/cultures/converters.py
 src/mapel/elections/cultures/euclidean.py
 src/mapel/elections/cultures/fake.py
 src/mapel/elections/cultures/group_separable.py
 src/mapel/elections/cultures/guardians.py
 src/mapel/elections/cultures/guardians_plus.py
+src/mapel/elections/cultures/identity.py
 src/mapel/elections/cultures/mallows.py
 src/mapel/elections/cultures/params.py
 src/mapel/elections/cultures/preflib.py
 src/mapel/elections/cultures/unused.py
 src/mapel/elections/cultures/urn.py
 src/mapel/elections/cultures/matrices/group_separable_matrices.py
 src/mapel/elections/cultures/matrices/single_crossing_matrices.py
@@ -28,40 +29,45 @@
 src/mapel/elections/cultures/nonstandard/parties.py
 src/mapel/elections/cultures/sampling/samplemat.py
 src/mapel/elections/cultures/to_be_removed/euclidean.py
 src/mapel/elections/cultures/to_be_removed/mallows_urn.py
 src/mapel/elections/distances/__init__.py
 src/mapel/elections/distances/committee_distances.py
 src/mapel/elections/distances/cppdistances.cpp
+src/mapel/elections/distances/feature_distance.py
 src/mapel/elections/distances/ilp_isomorphic.py
 src/mapel/elections/distances/lp.py
 src/mapel/elections/distances/main_approval_distances.py
 src/mapel/elections/distances/main_ordinal_distances.py
+src/mapel/elections/distances/positionwise_infty.py
 src/mapel/elections/features/__init__.py
 src/mapel/elections/features/approx.py
 src/mapel/elections/features/banzhaf_cc.py
 src/mapel/elections/features/clustering.py
 src/mapel/elections/features/cohesive.py
+src/mapel/elections/features/dap_approximate.py
 src/mapel/elections/features/dependent_rounding.py
 src/mapel/elections/features/dimensionality.py
 src/mapel/elections/features/distortion.py
 src/mapel/elections/features/diversity.py
+src/mapel/elections/features/entropy.py
 src/mapel/elections/features/justified_representation.py
 src/mapel/elections/features/other.py
 src/mapel/elections/features/partylist.py
 src/mapel/elections/features/power_index.py
 src/mapel/elections/features/proportionality_degree.py
 src/mapel/elections/features/ranging_cc.py
 src/mapel/elections/features/scores.py
 src/mapel/elections/features/vc_diversity.py
 src/mapel/elections/objects/ApprovalElection.py
 src/mapel/elections/objects/ApprovalElectionExperiment.py
 src/mapel/elections/objects/Election.py
 src/mapel/elections/objects/ElectionExperiment.py
 src/mapel/elections/objects/ElectionFamily.py
+src/mapel/elections/objects/ElectionFeatures.py
 src/mapel/elections/objects/OrdinalElection.py
 src/mapel/elections/objects/OrdinalElectionExperiment.py
 src/mapel/elections/objects/__init__.py
 src/mapel/elections/other/__init__.py
 src/mapel/elections/other/matrices.py
 src/mapel/elections/other/matrix2png.py
 src/mapel/elections/other/pabulib.py
```

