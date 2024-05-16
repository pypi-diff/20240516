# Comparing `tmp/arrakis_nd-2.0.1.tar.gz` & `tmp/arrakis_nd-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrakis_nd-2.0.1.tar", last modified: Tue May 14 18:40:41 2024, max compression
+gzip compressed data, was "arrakis_nd-2.0.2.tar", last modified: Thu May 16 16:11:45 2024, max compression
```

## Comparing `arrakis_nd-2.0.1.tar` & `arrakis_nd-2.0.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.471418 arrakis_nd-2.0.1/arrakis_nd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.475418 arrakis_nd-2.0.1/arrakis_nd/arrakis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/arrakis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62970 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/arrakis/arrakis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/arrakis/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.475418 arrakis_nd-2.0.1/arrakis_nd/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/dataset/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.479418 arrakis_nd-2.0.1/arrakis_nd/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/ancestor_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/blip_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/constraint_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/daughter_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/delta_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/empty_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/fragment_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/interaction_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/ion_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/michel_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/neutrino_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/neutron_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/parent_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/particle_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/photon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/proton_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/segment_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/shower_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/track_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/plugins/trackid_hit_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.479418 arrakis_nd-2.0.1/arrakis_nd/programs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/create_arrakis_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/plugin_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis_display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.479418 arrakis_nd-2.0.1/arrakis_nd/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/arrakis_nd/utils/display/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/arrakis_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/charge_light_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/marjolein_2x2_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/set_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    19024 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/display/vis_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/shower_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/track_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/arrakis_nd/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/arrakis_nd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 18:40:41.000000 arrakis_nd-2.0.1/arrakis_nd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:40:41.483418 arrakis_nd-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-14 18:40:33.000000 arrakis_nd-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.465163 arrakis_nd-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-16 16:11:45.465163 arrakis_nd-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.453163 arrakis_nd-2.0.2/arrakis_nd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.457163 arrakis_nd-2.0.2/arrakis_nd/arrakis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/arrakis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62970 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/arrakis/arrakis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/arrakis/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.457163 arrakis_nd-2.0.2/arrakis_nd/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/dataset/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.461163 arrakis_nd-2.0.2/arrakis_nd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/ancestor_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/blip_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/constraint_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/daughter_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/delta_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/empty_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/fragment_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/interaction_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/ion_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/michel_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/neutrino_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/neutron_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/parent_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/particle_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12525 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/photon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/proton_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/segment_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/shower_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/track_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/plugins/trackid_hit_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.461163 arrakis_nd-2.0.2/arrakis_nd/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/programs/create_arrakis_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/programs/plugin_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/programs/run_arrakis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/programs/run_arrakis_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.465163 arrakis_nd-2.0.2/arrakis_nd/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.465163 arrakis_nd-2.0.2/arrakis_nd/utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/arrakis_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/charge_light_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/marjolein_2x2_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/set_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19024 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/display/vis_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/shower_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/track_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/arrakis_nd/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:11:45.465163 arrakis_nd-2.0.2/arrakis_nd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-16 16:11:45.000000 arrakis_nd-2.0.2/arrakis_nd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-16 16:11:45.000000 arrakis_nd-2.0.2/arrakis_nd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:11:45.000000 arrakis_nd-2.0.2/arrakis_nd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-16 16:11:45.000000 arrakis_nd-2.0.2/arrakis_nd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-16 16:11:45.000000 arrakis_nd-2.0.2/arrakis_nd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 16:11:45.000000 arrakis_nd-2.0.2/arrakis_nd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:11:45.465163 arrakis_nd-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-16 16:11:37.000000 arrakis_nd-2.0.2/setup.py
```

### Comparing `arrakis_nd-2.0.1/LICENSE` & `arrakis_nd-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/PKG-INFO` & `arrakis_nd-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrakis_nd
-Version: 2.0.1
+Version: 2.0.2
 Summary: Arrakis module for near detector data.
 Home-page: https://github.com/Neutron-Calibration-in-DUNE/ArrakisND
 Author: Nicholas Carrara, Marjolein van Nuland, Luis Lepin
 Author-email: ncarrara.physics@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `arrakis_nd-2.0.1/README.md` & `arrakis_nd-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/arrakis/arrakis.py` & `arrakis_nd-2.0.2/arrakis_nd/arrakis/arrakis.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/arrakis/common.py` & `arrakis_nd-2.0.2/arrakis_nd/arrakis/common.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/dataset/common.py` & `arrakis_nd-2.0.2/arrakis_nd/dataset/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     Pion0Decay = 1
     PiPlusDecay = 2
     PiMinusDecay = 3
     Kaon0Decay = 4
     KaonShortDecay = 5
     KaonLongDecay = 6
     KaonPlusDecay = 7
-    KaonMinusdecay = 8
+    KaonMinusDecay = 8
     D0Decay = 9
     DPlusDecay = 10
     DMinusDecay = 11
     LambdaDecay = 12
     Sigma0Decay = 13
     SigmaPlusDecay = 14
     SigmaMinusDecay = 15
```

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/ancestor_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/ancestor_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/constraint_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/constraint_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,18 +192,25 @@
                 start_subprocess = trajectories_start_subprocess[traj_index]
                 end_process = trajectories_end_process[traj_index]
                 end_subprocess = trajectories_end_subprocess[traj_index]
                 parent_index = np.where(
                     (trajectories_traj_ids == parent_id) &
                     (trajectories_vertex_ids == vertex_id)
                 )
-                parent_start_process = trajectories_start_process[parent_index]
-                parent_start_subprocess = trajectories_start_subprocess[parent_index]
-                parent_end_process = trajectories_end_process[parent_index]
-                parent_end_subprocess = trajectories_end_subprocess[parent_index]
+                if parent_id != -1:
+                    parent_start_process = trajectories_start_process[parent_index]
+                    parent_start_subprocess = trajectories_start_subprocess[parent_index]
+                    parent_end_process = trajectories_end_process[parent_index]
+                    parent_end_subprocess = trajectories_end_subprocess[parent_index]
+                else:
+                    parent_start_process = -1
+                    parent_start_subprocess = -1
+                    parent_end_process = -1
+                    parent_end_subprocess = -1
+
                 undefined_data = np.array([(
                     event,
                     vertex_id,
                     traj_id,
                     parent_id,
                     pdg_id,
                     parent_pdg_id,
@@ -219,10 +226,10 @@
                     parent_end_process,
                     parent_end_subprocess)],
                     dtype=undefined_data_type
                 )
                 
                 """Add the undefined data to the event products"""
                 event_products['undefined'].append(undefined_data)
-
+                
         """Write changes to arrakis_file"""
         arrakis_file['charge/calib_final_hits/data'][event_indices['charge']] = arrakis_charge
```

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/daughter_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/daughter_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/delta_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/delta_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/empty_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/empty_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/fragment_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/fragment_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/ion_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/ion_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/michel_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/michel_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/neutrino_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/neutrino_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/neutron_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/neutron_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/parent_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/parent_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/particle_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/particle_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/photon_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/photon_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/proton_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/proton_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/segment_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/segment_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/shower_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/shower_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/track_plugin.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/track_plugin.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/plugins/trackid_hit_map.py` & `arrakis_nd-2.0.2/arrakis_nd/plugins/trackid_hit_map.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/programs/create_arrakis_runs.py` & `arrakis_nd-2.0.2/arrakis_nd/programs/create_arrakis_runs.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/programs/plugin_creator.py` & `arrakis_nd-2.0.2/arrakis_nd/programs/plugin_creator.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis.py` & `arrakis_nd-2.0.2/arrakis_nd/programs/run_arrakis.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/programs/run_arrakis_display.py` & `arrakis_nd-2.0.2/arrakis_nd/programs/run_arrakis_display.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/config.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/config.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/display/arrakis_display.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/display/arrakis_display.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/display/charge_light_display.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/display/charge_light_display.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/display/marjolein_2x2_display.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/display/marjolein_2x2_display.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/display/set_server.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/display/set_server.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/display/utils.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/display/utils.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/display/vis_event.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/display/vis_event.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/geometry.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/logger.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/logger.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/shower_utils.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/shower_utils.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/track_utils.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/track_utils.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd/utils/utils.py` & `arrakis_nd-2.0.2/arrakis_nd/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd.egg-info/PKG-INFO` & `arrakis_nd-2.0.2/arrakis_nd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrakis_nd
-Version: 2.0.1
+Version: 2.0.2
 Summary: Arrakis module for near detector data.
 Home-page: https://github.com/Neutron-Calibration-in-DUNE/ArrakisND
 Author: Nicholas Carrara, Marjolein van Nuland, Luis Lepin
 Author-email: ncarrara.physics@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `arrakis_nd-2.0.1/arrakis_nd.egg-info/SOURCES.txt` & `arrakis_nd-2.0.2/arrakis_nd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/arrakis_nd.egg-info/requires.txt` & `arrakis_nd-2.0.2/arrakis_nd.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `arrakis_nd-2.0.1/setup.py` & `arrakis_nd-2.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,23 @@
     long_description = file.read()
 
 # Function to read the list of requirements from requirements.txt
 def read_requirements():
     with open('requirements.txt') as req:
         return req.read().splitlines()
 
+major_version = 2
+minor_version = 0
+maintenance = 2
+
 setup(
     # name
     name="arrakis_nd",
     # current version
-    #   MAJOR VERSION:  02
-    #   MINOR VERSION:  00
-    #   Maintenance:    01
-    version="2.00.01",
+    version=f"{major_version}.{minor_version}.{maintenance}",
     # descriptions
     description="Arrakis module for near detector data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="",
     # my info
     author="Nicholas Carrara, Marjolein van Nuland, Luis Lepin",
```

