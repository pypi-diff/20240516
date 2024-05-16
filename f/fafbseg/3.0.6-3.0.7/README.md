# Comparing `tmp/fafbseg-3.0.6.tar.gz` & `tmp/fafbseg-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fafbseg-3.0.6.tar", last modified: Tue Apr  9 10:16:56 2024, max compression
+gzip compressed data, was "fafbseg-3.0.7.tar", last modified: Thu May 16 08:52:49 2024, max compression
```

## Comparing `fafbseg-3.0.6.tar` & `fafbseg-3.0.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.660322 fafbseg-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 10:16:52.000000 fafbseg-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 10:16:52.000000 fafbseg-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-09 10:16:56.660322 fafbseg-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 10:16:52.000000 fafbseg-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.636321 fafbseg-3.0.6/fafbseg/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.648321 fafbseg-3.0.6/fafbseg/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2425791 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/JFRC2NP.surf.fw.zip
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  6675604 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/global_area_ids.npy.zip
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/ngl_scenes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/volume_name_dict.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.652322 fafbseg-3.0.6/fafbseg/flywire/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/_synapses_spine.py
--rw-r--r--   0 runner    (1001) docker     (127)    91430 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.652322 fafbseg-3.0.6/fafbseg/flywire/blender/
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/blender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.652322 fafbseg-3.0.6/fafbseg/flywire/blender/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/blender/templates/blender_render.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    34585 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/l2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    63928 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/skeletonize.py
--rw-r--r--   0 runner    (1001) docker     (127)    58689 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/synapses.py
--rw-r--r--   0 runner    (1001) docker     (127)    26338 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/google/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31298 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/synapses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/move/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/merge_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/spine/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/spine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/spine/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/synapses/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/online.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/transmitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/xform/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/xform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/xform/xform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.660322 fafbseg-3.0.6/fafbseg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:16:56.660322 fafbseg-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 10:16:52.000000 fafbseg-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 08:52:47.000000 fafbseg-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 08:52:47.000000 fafbseg-3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 08:52:49.817164 fafbseg-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-16 08:52:47.000000 fafbseg-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.797164 fafbseg-3.0.7/fafbseg/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.809164 fafbseg-3.0.7/fafbseg/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2425791 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/JFRC2NP.surf.fw.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  6675604 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/global_area_ids.npy.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/ngl_scenes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/volume_name_dict.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/flywire/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/_synapses_spine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91701 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/flywire/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/blender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/flywire/blender/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/blender/templates/blender_render.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    34585 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63928 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/skeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57617 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/synapses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26338 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31298 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/synapses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/move/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/merge_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/spine/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/spine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/spine/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/fafbseg/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/online.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/transmitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/fafbseg/xform/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/xform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/xform/xform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/fafbseg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:52:49.817164 fafbseg-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-16 08:52:47.000000 fafbseg-3.0.7/setup.py
```

### Comparing `fafbseg-3.0.6/LICENSE` & `fafbseg-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/PKG-INFO` & `fafbseg-3.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 3.0.6
+Version: 3.0.7
 Summary: Tools to work with the FlyWire and Google segmentations of the FAFB EM dataset
 Home-page: https://fafbseg-py.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://fafbseg-py.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/fafbseg-py
@@ -73,7 +73,8 @@
 
 ## How to cite
 If you use `fafbseg` for your publication, please cite the two FlyWire papers:
 
 1. "_Whole-brain annotation and multi-connectome cell typing quantifies circuit stereotypy in Drosophila_" Schlegel _et al._, bioRxiv (2023); doi: https://doi.org/10.1101/2023.06.27.546055
 2. "_Neuronal wiring diagram of an adult brain_" Dorkenwald _et al._, bioRxiv (2023); doi: https://doi.org/10.1101/2023.06.27.546656
 
+Depending on what data you used (e.g. neurotransmitter predictions) you might need to cite additional publications. Please see the [Citation Guidelines](https://codex.flywire.ai/about_flywire) on Codex.
```

### Comparing `fafbseg-3.0.6/README.md` & `fafbseg-3.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -31,7 +31,8 @@
 
 ## How to cite
 If you use `fafbseg` for your publication, please cite the two FlyWire papers:
 
 1. "_Whole-brain annotation and multi-connectome cell typing quantifies circuit stereotypy in Drosophila_" Schlegel _et al._, bioRxiv (2023); doi: https://doi.org/10.1101/2023.06.27.546055
 2. "_Neuronal wiring diagram of an adult brain_" Dorkenwald _et al._, bioRxiv (2023); doi: https://doi.org/10.1101/2023.06.27.546656
 
+Depending on what data you used (e.g. neurotransmitter predictions) you might need to cite additional publications. Please see the [Citation Guidelines](https://codex.flywire.ai/about_flywire) on Codex.
```

### Comparing `fafbseg-3.0.6/fafbseg/__init__.py` & `fafbseg-3.0.7/fafbseg/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/data/JFRC2NP.surf.fw.zip` & `fafbseg-3.0.7/fafbseg/data/JFRC2NP.surf.fw.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/data/global_area_ids.npy.zip` & `fafbseg-3.0.7/fafbseg/data/global_area_ids.npy.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/data/ngl_scenes.json` & `fafbseg-3.0.7/fafbseg/data/ngl_scenes.json`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/data/volume_name_dict.json` & `fafbseg-3.0.7/fafbseg/data/volume_name_dict.json`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/__init__.py` & `fafbseg-3.0.7/fafbseg/flywire/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/_synapses_spine.py` & `fafbseg-3.0.7/fafbseg/flywire/_synapses_spine.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/annotations.py` & `fafbseg-3.0.7/fafbseg/flywire/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1539,33 +1539,43 @@
         except ValueError:
             pass
 
     return np.array(mats)
 
 
 @lru_cache
+def _get_github_session():
+    s = requests.Session()
+    if "GITHUB_PAT" in os.environ:
+        s.auth = ('user', 'pass')
+        s.headers.update({'Authorization': f"Bearer {os.environ['GITHUB_PAT']}"})
+
+    return s
+
+
+@lru_cache
 def _get_available_annotation_versions():
     # Get available tags
-    r = requests.get("https://api.github.com/repos/flyconnectome/flywire_annotations/tags")
+    r = _get_github_session().get("https://api.github.com/repos/flyconnectome/flywire_annotations/tags")
     r.raise_for_status()
     return r.json()
 
 
 @lru_cache
 def _get_available_commits():
     # Get available commits
-    r = requests.get("https://api.github.com/repos/flyconnectome/flywire_annotations/commits")
+    r = _get_github_session().get("https://api.github.com/repos/flyconnectome/flywire_annotations/commits")
     r.raise_for_status()
     return r.json()
 
 
 @lru_cache
 def _get_available_branches():
     # Get available tags
-    r = requests.get("https://api.github.com/repos/flyconnectome/flywire_annotations/branches")
+    r = _get_github_session().get("https://api.github.com/repos/flyconnectome/flywire_annotations/branches")
     r.raise_for_status()
     return r.json()
 
 
 def get_user_information(user_ids, field=None, raise_missing=True, dataset=None):
     """Fetch (and cache) user information (name, affiliation, etc.) from their IDs.
```

### Comparing `fafbseg-3.0.6/fafbseg/flywire/blender/__init__.py` & `fafbseg-3.0.7/fafbseg/flywire/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/blender/templates/blender_render.py.template` & `fafbseg-3.0.7/fafbseg/flywire/blender/templates/blender_render.py.template`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/l2.py` & `fafbseg-3.0.7/fafbseg/flywire/l2.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/merge.py` & `fafbseg-3.0.7/fafbseg/flywire/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/meshes.py` & `fafbseg-3.0.7/fafbseg/flywire/meshes.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,15 +358,16 @@
     except ImportError:
         raise ImportError("Meshing requires sparse-cubes:\n  pip3 install sparse-cubes")
 
     from .segmentation import get_voxels
 
     # Get voxels for this neuron
     vxl = get_voxels(
-        x, mip=mip, thin=thin, bounds=bounds, progress=progress, dataset=dataset
+        x, mip=mip, thin=thin, bounds=bounds, progress=progress, dataset=dataset,
+        use_mirror=False,  threads=10
     )
 
     vol = get_cloudvolume(dataset)
     spacing = vol.scales[mip]["resolution"]
 
     mesh = sc.marching_cubes(vxl, spacing=spacing)
```

### Comparing `fafbseg-3.0.6/fafbseg/flywire/neuroglancer.py` & `fafbseg-3.0.7/fafbseg/flywire/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/segmentation.py` & `fafbseg-3.0.7/fafbseg/flywire/segmentation.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/skeletonize.py` & `fafbseg-3.0.7/fafbseg/flywire/skeletonize.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/flywire/synapses.py` & `fafbseg-3.0.7/fafbseg/flywire/synapses.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,15 +513,15 @@
             # nb there is a bug in CAVE which causes empty results if we don't
             # ask for supervoxels
             select_columns=columns + sv_cols,
         )
     elif filtered:
         func = partial(
             retry(client.materialize.query_view),
-            view_name="valid_synapses_nt_v2_view",
+            view_name="valid_synapses_nt_np_v6",
             materialization_version=materialization,
             split_positions=True,
             select_columns=columns,
         )
     else:
         func = partial(
             retry(client.materialize.query_table),
@@ -827,24 +827,21 @@
             columns = ["pre_pt_root_id", "post_pt_root_id", "n_syn"]
             func = partial(
                 retry(client.materialize.query_view),
                 view_name="valid_connection_v2",
                 select_columns=columns,
                 materialization_version=materialization,
             )
-            filtered = False  # Set to false since we don't need the join
         else:
             func = partial(
-                retry(client.materialize.join_query),
-                tables=[
-                    [client.materialize.synapse_table, "id"],
-                    ["valid_synapses_nt_v2", "target_id"],
-                ],
+                retry(client.materialize.query_view),
+                view_name="valid_synapses_nt_np_v6",
                 materialization_version=materialization,
-                select_columns={client.materialize.synapse_table: columns},
+                split_positions=True,
+                select_columns=columns,
             )
     else:
         func = partial(
             retry(client.materialize.query_table),
             table=client.materialize.synapse_table,
             materialization_version=materialization,
             select_columns=columns,
@@ -857,25 +854,17 @@
         batch_size,
         desc="Fetching adjacency",
         disable=not progress or len(sources) <= batch_size,
     ):
         source_batch = sources[i : i + batch_size]
         for k in range(0, len(targets), batch_size):
             target_batch = targets[k : k + batch_size]
-
-            if not filtered or materialization == "live":
-                filter_in_dict = dict(
-                    post_pt_root_id=target_batch, pre_pt_root_id=source_batch
-                )
-            else:
-                filter_in_dict = dict(
-                    synapses_nt_v1=dict(
-                        post_pt_root_id=target_batch, pre_pt_root_id=source_batch
-                    )
-                )
+            filter_in_dict = dict(
+                post_pt_root_id=target_batch, pre_pt_root_id=source_batch
+            )
             this = func(filter_in_dict=filter_in_dict)
 
             # We need to drop the .attrs (which contain meta data from queries)
             # Otherwise we run into issues when concatenating
             this.attrs = {}
 
             if not this.empty:
@@ -1148,25 +1137,22 @@
                 columns += ["gaba", "ach", "glut", "oct", "ser", "da"]
             func = partial(
                 retry(client.materialize.query_view),
                 view_name="valid_connection_v2",
                 select_columns=columns,
                 materialization_version=materialization,
             )
-            filtered = False  # Set to false since we don't need the join
         # Otherwise we need to query the valid synapse view
         else:
             func = partial(
-                retry(client.materialize.join_query),
-                tables=[
-                    [client.materialize.synapse_table, "id"],
-                    ["valid_synapses_nt_v2", "target_id"],
-                ],
+                retry(client.materialize.query_view),
+                view_name="valid_synapses_nt_np_v6",
                 materialization_version=materialization,
-                select_columns={client.materialize.synapse_table: columns},
+                split_positions=True,
+                select_columns=columns,
             )
     else:
         func = partial(
             retry(client.materialize.query_table),
             table=client.materialize.synapse_table,
             materialization_version=materialization,
             select_columns=columns,
@@ -1178,25 +1164,17 @@
         len(ids),
         batch_size,
         desc="Fetching connectivity",
         disable=not progress or len(ids) <= batch_size,
     ):
         batch = ids[i : i + batch_size]
         if upstream:
-            if not filtered or materialization == "live":
-                filter_in_dict = dict(post_pt_root_id=batch)
-            else:
-                filter_in_dict = dict(synapses_nt_v1=dict(post_pt_root_id=batch))
-            syn.append(func(filter_in_dict=filter_in_dict))
+            syn.append(func(filter_in_dict=dict(post_pt_root_id=batch)))
         if downstream:
-            if not filtered or materialization == "live":
-                filter_in_dict = dict(pre_pt_root_id=batch)
-            else:
-                filter_in_dict = dict(synapses_nt_v1=dict(pre_pt_root_id=batch))
-            syn.append(func(filter_in_dict=filter_in_dict))
+            syn.append(func(filter_in_dict=dict(pre_pt_root_id=batch)))
 
     # Some clean-up
     for df in syn:
         # Drop supervoxel columns (if they exist)
         df.drop(sv_cols, axis=1, errors="ignore", inplace=True)
         # Drop `attrs`` to avoid issues when concatenating
         df.attrs = {}
```

### Comparing `fafbseg-3.0.6/fafbseg/flywire/utils.py` & `fafbseg-3.0.7/fafbseg/flywire/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/google/__init__.py` & `fafbseg-3.0.7/fafbseg/google/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/google/meshes.py` & `fafbseg-3.0.7/fafbseg/google/meshes.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/google/segmentation.py` & `fafbseg-3.0.7/fafbseg/google/segmentation.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/google/synapses.py` & `fafbseg-3.0.7/fafbseg/google/synapses.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/move/__init__.py` & `fafbseg-3.0.7/fafbseg/move/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/move/interfaces.py` & `fafbseg-3.0.7/fafbseg/move/interfaces.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/move/merge.py` & `fafbseg-3.0.7/fafbseg/move/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/move/merge_utils.py` & `fafbseg-3.0.7/fafbseg/move/merge_utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/spine/__init__.py` & `fafbseg-3.0.7/fafbseg/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/spine/base.py` & `fafbseg-3.0.7/fafbseg/spine/base.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/synapses/__init__.py` & `fafbseg-3.0.7/fafbseg/synapses/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/synapses/offline.py` & `fafbseg-3.0.7/fafbseg/synapses/offline.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/synapses/online.py` & `fafbseg-3.0.7/fafbseg/synapses/online.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/synapses/transmitters.py` & `fafbseg-3.0.7/fafbseg/synapses/transmitters.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/synapses/utils.py` & `fafbseg-3.0.7/fafbseg/synapses/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/utils.py` & `fafbseg-3.0.7/fafbseg/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/xform/__init__.py` & `fafbseg-3.0.7/fafbseg/xform/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg/xform/xform.py` & `fafbseg-3.0.7/fafbseg/xform/xform.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/fafbseg.egg-info/PKG-INFO` & `fafbseg-3.0.7/fafbseg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 3.0.6
+Version: 3.0.7
 Summary: Tools to work with the FlyWire and Google segmentations of the FAFB EM dataset
 Home-page: https://fafbseg-py.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://fafbseg-py.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/fafbseg-py
@@ -73,7 +73,8 @@
 
 ## How to cite
 If you use `fafbseg` for your publication, please cite the two FlyWire papers:
 
 1. "_Whole-brain annotation and multi-connectome cell typing quantifies circuit stereotypy in Drosophila_" Schlegel _et al._, bioRxiv (2023); doi: https://doi.org/10.1101/2023.06.27.546055
 2. "_Neuronal wiring diagram of an adult brain_" Dorkenwald _et al._, bioRxiv (2023); doi: https://doi.org/10.1101/2023.06.27.546656
 
+Depending on what data you used (e.g. neurotransmitter predictions) you might need to cite additional publications. Please see the [Citation Guidelines](https://codex.flywire.ai/about_flywire) on Codex.
```

### Comparing `fafbseg-3.0.6/fafbseg.egg-info/SOURCES.txt` & `fafbseg-3.0.7/fafbseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.6/setup.py` & `fafbseg-3.0.7/setup.py`

 * *Files identical despite different names*

