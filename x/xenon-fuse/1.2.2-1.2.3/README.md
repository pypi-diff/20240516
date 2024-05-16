# Comparing `tmp/xenon_fuse-1.2.2.tar.gz` & `tmp/xenon_fuse-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenon_fuse-1.2.2.tar", max compression
+gzip compressed data, was "xenon_fuse-1.2.3.tar", max compression
```

## Comparing `xenon_fuse-1.2.2.tar` & `xenon_fuse-1.2.3.tar`

### file list

```diff
@@ -1,60 +1,64 @@
--rw-r--r--   0        0        0     1536 2024-05-03 11:40:01.683310 xenon_fuse-1.2.2/LICENSE
--rw-r--r--   0        0        0     1823 2024-05-03 11:40:01.683310 xenon_fuse-1.2.2/README.md
--rw-r--r--   0        0        0      204 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/__init__.py
--rw-r--r--   0        0        0     9142 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/common.py
--rw-r--r--   0        0        0     9697 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/context.py
--rw-r--r--   0        0        0     2787 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/dtypes.py
--rw-r--r--   0        0        0     2639 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugin.py
--rw-r--r--   0        0        0      241 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/__init__.py
--rw-r--r--   0        0        0      478 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/README.md
--rw-r--r--   0        0        0      593 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/__init__.py
--rw-r--r--   0        0        0     7963 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/csv_input.py
--rw-r--r--   0        0        0      615 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/__init__.py
--rw-r--r--   0        0        0     1055 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
--rw-r--r--   0        0        0      803 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
--rw-r--r--   0        0        0     2562 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
--rw-r--r--   0        0        0      960 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
--rw-r--r--   0        0        0     2017 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
--rw-r--r--   0        0        0      837 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
--rw-r--r--   0        0        0     8539 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
--rw-r--r--   0        0        0    14728 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_drift.py
--rw-r--r--   0        0        0     4537 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_extraction.py
--rw-r--r--   0        0        0     3103 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_timing.py
--rw-r--r--   0        0        0     5457 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_hits.py
--rw-r--r--   0        0        0    13372 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_propagation.py
--rw-r--r--   0        0        0    35178 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/s2_photon_propagation.py
--rw-r--r--   0        0        0     9238 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/detector_physics/secondary_scintillation.py
--rw-r--r--   0        0        0      647 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/README.md
--rw-r--r--   0        0        0      459 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/__init__.py
--rw-r--r--   0        0        0     7280 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/detector_volumes.py
--rw-r--r--   0        0        0     2262 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/electric_field.py
--rw-r--r--   0        0        0     4556 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/find_cluster.py
--rw-r--r--   0        0        0    20236 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/input.py
--rw-r--r--   0        0        0     4424 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/merge_cluster.py
--rw-r--r--   0        0        0      456 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/microphysics_summary.py
--rw-r--r--   0        0        0     4305 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/wfsim_connection.py
--rw-r--r--   0        0        0    17364 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/micro_physics/yields.py
--rw-r--r--   0        0        0      152 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/README.md
--rw-r--r--   0        0        0      251 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/__init__.py
--rw-r--r--   0        0        0     9569 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/photon_pulses.py
--rw-r--r--   0        0        0      436 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/photon_summary.py
--rw-r--r--   0        0        0     8682 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
--rw-r--r--   0        0        0    20113 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
--rw-r--r--   0        0        0      293 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/__init__.py
--rw-r--r--   0        0        0     3892 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/cluster_tagging.py
--rw-r--r--   0        0        0     2730 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/event_truth.py
--rw-r--r--   0        0        0     8335 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/peak_truth.py
--rw-r--r--   0        0        0     4784 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/records_truth.py
--rw-r--r--   0        0        0     1543 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/plugins/truth_information/surviving_clusters.py
--rw-r--r--   0        0        0      895 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/vertical_merger_plugin.py
--rw-r--r--   0        0        0     1041 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/fuse/volume_plugin.py
--rw-r--r--   0        0        0     1169 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      823 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/_utils.py
--rw-r--r--   0        0        0     1770 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_DetectorPhysics_csv.py
--rw-r--r--   0        0        0     3530 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_FullChain.py
--rw-r--r--   0        0        0     4908 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_FullChain_w_DelayedElectrons.py
--rw-r--r--   0        0        0     2490 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_MicroPhysics.py
--rw-r--r--   0        0        0     4560 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_deterministic_seed.py
--rw-r--r--   0        0        0     7134 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_input.py
--rw-r--r--   0        0        0     5000 2024-05-03 11:40:01.707310 xenon_fuse-1.2.2/tests/test_plugin_random_seed.py
--rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 xenon_fuse-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1536 2024-05-16 08:51:19.943478 xenon_fuse-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1823 2024-05-16 08:51:19.947478 xenon_fuse-1.2.3/README.md
+-rw-r--r--   0        0        0      204 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/__init__.py
+-rw-r--r--   0        0        0     9142 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/common.py
+-rw-r--r--   0        0        0     9697 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/context.py
+-rw-r--r--   0        0        0     2787 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/dtypes.py
+-rw-r--r--   0        0        0     2639 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugin.py
+-rw-r--r--   0        0        0      241 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/__init__.py
+-rw-r--r--   0        0        0      478 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/README.md
+-rw-r--r--   0        0        0      593 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/__init__.py
+-rw-r--r--   0        0        0     7963 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/csv_input.py
+-rw-r--r--   0        0        0      615 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py
+-rw-r--r--   0        0        0      803 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py
+-rw-r--r--   0        0        0     2562 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py
+-rw-r--r--   0        0        0      960 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py
+-rw-r--r--   0        0        0     2017 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py
+-rw-r--r--   0        0        0      837 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py
+-rw-r--r--   0        0        0     8539 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py
+-rw-r--r--   0        0        0    14728 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/electron_drift.py
+-rw-r--r--   0        0        0     4537 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/electron_extraction.py
+-rw-r--r--   0        0        0     3103 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/electron_timing.py
+-rw-r--r--   0        0        0     5457 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/s1_photon_hits.py
+-rw-r--r--   0        0        0    13372 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/s1_photon_propagation.py
+-rw-r--r--   0        0        0    35178 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/s2_photon_propagation.py
+-rw-r--r--   0        0        0     9238 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/detector_physics/secondary_scintillation.py
+-rw-r--r--   0        0        0      647 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/README.md
+-rw-r--r--   0        0        0      459 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/__init__.py
+-rw-r--r--   0        0        0     7280 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/detector_volumes.py
+-rw-r--r--   0        0        0     2262 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/electric_field.py
+-rw-r--r--   0        0        0     4556 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/find_cluster.py
+-rw-r--r--   0        0        0    20236 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/input.py
+-rw-r--r--   0        0        0     4424 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/merge_cluster.py
+-rw-r--r--   0        0        0      456 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/microphysics_summary.py
+-rw-r--r--   0        0        0     4305 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/wfsim_connection.py
+-rw-r--r--   0        0        0    17372 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/micro_physics/yields.py
+-rw-r--r--   0        0        0      152 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/README.md
+-rw-r--r--   0        0        0      251 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/__init__.py
+-rw-r--r--   0        0        0     9569 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/photon_pulses.py
+-rw-r--r--   0        0        0      436 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/photon_summary.py
+-rw-r--r--   0        0        0     8682 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/pmt_afterpulses.py
+-rw-r--r--   0        0        0    20146 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py
+-rw-r--r--   0        0        0      293 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/truth_information/__init__.py
+-rw-r--r--   0        0        0     3892 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/truth_information/cluster_tagging.py
+-rw-r--r--   0        0        0     2730 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/truth_information/event_truth.py
+-rw-r--r--   0        0        0     8335 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/truth_information/peak_truth.py
+-rw-r--r--   0        0        0     4784 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/truth_information/records_truth.py
+-rw-r--r--   0        0        0     1543 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/plugins/truth_information/surviving_clusters.py
+-rw-r--r--   0        0        0      895 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/vertical_merger_plugin.py
+-rw-r--r--   0        0        0     1041 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/fuse/volume_plugin.py
+-rw-r--r--   0        0        0     1169 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      823 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/_utils.py
+-rw-r--r--   0        0        0     1770 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_DetectorPhysics_csv.py
+-rw-r--r--   0        0        0     4660 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_FullChain.py
+-rw-r--r--   0        0        0     4908 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_FullChain_w_DelayedElectrons.py
+-rw-r--r--   0        0        0     3499 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_MicroPhysics.py
+-rw-r--r--   0        0        0     2393 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_clustering_functions.py
+-rw-r--r--   0        0        0     2431 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_common_functions.py
+-rw-r--r--   0        0        0     4560 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_deterministic_seed.py
+-rw-r--r--   0        0        0     7134 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_input.py
+-rw-r--r--   0        0        0     5000 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_plugin_random_seed.py
+-rw-r--r--   0        0        0     1577 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_truth_plugins.py
+-rw-r--r--   0        0        0     3339 2024-05-16 08:51:19.971479 xenon_fuse-1.2.3/tests/test_waveform_building_functions.py
+-rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 xenon_fuse-1.2.3/PKG-INFO
```

### Comparing `xenon_fuse-1.2.2/LICENSE` & `xenon_fuse-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/README.md` & `xenon_fuse-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/common.py` & `xenon_fuse-1.2.3/fuse/common.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/context.py` & `xenon_fuse-1.2.3/fuse/context.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/dtypes.py` & `xenon_fuse-1.2.3/fuse/dtypes.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugin.py` & `xenon_fuse-1.2.3/fuse/plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/__init__.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/csv_input.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/csv_input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/__init__.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/__init__.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_drift.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_extraction.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_merger.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_s1photonhits.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_secondary_scintillation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/delayed_electrons_timing.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/delayed_electrons/photo_ionization_electrons.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_drift.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/electron_drift.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_extraction.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/electron_extraction.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/electron_timing.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/electron_timing.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_hits.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/s1_photon_hits.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/s1_photon_propagation.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/s1_photon_propagation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/s2_photon_propagation.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/s2_photon_propagation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/detector_physics/secondary_scintillation.py` & `xenon_fuse-1.2.3/fuse/plugins/detector_physics/secondary_scintillation.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/README.md` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/README.md`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/detector_volumes.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/detector_volumes.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/electric_field.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/electric_field.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/find_cluster.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/find_cluster.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/input.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/merge_cluster.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/merge_cluster.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/wfsim_connection.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/wfsim_connection.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/micro_physics/yields.py` & `xenon_fuse-1.2.3/fuse/plugins/micro_physics/yields.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
             drift_field=field,
         )
         q_ = self.nc.GetQuanta(y)
 
         return beta_photons, beta_electrons, q_.excitons
 
 
+@export
 class BBFYields(FuseBasePlugin):
     __version__ = "0.1.1"
 
     depends_on = ("interactions_in_roi", "electric_field_values")
     provides = "quanta"
 
     dtype = quanta_fields + strax.time_fields
```

### Comparing `xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/photon_pulses.py` & `xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/photon_pulses.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_afterpulses.py` & `xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/pmt_afterpulses.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py` & `xenon_fuse-1.2.3/fuse/plugins/pmt_and_daq/pmt_response_and_daq.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     First the single PMT waveform is simulated based on the photon
     timing and gain information. Next the waveform is converted to ADC
     counts, noise and a baseline are added. Then hitfinding is performed
     and the found intervals are split into multiple fragments of fixed
     length (if needed). Finally the data is saved as raw_records.
     """
 
-    __version__ = "0.1.4"
+    __version__ = "0.1.5"
 
     depends_on = ("photon_summary", "pulse_ids", "pulse_windows")
 
     provides = "raw_records"
     data_kind = "raw_records"
 
     dtype = strax.raw_record_dtype(samples_per_record=strax.DEFAULT_RECORD_LENGTH)
@@ -216,14 +216,15 @@
         )
 
     def compute(self, propagated_photons, pulse_windows, start, end):
         if len(propagated_photons) == 0 or len(pulse_windows) == 0:
             log.debug("No photons or pulse windows found for chunk!")
 
             yield self.chunk(start=start, end=end, data=np.zeros(0, dtype=self.dtype))
+            return  # Exit early
 
         # Split into "sub-chunks"
         pulse_gaps = pulse_windows["time"][1:] - strax.endtime(pulse_windows)[:-1]
         pulse_gaps = np.append(pulse_gaps, 0)  # Add 0 for last pulse gap
 
         split_index = find_split_index(
             pulse_windows,
```

### Comparing `xenon_fuse-1.2.2/fuse/plugins/truth_information/cluster_tagging.py` & `xenon_fuse-1.2.3/fuse/plugins/truth_information/cluster_tagging.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/truth_information/event_truth.py` & `xenon_fuse-1.2.3/fuse/plugins/truth_information/event_truth.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/truth_information/peak_truth.py` & `xenon_fuse-1.2.3/fuse/plugins/truth_information/peak_truth.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/truth_information/records_truth.py` & `xenon_fuse-1.2.3/fuse/plugins/truth_information/records_truth.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/plugins/truth_information/surviving_clusters.py` & `xenon_fuse-1.2.3/fuse/plugins/truth_information/surviving_clusters.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/vertical_merger_plugin.py` & `xenon_fuse-1.2.3/fuse/vertical_merger_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/fuse/volume_plugin.py` & `xenon_fuse-1.2.3/fuse/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/pyproject.toml` & `xenon_fuse-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xenon-fuse"
-version = "1.2.2"
+version = "1.2.3"
 description = "XENON Framework for Unified Simulations of Events"
 authors = [
   "Henning Schulze Eißing, <h_schu55@uni-muenster.de>",
   "Diego Ramírez García, <diego.ramirez@physik.uzh.ch>",
 ]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `xenon_fuse-1.2.2/tests/_utils.py` & `xenon_fuse-1.2.3/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/tests/test_DetectorPhysics_csv.py` & `xenon_fuse-1.2.3/tests/test_DetectorPhysics_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import unittest
 import tempfile
 import timeout_decorator
 import fuse
 from _utils import build_random_instructions
 
-TIMEOUT = 240
+TIMEOUT = 480
 
 
 class TestDetectorPhysicsCsv(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.temp_dir = tempfile.TemporaryDirectory()
```

### Comparing `xenon_fuse-1.2.2/tests/test_FullChain.py` & `xenon_fuse-1.2.3/tests/test_MicroPhysics.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,29 @@
 import unittest
 import tempfile
 import timeout_decorator
 import fuse
 import straxen
 from _utils import test_root_file_name
 
-TIMEOUT = 240
+TIMEOUT = 60
 
 
-class TestFullChain(unittest.TestCase):
-    __test__ = True
-
+class TestMicroPhysicsBase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.temp_dir = tempfile.TemporaryDirectory()
 
-        cls.test_context = fuse.context.full_chain_context(
-            output_folder=cls.temp_dir.name, run_without_proper_corrections=True
-        )
+        cls.test_context = fuse.context.microphysics_context(cls.temp_dir.name)
 
         cls.test_context.set_config(
             {
                 "path": cls.temp_dir.name,
                 "file_name": test_root_file_name,
-                "entry_stop": 5,
+                "entry_stop": 25,
             }
         )
 
         cls.run_number = "TestRun_00000"
 
     @classmethod
     def tearDownClass(cls):
@@ -42,61 +38,65 @@
         assert os.path.exists(os.path.join(self.temp_dir.name, test_root_file_name))
 
     def tearDown(self):
         # self.temp_dir.cleanup()
         shutil.rmtree(self.temp_dir.name)
         os.makedirs(self.temp_dir.name)
 
-    @timeout_decorator.timeout(TIMEOUT, exception_message="S1PhotonHits timed out")
-    def test_S1PhotonHits(self):
-        self.test_context.make(self.run_number, "s1_photon_hits")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="S1PhotonPropagation timed out")
-    def test_S1PhotonPropagation(self):
-        self.test_context.make(self.run_number, "propagated_s1_photons")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="ElectronDrift timed out")
-    def test_ElectronDrift(self):
-        self.test_context.make(self.run_number, "drifted_electrons")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="ElectronExtraction timed out")
-    def test_ElectronExtraction(self):
-        self.test_context.make(self.run_number, "extracted_electrons")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="ElectronTiming timed out")
-    def test_ElectronTiming(self):
-        self.test_context.make(self.run_number, "electron_time")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="SecondaryScintillation timed out")
-    def test_SecondaryScintillation(self):
-        self.test_context.make(self.run_number, "s2_photons")
-        # self.test_context.make(self.run_number, "s2_photons_sum")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="S2PhotonPropagation timed out")
-    def test_S2PhotonPropagation(self):
-        self.test_context.make(self.run_number, "propagated_s2_photons")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="PMTAfterPulses timed out")
-    def test_PMTAfterPulses(self):
-        self.test_context.make(self.run_number, "pmt_afterpulses")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="PulseWindow timed out")
-    def test_PulseWindow(self):
-        self.test_context.make(self.run_number, "pulse_windows")
-        # self.test_context.make(self.run_number, "pulse_ids")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="PMTResponseAndDAQ timed out")
-    def test_PMTResponseAndDAQ(self):
-        self.test_context.make(self.run_number, "raw_records")
 
+class TestMicroPhysics(TestMicroPhysicsBase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="ChunkInput timed out")
+    def test_ChunkInput(self):
+        self.test_context.make(self.run_number, "geant4_interactions")
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="FindCluster timed out")
+    def test_FindCluster(self):
+        self.test_context.make(self.run_number, "cluster_index")
 
-class TestChunkedFullChain(TestFullChain):
-    __test__ = True
+    @timeout_decorator.timeout(TIMEOUT, exception_message="MergeCluster timed out")
+    def test_MergeCluster(self):
+        self.test_context.make(self.run_number, "clustered_interactions")
 
+    @timeout_decorator.timeout(TIMEOUT, exception_message="VolumesMerger timed out")
+    def test_VolumesMerger(self):
+        self.test_context.make(self.run_number, "interactions_in_roi")
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="ElectricField timed out")
+    def test_ElectricField(self):
+        self.test_context.make(self.run_number, "electric_field_values")
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="NestYields timed out")
+    def test_NestYields(self):
+        self.test_context.make(self.run_number, "quanta")
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="MicroPhysicsSummary timed out")
+    def test_MicroPhysicsSummary(self):
+        self.test_context.make(self.run_number, "microphysics_summary")
+
+
+class TestMicroPhysicsAlternativePlugins(TestMicroPhysicsBase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
-        cls.test_context.set_config({"n_interactions_per_chunk": 2})
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="BBFYields timed out")
+    def test_BBFYields(self):
+        self.test_context.register(fuse.plugins.BBFYields)
+        self.test_context.make(self.run_number, "quanta")
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="WFSim connection timed out")
+    def test_WFSimConnection(self):
+        self.test_context.register(fuse.plugins.output_plugin)
+        self.test_context.make(self.run_number, "wfsim_instructions")
+
+    @timeout_decorator.timeout(TIMEOUT, exception_message="GasPhasePlugin timed out")
+    def test_GasPhasePlugin(self):
+        self.test_context.register(fuse.plugins.XENONnT_GasPhase)
+        self.test_context.make(self.run_number, "gas_phase_interactions")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `xenon_fuse-1.2.2/tests/test_FullChain_w_DelayedElectrons.py` & `xenon_fuse-1.2.3/tests/test_FullChain_w_DelayedElectrons.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/tests/test_MicroPhysics.py` & `xenon_fuse-1.2.3/tests/test_truth_plugins.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import unittest
 import tempfile
 import timeout_decorator
 import fuse
 import straxen
 from _utils import test_root_file_name
 
-TIMEOUT = 60
+TIMEOUT = 240
 
 
-class TestMicroPhysics(unittest.TestCase):
+class TestTruthPlugins(unittest.TestCase):
+    __test__ = True
+
     @classmethod
     def setUpClass(cls):
         cls.temp_dir = tempfile.TemporaryDirectory()
 
-        cls.test_context = fuse.context.microphysics_context(cls.temp_dir.name)
+        cls.test_context = fuse.context.full_chain_context(
+            output_folder=cls.temp_dir.name, run_without_proper_corrections=True
+        )
 
         cls.test_context.set_config(
             {
                 "path": cls.temp_dir.name,
                 "file_name": test_root_file_name,
-                "entry_stop": 25,
+                "entry_stop": 5,
             }
         )
 
         cls.run_number = "TestRun_00000"
 
     @classmethod
     def tearDownClass(cls):
@@ -33,43 +37,22 @@
 
     def setUp(self):
         downloader = straxen.MongoDownloader(store_files_at=(self.temp_dir.name,))
         downloader.download_single(test_root_file_name, human_readable_file_name=True)
 
         assert os.path.exists(os.path.join(self.temp_dir.name, test_root_file_name))
 
+        self.test_context.make(self.run_number, "photon_summary")
+        self.test_context.make(self.run_number, "raw_records")
+
     def tearDown(self):
         # self.temp_dir.cleanup()
         shutil.rmtree(self.temp_dir.name)
         os.makedirs(self.temp_dir.name)
 
-    @timeout_decorator.timeout(TIMEOUT, exception_message="ChunkInput timed out")
-    def test_ChunkInput(self):
-        self.test_context.make(self.run_number, "geant4_interactions")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="FindCluster timed out")
-    def test_FindCluster(self):
-        self.test_context.make(self.run_number, "cluster_index")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="MergeCluster timed out")
-    def test_MergeCluster(self):
-        self.test_context.make(self.run_number, "clustered_interactions")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="VolumesMerger timed out")
-    def test_VolumesMerger(self):
-        self.test_context.make(self.run_number, "interactions_in_roi")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="ElectricField timed out")
-    def test_ElectricField(self):
-        self.test_context.make(self.run_number, "electric_field_values")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="NestYields timed out")
-    def test_NestYields(self):
-        self.test_context.make(self.run_number, "quanta")
-
-    @timeout_decorator.timeout(TIMEOUT, exception_message="MicroPhysicsSummary timed out")
-    def test_MicroPhysicsSummary(self):
-        self.test_context.make(self.run_number, "microphysics_summary")
+    @timeout_decorator.timeout(TIMEOUT, exception_message="RecordsTruth timed out")
+    def test_RecordsTruth(self):
+        self.test_context.make(self.run_number, "records_truth")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `xenon_fuse-1.2.2/tests/test_deterministic_seed.py` & `xenon_fuse-1.2.3/tests/test_deterministic_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/tests/test_input.py` & `xenon_fuse-1.2.3/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/tests/test_plugin_random_seed.py` & `xenon_fuse-1.2.3/tests/test_plugin_random_seed.py`

 * *Files identical despite different names*

### Comparing `xenon_fuse-1.2.2/PKG-INFO` & `xenon_fuse-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenon-fuse
-Version: 1.2.2
+Version: 1.2.3
 Summary: XENON Framework for Unified Simulations of Events
 Home-page: https://github.com/XENONnT/fuse
 Author: Henning Schulze Eißing,
 Author-email: h_schu55@uni-muenster.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

