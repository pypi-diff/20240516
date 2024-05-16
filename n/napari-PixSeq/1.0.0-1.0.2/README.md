# Comparing `tmp/napari-PixSeq-1.0.0.tar.gz` & `tmp/napari_pixseq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-PixSeq\dist\.tmp-tp9wm8_s\napari-PixSeq-1.0.0.tar", last modified: Thu Feb 29 14:51:52 2024, max compression
+gzip compressed data, was "napari_pixseq-1.0.2.tar", last modified: Thu May 16 14:33:45 2024, max compression
```

## Comparing `napari-PixSeq-1.0.0.tar` & `napari_pixseq-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/
--rw-rw-rw-   0        0        0       53 2024-02-29 09:48:02.000000 napari-PixSeq-1.0.0/.gitignore
--rw-rw-rw-   0        0        0     1102 2023-11-24 12:31:51.000000 napari-PixSeq-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      101 2023-11-24 12:31:51.000000 napari-PixSeq-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4366 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3044 2024-02-29 10:45:02.000000 napari-PixSeq-1.0.0/README.md
--rw-rw-rw-   0        0        0     1306 2024-02-29 09:59:26.000000 napari-PixSeq-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1914 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/
--rw-rw-rw-   0        0        0     4366 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1387 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      179 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_pixseq/
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_pixseq/GUI/
--rw-rw-rw-   0        0        0        0 2024-02-29 10:23:46.000000 napari-PixSeq-1.0.0/src/napari_pixseq/GUI/__init__.py
--rw-rw-rw-   0        0        0    94879 2024-02-29 10:23:06.000000 napari-PixSeq-1.0.0/src/napari_pixseq/GUI/pixseq_ui.py
--rw-rw-rw-   0        0        0    91490 2024-02-29 09:58:46.000000 napari-PixSeq-1.0.0/src/napari_pixseq/GUI/pixseq_ui.ui
--rw-rw-rw-   0        0        0      197 2024-02-29 10:21:23.000000 napari-PixSeq-1.0.0/src/napari_pixseq/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_pixseq/_tests/
--rw-rw-rw-   0        0        0        0 2023-11-24 12:31:51.000000 napari-PixSeq-1.0.0/src/napari_pixseq/_tests/__init__.py
--rw-rw-rw-   0        0        0      667 2024-02-29 10:21:23.000000 napari-PixSeq-1.0.0/src/napari_pixseq/_tests/test_widget.py
--rw-rw-rw-   0        0        0      164 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_pixseq/_version.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:51:52.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/
--rw-rw-rw-   0        0        0        0 2024-02-29 10:30:27.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/__init__.py
--rw-rw-rw-   0        0        0     8024 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_align_utils.py
--rw-rw-rw-   0        0        0     6745 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_cluster_utils.py
--rw-rw-rw-   0        0        0     8186 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_colocalize_utils.py
--rw-rw-rw-   0        0        0    28101 2024-02-29 09:58:46.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_events.py
--rw-rw-rw-   0        0        0    19401 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_export_images_utils.py
--rw-rw-rw-   0        0        0    26876 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_export_traces_utils.py
--rw-rw-rw-   0        0        0    25751 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_import_utils.py
--rw-rw-rw-   0        0        0    32242 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_loc_utils.py
--rw-rw-rw-   0        0        0    20492 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_picasso_detect.py
--rw-rw-rw-   0        0        0    37435 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_plot_utils.py
--rw-rw-rw-   0        0        0    10067 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_temporal_filtering.py
--rw-rw-rw-   0        0        0    46733 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py
--rw-rw-rw-   0        0        0     9160 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_transform_utils.py
--rw-rw-rw-   0        0        0    12363 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_undrift_utils.py
--rw-rw-rw-   0        0        0     8299 2024-01-24 20:06:05.000000 napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_utils_compute.py
--rw-rw-rw-   0        0        0      502 2024-02-29 10:18:02.000000 napari-PixSeq-1.0.0/src/napari_pixseq/napari.yaml
--rw-rw-rw-   0        0        0    32073 2024-02-29 10:31:42.000000 napari-PixSeq-1.0.0/src/napari_pixseq/pixseq_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.033755 napari_pixseq-1.0.2/
+-rw-rw-rw-   0        0        0      120 2024-03-22 12:17:27.000000 napari_pixseq-1.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1102 2023-11-24 12:31:51.000000 napari_pixseq-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-11-24 12:31:51.000000 napari_pixseq-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5275 2024-05-16 14:33:45.033755 napari_pixseq-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3194 2024-03-04 16:12:02.000000 napari_pixseq-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1306 2024-02-29 09:59:26.000000 napari_pixseq-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1983 2024-05-16 14:33:45.033755 napari_pixseq-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.917924 napari_pixseq-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.018133 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/
+-rw-rw-rw-   0        0        0     5275 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1823 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.964762 napari_pixseq-1.0.2/src/napari_pixseq/
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.964762 napari_pixseq-1.0.2/src/napari_pixseq/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/GUI/__init__.py
+-rw-rw-rw-   0        0        0   136082 2024-05-15 16:44:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.py
+-rw-rw-rw-   0        0        0   135729 2024-05-15 16:44:26.000000 napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.ui
+-rw-rw-rw-   0        0        0      197 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.964762 napari_pixseq-1.0.2/src/napari_pixseq/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/_tests/__init__.py
+-rw-rw-rw-   0        0        0      667 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      427 2024-05-16 14:33:44.000000 napari_pixseq-1.0.2/src/napari_pixseq/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:44.986887 napari_pixseq-1.0.2/src/napari_pixseq/dev/
+-rw-rw-rw-   0        0        0        0 2024-05-13 10:26:25.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/__init__.py
+-rw-rw-rw-   0        0        0      438 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/ebfret_IO_dev.py
+-rw-rw-rw-   0        0        0     1818 2024-05-15 12:30:42.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/refactor.py
+-rw-rw-rw-   0        0        0     3226 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/dev/spot_mask_dev.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.018133 napari_pixseq-1.0.2/src/napari_pixseq/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/__init__.py
+-rw-rw-rw-   0        0        0     9122 2024-05-15 12:25:50.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_align_utils.py
+-rw-rw-rw-   0        0        0     7416 2024-05-15 12:25:50.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_cluster_utils.py
+-rw-rw-rw-   0        0        0     8349 2024-05-15 12:24:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_colocalize_utils.py
+-rw-rw-rw-   0        0        0    32871 2024-05-15 13:33:09.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_events.py
+-rw-rw-rw-   0        0        0    20369 2024-05-15 14:00:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_images_utils.py
+-rw-rw-rw-   0        0        0    35078 2024-05-15 14:01:09.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_traces_utils.py
+-rw-rw-rw-   0        0        0     6602 2024-05-15 12:24:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_filter_utils.py
+-rw-rw-rw-   0        0        0    32955 2024-05-15 16:14:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_import_utils.py
+-rw-rw-rw-   0        0        0    35046 2024-05-15 14:44:03.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_loc_utils.py
+-rw-rw-rw-   0        0        0    27024 2024-05-16 13:53:20.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_picasso_detect.py
+-rw-rw-rw-   0        0        0    37770 2024-05-15 13:59:09.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_plot_utils.py
+-rw-rw-rw-   0        0        0     3610 2024-05-15 11:32:04.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_segmentation_events.py
+-rw-rw-rw-   0        0        0    18616 2024-05-15 10:59:04.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_segmentation_utils.py
+-rw-rw-rw-   0        0        0    13712 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_simple_analysis_utils.py
+-rw-rw-rw-   0        0        0    10196 2024-05-10 10:04:52.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_temporal_filtering.py
+-rw-rw-rw-   0        0        0    49296 2024-05-15 13:53:33.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py
+-rw-rw-rw-   0        0        0     4548 2024-05-16 13:38:35.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_tracking_utils.py
+-rw-rw-rw-   0        0        0     9379 2024-05-15 12:24:02.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_transform_utils.py
+-rw-rw-rw-   0        0        0    12482 2024-05-15 12:24:40.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_undrift_utils.py
+-rw-rw-rw-   0        0        0    11991 2024-05-15 17:17:10.000000 napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_utils_compute.py
+-rw-rw-rw-   0        0        0      488 2024-03-04 16:14:23.000000 napari_pixseq-1.0.2/src/napari_pixseq/napari.yaml
+-rw-rw-rw-   0        0        0    27799 2024-05-15 14:13:49.000000 napari_pixseq-1.0.2/src/napari_pixseq/pixseq_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:45.018133 napari_pixseq-1.0.2/src/napari_pixseq/scripts/
+-rw-rw-rw-   0        0        0      232 2024-03-04 09:54:53.000000 napari_pixseq-1.0.2/src/napari_pixseq/scripts/pypi
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `napari-PixSeq-1.0.0/LICENSE` & `napari_pixseq-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-PixSeq-1.0.0/README.md` & `napari_pixseq-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # napari-PixSeq
 
 [![License MIT](https://img.shields.io/pypi/l/napari-GapSeq2.svg?color=green)](https://github.com/piedrro/napari-PixSeq/blob/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-GapSeq2.svg?color=green)](https://pypi.org/project/napari-PixSeq)
+[![PyPI](https://img.shields.io/pypi/v/napari-GapSeq2.svg?color=green)](https://pypi.org/project/napari-PixSeq/)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-GapSeq2.svg?color=green)](https://python.org)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-GapSeq2)](https://napari-hub.org/plugins/napari-PixSeq)
 
-A **Napari** plugin for extracting time series traces from **Single Molecule Localisation Microsocpy** (SMLM) data.
+A **Napari** plugin for extracting time series traces from single molecule FRET data.
 
-Napari-PixSeq uses **Picasso** (picassosr) as a backend and includes features for **aligning** image channels/datasets, **undrifting** images, **detecting/fitting** localisations and extracting **traces**, and supports both **ALEX** and **FRET** data. Traces can be exported in different formats for downstream analysis.
+napari-PixSeq uses **Picasso** (picassosr) as a backend and includes features for **aligning** image channels/datasets, **undrifting** images, **detecting/fitting** localisations and extracting **traces**, and supports both **ALEX** and **FRET** data. Traces can be exported in different formats for downstream analysis.
+
+napari-PixSeq traces can be analysed with TraceAnalyser: https://github.com/piedrro/TraceAnalyser
 
 This is still undergoing development, so some features may not work as expected.
 
 This was built by Dr Piers Turner from the Kapanidis Lab, University of Oxford.
 
 ----------------------------------
 
@@ -23,15 +25,19 @@
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
 -->
 
 ## Installation
 
-You can install `napari-GapSeq2` via [GitHub]:
+You can install `napari-PixSeq` via [pip]:
+
+    pip install napari-PixSeq
+
+You can install `napari-PixSeq` via [GitHub]:
 
     conda create –-name napari-pixseq python==3.9
     conda activate napari-pixseq
     conda install -c anaconda git
     conda update --all
 
     pip install git+https://github.com/piedrro/napari-PixSeq.git
```

### Comparing `napari-PixSeq-1.0.0/pyproject.toml` & `napari_pixseq-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-PixSeq-1.0.0/setup.cfg` & `napari_pixseq-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -78,43 +78,47 @@
 000004d0: 0d0a 0971 7470 790d 0a09 7363 6970 790d  ...qtpy...scipy.
 000004e0: 0a09 7079 7174 6772 6170 680d 0a09 7069  ..pyqtgraph...pi
 000004f0: 6361 7373 6f73 720d 0a09 7061 6e64 6173  cassosr...pandas
 00000500: 0d0a 096d 6174 706c 6f74 6c69 620d 0a09  ...matplotlib...
 00000510: 7363 6970 790d 0a09 6f70 656e 6376 2d70  scipy...opencv-p
 00000520: 7974 686f 6e0d 0a09 7471 646d 0d0a 096f  ython...tqdm...o
 00000530: 7269 6769 6e70 726f 0d0a 0970 7971 7435  riginpro...pyqt5
-00000540: 2d74 6f6f 6c73 0d0a 7079 7468 6f6e 5f72  -tools..python_r
-00000550: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
-00000560: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-00000570: 5f64 6174 6120 3d20 5472 7565 0d0a 7061  _data = True..pa
-00000580: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000590: 7372 630d 0a73 6574 7570 5f72 6571 7569  src..setup_requi
-000005a0: 7265 7320 3d20 7365 7475 7074 6f6f 6c73  res = setuptools
-000005b0: 5f73 636d 0d0a 0d0a 5b6f 7074 696f 6e73  _scm....[options
-000005c0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000005d0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-000005e0: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-000005f0: 6f69 6e74 735d 0d0a 6e61 7061 7269 2e6d  oints]..napari.m
-00000600: 616e 6966 6573 7420 3d20 6e61 7061 7269  anifest = napari
-00000610: 2d50 6978 5365 7120 3d20 6e61 7061 7269  -PixSeq = napari
-00000620: 5f70 6978 7365 713a 6e61 7061 7269 2e79  _pixseq:napari.y
-00000630: 616d 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e  aml....[options.
-00000640: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
-00000650: 0a74 6573 7469 6e67 203d 200d 0a09 746f  .testing = ...to
-00000660: 780d 0a09 7079 7465 7374 2020 2320 6874  x...pytest  # ht
-00000670: 7470 733a 2f2f 646f 6373 2e70 7974 6573  tps://docs.pytes
-00000680: 742e 6f72 672f 656e 2f6c 6174 6573 742f  t.org/en/latest/
-00000690: 636f 6e74 656e 7473 2e68 746d 6c0d 0a09  contents.html...
-000006a0: 7079 7465 7374 2d63 6f76 2020 2320 6874  pytest-cov  # ht
-000006b0: 7470 733a 2f2f 7079 7465 7374 2d63 6f76  tps://pytest-cov
-000006c0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000006d0: 656e 2f6c 6174 6573 742f 0d0a 0970 7974  en/latest/...pyt
-000006e0: 6573 742d 7174 2020 2320 6874 7470 733a  est-qt  # https:
-000006f0: 2f2f 7079 7465 7374 2d71 742e 7265 6164  //pytest-qt.read
-00000700: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000710: 7465 7374 2f0d 0a09 6e61 7061 7269 0d0a  test/...napari..
-00000720: 0970 7971 7435 0d0a 0d0a 5b6f 7074 696f  .pyqt5....[optio
-00000730: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000740: 0d0a 2a20 3d20 2a2e 7961 6d6c 0d0a 0d0a  ..* = *.yaml....
-00000750: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000760: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000770: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000540: 2d74 6f6f 6c73 0d0a 0974 6f72 6368 0d0a  -tools...torch..
+00000550: 0963 656c 6c70 6f73 6520 3e3d 2033 2e30  .cellpose >= 3.0
+00000560: 2e31 0d0a 096f 6d6e 6970 6f73 650d 0a09  .1...omnipose...
+00000570: 7472 6163 6b70 790d 0a09 7368 6170 656c  trackpy...shapel
+00000580: 790d 0a09 6173 7472 6f70 790d 0a70 7974  y...astropy..pyt
+00000590: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000005a0: 3d33 2e38 0d0a 696e 636c 7564 655f 7061  =3.8..include_pa
+000005b0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+000005c0: 650d 0a70 6163 6b61 6765 5f64 6972 203d  e..package_dir =
+000005d0: 200d 0a09 3d73 7263 0d0a 7365 7475 705f   ...=src..setup_
+000005e0: 7265 7175 6972 6573 203d 2073 6574 7570  requires = setup
+000005f0: 746f 6f6c 735f 7363 6d0d 0a0d 0a5b 6f70  tools_scm....[op
+00000600: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000610: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000620: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  c....[options.en
+00000630: 7472 795f 706f 696e 7473 5d0d 0a6e 6170  try_points]..nap
+00000640: 6172 692e 6d61 6e69 6665 7374 203d 206e  ari.manifest = n
+00000650: 6170 6172 692d 5069 7853 6571 203d 206e  apari-PixSeq = n
+00000660: 6170 6172 695f 7069 7873 6571 3a6e 6170  apari_pixseq:nap
+00000670: 6172 692e 7961 6d6c 0d0a 0d0a 5b6f 7074  ari.yaml....[opt
+00000680: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
+00000690: 6972 655d 0d0a 7465 7374 696e 6720 3d20  ire]..testing = 
+000006a0: 0d0a 0974 6f78 0d0a 0970 7974 6573 7420  ...tox...pytest 
+000006b0: 2023 2068 7474 7073 3a2f 2f64 6f63 732e   # https://docs.
+000006c0: 7079 7465 7374 2e6f 7267 2f65 6e2f 6c61  pytest.org/en/la
+000006d0: 7465 7374 2f63 6f6e 7465 6e74 732e 6874  test/contents.ht
+000006e0: 6d6c 0d0a 0970 7974 6573 742d 636f 7620  ml...pytest-cov 
+000006f0: 2023 2068 7474 7073 3a2f 2f70 7974 6573   # https://pytes
+00000700: 742d 636f 762e 7265 6164 7468 6564 6f63  t-cov.readthedoc
+00000710: 732e 696f 2f65 6e2f 6c61 7465 7374 2f0d  s.io/en/latest/.
+00000720: 0a09 7079 7465 7374 2d71 7420 2023 2068  ..pytest-qt  # h
+00000730: 7474 7073 3a2f 2f70 7974 6573 742d 7174  ttps://pytest-qt
+00000740: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000750: 656e 2f6c 6174 6573 742f 0d0a 096e 6170  en/latest/...nap
+00000760: 6172 690d 0a09 7079 7174 350d 0a0d 0a5b  ari...pyqt5....[
+00000770: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+00000780: 6461 7461 5d0d 0a2a 203d 202a 2e79 616d  data]..* = *.yam
+00000790: 6c0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  l....[egg_info].
+000007a0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000007b0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `napari-PixSeq-1.0.0/src/napari_PixSeq.egg-info/SOURCES.txt` & `napari_pixseq-1.0.2/src/napari_PixSeq.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,33 @@
 src/napari_pixseq/napari.yaml
 src/napari_pixseq/pixseq_widget.py
 src/napari_pixseq/GUI/__init__.py
 src/napari_pixseq/GUI/pixseq_ui.py
 src/napari_pixseq/GUI/pixseq_ui.ui
 src/napari_pixseq/_tests/__init__.py
 src/napari_pixseq/_tests/test_widget.py
+src/napari_pixseq/dev/__init__.py
+src/napari_pixseq/dev/ebfret_IO_dev.py
+src/napari_pixseq/dev/refactor.py
+src/napari_pixseq/dev/spot_mask_dev.py
 src/napari_pixseq/funcs/__init__.py
 src/napari_pixseq/funcs/pixseq_align_utils.py
 src/napari_pixseq/funcs/pixseq_cluster_utils.py
 src/napari_pixseq/funcs/pixseq_colocalize_utils.py
 src/napari_pixseq/funcs/pixseq_events.py
 src/napari_pixseq/funcs/pixseq_export_images_utils.py
 src/napari_pixseq/funcs/pixseq_export_traces_utils.py
+src/napari_pixseq/funcs/pixseq_filter_utils.py
 src/napari_pixseq/funcs/pixseq_import_utils.py
 src/napari_pixseq/funcs/pixseq_loc_utils.py
 src/napari_pixseq/funcs/pixseq_picasso_detect.py
 src/napari_pixseq/funcs/pixseq_plot_utils.py
+src/napari_pixseq/funcs/pixseq_segmentation_events.py
+src/napari_pixseq/funcs/pixseq_segmentation_utils.py
+src/napari_pixseq/funcs/pixseq_simple_analysis_utils.py
 src/napari_pixseq/funcs/pixseq_temporal_filtering.py
 src/napari_pixseq/funcs/pixseq_trace_compute_utils.py
+src/napari_pixseq/funcs/pixseq_tracking_utils.py
 src/napari_pixseq/funcs/pixseq_transform_utils.py
 src/napari_pixseq/funcs/pixseq_undrift_utils.py
-src/napari_pixseq/funcs/pixseq_utils_compute.py
+src/napari_pixseq/funcs/pixseq_utils_compute.py
+src/napari_pixseq/scripts/pypi
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/GUI/pixseq_ui.py` & `napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Frame(object):
     def setupUi(self, Frame):
         Frame.setObjectName("Frame")
-        Frame.resize(763, 625)
+        Frame.resize(661, 625)
         self.verticalLayout = QtWidgets.QVBoxLayout(Frame)
         self.verticalLayout.setObjectName("verticalLayout")
         self.tabWidget = QtWidgets.QTabWidget(Frame)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabWidget.sizePolicy().hasHeightForWidth())
@@ -51,14 +51,15 @@
         self.pixseq_import_mode.addItem("")
         self.pixseq_import_mode.addItem("")
         self.pixseq_import_mode.addItem("")
         self.pixseq_import_mode.addItem("")
         self.pixseq_import_mode.addItem("")
         self.pixseq_import_mode.addItem("")
         self.pixseq_import_mode.addItem("")
+        self.pixseq_import_mode.addItem("")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.pixseq_import_mode)
         self.pixseq_channel_layout_label = QtWidgets.QLabel(self.tab_15)
         self.pixseq_channel_layout_label.setObjectName("pixseq_channel_layout_label")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.pixseq_channel_layout_label)
         self.pixseq_channel_layout = QtWidgets.QComboBox(self.tab_15)
         self.pixseq_channel_layout.setObjectName("pixseq_channel_layout")
         self.pixseq_channel_layout.addItem("")
@@ -89,14 +90,17 @@
         self.pixseq_append_dataset = QtWidgets.QComboBox(self.tab_15)
         self.pixseq_append_dataset.setObjectName("pixseq_append_dataset")
         self.formLayout.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.pixseq_append_dataset)
         self.pixseq_append_dataset_label = QtWidgets.QLabel(self.tab_15)
         self.pixseq_append_dataset_label.setObjectName("pixseq_append_dataset_label")
         self.formLayout.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.pixseq_append_dataset_label)
         self.verticalLayout_18.addLayout(self.formLayout)
+        self.pixseq_concatenate = QtWidgets.QCheckBox(self.tab_15)
+        self.pixseq_concatenate.setObjectName("pixseq_concatenate")
+        self.verticalLayout_18.addWidget(self.pixseq_concatenate)
         self.pixseq_append = QtWidgets.QCheckBox(self.tab_15)
         self.pixseq_append.setObjectName("pixseq_append")
         self.verticalLayout_18.addWidget(self.pixseq_append)
         self.pixseq_import = QtWidgets.QPushButton(self.tab_15)
         self.pixseq_import.setObjectName("pixseq_import")
         self.verticalLayout_18.addWidget(self.pixseq_import)
         self.tabWidget_4.addTab(self.tab_15, "")
@@ -382,172 +386,674 @@
         spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_5.addItem(spacerItem6)
         self.tabWidget_5.addTab(self.tab_4, "")
         self.verticalLayout_13.addWidget(self.tabWidget_5)
         spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_13.addItem(spacerItem7)
         self.tabWidget.addTab(self.tab_10, "")
+        self.tab_19 = QtWidgets.QWidget()
+        self.tab_19.setObjectName("tab_19")
+        self.verticalLayout_22 = QtWidgets.QVBoxLayout(self.tab_19)
+        self.verticalLayout_22.setObjectName("verticalLayout_22")
+        self.label_94 = QtWidgets.QLabel(self.tab_19)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_94.setFont(font)
+        self.label_94.setObjectName("label_94")
+        self.verticalLayout_22.addWidget(self.label_94)
+        self.gridLayout_8 = QtWidgets.QGridLayout()
+        self.gridLayout_8.setObjectName("gridLayout_8")
+        self.add_line = QtWidgets.QPushButton(self.tab_19)
+        self.add_line.setObjectName("add_line")
+        self.gridLayout_8.addWidget(self.add_line, 0, 0, 1, 1)
+        self.add_box = QtWidgets.QPushButton(self.tab_19)
+        self.add_box.setObjectName("add_box")
+        self.gridLayout_8.addWidget(self.add_box, 0, 1, 1, 1)
+        self.add_background = QtWidgets.QPushButton(self.tab_19)
+        self.add_background.setObjectName("add_background")
+        self.gridLayout_8.addWidget(self.add_background, 0, 2, 1, 1)
+        self.verticalLayout_22.addLayout(self.gridLayout_8)
+        spacerItem8 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_22.addItem(spacerItem8)
+        self.label_88 = QtWidgets.QLabel(self.tab_19)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_88.setFont(font)
+        self.label_88.setObjectName("label_88")
+        self.verticalLayout_22.addWidget(self.label_88)
+        self.formLayout_17 = QtWidgets.QFormLayout()
+        self.formLayout_17.setObjectName("formLayout_17")
+        self.label_77 = QtWidgets.QLabel(self.tab_19)
+        self.label_77.setObjectName("label_77")
+        self.formLayout_17.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_77)
+        self.label_78 = QtWidgets.QLabel(self.tab_19)
+        self.label_78.setObjectName("label_78")
+        self.formLayout_17.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_78)
+        self.simple_plot_dataset = QtWidgets.QComboBox(self.tab_19)
+        self.simple_plot_dataset.setObjectName("simple_plot_dataset")
+        self.formLayout_17.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.simple_plot_dataset)
+        self.label_79 = QtWidgets.QLabel(self.tab_19)
+        self.label_79.setObjectName("label_79")
+        self.formLayout_17.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_79)
+        self.simple_plot_channel = QtWidgets.QComboBox(self.tab_19)
+        self.simple_plot_channel.setObjectName("simple_plot_channel")
+        self.formLayout_17.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.simple_plot_channel)
+        self.simple_plot_mode = QtWidgets.QComboBox(self.tab_19)
+        self.simple_plot_mode.setObjectName("simple_plot_mode")
+        self.simple_plot_mode.addItem("")
+        self.simple_plot_mode.addItem("")
+        self.simple_plot_mode.addItem("")
+        self.formLayout_17.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.simple_plot_mode)
+        self.verticalLayout_22.addLayout(self.formLayout_17)
+        self.simple_subtract_background = QtWidgets.QCheckBox(self.tab_19)
+        self.simple_subtract_background.setObjectName("simple_subtract_background")
+        self.verticalLayout_22.addWidget(self.simple_subtract_background)
+        self.simple_graph_container = QtWidgets.QWidget(self.tab_19)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.MinimumExpanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.simple_graph_container.sizePolicy().hasHeightForWidth())
+        self.simple_graph_container.setSizePolicy(sizePolicy)
+        self.simple_graph_container.setMinimumSize(QtCore.QSize(50, 0))
+        self.simple_graph_container.setToolTipDuration(0)
+        self.simple_graph_container.setObjectName("simple_graph_container")
+        self.verticalLayout_22.addWidget(self.simple_graph_container)
+        self.tabWidget.addTab(self.tab_19, "")
+        self.tab_25 = QtWidgets.QWidget()
+        self.tab_25.setObjectName("tab_25")
+        self.verticalLayout_27 = QtWidgets.QVBoxLayout(self.tab_25)
+        self.verticalLayout_27.setObjectName("verticalLayout_27")
+        self.tabWidget_7 = QtWidgets.QTabWidget(self.tab_25)
+        self.tabWidget_7.setObjectName("tabWidget_7")
+        self.tab_24 = QtWidgets.QWidget()
+        self.tab_24.setObjectName("tab_24")
+        self.verticalLayout_28 = QtWidgets.QVBoxLayout(self.tab_24)
+        self.verticalLayout_28.setObjectName("verticalLayout_28")
+        self.label_97 = QtWidgets.QLabel(self.tab_24)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_97.setFont(font)
+        self.label_97.setObjectName("label_97")
+        self.verticalLayout_28.addWidget(self.label_97)
+        self.formLayout_28 = QtWidgets.QFormLayout()
+        self.formLayout_28.setObjectName("formLayout_28")
+        self.label_101 = QtWidgets.QLabel(self.tab_24)
+        self.label_101.setObjectName("label_101")
+        self.formLayout_28.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_101)
+        self.cellpose_dataset = QtWidgets.QComboBox(self.tab_24)
+        self.cellpose_dataset.setObjectName("cellpose_dataset")
+        self.formLayout_28.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_dataset)
+        self.label_105 = QtWidgets.QLabel(self.tab_24)
+        self.label_105.setObjectName("label_105")
+        self.formLayout_28.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_105)
+        self.cellpose_channel = QtWidgets.QComboBox(self.tab_24)
+        self.cellpose_channel.setObjectName("cellpose_channel")
+        self.formLayout_28.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_channel)
+        self.verticalLayout_28.addLayout(self.formLayout_28)
+        spacerItem9 = QtWidgets.QSpacerItem(592, 17, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_28.addItem(spacerItem9)
+        self.label_102 = QtWidgets.QLabel(self.tab_24)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_102.setFont(font)
+        self.label_102.setObjectName("label_102")
+        self.verticalLayout_28.addWidget(self.label_102)
+        self.formLayout_27 = QtWidgets.QFormLayout()
+        self.formLayout_27.setObjectName("formLayout_27")
+        self.label_104 = QtWidgets.QLabel(self.tab_24)
+        self.label_104.setObjectName("label_104")
+        self.formLayout_27.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_104)
+        self.cellpose_model = QtWidgets.QComboBox(self.tab_24)
+        self.cellpose_model.setObjectName("cellpose_model")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.cellpose_model.addItem("")
+        self.formLayout_27.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_model)
+        self.label_123 = QtWidgets.QLabel(self.tab_24)
+        self.label_123.setObjectName("label_123")
+        self.formLayout_27.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_123)
+        self.cellpose_batchsize = QtWidgets.QComboBox(self.tab_24)
+        self.cellpose_batchsize.setObjectName("cellpose_batchsize")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.cellpose_batchsize.addItem("")
+        self.formLayout_27.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_batchsize)
+        self.verticalLayout_28.addLayout(self.formLayout_27)
+        self.gridLayout_11 = QtWidgets.QGridLayout()
+        self.gridLayout_11.setObjectName("gridLayout_11")
+        self.cellpose_flowthresh_label = QtWidgets.QLabel(self.tab_24)
+        self.cellpose_flowthresh_label.setMinimumSize(QtCore.QSize(28, 22))
+        self.cellpose_flowthresh_label.setObjectName("cellpose_flowthresh_label")
+        self.gridLayout_11.addWidget(self.cellpose_flowthresh_label, 0, 2, 1, 1, QtCore.Qt.AlignLeft)
+        self.cellpose_flowthresh = QtWidgets.QSlider(self.tab_24)
+        self.cellpose_flowthresh.setMaximum(100)
+        self.cellpose_flowthresh.setSingleStep(10)
+        self.cellpose_flowthresh.setPageStep(10)
+        self.cellpose_flowthresh.setSliderPosition(90)
+        self.cellpose_flowthresh.setOrientation(QtCore.Qt.Horizontal)
+        self.cellpose_flowthresh.setObjectName("cellpose_flowthresh")
+        self.gridLayout_11.addWidget(self.cellpose_flowthresh, 0, 1, 1, 1)
+        self.label_106 = QtWidgets.QLabel(self.tab_24)
+        self.label_106.setObjectName("label_106")
+        self.gridLayout_11.addWidget(self.label_106, 0, 0, 1, 1)
+        self.cellpose_maskthresh_label = QtWidgets.QLabel(self.tab_24)
+        self.cellpose_maskthresh_label.setMinimumSize(QtCore.QSize(28, 22))
+        self.cellpose_maskthresh_label.setObjectName("cellpose_maskthresh_label")
+        self.gridLayout_11.addWidget(self.cellpose_maskthresh_label, 1, 2, 1, 1, QtCore.Qt.AlignLeft)
+        self.cellpose_minsize_label = QtWidgets.QLabel(self.tab_24)
+        self.cellpose_minsize_label.setMinimumSize(QtCore.QSize(24, 22))
+        self.cellpose_minsize_label.setMaximumSize(QtCore.QSize(24, 16777215))
+        self.cellpose_minsize_label.setObjectName("cellpose_minsize_label")
+        self.gridLayout_11.addWidget(self.cellpose_minsize_label, 2, 2, 1, 1, QtCore.Qt.AlignLeft)
+        self.label_107 = QtWidgets.QLabel(self.tab_24)
+        self.label_107.setObjectName("label_107")
+        self.gridLayout_11.addWidget(self.label_107, 1, 0, 1, 1)
+        self.label_108 = QtWidgets.QLabel(self.tab_24)
+        self.label_108.setObjectName("label_108")
+        self.gridLayout_11.addWidget(self.label_108, 2, 0, 1, 1)
+        self.cellpose_minsize = QtWidgets.QSlider(self.tab_24)
+        self.cellpose_minsize.setMaximum(200)
+        self.cellpose_minsize.setSingleStep(10)
+        self.cellpose_minsize.setProperty("value", 15)
+        self.cellpose_minsize.setOrientation(QtCore.Qt.Horizontal)
+        self.cellpose_minsize.setTickPosition(QtWidgets.QSlider.NoTicks)
+        self.cellpose_minsize.setTickInterval(10)
+        self.cellpose_minsize.setObjectName("cellpose_minsize")
+        self.gridLayout_11.addWidget(self.cellpose_minsize, 2, 1, 1, 1)
+        self.cellpose_maskthresh = QtWidgets.QSlider(self.tab_24)
+        self.cellpose_maskthresh.setMaximum(100)
+        self.cellpose_maskthresh.setSingleStep(10)
+        self.cellpose_maskthresh.setPageStep(10)
+        self.cellpose_maskthresh.setOrientation(QtCore.Qt.Horizontal)
+        self.cellpose_maskthresh.setObjectName("cellpose_maskthresh")
+        self.gridLayout_11.addWidget(self.cellpose_maskthresh, 1, 1, 1, 1)
+        self.cellpose_diameter = QtWidgets.QSlider(self.tab_24)
+        self.cellpose_diameter.setMaximum(100)
+        self.cellpose_diameter.setSingleStep(10)
+        self.cellpose_diameter.setProperty("value", 15)
+        self.cellpose_diameter.setOrientation(QtCore.Qt.Horizontal)
+        self.cellpose_diameter.setObjectName("cellpose_diameter")
+        self.gridLayout_11.addWidget(self.cellpose_diameter, 3, 1, 1, 1)
+        self.label_109 = QtWidgets.QLabel(self.tab_24)
+        self.label_109.setObjectName("label_109")
+        self.gridLayout_11.addWidget(self.label_109, 3, 0, 1, 1)
+        self.cellpose_diameter_label = QtWidgets.QLabel(self.tab_24)
+        self.cellpose_diameter_label.setObjectName("cellpose_diameter_label")
+        self.gridLayout_11.addWidget(self.cellpose_diameter_label, 3, 2, 1, 1)
+        self.verticalLayout_28.addLayout(self.gridLayout_11)
+        self.cellpose_invert_images = QtWidgets.QCheckBox(self.tab_24)
+        self.cellpose_invert_images.setObjectName("cellpose_invert_images")
+        self.verticalLayout_28.addWidget(self.cellpose_invert_images)
+        spacerItem10 = QtWidgets.QSpacerItem(592, 17, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_28.addItem(spacerItem10)
+        self.label_110 = QtWidgets.QLabel(self.tab_24)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_110.setFont(font)
+        self.label_110.setObjectName("label_110")
+        self.verticalLayout_28.addWidget(self.label_110)
+        self.cellpose_load_model = QtWidgets.QPushButton(self.tab_24)
+        self.cellpose_load_model.setObjectName("cellpose_load_model")
+        self.verticalLayout_28.addWidget(self.cellpose_load_model)
+        self.gridLayout_12 = QtWidgets.QGridLayout()
+        self.gridLayout_12.setObjectName("gridLayout_12")
+        self.segment_all = QtWidgets.QPushButton(self.tab_24)
+        self.segment_all.setObjectName("segment_all")
+        self.gridLayout_12.addWidget(self.segment_all, 0, 1, 1, 1)
+        self.segment_active = QtWidgets.QPushButton(self.tab_24)
+        self.segment_active.setObjectName("segment_active")
+        self.gridLayout_12.addWidget(self.segment_active, 0, 0, 1, 1)
+        self.verticalLayout_28.addLayout(self.gridLayout_12)
+        self.cellpose_progress = QtWidgets.QProgressBar(self.tab_24)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.cellpose_progress.sizePolicy().hasHeightForWidth())
+        self.cellpose_progress.setSizePolicy(sizePolicy)
+        self.cellpose_progress.setMinimumSize(QtCore.QSize(0, 0))
+        self.cellpose_progress.setMaximumSize(QtCore.QSize(16777215, 10))
+        self.cellpose_progress.setProperty("value", 0)
+        self.cellpose_progress.setObjectName("cellpose_progress")
+        self.verticalLayout_28.addWidget(self.cellpose_progress)
+        spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_28.addItem(spacerItem11)
+        self.tabWidget_7.addTab(self.tab_24, "")
+        self.tab_26 = QtWidgets.QWidget()
+        self.tab_26.setObjectName("tab_26")
+        self.verticalLayout_30 = QtWidgets.QVBoxLayout(self.tab_26)
+        self.verticalLayout_30.setObjectName("verticalLayout_30")
+        self.label_103 = QtWidgets.QLabel(self.tab_26)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_103.setFont(font)
+        self.label_103.setObjectName("label_103")
+        self.verticalLayout_30.addWidget(self.label_103)
+        self.formLayout_26 = QtWidgets.QFormLayout()
+        self.formLayout_26.setObjectName("formLayout_26")
+        self.label_111 = QtWidgets.QLabel(self.tab_26)
+        self.label_111.setObjectName("label_111")
+        self.formLayout_26.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_111)
+        self.dilatation_size = QtWidgets.QDoubleSpinBox(self.tab_26)
+        self.dilatation_size.setDecimals(1)
+        self.dilatation_size.setMinimum(0.1)
+        self.dilatation_size.setMaximum(10.0)
+        self.dilatation_size.setProperty("value", 1.0)
+        self.dilatation_size.setObjectName("dilatation_size")
+        self.formLayout_26.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.dilatation_size)
+        self.verticalLayout_30.addLayout(self.formLayout_26)
+        self.dilate_segmentations = QtWidgets.QPushButton(self.tab_26)
+        self.dilate_segmentations.setObjectName("dilate_segmentations")
+        self.verticalLayout_30.addWidget(self.dilate_segmentations)
+        spacerItem12 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_30.addItem(spacerItem12)
+        self.tabWidget_7.addTab(self.tab_26, "")
+        self.verticalLayout_27.addWidget(self.tabWidget_7)
+        spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_27.addItem(spacerItem13)
+        self.tabWidget.addTab(self.tab_25, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
-        self.label_3 = QtWidgets.QLabel(self.tab_2)
+        self.tabWidget_6 = QtWidgets.QTabWidget(self.tab_2)
+        self.tabWidget_6.setObjectName("tabWidget_6")
+        self.tab_21 = QtWidgets.QWidget()
+        self.tab_21.setObjectName("tab_21")
+        self.verticalLayout_23 = QtWidgets.QVBoxLayout(self.tab_21)
+        self.verticalLayout_23.setObjectName("verticalLayout_23")
+        self.label_3 = QtWidgets.QLabel(self.tab_21)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_3.setFont(font)
         self.label_3.setObjectName("label_3")
-        self.verticalLayout_3.addWidget(self.label_3)
+        self.verticalLayout_23.addWidget(self.label_3)
         self.formLayout_3 = QtWidgets.QFormLayout()
         self.formLayout_3.setObjectName("formLayout_3")
-        self.label_7 = QtWidgets.QLabel(self.tab_2)
+        self.label_7 = QtWidgets.QLabel(self.tab_21)
         self.label_7.setObjectName("label_7")
         self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_7)
-        self.picasso_detect_mode = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_detect_mode = QtWidgets.QComboBox(self.tab_21)
         self.picasso_detect_mode.setObjectName("picasso_detect_mode")
         self.picasso_detect_mode.addItem("")
         self.picasso_detect_mode.addItem("")
         self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_detect_mode)
-        self.label_11 = QtWidgets.QLabel(self.tab_2)
+        self.label_11 = QtWidgets.QLabel(self.tab_21)
         self.label_11.setObjectName("label_11")
         self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_11)
-        self.picasso_dataset = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_dataset = QtWidgets.QComboBox(self.tab_21)
         self.picasso_dataset.setObjectName("picasso_dataset")
         self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_dataset)
-        self.label_6 = QtWidgets.QLabel(self.tab_2)
+        self.label_6 = QtWidgets.QLabel(self.tab_21)
         self.label_6.setObjectName("label_6")
         self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_6)
-        self.picasso_channel = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_channel = QtWidgets.QComboBox(self.tab_21)
         self.picasso_channel.setObjectName("picasso_channel")
         self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_channel)
-        self.label_8 = QtWidgets.QLabel(self.tab_2)
+        self.label_8 = QtWidgets.QLabel(self.tab_21)
         self.label_8.setObjectName("label_8")
         self.formLayout_3.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_8)
-        self.picasso_frame_mode = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_frame_mode = QtWidgets.QComboBox(self.tab_21)
         self.picasso_frame_mode.setObjectName("picasso_frame_mode")
         self.picasso_frame_mode.addItem("")
         self.picasso_frame_mode.addItem("")
         self.formLayout_3.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.picasso_frame_mode)
-        self.label_5 = QtWidgets.QLabel(self.tab_2)
+        self.label_5 = QtWidgets.QLabel(self.tab_21)
         self.label_5.setObjectName("label_5")
         self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_5)
-        self.picasso_min_net_gradient = QtWidgets.QLineEdit(self.tab_2)
+        self.picasso_min_net_gradient = QtWidgets.QLineEdit(self.tab_21)
         self.picasso_min_net_gradient.setObjectName("picasso_min_net_gradient")
         self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.picasso_min_net_gradient)
-        self.label_28 = QtWidgets.QLabel(self.tab_2)
+        self.label_28 = QtWidgets.QLabel(self.tab_21)
         self.label_28.setObjectName("label_28")
         self.formLayout_3.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_28)
-        self.picasso_box_size = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_box_size = QtWidgets.QComboBox(self.tab_21)
         self.picasso_box_size.setObjectName("picasso_box_size")
         self.picasso_box_size.addItem("")
         self.picasso_box_size.addItem("")
         self.picasso_box_size.addItem("")
         self.picasso_box_size.addItem("")
+        self.picasso_box_size.addItem("")
+        self.picasso_box_size.addItem("")
+        self.picasso_box_size.addItem("")
         self.formLayout_3.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.picasso_box_size)
-        self.label_35 = QtWidgets.QLabel(self.tab_2)
+        self.label_35 = QtWidgets.QLabel(self.tab_21)
         self.label_35.setObjectName("label_35")
         self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_35)
-        self.picasso_roi_border_width = QtWidgets.QLineEdit(self.tab_2)
+        self.picasso_roi_border_width = QtWidgets.QLineEdit(self.tab_21)
         self.picasso_roi_border_width.setObjectName("picasso_roi_border_width")
         self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.picasso_roi_border_width)
-        self.verticalLayout_3.addLayout(self.formLayout_3)
-        self.picasso_remove_overlapping = QtWidgets.QCheckBox(self.tab_2)
+        self.verticalLayout_23.addLayout(self.formLayout_3)
+        self.picasso_remove_overlapping = QtWidgets.QCheckBox(self.tab_21)
         self.picasso_remove_overlapping.setChecked(True)
         self.picasso_remove_overlapping.setObjectName("picasso_remove_overlapping")
-        self.verticalLayout_3.addWidget(self.picasso_remove_overlapping)
-        self.picasso_window_cropping = QtWidgets.QCheckBox(self.tab_2)
+        self.verticalLayout_23.addWidget(self.picasso_remove_overlapping)
+        self.picasso_window_cropping = QtWidgets.QCheckBox(self.tab_21)
         self.picasso_window_cropping.setObjectName("picasso_window_cropping")
-        self.verticalLayout_3.addWidget(self.picasso_window_cropping)
+        self.verticalLayout_23.addWidget(self.picasso_window_cropping)
+        self.picasso_segmentation_filtering = QtWidgets.QCheckBox(self.tab_21)
+        self.picasso_segmentation_filtering.setObjectName("picasso_segmentation_filtering")
+        self.verticalLayout_23.addWidget(self.picasso_segmentation_filtering)
+        self.picasso_minimise_ram = QtWidgets.QCheckBox(self.tab_21)
+        self.picasso_minimise_ram.setObjectName("picasso_minimise_ram")
+        self.verticalLayout_23.addWidget(self.picasso_minimise_ram)
         self.gridLayout_6 = QtWidgets.QGridLayout()
         self.gridLayout_6.setObjectName("gridLayout_6")
-        self.picasso_fit = QtWidgets.QPushButton(self.tab_2)
+        self.picasso_fit = QtWidgets.QPushButton(self.tab_21)
         self.picasso_fit.setObjectName("picasso_fit")
         self.gridLayout_6.addWidget(self.picasso_fit, 0, 1, 1, 1)
-        self.picasso_detect = QtWidgets.QPushButton(self.tab_2)
+        self.picasso_detect = QtWidgets.QPushButton(self.tab_21)
         self.picasso_detect.setObjectName("picasso_detect")
         self.gridLayout_6.addWidget(self.picasso_detect, 0, 0, 1, 1)
-        self.picasso_detectfit = QtWidgets.QPushButton(self.tab_2)
+        self.picasso_detectfit = QtWidgets.QPushButton(self.tab_21)
         self.picasso_detectfit.setObjectName("picasso_detectfit")
         self.gridLayout_6.addWidget(self.picasso_detectfit, 0, 2, 1, 1)
-        self.verticalLayout_3.addLayout(self.gridLayout_6)
-        self.picasso_progressbar = QtWidgets.QProgressBar(self.tab_2)
+        self.verticalLayout_23.addLayout(self.gridLayout_6)
+        self.picasso_progressbar = QtWidgets.QProgressBar(self.tab_21)
         self.picasso_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.picasso_progressbar.setProperty("value", 0)
         self.picasso_progressbar.setObjectName("picasso_progressbar")
-        self.verticalLayout_3.addWidget(self.picasso_progressbar)
-        spacerItem8 = QtWidgets.QSpacerItem(354, 2, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem8)
-        self.label_27 = QtWidgets.QLabel(self.tab_2)
+        self.verticalLayout_23.addWidget(self.picasso_progressbar)
+        spacerItem14 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.MinimumExpanding)
+        self.verticalLayout_23.addItem(spacerItem14)
+        self.tabWidget_6.addTab(self.tab_21, "")
+        self.tab_23 = QtWidgets.QWidget()
+        self.tab_23.setObjectName("tab_23")
+        self.verticalLayout_26 = QtWidgets.QVBoxLayout(self.tab_23)
+        self.verticalLayout_26.setObjectName("verticalLayout_26")
+        self.label_92 = QtWidgets.QLabel(self.tab_23)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_92.setFont(font)
+        self.label_92.setObjectName("label_92")
+        self.verticalLayout_26.addWidget(self.label_92)
+        self.formLayout_24 = QtWidgets.QFormLayout()
+        self.formLayout_24.setObjectName("formLayout_24")
+        self.picasso_filter_dataset_label = QtWidgets.QLabel(self.tab_23)
+        self.picasso_filter_dataset_label.setObjectName("picasso_filter_dataset_label")
+        self.formLayout_24.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.picasso_filter_dataset_label)
+        self.picasso_filter_dataset = QtWidgets.QComboBox(self.tab_23)
+        self.picasso_filter_dataset.setObjectName("picasso_filter_dataset")
+        self.formLayout_24.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_filter_dataset)
+        self.label_89 = QtWidgets.QLabel(self.tab_23)
+        self.label_89.setObjectName("label_89")
+        self.formLayout_24.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_89)
+        self.picasso_filter_channel = QtWidgets.QComboBox(self.tab_23)
+        self.picasso_filter_channel.setObjectName("picasso_filter_channel")
+        self.formLayout_24.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_filter_channel)
+        self.label_90 = QtWidgets.QLabel(self.tab_23)
+        self.label_90.setObjectName("label_90")
+        self.formLayout_24.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_90)
+        self.filter_criterion = QtWidgets.QComboBox(self.tab_23)
+        self.filter_criterion.setObjectName("filter_criterion")
+        self.formLayout_24.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.filter_criterion)
+        self.label_93 = QtWidgets.QLabel(self.tab_23)
+        self.label_93.setObjectName("label_93")
+        self.formLayout_24.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_93)
+        self.picasso_filter_type = QtWidgets.QComboBox(self.tab_23)
+        self.picasso_filter_type.setObjectName("picasso_filter_type")
+        self.picasso_filter_type.addItem("")
+        self.picasso_filter_type.addItem("")
+        self.formLayout_24.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_filter_type)
+        self.verticalLayout_26.addLayout(self.formLayout_24)
+        self.filter_graph_container = QtWidgets.QWidget(self.tab_23)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.filter_graph_container.sizePolicy().hasHeightForWidth())
+        self.filter_graph_container.setSizePolicy(sizePolicy)
+        self.filter_graph_container.setObjectName("filter_graph_container")
+        self.verticalLayout_26.addWidget(self.filter_graph_container)
+        self.label_91 = QtWidgets.QLabel(self.tab_23)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_91.setFont(font)
+        self.label_91.setObjectName("label_91")
+        self.verticalLayout_26.addWidget(self.label_91)
+        self.gridLayout_7 = QtWidgets.QGridLayout()
+        self.gridLayout_7.setObjectName("gridLayout_7")
+        self.formLayout_22 = QtWidgets.QFormLayout()
+        self.formLayout_22.setObjectName("formLayout_22")
+        self.label_86 = QtWidgets.QLabel(self.tab_23)
+        self.label_86.setObjectName("label_86")
+        self.formLayout_22.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_86)
+        self.filter_min = QtWidgets.QDoubleSpinBox(self.tab_23)
+        self.filter_min.setMinimum(-999999999.0)
+        self.filter_min.setMaximum(9999999999.0)
+        self.filter_min.setObjectName("filter_min")
+        self.formLayout_22.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.filter_min)
+        self.gridLayout_7.addLayout(self.formLayout_22, 0, 0, 1, 1)
+        self.formLayout_23 = QtWidgets.QFormLayout()
+        self.formLayout_23.setObjectName("formLayout_23")
+        self.label_87 = QtWidgets.QLabel(self.tab_23)
+        self.label_87.setObjectName("label_87")
+        self.formLayout_23.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_87)
+        self.filter_max = QtWidgets.QDoubleSpinBox(self.tab_23)
+        self.filter_max.setMinimum(-99999999999.0)
+        self.filter_max.setMaximum(9999999999.0)
+        self.filter_max.setObjectName("filter_max")
+        self.formLayout_23.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.filter_max)
+        self.gridLayout_7.addLayout(self.formLayout_23, 0, 1, 1, 1)
+        self.verticalLayout_26.addLayout(self.gridLayout_7)
+        self.filter_localisations = QtWidgets.QPushButton(self.tab_23)
+        self.filter_localisations.setObjectName("filter_localisations")
+        self.verticalLayout_26.addWidget(self.filter_localisations)
+        self.tabWidget_6.addTab(self.tab_23, "")
+        self.tab_20 = QtWidgets.QWidget()
+        self.tab_20.setObjectName("tab_20")
+        self.verticalLayout_25 = QtWidgets.QVBoxLayout(self.tab_20)
+        self.verticalLayout_25.setObjectName("verticalLayout_25")
+        self.label_85 = QtWidgets.QLabel(self.tab_20)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_85.setFont(font)
+        self.label_85.setObjectName("label_85")
+        self.verticalLayout_25.addWidget(self.label_85)
+        self.formLayout_20 = QtWidgets.QFormLayout()
+        self.formLayout_20.setObjectName("formLayout_20")
+        self.label_81 = QtWidgets.QLabel(self.tab_20)
+        self.label_81.setObjectName("label_81")
+        self.formLayout_20.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_81)
+        self.picasso_render_dataset = QtWidgets.QComboBox(self.tab_20)
+        self.picasso_render_dataset.setObjectName("picasso_render_dataset")
+        self.formLayout_20.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.picasso_render_dataset)
+        self.label_82 = QtWidgets.QLabel(self.tab_20)
+        self.label_82.setObjectName("label_82")
+        self.formLayout_20.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_82)
+        self.picasso_render_channel = QtWidgets.QComboBox(self.tab_20)
+        self.picasso_render_channel.setObjectName("picasso_render_channel")
+        self.formLayout_20.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.picasso_render_channel)
+        self.label_83 = QtWidgets.QLabel(self.tab_20)
+        self.label_83.setObjectName("label_83")
+        self.formLayout_20.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_83)
+        self.picasso_render_blur_method = QtWidgets.QComboBox(self.tab_20)
+        self.picasso_render_blur_method.setObjectName("picasso_render_blur_method")
+        self.picasso_render_blur_method.addItem("")
+        self.picasso_render_blur_method.addItem("")
+        self.picasso_render_blur_method.addItem("")
+        self.picasso_render_blur_method.addItem("")
+        self.picasso_render_blur_method.addItem("")
+        self.formLayout_20.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_render_blur_method)
+        self.label_84 = QtWidgets.QLabel(self.tab_20)
+        self.label_84.setObjectName("label_84")
+        self.formLayout_20.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_84)
+        self.picasso_render_min_blur = QtWidgets.QDoubleSpinBox(self.tab_20)
+        self.picasso_render_min_blur.setSingleStep(0.1)
+        self.picasso_render_min_blur.setObjectName("picasso_render_min_blur")
+        self.formLayout_20.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.picasso_render_min_blur)
+        self.verticalLayout_25.addLayout(self.formLayout_20)
+        self.picasso_render = QtWidgets.QPushButton(self.tab_20)
+        self.picasso_render.setObjectName("picasso_render")
+        self.verticalLayout_25.addWidget(self.picasso_render)
+        spacerItem15 = QtWidgets.QSpacerItem(413, 173, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_25.addItem(spacerItem15)
+        self.tabWidget_6.addTab(self.tab_20, "")
+        self.tab_27 = QtWidgets.QWidget()
+        self.tab_27.setObjectName("tab_27")
+        self.verticalLayout_29 = QtWidgets.QVBoxLayout(self.tab_27)
+        self.verticalLayout_29.setObjectName("verticalLayout_29")
+        self.label_80 = QtWidgets.QLabel(self.tab_27)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_80.setFont(font)
+        self.label_80.setObjectName("label_80")
+        self.verticalLayout_29.addWidget(self.label_80)
+        self.formLayout_25 = QtWidgets.QFormLayout()
+        self.formLayout_25.setObjectName("formLayout_25")
+        self.label_95 = QtWidgets.QLabel(self.tab_27)
+        self.label_95.setObjectName("label_95")
+        self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_95)
+        self.tracking_dataset = QtWidgets.QComboBox(self.tab_27)
+        self.tracking_dataset.setObjectName("tracking_dataset")
+        self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.tracking_dataset)
+        self.label_96 = QtWidgets.QLabel(self.tab_27)
+        self.label_96.setObjectName("label_96")
+        self.formLayout_25.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_96)
+        self.tracking_channel = QtWidgets.QComboBox(self.tab_27)
+        self.tracking_channel.setObjectName("tracking_channel")
+        self.formLayout_25.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.tracking_channel)
+        self.label_98 = QtWidgets.QLabel(self.tab_27)
+        self.label_98.setObjectName("label_98")
+        self.formLayout_25.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_98)
+        self.trackpy_search_range = QtWidgets.QDoubleSpinBox(self.tab_27)
+        self.trackpy_search_range.setProperty("value", 1.0)
+        self.trackpy_search_range.setObjectName("trackpy_search_range")
+        self.formLayout_25.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.trackpy_search_range)
+        self.label_99 = QtWidgets.QLabel(self.tab_27)
+        self.label_99.setObjectName("label_99")
+        self.formLayout_25.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_99)
+        self.trackpy_memory = QtWidgets.QSpinBox(self.tab_27)
+        self.trackpy_memory.setObjectName("trackpy_memory")
+        self.formLayout_25.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.trackpy_memory)
+        self.label_100 = QtWidgets.QLabel(self.tab_27)
+        self.label_100.setObjectName("label_100")
+        self.formLayout_25.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_100)
+        self.min_track_length = QtWidgets.QSpinBox(self.tab_27)
+        self.min_track_length.setMinimum(1)
+        self.min_track_length.setObjectName("min_track_length")
+        self.formLayout_25.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.min_track_length)
+        self.verticalLayout_29.addLayout(self.formLayout_25)
+        self.remove_unlinked = QtWidgets.QCheckBox(self.tab_27)
+        self.remove_unlinked.setObjectName("remove_unlinked")
+        self.verticalLayout_29.addWidget(self.remove_unlinked)
+        self.link_localisations = QtWidgets.QPushButton(self.tab_27)
+        self.link_localisations.setObjectName("link_localisations")
+        self.verticalLayout_29.addWidget(self.link_localisations)
+        spacerItem16 = QtWidgets.QSpacerItem(20, 122, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_29.addItem(spacerItem16)
+        self.tabWidget_6.addTab(self.tab_27, "")
+        self.tab_22 = QtWidgets.QWidget()
+        self.tab_22.setObjectName("tab_22")
+        self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.tab_22)
+        self.verticalLayout_24.setObjectName("verticalLayout_24")
+        self.label_27 = QtWidgets.QLabel(self.tab_22)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_27.setFont(font)
         self.label_27.setObjectName("label_27")
-        self.verticalLayout_3.addWidget(self.label_27)
+        self.verticalLayout_24.addWidget(self.label_27)
         self.gridLayout_14 = QtWidgets.QGridLayout()
         self.gridLayout_14.setObjectName("gridLayout_14")
-        self.picasso_vis_size = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_vis_size = QtWidgets.QComboBox(self.tab_22)
         self.picasso_vis_size.setObjectName("picasso_vis_size")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.picasso_vis_size.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_size, 0, 3, 1, 1)
-        self.label_114 = QtWidgets.QLabel(self.tab_2)
+        self.label_114 = QtWidgets.QLabel(self.tab_22)
         self.label_114.setObjectName("label_114")
         self.gridLayout_14.addWidget(self.label_114, 0, 0, 1, 1)
-        self.picasso_vis_mode = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_vis_mode = QtWidgets.QComboBox(self.tab_22)
         self.picasso_vis_mode.setObjectName("picasso_vis_mode")
         self.picasso_vis_mode.addItem("")
         self.picasso_vis_mode.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_mode, 0, 1, 1, 1)
-        self.label_115 = QtWidgets.QLabel(self.tab_2)
+        self.label_115 = QtWidgets.QLabel(self.tab_22)
         self.label_115.setObjectName("label_115")
         self.gridLayout_14.addWidget(self.label_115, 0, 2, 1, 1)
-        self.label_120 = QtWidgets.QLabel(self.tab_2)
+        self.label_120 = QtWidgets.QLabel(self.tab_22)
         self.label_120.setObjectName("label_120")
         self.gridLayout_14.addWidget(self.label_120, 1, 0, 1, 1)
-        self.picasso_vis_opacity = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_vis_opacity = QtWidgets.QComboBox(self.tab_22)
         self.picasso_vis_opacity.setObjectName("picasso_vis_opacity")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.picasso_vis_opacity.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_opacity, 1, 1, 1, 1)
-        self.label_121 = QtWidgets.QLabel(self.tab_2)
+        self.label_121 = QtWidgets.QLabel(self.tab_22)
         self.label_121.setObjectName("label_121")
         self.gridLayout_14.addWidget(self.label_121, 1, 2, 1, 1)
-        self.picasso_vis_edge_width = QtWidgets.QComboBox(self.tab_2)
+        self.picasso_vis_edge_width = QtWidgets.QComboBox(self.tab_22)
         self.picasso_vis_edge_width.setObjectName("picasso_vis_edge_width")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_edge_width, 1, 3, 1, 1)
-        self.verticalLayout_3.addLayout(self.gridLayout_14)
-        spacerItem9 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem9)
+        self.verticalLayout_24.addLayout(self.gridLayout_14)
+        spacerItem17 = QtWidgets.QSpacerItem(354, 254, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_24.addItem(spacerItem17)
+        self.tabWidget_6.addTab(self.tab_22, "")
+        self.verticalLayout_3.addWidget(self.tabWidget_6)
+        spacerItem18 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem18)
         self.tabWidget.addTab(self.tab_2, "")
         self.tab_5 = QtWidgets.QWidget()
         self.tab_5.setObjectName("tab_5")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.tab_5)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.traces_tab_widget = QtWidgets.QTabWidget(self.tab_5)
         self.traces_tab_widget.setObjectName("traces_tab_widget")
@@ -635,16 +1141,16 @@
         self.compute_traces.setObjectName("compute_traces")
         self.verticalLayout_9.addWidget(self.compute_traces)
         self.compute_traces_progressbar = QtWidgets.QProgressBar(self.compute_tab_2)
         self.compute_traces_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.compute_traces_progressbar.setProperty("value", 0)
         self.compute_traces_progressbar.setObjectName("compute_traces_progressbar")
         self.verticalLayout_9.addWidget(self.compute_traces_progressbar)
-        spacerItem10 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_9.addItem(spacerItem10)
+        spacerItem19 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_9.addItem(spacerItem19)
         self.traces_tab_widget.addTab(self.compute_tab_2, "")
         self.view_tab_2 = QtWidgets.QWidget()
         self.view_tab_2.setObjectName("view_tab_2")
         self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.view_tab_2)
         self.verticalLayout_10.setObjectName("verticalLayout_10")
         self.formLayout_12 = QtWidgets.QFormLayout()
         self.formLayout_12.setObjectName("formLayout_12")
@@ -785,14 +1291,16 @@
         self.traces_export_mode.setObjectName("traces_export_mode")
         self.traces_export_mode.addItem("")
         self.traces_export_mode.addItem("")
         self.traces_export_mode.addItem("")
         self.traces_export_mode.addItem("")
         self.traces_export_mode.addItem("")
         self.traces_export_mode.addItem("")
+        self.traces_export_mode.addItem("")
+        self.traces_export_mode.addItem("")
         self.formLayout_13.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.traces_export_mode)
         self.label_45 = QtWidgets.QLabel(self.tab_9)
         self.label_45.setObjectName("label_45")
         self.formLayout_13.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_45)
         self.traces_export_dataset = QtWidgets.QComboBox(self.tab_9)
         self.traces_export_dataset.setObjectName("traces_export_dataset")
         self.traces_export_dataset.addItem("")
@@ -841,48 +1349,57 @@
         self.label_74 = QtWidgets.QLabel(self.tab_14)
         self.label_74.setObjectName("label_74")
         self.verticalLayout_17.addWidget(self.label_74)
         self.formLayout_19 = QtWidgets.QFormLayout()
         self.formLayout_19.setObjectName("formLayout_19")
         self.label_72 = QtWidgets.QLabel(self.tab_14)
         self.label_72.setObjectName("label_72")
-        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_72)
+        self.formLayout_19.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_72)
         self.locs_export_dataset = QtWidgets.QComboBox(self.tab_14)
         self.locs_export_dataset.setObjectName("locs_export_dataset")
-        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.locs_export_dataset)
+        self.formLayout_19.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.locs_export_dataset)
         self.label_73 = QtWidgets.QLabel(self.tab_14)
         self.label_73.setObjectName("label_73")
-        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_73)
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_73)
+        self.locs_export_type = QtWidgets.QComboBox(self.tab_14)
+        self.locs_export_type.setObjectName("locs_export_type")
+        self.locs_export_type.addItem("")
+        self.locs_export_type.addItem("")
+        self.locs_export_type.addItem("")
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.locs_export_type)
+        self.locs_export_channel = QtWidgets.QComboBox(self.tab_14)
+        self.locs_export_channel.setObjectName("locs_export_channel")
+        self.formLayout_19.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.locs_export_channel)
+        self.label_71 = QtWidgets.QLabel(self.tab_14)
+        self.label_71.setObjectName("label_71")
+        self.formLayout_19.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_71)
+        self.label_112 = QtWidgets.QLabel(self.tab_14)
+        self.label_112.setObjectName("label_112")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_112)
         self.locs_export_mode = QtWidgets.QComboBox(self.tab_14)
         self.locs_export_mode.setObjectName("locs_export_mode")
         self.locs_export_mode.addItem("")
         self.locs_export_mode.addItem("")
         self.locs_export_mode.addItem("")
         self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.locs_export_mode)
-        self.locs_export_channel = QtWidgets.QComboBox(self.tab_14)
-        self.locs_export_channel.setObjectName("locs_export_channel")
-        self.formLayout_19.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.locs_export_channel)
-        self.label_71 = QtWidgets.QLabel(self.tab_14)
-        self.label_71.setObjectName("label_71")
-        self.formLayout_19.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_71)
         self.verticalLayout_17.addLayout(self.formLayout_19)
         self.pixseq_export_locs = QtWidgets.QPushButton(self.tab_14)
         self.pixseq_export_locs.setObjectName("pixseq_export_locs")
         self.verticalLayout_17.addWidget(self.pixseq_export_locs)
-        spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_17.addItem(spacerItem11)
+        spacerItem20 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_17.addItem(spacerItem20)
         self.tabWidget_2.addTab(self.tab_14, "")
         self.verticalLayout_11.addWidget(self.tabWidget_2)
         self.export_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.export_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
         self.verticalLayout_11.addWidget(self.export_progressbar)
-        spacerItem12 = QtWidgets.QSpacerItem(354, 414, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_11.addItem(spacerItem12)
+        spacerItem21 = QtWidgets.QSpacerItem(354, 414, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_11.addItem(spacerItem21)
         self.tabWidget.addTab(self.tab_6, "")
         self.tab_7 = QtWidgets.QWidget()
         self.tab_7.setObjectName("tab_7")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_7)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.tabWidget_3 = QtWidgets.QTabWidget(self.tab_7)
         self.tabWidget_3.setObjectName("tabWidget_3")
@@ -911,16 +1428,16 @@
         self.pixseq_new_dataset_name = QtWidgets.QLineEdit(self.tab_11)
         self.pixseq_new_dataset_name.setObjectName("pixseq_new_dataset_name")
         self.formLayout_9.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.pixseq_new_dataset_name)
         self.verticalLayout_14.addLayout(self.formLayout_9)
         self.pixseq_update_dataset_name = QtWidgets.QPushButton(self.tab_11)
         self.pixseq_update_dataset_name.setObjectName("pixseq_update_dataset_name")
         self.verticalLayout_14.addWidget(self.pixseq_update_dataset_name)
-        spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_14.addItem(spacerItem13)
+        spacerItem22 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_14.addItem(spacerItem22)
         self.label_64 = QtWidgets.QLabel(self.tab_11)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_64.setFont(font)
         self.label_64.setObjectName("label_64")
         self.verticalLayout_14.addWidget(self.label_64)
@@ -932,16 +1449,16 @@
         self.delete_dataset_name = QtWidgets.QComboBox(self.tab_11)
         self.delete_dataset_name.setObjectName("delete_dataset_name")
         self.formLayout_16.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.delete_dataset_name)
         self.verticalLayout_14.addLayout(self.formLayout_16)
         self.pixseq_delete_dataset = QtWidgets.QPushButton(self.tab_11)
         self.pixseq_delete_dataset.setObjectName("pixseq_delete_dataset")
         self.verticalLayout_14.addWidget(self.pixseq_delete_dataset)
-        spacerItem14 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_14.addItem(spacerItem14)
+        spacerItem23 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_14.addItem(spacerItem23)
         self.label_66 = QtWidgets.QLabel(self.tab_11)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_66.setFont(font)
         self.label_66.setObjectName("label_66")
         self.verticalLayout_14.addWidget(self.label_66)
@@ -977,16 +1494,16 @@
         self.gap_label.addItem("")
         self.gap_label.addItem("")
         self.formLayout_18.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.gap_label)
         self.verticalLayout_14.addLayout(self.formLayout_18)
         self.pixseq_update_labels = QtWidgets.QPushButton(self.tab_11)
         self.pixseq_update_labels.setObjectName("pixseq_update_labels")
         self.verticalLayout_14.addWidget(self.pixseq_update_labels)
-        spacerItem15 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_14.addItem(spacerItem15)
+        spacerItem24 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_14.addItem(spacerItem24)
         self.tabWidget_3.addTab(self.tab_11, "")
         self.tab_12 = QtWidgets.QWidget()
         self.tab_12.setObjectName("tab_12")
         self.verticalLayout_15 = QtWidgets.QVBoxLayout(self.tab_12)
         self.verticalLayout_15.setObjectName("verticalLayout_15")
         self.label_34 = QtWidgets.QLabel(self.tab_12)
         font = QtGui.QFont()
@@ -1039,16 +1556,16 @@
         self.colo_bboxes.setChecked(True)
         self.colo_bboxes.setObjectName("colo_bboxes")
         self.gridLayout_2.addWidget(self.colo_bboxes, 0, 1, 1, 1)
         self.verticalLayout_15.addLayout(self.gridLayout_2)
         self.pixseq_colocalize = QtWidgets.QPushButton(self.tab_12)
         self.pixseq_colocalize.setObjectName("pixseq_colocalize")
         self.verticalLayout_15.addWidget(self.pixseq_colocalize)
-        spacerItem16 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_15.addItem(spacerItem16)
+        spacerItem25 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_15.addItem(spacerItem25)
         self.label_26 = QtWidgets.QLabel(self.tab_12)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_26.setFont(font)
         self.label_26.setObjectName("label_26")
         self.verticalLayout_15.addWidget(self.label_26)
@@ -1089,16 +1606,16 @@
         self.verticalLayout_15.addLayout(self.formLayout_6)
         self.dbscan_remove_overlapping = QtWidgets.QCheckBox(self.tab_12)
         self.dbscan_remove_overlapping.setObjectName("dbscan_remove_overlapping")
         self.verticalLayout_15.addWidget(self.dbscan_remove_overlapping)
         self.cluster_localisations = QtWidgets.QPushButton(self.tab_12)
         self.cluster_localisations.setObjectName("cluster_localisations")
         self.verticalLayout_15.addWidget(self.cluster_localisations)
-        spacerItem17 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_15.addItem(spacerItem17)
+        spacerItem26 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_15.addItem(spacerItem26)
         self.tabWidget_3.addTab(self.tab_12, "")
         self.tab_13 = QtWidgets.QWidget()
         self.tab_13.setObjectName("tab_13")
         self.verticalLayout_16 = QtWidgets.QVBoxLayout(self.tab_13)
         self.verticalLayout_16.setObjectName("verticalLayout_16")
         self.dev_verbose = QtWidgets.QCheckBox(self.tab_13)
         self.dev_verbose.setObjectName("dev_verbose")
@@ -1143,14 +1660,16 @@
         self.gridLayout.addWidget(self.pixseq_show_aa, 1, 1, 1, 1)
         self.verticalLayout.addLayout(self.gridLayout)
 
         self.retranslateUi(Frame)
         self.tabWidget.setCurrentIndex(0)
         self.tabWidget_4.setCurrentIndex(0)
         self.tabWidget_5.setCurrentIndex(0)
+        self.tabWidget_7.setCurrentIndex(0)
+        self.tabWidget_6.setCurrentIndex(0)
         self.picasso_box_size.setCurrentIndex(0)
         self.picasso_vis_size.setCurrentIndex(4)
         self.picasso_vis_opacity.setCurrentIndex(9)
         self.picasso_vis_edge_width.setCurrentIndex(0)
         self.traces_tab_widget.setCurrentIndex(0)
         self.traces_spot_size.setCurrentIndex(0)
         self.traces_background_buffer.setCurrentIndex(1)
@@ -1159,22 +1678,23 @@
         self.tabWidget_3.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(Frame)
 
     def retranslateUi(self, Frame):
         _translate = QtCore.QCoreApplication.translate
         Frame.setWindowTitle(_translate("Frame", "Frame"))
         self.label.setText(_translate("Frame", "Import Mode"))
-        self.pixseq_import_mode.setItemText(0, _translate("Frame", "FRET"))
-        self.pixseq_import_mode.setItemText(1, _translate("Frame", "Donor"))
-        self.pixseq_import_mode.setItemText(2, _translate("Frame", "Acceptor"))
-        self.pixseq_import_mode.setItemText(3, _translate("Frame", "ALEX"))
-        self.pixseq_import_mode.setItemText(4, _translate("Frame", "DA"))
-        self.pixseq_import_mode.setItemText(5, _translate("Frame", "DD"))
-        self.pixseq_import_mode.setItemText(6, _translate("Frame", "AA"))
-        self.pixseq_import_mode.setItemText(7, _translate("Frame", "AD"))
+        self.pixseq_import_mode.setItemText(0, _translate("Frame", "Single Channel"))
+        self.pixseq_import_mode.setItemText(1, _translate("Frame", "FRET"))
+        self.pixseq_import_mode.setItemText(2, _translate("Frame", "Donor"))
+        self.pixseq_import_mode.setItemText(3, _translate("Frame", "Acceptor"))
+        self.pixseq_import_mode.setItemText(4, _translate("Frame", "ALEX"))
+        self.pixseq_import_mode.setItemText(5, _translate("Frame", "DA"))
+        self.pixseq_import_mode.setItemText(6, _translate("Frame", "DD"))
+        self.pixseq_import_mode.setItemText(7, _translate("Frame", "AA"))
+        self.pixseq_import_mode.setItemText(8, _translate("Frame", "AD"))
         self.pixseq_channel_layout_label.setText(_translate("Frame", "Channel Layout"))
         self.pixseq_channel_layout.setItemText(0, _translate("Frame", "Donor-Acceptor"))
         self.pixseq_channel_layout.setItemText(1, _translate("Frame", "Acceptor-Donor"))
         self.pixseq_alex_first_frame_label.setText(_translate("Frame", "ALEX First Frame Excitation"))
         self.pixseq_alex_first_frame.setItemText(0, _translate("Frame", "Donor"))
         self.pixseq_alex_first_frame.setItemText(1, _translate("Frame", "Acceptor"))
         self.label_32.setText(_translate("Frame", "Import Limit"))
@@ -1183,45 +1703,46 @@
         self.pixseq_import_limt.setItemText(2, _translate("Frame", "50"))
         self.pixseq_import_limt.setItemText(3, _translate("Frame", "100"))
         self.pixseq_import_limt.setItemText(4, _translate("Frame", "200"))
         self.pixseq_import_limt.setItemText(5, _translate("Frame", "300"))
         self.pixseq_import_limt.setItemText(6, _translate("Frame", "400"))
         self.pixseq_import_limt.setItemText(7, _translate("Frame", "500"))
         self.pixseq_append_dataset_label.setText(_translate("Frame", "Append Channels to Dataset:"))
+        self.pixseq_concatenate.setText(_translate("Frame", "Concatenate Files"))
         self.pixseq_append.setText(_translate("Frame", "Append Channel(s) To Exisiting Dataset"))
         self.pixseq_import.setText(_translate("Frame", "Import"))
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_15), _translate("Frame", "Import Images"))
         self.label_2.setText(_translate("Frame", "Dataset"))
         self.label_75.setText(_translate("Frame", "Channel"))
         self.label_76.setText(_translate("Frame", "Localisation Type"))
-        self.import_picasso_type.setItemText(0, _translate("Frame", "Fiducials"))
+        self.import_picasso_type.setItemText(0, _translate("Frame", "Localisations"))
         self.import_picasso_type.setItemText(1, _translate("Frame", "Bounding Boxes"))
         self.import_picasso.setText(_translate("Frame", "Import Picasso Localisations"))
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_16), _translate("Frame", "Import Localisations"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab), _translate("Frame", "Import"))
         self.label_20.setText(_translate("Frame", "Import Transform Matrix"))
         self.pixseq_import_tform.setText(_translate("Frame", "Import Tranform Matrix"))
-        self.label_9.setText(_translate("Frame", "Compute Transform Matrix (with Fiducials)"))
+        self.label_9.setText(_translate("Frame", "Compute Transform Matrix (with Localisations)"))
         self.label_22.setText(_translate("Frame", "Dataset"))
         self.label_23.setText(_translate("Frame", "Reference Donor Channel"))
         self.label_24.setText(_translate("Frame", "Target Acceptor Channel"))
         self.save_tform.setText(_translate("Frame", "Save Transform Matrix"))
         self.pixseq_compute_tform.setText(_translate("Frame", "Compute Transform Matrix"))
         self.label_21.setText(_translate("Frame", "Apply Transform Matrix (all datasets)"))
         self.label_25.setText(_translate("Frame", "Target Channel(s)"))
         self.tform_apply_target.setItemText(0, _translate("Frame", "Acceptor/DA/AA"))
         self.tform_apply_target.setItemText(1, _translate("Frame", "Donor/DD/AD"))
         self.pixseq_apply_tform.setText(_translate("Frame", "Apply Transform Matrix"))
         self.tabWidget_5.setTabText(self.tabWidget_5.indexOf(self.tab_17), _translate("Frame", "Transform"))
-        self.label_10.setText(_translate("Frame", "Compute Image Drift using Fitted Fiducials"))
+        self.label_10.setText(_translate("Frame", "Compute Image Drift using Fitted Localisations"))
         self.label_46.setText(_translate("Frame", "Undrift Dataset(s)"))
         self.label_15.setText(_translate("Frame", "Undrift Channel"))
         self.picasso_undrift.setText(_translate("Frame", "Undrift Image(s)"))
         self.tabWidget_5.setTabText(self.tabWidget_5.indexOf(self.tab_18), _translate("Frame", "Undirft"))
-        self.label_30.setText(_translate("Frame", "Align Datasets Using Fitted Fiducials"))
+        self.label_30.setText(_translate("Frame", "Align Datasets Using Fitted Localisations"))
         self.label_31.setText(_translate("Frame", "Reference Dataset"))
         self.label_33.setText(_translate("Frame", "Reference Channel"))
         self.pixseq_align_datasets.setText(_translate("Frame", "Align Datasets"))
         self.tabWidget_5.setTabText(self.tabWidget_5.indexOf(self.tab_3), _translate("Frame", "Align"))
         self.label_42.setText(_translate("Frame", "Temporal Filtering"))
         self.label_57.setText(_translate("Frame", "Works best with images that have been undrifted"))
         self.label_47.setText(_translate("Frame", "Dataset(s)"))
@@ -1239,38 +1760,144 @@
         self.filtering_filter_size.setItemText(6, _translate("Frame", "7"))
         self.filtering_filter_size.setItemText(7, _translate("Frame", "8"))
         self.filtering_filter_size.setItemText(8, _translate("Frame", "9"))
         self.filtering_filter_size.setItemText(9, _translate("Frame", "10"))
         self.filtering_start.setText(_translate("Frame", "Apply Temporal Filtering"))
         self.tabWidget_5.setTabText(self.tabWidget_5.indexOf(self.tab_4), _translate("Frame", "Filtering"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_10), _translate("Frame", "Image Processing"))
+        self.label_94.setText(_translate("Frame", "Add Shapes"))
+        self.add_line.setText(_translate("Frame", "Add Line Profile"))
+        self.add_box.setText(_translate("Frame", "Add Box Profile"))
+        self.add_background.setText(_translate("Frame", "Add Background Box"))
+        self.label_88.setText(_translate("Frame", "Plot Settings"))
+        self.label_77.setText(_translate("Frame", "Plot Mode"))
+        self.label_78.setText(_translate("Frame", "Plot Dataset"))
+        self.label_79.setText(_translate("Frame", "Plot Channel"))
+        self.simple_plot_mode.setItemText(0, _translate("Frame", "Line Profiles"))
+        self.simple_plot_mode.setItemText(1, _translate("Frame", "Line Profiles With Gaussian Fit"))
+        self.simple_plot_mode.setItemText(2, _translate("Frame", "Single Molecule Time Series"))
+        self.simple_subtract_background.setText(_translate("Frame", "Subtract Background (Single Molecule Time Series)"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_19), _translate("Frame", "Simple Analysis"))
+        self.label_97.setText(_translate("Frame", "Data Selection"))
+        self.label_101.setText(_translate("Frame", "Dataset"))
+        self.label_105.setText(_translate("Frame", "Reference Channel"))
+        self.label_102.setText(_translate("Frame", "Cellpose/Omnipose Settings"))
+        self.label_104.setText(_translate("Frame", "Model"))
+        self.cellpose_model.setItemText(0, _translate("Frame", "cyto"))
+        self.cellpose_model.setItemText(1, _translate("Frame", "nuclei"))
+        self.cellpose_model.setItemText(2, _translate("Frame", "tissuenet"))
+        self.cellpose_model.setItemText(3, _translate("Frame", "livecell"))
+        self.cellpose_model.setItemText(4, _translate("Frame", "cyto2"))
+        self.cellpose_model.setItemText(5, _translate("Frame", "general"))
+        self.cellpose_model.setItemText(6, _translate("Frame", "bact_phase_omni"))
+        self.cellpose_model.setItemText(7, _translate("Frame", "bact_fluor_omni"))
+        self.cellpose_model.setItemText(8, _translate("Frame", "worm_omni"))
+        self.cellpose_model.setItemText(9, _translate("Frame", "worm_bact_omni"))
+        self.cellpose_model.setItemText(10, _translate("Frame", "worm_high_res_omni"))
+        self.cellpose_model.setItemText(11, _translate("Frame", "cyto2_omni"))
+        self.cellpose_model.setItemText(12, _translate("Frame", "plant_omni"))
+        self.cellpose_model.setItemText(13, _translate("Frame", "custom"))
+        self.label_123.setText(_translate("Frame", "Batch Size"))
+        self.cellpose_batchsize.setItemText(0, _translate("Frame", "1"))
+        self.cellpose_batchsize.setItemText(1, _translate("Frame", "5"))
+        self.cellpose_batchsize.setItemText(2, _translate("Frame", "10"))
+        self.cellpose_batchsize.setItemText(3, _translate("Frame", "20"))
+        self.cellpose_batchsize.setItemText(4, _translate("Frame", "30"))
+        self.cellpose_batchsize.setItemText(5, _translate("Frame", "40"))
+        self.cellpose_batchsize.setItemText(6, _translate("Frame", "50"))
+        self.cellpose_batchsize.setItemText(7, _translate("Frame", "60"))
+        self.cellpose_batchsize.setItemText(8, _translate("Frame", "70"))
+        self.cellpose_batchsize.setItemText(9, _translate("Frame", "80"))
+        self.cellpose_batchsize.setItemText(10, _translate("Frame", "90"))
+        self.cellpose_batchsize.setItemText(11, _translate("Frame", "100"))
+        self.cellpose_batchsize.setItemText(12, _translate("Frame", "200"))
+        self.cellpose_batchsize.setItemText(13, _translate("Frame", "500"))
+        self.cellpose_batchsize.setItemText(14, _translate("Frame", "auto"))
+        self.cellpose_flowthresh_label.setText(_translate("Frame", "0.9"))
+        self.label_106.setText(_translate("Frame", "Flow Threshold"))
+        self.cellpose_maskthresh_label.setText(_translate("Frame", "0.0"))
+        self.cellpose_minsize_label.setText(_translate("Frame", "15"))
+        self.label_107.setText(_translate("Frame", "Mask Threshold"))
+        self.label_108.setText(_translate("Frame", "Min Size"))
+        self.label_109.setText(_translate("Frame", "Diameter"))
+        self.cellpose_diameter_label.setText(_translate("Frame", "15"))
+        self.cellpose_invert_images.setText(_translate("Frame", "Invert Images"))
+        self.label_110.setText(_translate("Frame", "Cellpose/Omnipose Functions"))
+        self.cellpose_load_model.setText(_translate("Frame", "Load Custom Model"))
+        self.segment_all.setText(_translate("Frame", "Segment All Images"))
+        self.segment_active.setText(_translate("Frame", "Segment Active Image"))
+        self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_24), _translate("Frame", "Cellpose"))
+        self.label_103.setText(_translate("Frame", "Dilate Segmentations"))
+        self.label_111.setText(_translate("Frame", "Pixels"))
+        self.dilate_segmentations.setText(_translate("Frame", "Dilate Segmentations"))
+        self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_26), _translate("Frame", "Curate"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_25), _translate("Frame", "Segment"))
         self.label_3.setText(_translate("Frame", "Detect Localisations (Picasso)"))
         self.label_7.setText(_translate("Frame", "Detect/Fit Mode"))
-        self.picasso_detect_mode.setItemText(0, _translate("Frame", "Fiducials"))
+        self.picasso_detect_mode.setItemText(0, _translate("Frame", "Localisations"))
         self.picasso_detect_mode.setItemText(1, _translate("Frame", "Bounding Boxes"))
         self.label_11.setText(_translate("Frame", "Dataset"))
         self.label_6.setText(_translate("Frame", "Channel"))
         self.label_8.setText(_translate("Frame", "Frame Mode"))
         self.picasso_frame_mode.setItemText(0, _translate("Frame", "Active"))
         self.picasso_frame_mode.setItemText(1, _translate("Frame", "All"))
         self.label_5.setText(_translate("Frame", "Min Net Gradient"))
         self.picasso_min_net_gradient.setText(_translate("Frame", "1000"))
         self.label_28.setText(_translate("Frame", "Box Size"))
         self.picasso_box_size.setItemText(0, _translate("Frame", "3"))
         self.picasso_box_size.setItemText(1, _translate("Frame", "5"))
         self.picasso_box_size.setItemText(2, _translate("Frame", "7"))
         self.picasso_box_size.setItemText(3, _translate("Frame", "9"))
+        self.picasso_box_size.setItemText(4, _translate("Frame", "11"))
+        self.picasso_box_size.setItemText(5, _translate("Frame", "13"))
+        self.picasso_box_size.setItemText(6, _translate("Frame", "15"))
         self.label_35.setText(_translate("Frame", "ROI Border Width (Pixels)"))
         self.picasso_roi_border_width.setText(_translate("Frame", "5"))
-        self.picasso_remove_overlapping.setText(_translate("Frame", "Remove Overlapping Fiducials/Bounding Boxes (determined by Picaso Box Size)"))
+        self.picasso_remove_overlapping.setText(_translate("Frame", "Remove Overlapping Localisations/Bounding Boxes (determined by Picaso Box Size)"))
         self.picasso_window_cropping.setText(_translate("Frame", "Remove Localisations Outside Field Of View (FOV)"))
+        self.picasso_segmentation_filtering.setText(_translate("Frame", "Remove Localisations Outside Segmentations"))
+        self.picasso_minimise_ram.setText(_translate("Frame", "Minimise RAM usage"))
         self.picasso_fit.setText(_translate("Frame", "Fit"))
         self.picasso_detect.setText(_translate("Frame", "Detect"))
         self.picasso_detectfit.setText(_translate("Frame", "Detect and Fit"))
-        self.label_27.setText(_translate("Frame", "Update Localisation Visualisation Settings"))
+        self.tabWidget_6.setTabText(self.tabWidget_6.indexOf(self.tab_21), _translate("Frame", "Detect"))
+        self.label_92.setText(_translate("Frame", "Filter Localisations (Picasso)"))
+        self.picasso_filter_dataset_label.setText(_translate("Frame", "Dataset"))
+        self.label_89.setText(_translate("Frame", "Channel"))
+        self.label_90.setText(_translate("Frame", "Filter By"))
+        self.label_93.setText(_translate("Frame", "Type"))
+        self.picasso_filter_type.setItemText(0, _translate("Frame", "Localisations"))
+        self.picasso_filter_type.setItemText(1, _translate("Frame", "Bounding Boxes"))
+        self.label_91.setText(_translate("Frame", "Filter Ranges"))
+        self.label_86.setText(_translate("Frame", "Min"))
+        self.label_87.setText(_translate("Frame", "Max"))
+        self.filter_localisations.setText(_translate("Frame", "Filter Localisations"))
+        self.tabWidget_6.setTabText(self.tabWidget_6.indexOf(self.tab_23), _translate("Frame", "Filter"))
+        self.label_85.setText(_translate("Frame", "Render Localisations (Picasso)"))
+        self.label_81.setText(_translate("Frame", "Dataset"))
+        self.label_82.setText(_translate("Frame", "Channel"))
+        self.label_83.setText(_translate("Frame", "Blur Method"))
+        self.picasso_render_blur_method.setItemText(0, _translate("Frame", "None"))
+        self.picasso_render_blur_method.setItemText(1, _translate("Frame", "One-Pixel-Blur"))
+        self.picasso_render_blur_method.setItemText(2, _translate("Frame", "Global Localisation Precision"))
+        self.picasso_render_blur_method.setItemText(3, _translate("Frame", "Individual Localisation Precision"))
+        self.picasso_render_blur_method.setItemText(4, _translate("Frame", "Individual Localisation Precision, iso"))
+        self.label_84.setText(_translate("Frame", "Min. Blur (cam. pixel)"))
+        self.picasso_render.setText(_translate("Frame", "Render Localisations"))
+        self.tabWidget_6.setTabText(self.tabWidget_6.indexOf(self.tab_20), _translate("Frame", "Render"))
+        self.label_80.setText(_translate("Frame", "Link Localisations (TrackPy)"))
+        self.label_95.setText(_translate("Frame", "Dataset"))
+        self.label_96.setText(_translate("Frame", "Channel"))
+        self.label_98.setText(_translate("Frame", "Search Range (Pixels)"))
+        self.label_99.setText(_translate("Frame", "Memory (Frames)"))
+        self.label_100.setText(_translate("Frame", "Min Track Length (Frames)"))
+        self.remove_unlinked.setText(_translate("Frame", "Remove Unlinked Localisations"))
+        self.link_localisations.setText(_translate("Frame", "Link Localisatons"))
+        self.tabWidget_6.setTabText(self.tabWidget_6.indexOf(self.tab_27), _translate("Frame", "Tracking"))
+        self.label_27.setText(_translate("Frame", "Localisation Visualisation Settings"))
         self.picasso_vis_size.setItemText(0, _translate("Frame", "1"))
         self.picasso_vis_size.setItemText(1, _translate("Frame", "2"))
         self.picasso_vis_size.setItemText(2, _translate("Frame", "3"))
         self.picasso_vis_size.setItemText(3, _translate("Frame", "4"))
         self.picasso_vis_size.setItemText(4, _translate("Frame", "5"))
         self.picasso_vis_size.setItemText(5, _translate("Frame", "6"))
         self.picasso_vis_size.setItemText(6, _translate("Frame", "7"))
@@ -1300,15 +1927,16 @@
         self.picasso_vis_edge_width.setItemText(3, _translate("Frame", "0.4"))
         self.picasso_vis_edge_width.setItemText(4, _translate("Frame", "0.5"))
         self.picasso_vis_edge_width.setItemText(5, _translate("Frame", "0.6"))
         self.picasso_vis_edge_width.setItemText(6, _translate("Frame", "0.7"))
         self.picasso_vis_edge_width.setItemText(7, _translate("Frame", "0.8"))
         self.picasso_vis_edge_width.setItemText(8, _translate("Frame", "0.9"))
         self.picasso_vis_edge_width.setItemText(9, _translate("Frame", "1.0"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Frame", "Detect"))
+        self.tabWidget_6.setTabText(self.tabWidget_6.indexOf(self.tab_22), _translate("Frame", "Visualisation Settings"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Frame", "SMLM"))
         self.label_37.setText(_translate("Frame", "Compute Settings"))
         self.label_70.setText(_translate("Frame", "Traces are computed from Bounding Boxes"))
         self.label_38.setText(_translate("Frame", "Mask Size (Pixels)"))
         self.traces_spot_size.setItemText(0, _translate("Frame", "3"))
         self.traces_spot_size.setItemText(1, _translate("Frame", "4"))
         self.traces_spot_size.setItemText(2, _translate("Frame", "5"))
         self.traces_spot_size.setItemText(3, _translate("Frame", "6"))
@@ -1359,14 +1987,16 @@
         self.label_36.setText(_translate("Frame", "Export Mode"))
         self.traces_export_mode.setItemText(0, _translate("Frame", "JSON Dataset"))
         self.traces_export_mode.setItemText(1, _translate("Frame", "Excel"))
         self.traces_export_mode.setItemText(2, _translate("Frame", "OriginLab"))
         self.traces_export_mode.setItemText(3, _translate("Frame", "Dat (.dat)"))
         self.traces_export_mode.setItemText(4, _translate("Frame", "Text (.txt)"))
         self.traces_export_mode.setItemText(5, _translate("Frame", "CSV (.csv)"))
+        self.traces_export_mode.setItemText(6, _translate("Frame", "Nero (.dat)"))
+        self.traces_export_mode.setItemText(7, _translate("Frame", "ebFRET SMD (.mat)"))
         self.label_45.setText(_translate("Frame", "Data Selection"))
         self.traces_export_dataset.setItemText(0, _translate("Frame", "All Images"))
         self.label_63.setText(_translate("Frame", "Channel"))
         self.traces_export_channel.setItemText(0, _translate("Frame", "Donor"))
         self.traces_export_channel.setItemText(1, _translate("Frame", "Acceptor"))
         self.traces_export_channel.setItemText(2, _translate("Frame", "FRET Data"))
         self.traces_export_channel.setItemText(3, _translate("Frame", "FRET Efficiency"))
@@ -1380,21 +2010,25 @@
         self.traces_export_metric.setItemText(2, _translate("Frame", "Bounding Box Sum"))
         self.label_59.setText(_translate("Frame", "Background Subtraction"))
         self.traces_export_background.setItemText(0, _translate("Frame", "None"))
         self.traces_export_background.setItemText(1, _translate("Frame", "Mask (Local Background)"))
         self.traces_export_background.setItemText(2, _translate("Frame", "Mask (Global Background)"))
         self.pixseq_export_traces.setText(_translate("Frame", "Export Traces"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_9), _translate("Frame", "Export Traces"))
-        self.label_74.setText(_translate("Frame", "Picasso HDF5 Localisations will be exported at the Dataset import directory"))
+        self.label_74.setText(_translate("Frame", "Localisations will be exported at the import directory"))
         self.label_72.setText(_translate("Frame", "Dataset"))
         self.label_73.setText(_translate("Frame", "Localisation Type"))
-        self.locs_export_mode.setItemText(0, _translate("Frame", "All"))
-        self.locs_export_mode.setItemText(1, _translate("Frame", "Bounding Boxes"))
-        self.locs_export_mode.setItemText(2, _translate("Frame", "Fiducials"))
+        self.locs_export_type.setItemText(0, _translate("Frame", "All"))
+        self.locs_export_type.setItemText(1, _translate("Frame", "Bounding Boxes"))
+        self.locs_export_type.setItemText(2, _translate("Frame", "Localisations"))
         self.label_71.setText(_translate("Frame", "Channel"))
+        self.label_112.setText(_translate("Frame", "Export Mode"))
+        self.locs_export_mode.setItemText(0, _translate("Frame", "Picasso HDF5"))
+        self.locs_export_mode.setItemText(1, _translate("Frame", "CSV"))
+        self.locs_export_mode.setItemText(2, _translate("Frame", "POS.OUT"))
         self.pixseq_export_locs.setText(_translate("Frame", "Export Localisations"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_14), _translate("Frame", "Export Localisations"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Export"))
         self.label_4.setText(_translate("Frame", "Update Dataset Name"))
         self.label_13.setText(_translate("Frame", "Old Dataset Name"))
         self.label_29.setText(_translate("Frame", "New Dataset Name"))
         self.pixseq_new_dataset_name.setText(_translate("Frame", "Dataset1"))
@@ -1436,15 +2070,15 @@
         self.colo_bboxes.setText(_translate("Frame", "Generate Bounding Boxes"))
         self.pixseq_colocalize.setText(_translate("Frame", "Co-Localize Fiducials"))
         self.label_26.setText(_translate("Frame", "Cluster Localisations (DBSCAN)"))
         self.label_17.setText(_translate("Frame", "Dataset"))
         self.label_18.setText(_translate("Frame", "Channel"))
         self.label_19.setText(_translate("Frame", "Mode"))
         self.cluster_mode.setItemText(0, _translate("Frame", "Create Bounding Boxes From Cluster Centers"))
-        self.cluster_mode.setItemText(1, _translate("Frame", "Create Fiducials From Cluster Centers"))
+        self.cluster_mode.setItemText(1, _translate("Frame", "Create Localisations From Cluster Centers"))
         self.label_60.setText(_translate("Frame", "Distance (EPS)"))
         self.cluster_eps.setText(_translate("Frame", "0.2"))
         self.label_61.setText(_translate("Frame", "Min Frames "))
         self.dbscan_min_samples.setText(_translate("Frame", "20"))
         self.dbscan_remove_overlapping.setText(_translate("Frame", "Remove Overlapping Localisations"))
         self.cluster_localisations.setText(_translate("Frame", "Cluster Localisations"))
         self.tabWidget_3.setTabText(self.tabWidget_3.indexOf(self.tab_12), _translate("Frame", "Localisation Utils"))
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/GUI/pixseq_ui.ui` & `napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.ui`

 * *Files 14% similar despite different names*

#### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/GUI/pixseq_ui.ui` & `napari_pixseq-1.0.2/src/napari_pixseq/GUI/pixseq_ui.ui`

```diff
@@ -2,15 +2,15 @@
 <ui version="4.0">
   <class>Frame</class>
   <widget class="QFrame" name="Frame">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>763</width>
+        <width>661</width>
         <height>625</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Frame</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
@@ -61,14 +61,19 @@
                               </property>
                             </widget>
                           </item>
                           <item row="0" column="1">
                             <widget class="QComboBox" name="pixseq_import_mode">
                               <item>
                                 <property name="text">
+                                  <string>Single Channel</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
                                   <string>FRET</string>
                                 </property>
                               </item>
                               <item>
                                 <property name="text">
                                   <string>Donor</string>
                                 </property>
@@ -207,14 +212,21 @@
                                 <string>Append Channels to Dataset:</string>
                               </property>
                             </widget>
                           </item>
                         </layout>
                       </item>
                       <item>
+                        <widget class="QCheckBox" name="pixseq_concatenate">
+                          <property name="text">
+                            <string>Concatenate Files</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
                         <widget class="QCheckBox" name="pixseq_append">
                           <property name="text">
                             <string>Append Channel(s) To Exisiting Dataset</string>
                           </property>
                         </widget>
                       </item>
                       <item>
@@ -260,15 +272,15 @@
                               </property>
                             </widget>
                           </item>
                           <item row="0" column="1">
                             <widget class="QComboBox" name="import_picasso_type">
                               <item>
                                 <property name="text">
-                                  <string>Fiducials</string>
+                                  <string>Localisations</string>
                                 </property>
                               </item>
                               <item>
                                 <property name="text">
                                   <string>Bounding Boxes</string>
                                 </property>
                               </item>
@@ -390,15 +402,15 @@
                           <property name="font">
                             <font>
                               <weight>75</weight>
                               <bold>true</bold>
                             </font>
                           </property>
                           <property name="text">
-                            <string>Compute Transform Matrix (with Fiducials)</string>
+                            <string>Compute Transform Matrix (with Localisations)</string>
                           </property>
                         </widget>
                       </item>
                       <item>
                         <layout class="QFormLayout" name="formLayout_7">
                           <item row="0" column="0">
                             <widget class="QLabel" name="label_22">
@@ -535,15 +547,15 @@
                           <property name="font">
                             <font>
                               <weight>75</weight>
                               <bold>true</bold>
                             </font>
                           </property>
                           <property name="text">
-                            <string>Compute Image Drift using Fitted Fiducials</string>
+                            <string>Compute Image Drift using Fitted Localisations</string>
                           </property>
                         </widget>
                       </item>
                       <item>
                         <layout class="QFormLayout" name="formLayout_4">
                           <item row="0" column="0">
                             <widget class="QLabel" name="label_46">
@@ -612,15 +624,15 @@
                           <property name="font">
                             <font>
                               <weight>75</weight>
                               <bold>true</bold>
                             </font>
                           </property>
                           <property name="text">
-                            <string>Align Datasets Using Fitted Fiducials</string>
+                            <string>Align Datasets Using Fitted Localisations</string>
                           </property>
                         </widget>
                       </item>
                       <item>
                         <layout class="QFormLayout" name="formLayout_10">
                           <item row="0" column="0">
                             <widget class="QLabel" name="label_31">
@@ -876,460 +888,1644 @@
                       <height>40</height>
                     </size>
                   </property>
                 </spacer>
               </item>
             </layout>
           </widget>
-          <widget class="QWidget" name="tab_2">
+          <widget class="QWidget" name="tab_19">
             <attribute name="title">
-              <string>Detect</string>
+              <string>Simple Analysis</string>
             </attribute>
-            <layout class="QVBoxLayout" name="verticalLayout_3">
+            <layout class="QVBoxLayout" name="verticalLayout_22">
               <item>
-                <widget class="QLabel" name="label_3">
+                <widget class="QLabel" name="label_94">
                   <property name="font">
                     <font>
                       <weight>75</weight>
                       <bold>true</bold>
                     </font>
                   </property>
                   <property name="text">
-                    <string>Detect Localisations (Picasso)</string>
+                    <string>Add Shapes</string>
                   </property>
                 </widget>
               </item>
               <item>
-                <layout class="QFormLayout" name="formLayout_3">
+                <layout class="QGridLayout" name="gridLayout_8">
                   <item row="0" column="0">
-                    <widget class="QLabel" name="label_7">
+                    <widget class="QPushButton" name="add_line">
                       <property name="text">
-                        <string>Detect/Fit Mode</string>
+                        <string>Add Line Profile</string>
                       </property>
                     </widget>
                   </item>
                   <item row="0" column="1">
-                    <widget class="QComboBox" name="picasso_detect_mode">
-                      <item>
-                        <property name="text">
-                          <string>Fiducials</string>
-                        </property>
-                      </item>
-                      <item>
-                        <property name="text">
-                          <string>Bounding Boxes</string>
-                        </property>
-                      </item>
-                    </widget>
-                  </item>
-                  <item row="1" column="0">
-                    <widget class="QLabel" name="label_11">
+                    <widget class="QPushButton" name="add_box">
                       <property name="text">
-                        <string>Dataset</string>
+                        <string>Add Box Profile</string>
                       </property>
                     </widget>
                   </item>
-                  <item row="1" column="1">
-                    <widget class="QComboBox" name="picasso_dataset"/>
-                  </item>
-                  <item row="2" column="0">
-                    <widget class="QLabel" name="label_6">
+                  <item row="0" column="2">
+                    <widget class="QPushButton" name="add_background">
                       <property name="text">
-                        <string>Channel</string>
+                        <string>Add Background Box</string>
                       </property>
                     </widget>
                   </item>
-                  <item row="2" column="1">
-                    <widget class="QComboBox" name="picasso_channel"/>
-                  </item>
-                  <item row="3" column="0">
-                    <widget class="QLabel" name="label_8">
+                </layout>
+              </item>
+              <item>
+                <spacer name="verticalSpacer_21">
+                  <property name="orientation">
+                    <enum>Qt::Vertical</enum>
+                  </property>
+                  <property name="sizeType">
+                    <enum>QSizePolicy::Minimum</enum>
+                  </property>
+                  <property name="sizeHint" stdset="0">
+                    <size>
+                      <width>20</width>
+                      <height>20</height>
+                    </size>
+                  </property>
+                </spacer>
+              </item>
+              <item>
+                <widget class="QLabel" name="label_88">
+                  <property name="font">
+                    <font>
+                      <weight>75</weight>
+                      <bold>true</bold>
+                    </font>
+                  </property>
+                  <property name="text">
+                    <string>Plot Settings</string>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <layout class="QFormLayout" name="formLayout_17">
+                  <item row="0" column="0">
+                    <widget class="QLabel" name="label_77">
                       <property name="text">
-                        <string>Frame Mode</string>
+                        <string>Plot Mode</string>
                       </property>
                     </widget>
                   </item>
-                  <item row="3" column="1">
-                    <widget class="QComboBox" name="picasso_frame_mode">
-                      <item>
-                        <property name="text">
-                          <string>Active</string>
-                        </property>
-                      </item>
-                      <item>
-                        <property name="text">
-                          <string>All</string>
-                        </property>
-                      </item>
-                    </widget>
-                  </item>
-                  <item row="5" column="0">
-                    <widget class="QLabel" name="label_5">
+                  <item row="1" column="0">
+                    <widget class="QLabel" name="label_78">
                       <property name="text">
-                        <string>Min Net Gradient</string>
+                        <string>Plot Dataset</string>
                       </property>
                     </widget>
                   </item>
-                  <item row="5" column="1">
-                    <widget class="QLineEdit" name="picasso_min_net_gradient">
-                      <property name="text">
-                        <string>1000</string>
-                      </property>
-                    </widget>
+                  <item row="1" column="1">
+                    <widget class="QComboBox" name="simple_plot_dataset"/>
                   </item>
-                  <item row="4" column="0">
-                    <widget class="QLabel" name="label_28">
+                  <item row="2" column="0">
+                    <widget class="QLabel" name="label_79">
                       <property name="text">
-                        <string>Box Size</string>
+                        <string>Plot Channel</string>
                       </property>
                     </widget>
                   </item>
-                  <item row="4" column="1">
-                    <widget class="QComboBox" name="picasso_box_size">
-                      <property name="currentIndex">
-                        <number>0</number>
-                      </property>
-                      <item>
-                        <property name="text">
-                          <string>3</string>
-                        </property>
-                      </item>
+                  <item row="2" column="1">
+                    <widget class="QComboBox" name="simple_plot_channel"/>
+                  </item>
+                  <item row="0" column="1">
+                    <widget class="QComboBox" name="simple_plot_mode">
                       <item>
                         <property name="text">
-                          <string>5</string>
+                          <string>Line Profiles</string>
                         </property>
                       </item>
                       <item>
                         <property name="text">
-                          <string>7</string>
+                          <string>Line Profiles With Gaussian Fit</string>
                         </property>
                       </item>
                       <item>
                         <property name="text">
-                          <string>9</string>
+                          <string>Single Molecule Time Series</string>
                         </property>
                       </item>
                     </widget>
                   </item>
-                  <item row="6" column="0">
-                    <widget class="QLabel" name="label_35">
-                      <property name="text">
-                        <string>ROI Border Width (Pixels)</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="6" column="1">
-                    <widget class="QLineEdit" name="picasso_roi_border_width">
-                      <property name="text">
-                        <string>5</string>
-                      </property>
-                    </widget>
-                  </item>
                 </layout>
               </item>
               <item>
-                <widget class="QCheckBox" name="picasso_remove_overlapping">
+                <widget class="QCheckBox" name="simple_subtract_background">
                   <property name="text">
-                    <string>Remove Overlapping Fiducials/Bounding Boxes (determined by Picaso Box Size)</string>
-                  </property>
-                  <property name="checked">
-                    <bool>true</bool>
+                    <string>Subtract Background (Single Molecule Time Series)</string>
                   </property>
                 </widget>
               </item>
               <item>
-                <widget class="QCheckBox" name="picasso_window_cropping">
-                  <property name="text">
-                    <string>Remove Localisations Outside Field Of View (FOV)</string>
+                <widget class="QWidget" name="simple_graph_container" native="true">
+                  <property name="sizePolicy">
+                    <sizepolicy hsizetype="MinimumExpanding" vsizetype="MinimumExpanding">
+                      <horstretch>0</horstretch>
+                      <verstretch>0</verstretch>
+                    </sizepolicy>
                   </property>
-                </widget>
-              </item>
-              <item>
-                <layout class="QGridLayout" name="gridLayout_6">
-                  <item row="0" column="1">
-                    <widget class="QPushButton" name="picasso_fit">
-                      <property name="text">
-                        <string>Fit</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="0" column="0">
-                    <widget class="QPushButton" name="picasso_detect">
-                      <property name="text">
-                        <string>Detect</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="0" column="2">
-                    <widget class="QPushButton" name="picasso_detectfit">
-                      <property name="text">
-                        <string>Detect and Fit</string>
-                      </property>
-                    </widget>
-                  </item>
-                </layout>
-              </item>
-              <item>
-                <widget class="QProgressBar" name="picasso_progressbar">
-                  <property name="maximumSize">
+                  <property name="minimumSize">
                     <size>
-                      <width>16777215</width>
-                      <height>10</height>
+                      <width>50</width>
+                      <height>0</height>
                     </size>
                   </property>
-                  <property name="value">
+                  <property name="toolTipDuration">
                     <number>0</number>
                   </property>
                 </widget>
               </item>
+            </layout>
+          </widget>
+          <widget class="QWidget" name="tab_25">
+            <attribute name="title">
+              <string>Segment</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_27">
               <item>
-                <spacer name="verticalSpacer_10">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>354</width>
-                      <height>2</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item>
-                <widget class="QLabel" name="label_27">
-                  <property name="font">
-                    <font>
-                      <weight>75</weight>
-                      <bold>true</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Update Localisation Visualisation Settings</string>
+                <widget class="QTabWidget" name="tabWidget_7">
+                  <property name="currentIndex">
+                    <number>0</number>
                   </property>
-                </widget>
-              </item>
-              <item>
-                <layout class="QGridLayout" name="gridLayout_14">
-                  <item row="0" column="3">
-                    <widget class="QComboBox" name="picasso_vis_size">
-                      <property name="currentIndex">
-                        <number>4</number>
-                      </property>
+                  <widget class="QWidget" name="tab_24">
+                    <attribute name="title">
+                      <string>Cellpose</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_28">
                       <item>
-                        <property name="text">
-                          <string>1</string>
-                        </property>
+                        <widget class="QLabel" name="label_97">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Data Selection</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>2</string>
-                        </property>
+                        <layout class="QFormLayout" name="formLayout_28">
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_101">
+                              <property name="text">
+                                <string>Dataset</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="cellpose_dataset"/>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_105">
+                              <property name="text">
+                                <string>Reference Channel</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="cellpose_channel"/>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>3</string>
-                        </property>
+                        <spacer name="verticalSpacer_24">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeType">
+                            <enum>QSizePolicy::Minimum</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>592</width>
+                              <height>17</height>
+                            </size>
+                          </property>
+                        </spacer>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>4</string>
-                        </property>
+                        <widget class="QLabel" name="label_102">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Cellpose/Omnipose Settings</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>5</string>
-                        </property>
+                        <layout class="QFormLayout" name="formLayout_27">
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_104">
+                              <property name="text">
+                                <string>Model</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="cellpose_model">
+                              <item>
+                                <property name="text">
+                                  <string>cyto</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>nuclei</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>tissuenet</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>livecell</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>cyto2</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>general</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>bact_phase_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>bact_fluor_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>worm_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>worm_bact_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>worm_high_res_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>cyto2_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>plant_omni</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>custom</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_123">
+                              <property name="text">
+                                <string>Batch Size</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="cellpose_batchsize">
+                              <item>
+                                <property name="text">
+                                  <string>1</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>5</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>10</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>20</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>30</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>40</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>50</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>60</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>70</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>80</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>90</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>100</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>200</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>500</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>auto</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>6</string>
-                        </property>
+                        <layout class="QGridLayout" name="gridLayout_11">
+                          <item row="0" column="2" alignment="Qt::AlignLeft">
+                            <widget class="QLabel" name="cellpose_flowthresh_label">
+                              <property name="minimumSize">
+                                <size>
+                                  <width>28</width>
+                                  <height>22</height>
+                                </size>
+                              </property>
+                              <property name="text">
+                                <string>0.9</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QSlider" name="cellpose_flowthresh">
+                              <property name="maximum">
+                                <number>100</number>
+                              </property>
+                              <property name="singleStep">
+                                <number>10</number>
+                              </property>
+                              <property name="pageStep">
+                                <number>10</number>
+                              </property>
+                              <property name="sliderPosition">
+                                <number>90</number>
+                              </property>
+                              <property name="orientation">
+                                <enum>Qt::Horizontal</enum>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_106">
+                              <property name="text">
+                                <string>Flow Threshold</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="2" alignment="Qt::AlignLeft">
+                            <widget class="QLabel" name="cellpose_maskthresh_label">
+                              <property name="minimumSize">
+                                <size>
+                                  <width>28</width>
+                                  <height>22</height>
+                                </size>
+                              </property>
+                              <property name="text">
+                                <string>0.0</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="2" alignment="Qt::AlignLeft">
+                            <widget class="QLabel" name="cellpose_minsize_label">
+                              <property name="minimumSize">
+                                <size>
+                                  <width>24</width>
+                                  <height>22</height>
+                                </size>
+                              </property>
+                              <property name="maximumSize">
+                                <size>
+                                  <width>24</width>
+                                  <height>16777215</height>
+                                </size>
+                              </property>
+                              <property name="text">
+                                <string>15</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_107">
+                              <property name="text">
+                                <string>Mask Threshold</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="0">
+                            <widget class="QLabel" name="label_108">
+                              <property name="text">
+                                <string>Min Size</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="1">
+                            <widget class="QSlider" name="cellpose_minsize">
+                              <property name="maximum">
+                                <number>200</number>
+                              </property>
+                              <property name="singleStep">
+                                <number>10</number>
+                              </property>
+                              <property name="value">
+                                <number>15</number>
+                              </property>
+                              <property name="orientation">
+                                <enum>Qt::Horizontal</enum>
+                              </property>
+                              <property name="tickPosition">
+                                <enum>QSlider::NoTicks</enum>
+                              </property>
+                              <property name="tickInterval">
+                                <number>10</number>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QSlider" name="cellpose_maskthresh">
+                              <property name="maximum">
+                                <number>100</number>
+                              </property>
+                              <property name="singleStep">
+                                <number>10</number>
+                              </property>
+                              <property name="pageStep">
+                                <number>10</number>
+                              </property>
+                              <property name="orientation">
+                                <enum>Qt::Horizontal</enum>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="1">
+                            <widget class="QSlider" name="cellpose_diameter">
+                              <property name="maximum">
+                                <number>100</number>
+                              </property>
+                              <property name="singleStep">
+                                <number>10</number>
+                              </property>
+                              <property name="value">
+                                <number>15</number>
+                              </property>
+                              <property name="orientation">
+                                <enum>Qt::Horizontal</enum>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="0">
+                            <widget class="QLabel" name="label_109">
+                              <property name="text">
+                                <string>Diameter</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="2">
+                            <widget class="QLabel" name="cellpose_diameter_label">
+                              <property name="text">
+                                <string>15</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>7</string>
-                        </property>
+                        <widget class="QCheckBox" name="cellpose_invert_images">
+                          <property name="text">
+                            <string>Invert Images</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>8</string>
-                        </property>
+                        <spacer name="verticalSpacer_23">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeType">
+                            <enum>QSizePolicy::Minimum</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>592</width>
+                              <height>17</height>
+                            </size>
+                          </property>
+                        </spacer>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>9</string>
-                        </property>
+                        <widget class="QLabel" name="label_110">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Cellpose/Omnipose Functions</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>10</string>
-                        </property>
+                        <widget class="QPushButton" name="cellpose_load_model">
+                          <property name="text">
+                            <string>Load Custom Model</string>
+                          </property>
+                        </widget>
                       </item>
-                    </widget>
-                  </item>
-                  <item row="0" column="0">
-                    <widget class="QLabel" name="label_114">
-                      <property name="text">
-                        <string>Mode</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="0" column="1">
-                    <widget class="QComboBox" name="picasso_vis_mode">
                       <item>
-                        <property name="text">
-                          <string>Disk</string>
-                        </property>
+                        <layout class="QGridLayout" name="gridLayout_12">
+                          <item row="0" column="1">
+                            <widget class="QPushButton" name="segment_all">
+                              <property name="text">
+                                <string>Segment All Images</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="0">
+                            <widget class="QPushButton" name="segment_active">
+                              <property name="text">
+                                <string>Segment Active Image</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>Square</string>
-                        </property>
+                        <widget class="QProgressBar" name="cellpose_progress">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="minimumSize">
+                            <size>
+                              <width>0</width>
+                              <height>0</height>
+                            </size>
+                          </property>
+                          <property name="maximumSize">
+                            <size>
+                              <width>16777215</width>
+                              <height>10</height>
+                            </size>
+                          </property>
+                          <property name="value">
+                            <number>0</number>
+                          </property>
+                        </widget>
                       </item>
-                    </widget>
-                  </item>
-                  <item row="0" column="2">
-                    <widget class="QLabel" name="label_115">
-                      <property name="text">
-                        <string>Size</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="1" column="0">
-                    <widget class="QLabel" name="label_120">
-                      <property name="text">
-                        <string>Opacity</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="1" column="1">
-                    <widget class="QComboBox" name="picasso_vis_opacity">
-                      <property name="currentIndex">
-                        <number>9</number>
-                      </property>
                       <item>
-                        <property name="text">
-                          <string>0.1</string>
-                        </property>
+                        <spacer name="verticalSpacer_22">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>40</height>
+                            </size>
+                          </property>
+                        </spacer>
                       </item>
+                    </layout>
+                  </widget>
+                  <widget class="QWidget" name="tab_26">
+                    <attribute name="title">
+                      <string>Curate</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_30">
                       <item>
-                        <property name="text">
-                          <string>0.2</string>
-                        </property>
+                        <widget class="QLabel" name="label_103">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Dilate Segmentations</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.3</string>
-                        </property>
+                        <layout class="QFormLayout" name="formLayout_26">
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_111">
+                              <property name="text">
+                                <string>Pixels</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QDoubleSpinBox" name="dilatation_size">
+                              <property name="decimals">
+                                <number>1</number>
+                              </property>
+                              <property name="minimum">
+                                <double>0.100000000000000</double>
+                              </property>
+                              <property name="maximum">
+                                <double>10.000000000000000</double>
+                              </property>
+                              <property name="value">
+                                <double>1.000000000000000</double>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.4</string>
-                        </property>
+                        <widget class="QPushButton" name="dilate_segmentations">
+                          <property name="text">
+                            <string>Dilate Segmentations</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.5</string>
-                        </property>
+                        <spacer name="verticalSpacer_27">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>40</height>
+                            </size>
+                          </property>
+                        </spacer>
                       </item>
+                    </layout>
+                  </widget>
+                </widget>
+              </item>
+              <item>
+                <spacer name="verticalSpacer_25">
+                  <property name="orientation">
+                    <enum>Qt::Vertical</enum>
+                  </property>
+                  <property name="sizeHint" stdset="0">
+                    <size>
+                      <width>20</width>
+                      <height>40</height>
+                    </size>
+                  </property>
+                </spacer>
+              </item>
+            </layout>
+          </widget>
+          <widget class="QWidget" name="tab_2">
+            <attribute name="title">
+              <string>SMLM</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_3">
+              <item>
+                <widget class="QTabWidget" name="tabWidget_6">
+                  <property name="currentIndex">
+                    <number>0</number>
+                  </property>
+                  <widget class="QWidget" name="tab_21">
+                    <attribute name="title">
+                      <string>Detect</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_23">
                       <item>
-                        <property name="text">
-                          <string>0.6</string>
-                        </property>
+                        <widget class="QLabel" name="label_3">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Detect Localisations (Picasso)</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.7</string>
-                        </property>
+                        <layout class="QFormLayout" name="formLayout_3">
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_7">
+                              <property name="text">
+                                <string>Detect/Fit Mode</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="picasso_detect_mode">
+                              <item>
+                                <property name="text">
+                                  <string>Localisations</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>Bounding Boxes</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_11">
+                              <property name="text">
+                                <string>Dataset</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="picasso_dataset"/>
+                          </item>
+                          <item row="2" column="0">
+                            <widget class="QLabel" name="label_6">
+                              <property name="text">
+                                <string>Channel</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="1">
+                            <widget class="QComboBox" name="picasso_channel"/>
+                          </item>
+                          <item row="3" column="0">
+                            <widget class="QLabel" name="label_8">
+                              <property name="text">
+                                <string>Frame Mode</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="1">
+                            <widget class="QComboBox" name="picasso_frame_mode">
+                              <item>
+                                <property name="text">
+                                  <string>Active</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>All</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="5" column="0">
+                            <widget class="QLabel" name="label_5">
+                              <property name="text">
+                                <string>Min Net Gradient</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="5" column="1">
+                            <widget class="QLineEdit" name="picasso_min_net_gradient">
+                              <property name="text">
+                                <string>1000</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="4" column="0">
+                            <widget class="QLabel" name="label_28">
+                              <property name="text">
+                                <string>Box Size</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="4" column="1">
+                            <widget class="QComboBox" name="picasso_box_size">
+                              <property name="currentIndex">
+                                <number>0</number>
+                              </property>
+                              <item>
+                                <property name="text">
+                                  <string>3</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>5</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>7</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>9</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>11</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>13</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>15</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="6" column="0">
+                            <widget class="QLabel" name="label_35">
+                              <property name="text">
+                                <string>ROI Border Width (Pixels)</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="6" column="1">
+                            <widget class="QLineEdit" name="picasso_roi_border_width">
+                              <property name="text">
+                                <string>5</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.8</string>
-                        </property>
+                        <widget class="QCheckBox" name="picasso_remove_overlapping">
+                          <property name="text">
+                            <string>Remove Overlapping Localisations/Bounding Boxes (determined by Picaso Box Size)</string>
+                          </property>
+                          <property name="checked">
+                            <bool>true</bool>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.9</string>
-                        </property>
+                        <widget class="QCheckBox" name="picasso_window_cropping">
+                          <property name="text">
+                            <string>Remove Localisations Outside Field Of View (FOV)</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>1.0</string>
-                        </property>
+                        <widget class="QCheckBox" name="picasso_segmentation_filtering">
+                          <property name="text">
+                            <string>Remove Localisations Outside Segmentations</string>
+                          </property>
+                        </widget>
                       </item>
-                    </widget>
-                  </item>
-                  <item row="1" column="2">
-                    <widget class="QLabel" name="label_121">
-                      <property name="text">
-                        <string>Edge Width</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item row="1" column="3">
-                    <widget class="QComboBox" name="picasso_vis_edge_width">
-                      <property name="currentText">
-                        <string>0.1</string>
-                      </property>
-                      <property name="currentIndex">
-                        <number>0</number>
-                      </property>
                       <item>
-                        <property name="text">
-                          <string>0.1</string>
-                        </property>
+                        <widget class="QCheckBox" name="picasso_minimise_ram">
+                          <property name="text">
+                            <string>Minimise RAM usage</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.2</string>
-                        </property>
+                        <layout class="QGridLayout" name="gridLayout_6">
+                          <item row="0" column="1">
+                            <widget class="QPushButton" name="picasso_fit">
+                              <property name="text">
+                                <string>Fit</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="0">
+                            <widget class="QPushButton" name="picasso_detect">
+                              <property name="text">
+                                <string>Detect</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="2">
+                            <widget class="QPushButton" name="picasso_detectfit">
+                              <property name="text">
+                                <string>Detect and Fit</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.3</string>
-                        </property>
+                        <widget class="QProgressBar" name="picasso_progressbar">
+                          <property name="maximumSize">
+                            <size>
+                              <width>16777215</width>
+                              <height>10</height>
+                            </size>
+                          </property>
+                          <property name="value">
+                            <number>0</number>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.4</string>
-                        </property>
+                        <spacer name="verticalSpacer_11">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeType">
+                            <enum>QSizePolicy::MinimumExpanding</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>0</height>
+                            </size>
+                          </property>
+                        </spacer>
                       </item>
+                    </layout>
+                  </widget>
+                  <widget class="QWidget" name="tab_23">
+                    <attribute name="title">
+                      <string>Filter</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_26">
                       <item>
-                        <property name="text">
-                          <string>0.5</string>
-                        </property>
+                        <widget class="QLabel" name="label_92">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Filter Localisations (Picasso)</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.6</string>
-                        </property>
+                        <layout class="QFormLayout" name="formLayout_24">
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="picasso_filter_dataset_label">
+                              <property name="text">
+                                <string>Dataset</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="picasso_filter_dataset"/>
+                          </item>
+                          <item row="2" column="0">
+                            <widget class="QLabel" name="label_89">
+                              <property name="text">
+                                <string>Channel</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="1">
+                            <widget class="QComboBox" name="picasso_filter_channel"/>
+                          </item>
+                          <item row="3" column="0">
+                            <widget class="QLabel" name="label_90">
+                              <property name="text">
+                                <string>Filter By</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="1">
+                            <widget class="QComboBox" name="filter_criterion"/>
+                          </item>
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_93">
+                              <property name="text">
+                                <string>Type</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="picasso_filter_type">
+                              <item>
+                                <property name="text">
+                                  <string>Localisations</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>Bounding Boxes</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.7</string>
-                        </property>
+                        <widget class="QWidget" name="filter_graph_container" native="true">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.8</string>
-                        </property>
+                        <widget class="QLabel" name="label_91">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Filter Ranges</string>
+                          </property>
+                        </widget>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>0.9</string>
-                        </property>
+                        <layout class="QGridLayout" name="gridLayout_7">
+                          <item row="0" column="0">
+                            <layout class="QFormLayout" name="formLayout_22">
+                              <item row="0" column="0">
+                                <widget class="QLabel" name="label_86">
+                                  <property name="text">
+                                    <string>Min</string>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item row="0" column="1">
+                                <widget class="QDoubleSpinBox" name="filter_min">
+                                  <property name="minimum">
+                                    <double>-999999999.000000000000000</double>
+                                  </property>
+                                  <property name="maximum">
+                                    <double>9999999999.000000000000000</double>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </item>
+                          <item row="0" column="1">
+                            <layout class="QFormLayout" name="formLayout_23">
+                              <item row="0" column="0">
+                                <widget class="QLabel" name="label_87">
+                                  <property name="text">
+                                    <string>Max</string>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item row="0" column="1">
+                                <widget class="QDoubleSpinBox" name="filter_max">
+                                  <property name="minimum">
+                                    <double>-99999999999.000000000000000</double>
+                                  </property>
+                                  <property name="maximum">
+                                    <double>9999999999.000000000000000</double>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </item>
+                        </layout>
                       </item>
                       <item>
-                        <property name="text">
-                          <string>1.0</string>
-                        </property>
+                        <widget class="QPushButton" name="filter_localisations">
+                          <property name="text">
+                            <string>Filter Localisations</string>
+                          </property>
+                        </widget>
                       </item>
-                    </widget>
-                  </item>
-                </layout>
+                    </layout>
+                  </widget>
+                  <widget class="QWidget" name="tab_20">
+                    <attribute name="title">
+                      <string>Render</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_25">
+                      <item>
+                        <widget class="QLabel" name="label_85">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Render Localisations (Picasso)</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <layout class="QFormLayout" name="formLayout_20">
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_81">
+                              <property name="text">
+                                <string>Dataset</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="picasso_render_dataset"/>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_82">
+                              <property name="text">
+                                <string>Channel</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="picasso_render_channel"/>
+                          </item>
+                          <item row="2" column="0">
+                            <widget class="QLabel" name="label_83">
+                              <property name="text">
+                                <string>Blur Method</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="1">
+                            <widget class="QComboBox" name="picasso_render_blur_method">
+                              <item>
+                                <property name="text">
+                                  <string>None</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>One-Pixel-Blur</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>Global Localisation Precision</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>Individual Localisation Precision</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>Individual Localisation Precision, iso</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="3" column="0">
+                            <widget class="QLabel" name="label_84">
+                              <property name="text">
+                                <string>Min. Blur (cam. pixel)</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="1">
+                            <widget class="QDoubleSpinBox" name="picasso_render_min_blur">
+                              <property name="singleStep">
+                                <double>0.100000000000000</double>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="picasso_render">
+                          <property name="text">
+                            <string>Render Localisations</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="verticalSpacer_19">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>413</width>
+                              <height>173</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </widget>
+                  <widget class="QWidget" name="tab_27">
+                    <attribute name="title">
+                      <string>Tracking</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_29">
+                      <item>
+                        <widget class="QLabel" name="label_80">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Link Localisations (TrackPy)</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <layout class="QFormLayout" name="formLayout_25">
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_95">
+                              <property name="text">
+                                <string>Dataset</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="tracking_dataset"/>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_96">
+                              <property name="text">
+                                <string>Channel</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="tracking_channel"/>
+                          </item>
+                          <item row="2" column="0">
+                            <widget class="QLabel" name="label_98">
+                              <property name="text">
+                                <string>Search Range (Pixels)</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="2" column="1">
+                            <widget class="QDoubleSpinBox" name="trackpy_search_range">
+                              <property name="value">
+                                <double>1.000000000000000</double>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="0">
+                            <widget class="QLabel" name="label_99">
+                              <property name="text">
+                                <string>Memory (Frames)</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="3" column="1">
+                            <widget class="QSpinBox" name="trackpy_memory"/>
+                          </item>
+                          <item row="4" column="0">
+                            <widget class="QLabel" name="label_100">
+                              <property name="text">
+                                <string>Min Track Length (Frames)</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="4" column="1">
+                            <widget class="QSpinBox" name="min_track_length">
+                              <property name="minimum">
+                                <number>1</number>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
+                      </item>
+                      <item>
+                        <widget class="QCheckBox" name="remove_unlinked">
+                          <property name="text">
+                            <string>Remove Unlinked Localisations</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="link_localisations">
+                          <property name="text">
+                            <string>Link Localisatons</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="verticalSpacer_26">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>122</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </widget>
+                  <widget class="QWidget" name="tab_22">
+                    <attribute name="title">
+                      <string>Visualisation Settings</string>
+                    </attribute>
+                    <layout class="QVBoxLayout" name="verticalLayout_24">
+                      <item>
+                        <widget class="QLabel" name="label_27">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="text">
+                            <string>Localisation Visualisation Settings</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <layout class="QGridLayout" name="gridLayout_14">
+                          <item row="0" column="3">
+                            <widget class="QComboBox" name="picasso_vis_size">
+                              <property name="currentIndex">
+                                <number>4</number>
+                              </property>
+                              <item>
+                                <property name="text">
+                                  <string>1</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>2</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>3</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>4</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>5</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>6</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>7</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>8</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>9</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>10</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_114">
+                              <property name="text">
+                                <string>Mode</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="picasso_vis_mode">
+                              <item>
+                                <property name="text">
+                                  <string>Disk</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>Square</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="0" column="2">
+                            <widget class="QLabel" name="label_115">
+                              <property name="text">
+                                <string>Size</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="0">
+                            <widget class="QLabel" name="label_120">
+                              <property name="text">
+                                <string>Opacity</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="picasso_vis_opacity">
+                              <property name="currentIndex">
+                                <number>9</number>
+                              </property>
+                              <item>
+                                <property name="text">
+                                  <string>0.1</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.2</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.3</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.4</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.5</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.6</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.7</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.8</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.9</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>1.0</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                          <item row="1" column="2">
+                            <widget class="QLabel" name="label_121">
+                              <property name="text">
+                                <string>Edge Width</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="1" column="3">
+                            <widget class="QComboBox" name="picasso_vis_edge_width">
+                              <property name="currentText">
+                                <string>0.1</string>
+                              </property>
+                              <property name="currentIndex">
+                                <number>0</number>
+                              </property>
+                              <item>
+                                <property name="text">
+                                  <string>0.1</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.2</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.3</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.4</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.5</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.6</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.7</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.8</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>0.9</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>1.0</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
+                        </layout>
+                      </item>
+                      <item>
+                        <spacer name="verticalSpacer_10">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>354</width>
+                              <height>254</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </widget>
+                </widget>
               </item>
               <item>
                 <spacer name="verticalSpacer_2">
                   <property name="orientation">
                     <enum>Qt::Vertical</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
@@ -1890,14 +3086,24 @@
                                 </property>
                               </item>
                               <item>
                                 <property name="text">
                                   <string>CSV (.csv)</string>
                                 </property>
                               </item>
+                              <item>
+                                <property name="text">
+                                  <string>Nero (.dat)</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>ebFRET SMD (.mat)</string>
+                                </property>
+                              </item>
                             </widget>
                           </item>
                           <item row="1" column="0">
                             <widget class="QLabel" name="label_45">
                               <property name="text">
                                 <string>Data Selection</string>
                               </property>
@@ -2030,66 +3236,92 @@
                     <attribute name="title">
                       <string>Export Localisations</string>
                     </attribute>
                     <layout class="QVBoxLayout" name="verticalLayout_17">
                       <item>
                         <widget class="QLabel" name="label_74">
                           <property name="text">
-                            <string>Picasso HDF5 Localisations will be exported at the Dataset import directory</string>
+                            <string>Localisations will be exported at the import directory</string>
                           </property>
                         </widget>
                       </item>
                       <item>
                         <layout class="QFormLayout" name="formLayout_19">
-                          <item row="1" column="0">
+                          <item row="2" column="0">
                             <widget class="QLabel" name="label_72">
                               <property name="text">
                                 <string>Dataset</string>
                               </property>
                             </widget>
                           </item>
-                          <item row="1" column="1">
+                          <item row="2" column="1">
                             <widget class="QComboBox" name="locs_export_dataset"/>
                           </item>
-                          <item row="0" column="0">
+                          <item row="1" column="0">
                             <widget class="QLabel" name="label_73">
                               <property name="text">
                                 <string>Localisation Type</string>
                               </property>
                             </widget>
                           </item>
-                          <item row="0" column="1">
-                            <widget class="QComboBox" name="locs_export_mode">
+                          <item row="1" column="1">
+                            <widget class="QComboBox" name="locs_export_type">
                               <item>
                                 <property name="text">
                                   <string>All</string>
                                 </property>
                               </item>
                               <item>
                                 <property name="text">
                                   <string>Bounding Boxes</string>
                                 </property>
                               </item>
                               <item>
                                 <property name="text">
-                                  <string>Fiducials</string>
+                                  <string>Localisations</string>
                                 </property>
                               </item>
                             </widget>
                           </item>
-                          <item row="2" column="1">
+                          <item row="3" column="1">
                             <widget class="QComboBox" name="locs_export_channel"/>
                           </item>
-                          <item row="2" column="0">
+                          <item row="3" column="0">
                             <widget class="QLabel" name="label_71">
                               <property name="text">
                                 <string>Channel</string>
                               </property>
                             </widget>
                           </item>
+                          <item row="0" column="0">
+                            <widget class="QLabel" name="label_112">
+                              <property name="text">
+                                <string>Export Mode</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item row="0" column="1">
+                            <widget class="QComboBox" name="locs_export_mode">
+                              <item>
+                                <property name="text">
+                                  <string>Picasso HDF5</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>CSV</string>
+                                </property>
+                              </item>
+                              <item>
+                                <property name="text">
+                                  <string>POS.OUT</string>
+                                </property>
+                              </item>
+                            </widget>
+                          </item>
                         </layout>
                       </item>
                       <item>
                         <widget class="QPushButton" name="pixseq_export_locs">
                           <property name="text">
                             <string>Export Localisations</string>
                           </property>
@@ -2582,15 +3814,15 @@
                               <item>
                                 <property name="text">
                                   <string>Create Bounding Boxes From Cluster Centers</string>
                                 </property>
                               </item>
                               <item>
                                 <property name="text">
-                                  <string>Create Fiducials From Cluster Centers</string>
+                                  <string>Create Localisations From Cluster Centers</string>
                                 </property>
                               </item>
                             </widget>
                           </item>
                           <item row="3" column="0">
                             <widget class="QLabel" name="label_60">
                               <property name="text">
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/_tests/test_widget.py` & `napari_pixseq-1.0.2/src/napari_pixseq/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_align_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_align_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 
             acceptor_channels = np.unique(acceptor_channels).tolist()
             donor_channels = np.unique(donor_channels).tolist()
 
             acceptor_channels = "Acceptor Channels: [" + "/ ".join(acceptor_channels) + "]"
             donor_channels = "Donor Channels: [" + "/".join(donor_channels) + "]"
 
-            self.align_reference_channel.blockSignals(True)
-            self.align_reference_channel.clear()
-            self.align_reference_channel.addItem(acceptor_channels)
-            self.align_reference_channel.addItem(donor_channels)
-            self.align_reference_channel.blockSignals(False)
+            self.gui.align_reference_channel.blockSignals(True)
+            self.gui.align_reference_channel.clear()
+            self.gui.align_reference_channel.addItem(acceptor_channels)
+            self.gui.align_reference_channel.addItem(donor_channels)
+            self.gui.align_reference_channel.blockSignals(False)
 
         except:
             pass
 
     def affine_transform_matrix(self, points_src, points_dst):
         # Function to optimize
         def min_func(params):
@@ -85,16 +85,16 @@
             print(traceback.format_exc())
             pass
 
     def _align_datasets(self, progress_callback, align_dict):
 
         try:
 
-            reference_dataset = self.align_reference_dataset.currentText()
-            reference_channel = self.align_reference_channel.currentText()
+            reference_dataset = self.gui.align_reference_dataset.currentText()
+            reference_channel = self.gui.align_reference_channel.currentText()
 
             dataset_list = list(self.dataset_dict.keys())
             dataset_list.remove(reference_dataset)
 
             total_frames = 0
             for dataset in dataset_list:
                 for channel_name, channel_dict in self.dataset_dict[dataset].items():
@@ -118,89 +118,113 @@
 
                 matches = bf.match(dst_pts, src_pts)
                 matches = sorted(matches, key=lambda x: x.distance)
 
                 dst_pts = np.float32([dst_pts[m.queryIdx] for m in matches]).reshape(-1, 2)
                 src_pts = np.float32([src_pts[m.trainIdx] for m in matches]).reshape(-1, 2)
 
-                transform_matrix, _ = cv2.findHomography(src_pts, dst_pts, cv2.RANSAC, 5.0)
+                if len(dst_pts) > 0:
 
-                if transform_matrix.shape == (3,3):
+                    if len(dst_pts) == 1 or len(dst_pts) == 2:
 
-                    for channel_name, channel_dict in self.dataset_dict[dataset].items():
+                        dst_point = dst_pts[0]
+                        src_point = src_pts[0]
 
-                        print(f"Aligning {dataset} {channel_name}...")
+                        # Calculate translation vector
+                        tx = dst_point[0] - src_point[0]
+                        ty = dst_point[1] - src_point[1]
 
-                        img = channel_dict["data"].copy()
+                        # Translation matrix
+                        transform_matrix = np.float32([[1, 0, tx], [0, 1, ty]])
+                        transform_mode = "affine"
 
-                        def transform_progress(progress):
-                            nonlocal iter
-                            iter += progress
-                            progress = int((iter / total_frames) * 100)
-                            progress_callback.emit(progress)
+                    elif len(dst_pts) == 3:
 
-                        img = transform_image(img, transform_matrix, progress_callback=transform_progress)
+                        transform_matrix = cv2.getAffineTransform(src_pts, dst_pts)
+                        transform_mode = "affine"
 
-                        self.dataset_dict[dataset][channel_name.lower()]["data"] = img.copy()
+                    elif len(dst_pts) > 3:
+                        transform_matrix, _ = cv2.findHomography(src_pts, dst_pts, cv2.RANSAC, 5.0)
+                        transform_mode = "homography"
+
+                    if transform_matrix.shape in [(2, 3), (3, 3)]:
+
+                        for channel_name, channel_dict in self.dataset_dict[dataset].items():
+
+                            self.pixseq_notification(f"Aligning {dataset} {channel_name}...")
+
+                            img = channel_dict["data"].copy()
+
+                            def transform_progress(progress):
+                                nonlocal iter
+                                iter += progress
+                                progress = int((iter / total_frames) * 100)
+                                progress_callback.emit(progress)
+
+                            img = transform_image(img, transform_matrix,
+                                transform_mode = transform_mode,
+                                progress_callback=transform_progress)
+
+                            self.dataset_dict[dataset][channel_name.lower()]["data"] = img.copy()
 
         except:
             print(traceback.format_exc())
             pass
 
 
     def align_datasets(self):
 
         try:
 
             if self.dataset_dict != {}:
 
-                align_dataset = self.align_reference_dataset.currentText()
-                align_channel = self.align_reference_channel.currentText()
+                align_dataset = self.gui.align_reference_dataset.currentText()
+                align_channel = self.gui.align_reference_channel.currentText()
 
                 if "Donor Channels" in align_channel:
                     channel_mode = "Donor"
                     target_channels = ["donor", "dd", "ad"]
                 else:
                     channel_mode = "Acceptor"
                     target_channels = ["acceptor", "aa", "da"]
 
                 missing_fiducial_list = []
 
                 align_dict = {}
 
                 for dataset_name in self.dataset_dict.keys():
-                    if dataset_name not in self.localisation_dict["fiducials"].keys():
+                    if dataset_name not in self.localisation_dict["localisations"].keys():
                         missing_fiducial_list.append(dataset_name)
                     else:
                         dataset_channels = list(self.dataset_dict[dataset_name].keys())
                         reference_channels = [channel.lower() for channel in dataset_channels if channel in target_channels]
 
                         for channel in reference_channels:
-                            if channel not in self.localisation_dict["fiducials"][dataset_name].keys():
+                            if channel not in self.localisation_dict["localisations"][dataset_name].keys():
                                 missing_fiducial_list.append(dataset_name)
                             else:
-                                localisation_dict = self.localisation_dict["fiducials"][dataset_name][channel]
+                                localisation_dict = self.localisation_dict["localisations"][dataset_name][channel]
                                 if "fitted" not in localisation_dict.keys():
                                     missing_fiducial_list.append(dataset_name)
                                 else:
                                     if localisation_dict["fitted"] == False:
                                         missing_fiducial_list.append(dataset_name)
                                     else:
                                         align_dict[dataset_name] = localisation_dict["localisations"]
 
 
                 if len(missing_fiducial_list) > 0:
                     missing_fiducial_list = ", ".join(missing_fiducial_list)
-                    print(f"Missing fitted {channel_mode} fiducials for {missing_fiducial_list}")
+                    self.pixseq_notification(f"Missing fitted {channel_mode} localisations for {missing_fiducial_list}")
                 else:
 
                     self.update_ui(init=True)
 
                     self.worker = Worker(self._align_datasets, align_dict=align_dict)
-                    self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.align_progressbar))
+                    self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.gui.align_progressbar))
                     self.worker.signals.finished.connect(self._align_datasets_finished)
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
         except:
             print(traceback.format_exc())
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_cluster_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_cluster_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 
 class _cluster_utils:
 
     def _cluster_localisations_finished(self):
 
         try:
-            mode = self.cluster_mode.currentText()
+            mode = self.gui.cluster_mode.currentText()
 
-            if "fiducials" in mode.lower():
-                self.draw_fiducials(update_vis=True)
+            if "localisations" in mode.lower():
+                self.draw_localisations(update_vis=True)
             else:
                 self.draw_bounding_boxes()
 
             self.update_ui()
 
         except:
             print(traceback.format_exc())
@@ -52,20 +52,20 @@
 
     def _cluster_localisations(self, progress_callback=None, eps=0.1, min_samples=20):
 
         result = None, None, None
 
         try:
 
-            mode = self.cluster_mode.currentText()
-            dataset = self.cluster_dataset.currentText()
-            channel = self.cluster_channel.currentText()
-            remove_overlapping = self.dbscan_remove_overlapping.isChecked()
+            mode = self.gui.cluster_mode.currentText()
+            dataset = self.gui.cluster_dataset.currentText()
+            channel = self.gui.cluster_channel.currentText()
+            remove_overlapping = self.gui.dbscan_remove_overlapping.isChecked()
 
-            loc_dict, n_locs, fitted = self.get_loc_dict(dataset, channel.lower(), type = "fiducials")
+            loc_dict, n_locs, fitted = self.get_loc_dict(dataset, channel.lower(), type = "localisations")
 
             locs = loc_dict["localisations"]
             box_size = loc_dict["box_size"]
 
             n_frames = len(np.unique([loc.frame for loc in locs]))
 
             cluster_dataset = np.vstack((locs.x, locs.y)).T
@@ -90,15 +90,15 @@
             # Finding cluster centers
             cluster_centers = np.array([filtered_data[filtered_labels == i].mean(axis=0) for i in range(n_clusters)])
 
             if remove_overlapping:
                 cluster_centers = self.remove_overlapping_coords(cluster_centers,
                     min_distance = box_size)
 
-            if "fiducials" not in mode.lower():
+            if "localisations" not in mode.lower():
                 n_frames = 1
 
             clustered_locs = []
             clustered_loc_centers = []
             render_locs = {}
 
             for cluster_index in range(len(cluster_centers)):
@@ -129,30 +129,42 @@
 
         try:
 
             if result is not None:
 
                 locs, loc_centers, render_locs = result
 
-                mode = self.cluster_mode.currentText()
-                dataset = self.cluster_dataset.currentText()
-                channel = self.cluster_channel.currentText()
-
-                if "fiducials" in mode.lower():
-
-                    self.localisation_dict["fiducials"][dataset][channel.lower()]["localisations"] = locs
-                    self.localisation_dict["fiducials"][dataset][channel.lower()]["localisation_centres"] = loc_centers
-                    self.localisation_dict["fiducials"][dataset][channel.lower()]["render_locs"] = render_locs
+                mode = self.gui.cluster_mode.currentText()
+                dataset = self.gui.cluster_dataset.currentText()
+                channel = self.gui.cluster_channel.currentText()
+
+                fiducial_dict = self.localisation_dict["localisations"][dataset][channel.lower()]
+                bbox_dict = self.localisation_dict["bounding_boxes"]
+
+                if "localisations" in mode.lower():
+
+                    fiducial_dict = self.localisation_dict["localisations"][dataset][channel.lower()]
+
+                    fiducial_dict["localisations"] = locs
+                    fiducial_dict["localisation_centres"] = loc_centers
+                    fiducial_dict["render_locs"] = render_locs
 
                 else:
 
-                    self.localisation_dict["bounding_boxes"]["localisations"] = locs
-                    self.localisation_dict["bounding_boxes"]["localisation_centres"] = loc_centers
+                    if "box_size" in fiducial_dict.keys():
+                        box_size = fiducial_dict["box_size"]
+                    else:
+                        box_size = int(self.gui.picasso_box_size.currentText())
+
+                    bbox_dict["localisations"] = locs
+                    bbox_dict["localisation_centres"] = loc_centers
+                    bbox_dict["box_size"] = box_size
 
         except:
+            print(traceback.format_exc())
             pass
 
 
 
     def check_number(self, string):
 
         if string.isdigit():
@@ -164,25 +176,28 @@
 
         return number
 
     def pixseq_cluster_localisations(self):
 
         try:
 
-            dataset = self.cluster_dataset.currentText()
-            channel = self.cluster_channel.currentText()
-
-            eps = self.cluster_eps.text()
-            min_samples = self.dbscan_min_samples.text()
+            dataset = self.gui.cluster_dataset.currentText()
+            channel = self.gui.cluster_channel.currentText()
+            mode = self.gui.cluster_mode.currentText()
+            eps = self.gui.cluster_eps.text()
+            min_samples = self.gui.dbscan_min_samples.text()
 
             eps = self.check_number(eps)
             min_samples = self.check_number(min_samples)
 
             loc_dict, n_locs, fitted = self.get_loc_dict(dataset, channel.lower())
 
+            if n_locs == 0 or fitted == False:
+                self.pixseq_notification("Localisation clustering requires fitted localisations.")
+
             if n_locs > 0 and fitted and eps is not None and min_samples is not None:
 
                 self.update_ui(init = True)
 
                 worker = Worker(self._cluster_localisations, eps=eps, min_samples=min_samples)
                 worker.signals.result.connect(self._cluster_localisations_result)
                 worker.signals.finished.connect(self._cluster_localisations_finished)
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_colocalize_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_colocalize_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
         return filtered_locs, filtered_render_locs, filtered_loc_centers
 
 
 
 
 
-    def _pixseq_colocalize_fiducials(self, progress_callback=None):
+    def _pixseq_colocalize_localisations(self, progress_callback=None):
 
         try:
 
-            dataset = self.colo_dataset.currentText()
-            channel1 = self.colo_channel1.currentText()
-            channel2 = self.colo_channel2.currentText()
-            max_dist = float(self.colo_max_dist.currentText())
+            dataset = self.gui.colo_dataset.currentText()
+            channel1 = self.gui.colo_channel1.currentText()
+            channel2 = self.gui.colo_channel2.currentText()
+            max_dist = float(self.gui.colo_max_dist.currentText())
 
             ch1_loc_dict, ch1_n_locs, _ = self.get_loc_dict(dataset, channel1.lower())
             ch2_loc_dict, ch2_n_locs, _ = self.get_loc_dict(dataset, channel2.lower())
 
             ch1_locs = ch1_loc_dict["localisations"].copy()
             ch2_locs = ch2_loc_dict["localisations"].copy()
 
@@ -135,87 +135,86 @@
             colo_locs = np.rec.fromrecords(colo_locs, dtype=filtered_ch1_locs.dtype)
             colo_loc_centers = self.get_localisation_centres(colo_locs)
 
             result_dict = {"localisations": colo_locs,
                            "localisation_centres": colo_loc_centers,
                            "render_locs": colo_render_locs}
 
-            print(f"Found {len(colo_locs)} colocalisations between {channel1} and {channel2}")
+            self.pixseq_notification(f"Found {len(colo_locs)} colocalisations between {channel1} and {channel2}")
 
         except:
             print(traceback.format_exc())
             ch1_result_dict = None
             ch2_result_dict = None
             result_dict = None
             pass
 
         return result_dict
 
-    def _pixseq_colocalize_fiducials_result(self, colo_locs):
+    def _pixseq_colocalize_localisations_result(self, colo_locs):
 
         try:
 
             if colo_locs is not None:
 
-                dataset = self.colo_dataset.currentText()
-                channel1 = self.colo_channel1.currentText()
-                channel2 = self.colo_channel2.currentText()
+                dataset = self.gui.colo_dataset.currentText()
+                channel1 = self.gui.colo_channel1.currentText()
+                channel2 = self.gui.colo_channel2.currentText()
 
-                if self.colo_fiducials.isChecked():
+                if self.gui.colo_localisations.isChecked():
 
-                    self.localisation_dict["fiducials"][dataset][channel1.lower()]["localisations"] = colo_locs["localisations"]
-                    self.localisation_dict["fiducials"][dataset][channel1.lower()]["localisation_centres"] = colo_locs["localisation_centres"]
-                    self.localisation_dict["fiducials"][dataset][channel1.lower()]["render_locs"] = colo_locs["render_locs"]
+                    self.localisation_dict["localisations"][dataset][channel1.lower()]["localisations"] = colo_locs["localisations"]
+                    self.localisation_dict["localisations"][dataset][channel1.lower()]["localisation_centres"] = colo_locs["localisation_centres"]
+                    self.localisation_dict["localisations"][dataset][channel1.lower()]["render_locs"] = colo_locs["render_locs"]
 
-                    self.localisation_dict["fiducials"][dataset][channel2.lower()]["localisations"] = colo_locs["localisations"]
-                    self.localisation_dict["fiducials"][dataset][channel2.lower()]["localisation_centres"] = colo_locs["localisation_centres"]
-                    self.localisation_dict["fiducials"][dataset][channel2.lower()]["render_locs"] = colo_locs["render_locs"]
+                    self.localisation_dict["localisations"][dataset][channel2.lower()]["localisations"] = colo_locs["localisations"]
+                    self.localisation_dict["localisations"][dataset][channel2.lower()]["localisation_centres"] = colo_locs["localisation_centres"]
+                    self.localisation_dict["localisations"][dataset][channel2.lower()]["render_locs"] = colo_locs["render_locs"]
 
-                    self.draw_fiducials(update_vis=True)
+                    self.draw_localisations(update_vis=True)
 
-                if self.colo_bboxes.isChecked():
+                if self.gui.colo_bboxes.isChecked():
 
                     self.localisation_dict["bounding_boxes"]["localisations"] = colo_locs["localisations"]
                     self.localisation_dict["bounding_boxes"]["localisation_centres"] = colo_locs["localisation_centres"]
 
                     self.draw_bounding_boxes()
 
         except:
             print(traceback.format_exc())
             pass
 
-    def _pixseq_colocalize_fiducials_finished(self):
+    def _pixseq_colocalize_localisations_finished(self):
 
         self.update_ui()
 
 
-    def pixseq_colocalize_fiducials(self):
+    def pixseq_colocalize_localisations(self):
 
         try:
 
-            dataset = self.colo_dataset.currentText()
-            channel1 = self.colo_channel1.currentText()
-            channel2 = self.colo_channel2.currentText()
+            dataset = self.gui.colo_dataset.currentText()
+            channel1 = self.gui.colo_channel1.currentText()
+            channel2 = self.gui.colo_channel2.currentText()
 
             ch1_loc_dict, ch1_n_locs, _ = self.get_loc_dict(dataset, channel1.lower())
             ch2_loc_dict, ch2_n_locs, _ = self.get_loc_dict(dataset, channel2.lower())
 
             if channel1 == channel2:
-                print("Channels must be different for colocalisation")
+                self.pixseq_notification("Channels must be different for colocalisation")
 
             elif ch1_n_locs == 0 or ch2_n_locs == 0:
-
-                print("No localisations found in one or both channels.")
+                self.pixseq_notification("No localisations found in one or both channels.")
 
             else:
                 self.update_ui(init=True)
 
-                self.worker = Worker(self._pixseq_colocalize_fiducials)
-                self.worker.signals.result.connect(self._pixseq_colocalize_fiducials_result)
-                self.worker.signals.finished.connect(self._pixseq_colocalize_fiducials_finished)
+                self.worker = Worker(self._pixseq_colocalize_localisations)
+                self.worker.signals.result.connect(self._pixseq_colocalize_localisations_result)
+                self.worker.signals.finished.connect(self._pixseq_colocalize_localisations_finished)
                 self.worker.signals.error.connect(self.update_ui)
                 self.threadpool.start(self.worker)
 
         except:
             print(traceback.format_exc())
             pass
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_events.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os.path
 import traceback
 import numpy as np
 from functools import partial, wraps
 from qtpy.QtWidgets import (QSlider, QLabel)
 import time
-
+from napari.utils.notifications import show_info
 
 class _events_utils:
 
+    def pixseq_notification(self, message):
+        show_info(message)
+
     def update_ui(self, error=None, init = False):
 
         try:
 
             if self.verbose:
                 print(f"Updating UI, init = {init}")
 
@@ -21,43 +24,49 @@
                         "picasso_undrift","pixseq_align_datasets",
                         "filtering_start",
                         "compute_traces",
                         "pixseq_export_data","pixseq_export_traces",
                         "pixseq_update_dataset_name",
                         "pixseq_colocalize",
                         "cluster_localisations",
+                        "filter_localisations",
+                        "segment_active",
+                        "segment_all",
+                        "cellpose_load_model",
+                        "link_localisations",
+                        "dilate_segmentations",
                         ]
 
             progressbars = ["pixseq_import_progressbar",
                             "picasso_progressbar",
                             "tform_apply_progressbar",
                             "undrift_progressbar",
                             "align_progressbar",
                             "filtering_progressbar",
                             "compute_traces_progressbar",
                             "plot_compute_progress",
                             "export_progressbar",
                             ]
 
             for progressbar in progressbars:
-                if hasattr(self, progressbar):
-                    getattr(self, progressbar).setValue(0)
+                if hasattr(self.gui, progressbar):
+                    getattr(self.gui, progressbar).setValue(0)
 
             if init is True:
 
                 for control in controls:
-                    getattr(self, control).setEnabled(False)
+                    getattr(self.gui, control).setEnabled(False)
 
                 self.stop_event.clear()
                 self.multiprocessing_active = True
 
             else:
 
                 for control in controls:
-                    getattr(self, control).setEnabled(True)
+                    getattr(self.gui, control).setEnabled(True)
 
                 self.multiprocessing_active = False
 
                 self.stop_event.clear()
                 self.multiprocessing_active = False
 
             if error is not None:
@@ -98,15 +107,15 @@
                     new_dataset_index = current_dataset_index - 1
 
                 if new_dataset_index < 0:
                     new_dataset_index = len(dataset_list) - 1
                 elif new_dataset_index > len(dataset_list) - 1:
                     new_dataset_index = 0
 
-                self.pixseq_dataset_selector.setCurrentIndex(new_dataset_index)
+                self.gui.pixseq_dataset_selector.setCurrentIndex(new_dataset_index)
 
         except:
             print(traceback.format_exc())
             pass
 
     def named_partial(self, func, *args, **kwargs):
         partial_func = partial(func, *args, **kwargs)
@@ -120,15 +129,15 @@
 
     def update_overlay_text(self):
 
         try:
 
             if self.dataset_dict  != {}:
 
-                dataset_name = self.pixseq_dataset_selector.currentText()
+                dataset_name = self.gui.pixseq_dataset_selector.currentText()
                 channel_name = self.active_channel
 
                 if dataset_name in self.dataset_dict.keys():
                     if channel_name in self.dataset_dict[dataset_name].keys():
 
                         channel_dict = self.dataset_dict[dataset_name][channel_name].copy()
 
@@ -178,54 +187,94 @@
     def select_channel_donor(self, event=None):
         self.update_active_image(channel="donor")
 
     def select_channel_acceptor(self, event=None):
         self.update_active_image(channel="acceptor")
 
 
-    def image_layer_auto_contrast(self, image):
+    def image_layer_auto_contrast(self, image, dataset, channel):
 
         contrast_limits = None
 
         try:
-            full_range = [np.min(image), np.max(image)]
+            autocontrast = True
 
-            if max(full_range) > min(full_range):
-                contrast_limits = np.percentile(image[:10].copy(), [0.1, 99.99])
+            if dataset in self.contrast_dict.keys():
+                if channel in self.contrast_dict[dataset].keys():
 
-                gamma = 1.0
-                if contrast_limits[1] > contrast_limits[0]:
-                    gamma = np.log(0.5) / np.log((contrast_limits[1] - contrast_limits[0]) / (full_range[1] - full_range[0]))
+                    autocontrast = False
 
-                if hasattr(self, "image_layer"):
-                    self.image_layer.gamma = gamma
-                    self.image_layer.contrast_limits = contrast_limits
+                    contrast_limits = self.contrast_dict[dataset][channel]["contrast_limits"]
+                    gamma = self.contrast_dict[dataset][channel]["gamma"]
+
+                    if hasattr(self, "image_layer"):
+                        self.image_layer.gamma = gamma
+                        self.image_layer.contrast_limits = contrast_limits
+
+            if autocontrast is True:
 
+                full_range = [np.min(image), np.max(image)]
+
+                if max(full_range) > min(full_range):
+                    contrast_limits = np.percentile(image[:10].copy(), [0.1, 99.99])
+
+                    gamma = 1.0
+                    if contrast_limits[1] > contrast_limits[0]:
+                        gamma = np.log(0.5) / np.log((contrast_limits[1] - contrast_limits[0]) / (full_range[1] - full_range[0]))
+
+                    if hasattr(self, "image_layer"):
+                        self.image_layer.gamma = gamma
+                        self.image_layer.contrast_limits = contrast_limits
 
         except:
             print(traceback.format_exc())
 
         return contrast_limits
 
+    def update_contrast_dict(self):
 
+        try:
+            dataset = self.active_dataset
+            channel = self.active_channel
+
+            if dataset not in self.contrast_dict.keys():
+                self.contrast_dict[dataset] = {}
+            if channel not in self.contrast_dict[dataset].keys():
+                self.contrast_dict[dataset][channel] = {}
+
+            layer_name = [layer.name for layer in self.viewer.layers if dataset in layer.name]
+
+            if len(layer_name) > 0:
+
+                image_layer = self.viewer.layers[layer_name[0]]
+                contrast_limits = image_layer.contrast_limits
+                gamma = image_layer.gamma
+
+                self.contrast_dict[dataset][channel] = {"contrast_limits": contrast_limits,
+                                                        "gamma": gamma}
+
+        except:
+            print(traceback.format_exc())
 
     def update_active_image(self, channel=None, dataset=None, event=None):
 
         try:
 
             if self.verbose:
                 print(f"Updating active image to channel {channel} and dataset {dataset}")
 
             if dataset == None or dataset not in self.dataset_dict.keys():
-                dataset_name = self.pixseq_dataset_selector.currentText()
+                dataset_name = self.gui.pixseq_dataset_selector.currentText()
             else:
                 dataset_name = dataset
 
             if dataset_name in self.dataset_dict.keys():
 
+                self.update_contrast_dict()
+
                 channel_names = [channel for channel in self.dataset_dict[dataset_name].keys()]
 
                 if channel not in channel_names:
                     if self.active_channel in channel_names:
                         channel = self.active_channel
                     else:
                         channel = channel_names[0]
@@ -250,47 +299,58 @@
                             name=layer_name,
                             colormap="gray",
                             blending="additive",
                             visible=True)
 
                         self.image_layer.mouse_drag_callbacks.append(self._mouse_event)
 
-
                     else:
                         self.image_layer.data = image
                         self.image_layer.name = layer_name
                         self.image_layer.refresh()
 
-                    self.image_layer_auto_contrast(image)
+                    self.image_layer_auto_contrast(image, dataset_name, channel)
+
+                    dataset_names = self.dataset_dict.keys()
+                    active_dataset_index = list(dataset_names).index(dataset_name)
+
+                    dataset_selector = self.gui.pixseq_dataset_selector
+
+                    dataset_selector.blockSignals(True)
+                    dataset_selector.clear()
+                    dataset_selector.addItems(dataset_names)
+                    dataset_selector.setCurrentIndex(active_dataset_index)
+                    dataset_selector.blockSignals(False)
 
             else:
                 if hasattr(self, "image_layer"):
                     self.viewer.layers.remove(self.image_layer)
 
                 self.active_dataset = None
                 self.active_channel = None
 
-            self.draw_fiducials(update_vis=True)
+            self.draw_localisations(update_vis=True)
             self.update_overlay_text()
 
         except:
             print(traceback.format_exc())
             pass
 
-    def update_channel_selector(self, dataset_selector, channel_selector, event=None, channel_type = "all", efficiency=False, block_signals=False):
+    def update_channel_selector(self, dataset_selector,
+            channel_selector, event=None, channel_type = "all", efficiency=False, block_signals=False):
 
         try:
 
             if self.verbose:
                 print(f"Updating channel selector for dataset {dataset_selector} and channel {channel_selector}")
 
-            if hasattr(self, channel_selector) and hasattr(self, dataset_selector):
+            if hasattr(self.gui, channel_selector) and hasattr(self.gui, dataset_selector):
 
-                channel_selector = getattr(self, channel_selector)
-                dataset_selector = getattr(self, dataset_selector)
+                channel_selector = getattr(self.gui, channel_selector)
+                dataset_selector = getattr(self.gui, dataset_selector)
 
                 dataset_name = dataset_selector.currentText()
 
                 if block_signals == True:
                     channel_selector.blockSignals(True)
 
                 channel_selector_list = []
@@ -306,15 +366,15 @@
 
                     for channel in channel_names:
 
                         if "efficiency" not in channel.lower():
 
                             if channel in ["da", "dd", "aa", "ad"]:
                                 channel_selector_list.append(channel.upper())
-                            elif channel in ["donor", "acceptor"]:
+                            elif channel in ["donor", "acceptor","data"]:
                                 channel_selector_list.append(channel.capitalize())
 
                             if efficiency == True:
                                 if set(["donor", "acceptor"]).issubset(set(channel_names)):
                                     channel_selector_list.append("FRET Efficiency")
                                 if set(["dd", "da"]).issubset(set(channel_names)):
                                     channel_selector_list.append("ALEX Efficiency")
@@ -331,15 +391,15 @@
 
                     for channel in channel_names:
 
                         if "efficiency" not in channel.lower():
 
                             if channel in ["da", "dd", "aa", "ad"]:
                                 channel_selector_list.append(channel.upper())
-                            elif channel in ["donor", "acceptor"]:
+                            elif channel in ["donor", "acceptor", "data"]:
                                 channel_selector_list.append(channel.capitalize())
 
                             if efficiency == True:
                                 if set(["donor", "acceptor"]).issubset(set(channel_names)):
                                     channel_selector_list.append("FRET Efficiency")
                                 if set(["dd", "da"]).issubset(set(channel_names)):
                                     channel_selector_list.append("ALEX Efficiency")
@@ -367,129 +427,145 @@
             self.update_channel_selector(dataset_selector="import_picasso_dataset", channel_selector="import_picasso_channel", efficiency=False)
             self.update_channel_selector(dataset_selector="undrift_dataset_selector", channel_selector="undrift_channel_selector")
             self.update_channel_selector(dataset_selector="cluster_dataset", channel_selector="cluster_channel")
             self.update_channel_selector(dataset_selector="tform_compute_dataset", channel_selector="tform_compute_ref_channel", channel_type="donor")
             self.update_channel_selector(dataset_selector="tform_compute_dataset", channel_selector="tform_compute_target_channel", channel_type="acceptor")
             self.update_channel_selector(dataset_selector="colo_dataset", channel_selector="colo_channel1")
             self.update_channel_selector(dataset_selector="colo_dataset", channel_selector="colo_channel2")
+            self.update_channel_selector(dataset_selector="simple_plot_dataset", channel_selector="simple_plot_channel", efficiency=True)
+            self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel")
+            self.update_channel_selector(dataset_selector="picasso_filter_dataset", channel_selector="picasso_filter_channel")
+            self.update_channel_selector(dataset_selector="cellpose_dataset", channel_selector="cellpose_channel")
+            self.update_channel_selector(dataset_selector="tracking_dataset", channel_selector="tracking_channel")
 
         except:
             print(traceback.format_exc())
             pass
 
 
 
     def update_channel_select_buttons(self):
 
         try:
-            datast_name = self.pixseq_dataset_selector.currentText()
+            datast_name = self.gui.pixseq_dataset_selector.currentText()
 
             if datast_name in self.dataset_dict.keys():
 
                 if self.verbose:
                     print(f"Updating channel select buttons for dataset {datast_name}")
 
+                import_modes = [self.dataset_dict[datast_name][channel]["import_mode"] for channel in self.dataset_dict[datast_name].keys()]
                 fret_modes = [self.dataset_dict[datast_name][channel]["FRET"] for channel in self.dataset_dict[datast_name].keys()]
                 channel_refs = [self.dataset_dict[datast_name][channel]["channel_ref"] for channel in self.dataset_dict[datast_name].keys()]
 
                 channel_refs = list(set(channel_refs))
                 fret_mode = list(set(fret_modes))[0]
+                import_mode = list(set(import_modes))[0]
 
-                self.pixseq_show_dd.clicked.connect(lambda: None)
-                self.pixseq_show_da.clicked.connect(lambda: None)
-                self.pixseq_show_aa.clicked.connect(lambda: None)
-                self.pixseq_show_ad.clicked.connect(lambda: None)
-
-                if fret_mode == True:
-
-                    self.pixseq_show_dd.setVisible(True)
-                    self.pixseq_show_da.setVisible(True)
-                    self.pixseq_show_aa.setVisible(False)
-                    self.pixseq_show_ad.setVisible(False)
+                print(datast_name, import_mode)
+
+                self.gui.pixseq_show_dd.clicked.connect(lambda: None)
+                self.gui.pixseq_show_da.clicked.connect(lambda: None)
+                self.gui.pixseq_show_aa.clicked.connect(lambda: None)
+                self.gui.pixseq_show_ad.clicked.connect(lambda: None)
+
+                if import_mode.lower() == "fret":
+
+                    self.gui.pixseq_show_dd.setVisible(True)
+                    self.gui.pixseq_show_da.setVisible(True)
+                    self.gui.pixseq_show_aa.setVisible(False)
+                    self.gui.pixseq_show_ad.setVisible(False)
 
                     if "dd" in channel_refs:
-                        self.pixseq_show_dd.setEnabled(True)
-                        self.pixseq_show_dd.setText("Donor [F1]")
+                        self.gui.pixseq_show_dd.setEnabled(True)
+                        self.gui.pixseq_show_dd.setText("Donor [F1]")
                         self.viewer.bind_key(key="F1", func=self.select_channel_donor, overwrite=True)
-                        self.pixseq_show_dd.clicked.connect(partial(self.update_active_image, channel="donor"))
+                        self.gui.pixseq_show_dd.clicked.connect(partial(self.update_active_image, channel="donor"))
                     else:
-                        self.pixseq_show_dd.setEnabled(False)
-                        self.pixseq_show_dd.setText("")
+                        self.gui.pixseq_show_dd.setEnabled(False)
+                        self.gui.pixseq_show_dd.setText("")
 
                     if "da" in channel_refs:
-                        self.pixseq_show_da.setEnabled(True)
-                        self.pixseq_show_da.setText("Acceptor [F2]")
+                        self.gui.pixseq_show_da.setEnabled(True)
+                        self.gui.pixseq_show_da.setText("Acceptor [F2]")
                         self.viewer.bind_key(key="F2", func=self.select_channel_acceptor, overwrite=True)
-                        self.pixseq_show_da.clicked.connect(partial(self.update_active_image, channel="acceptor"))
+                        self.gui.pixseq_show_da.clicked.connect(partial(self.update_active_image, channel="acceptor"))
                     else:
-                        self.pixseq_show_da.setEnabled(False)
-                        self.pixseq_show_da.setText("")
+                        self.gui.pixseq_show_da.setEnabled(False)
+                        self.gui.pixseq_show_da.setText("")
+
+                elif import_mode.lower() == "single channel":
+
+                    self.gui.pixseq_show_dd.setVisible(False)
+                    self.gui.pixseq_show_da.setVisible(False)
+                    self.gui.pixseq_show_aa.setVisible(False)
+                    self.gui.pixseq_show_ad.setVisible(False)
 
                 else:
 
-                    self.pixseq_show_dd.setVisible(True)
-                    self.pixseq_show_da.setVisible(True)
-                    self.pixseq_show_aa.setVisible(True)
-                    self.pixseq_show_ad.setVisible(True)
+                    self.gui.pixseq_show_dd.setVisible(True)
+                    self.gui.pixseq_show_da.setVisible(True)
+                    self.gui.pixseq_show_aa.setVisible(True)
+                    self.gui.pixseq_show_ad.setVisible(True)
 
                     if "dd" in channel_refs:
-                        self.pixseq_show_dd.setText("DD [F1]")
-                        self.pixseq_show_dd.setEnabled(True)
+                        self.gui.pixseq_show_dd.setText("DD [F1]")
+                        self.gui.pixseq_show_dd.setEnabled(True)
                         self.viewer.bind_key(key="F1", func=self.select_channel_dd, overwrite=True)
-                        self.pixseq_show_dd.clicked.connect(partial(self.update_active_image, channel="dd"))
+                        self.gui.pixseq_show_dd.clicked.connect(partial(self.update_active_image, channel="dd"))
 
                     else:
-                        self.pixseq_show_dd.setText("")
-                        self.pixseq_show_dd.setEnabled(False)
+                        self.gui.pixseq_show_dd.setText("")
+                        self.gui.pixseq_show_dd.setEnabled(False)
 
                     if "da" in channel_refs:
-                        self.pixseq_show_da.setText("DA [F2]")
-                        self.pixseq_show_da.setEnabled(True)
+                        self.gui.pixseq_show_da.setText("DA [F2]")
+                        self.gui.pixseq_show_da.setEnabled(True)
                         self.viewer.bind_key(key="F2", func=self.select_channel_da, overwrite=True)
-                        self.pixseq_show_da.clicked.connect(partial(self.update_active_image, channel="da"))
+                        self.gui.pixseq_show_da.clicked.connect(partial(self.update_active_image, channel="da"))
                     else:
-                        self.pixseq_show_da.setText("")
-                        self.pixseq_show_da.setEnabled(False)
+                        self.gui.pixseq_show_da.setText("")
+                        self.gui.pixseq_show_da.setEnabled(False)
 
                     if "ad" in channel_refs:
-                        self.pixseq_show_ad.setText("AD [F3]")
-                        self.pixseq_show_ad.setEnabled(True)
+                        self.gui.pixseq_show_ad.setText("AD [F3]")
+                        self.gui.pixseq_show_ad.setEnabled(True)
                         self.viewer.bind_key(key="F3", func=self.select_channel_ad, overwrite=True)
-                        self.pixseq_show_ad.clicked.connect(partial(self.update_active_image, channel="ad"))
+                        self.gui.pixseq_show_ad.clicked.connect(partial(self.update_active_image, channel="ad"))
                     else:
-                        self.pixseq_show_ad.setText("")
-                        self.pixseq_show_ad.setEnabled(False)
+                        self.gui.pixseq_show_ad.setText("")
+                        self.gui.pixseq_show_ad.setEnabled(False)
 
                     if "aa" in channel_refs:
-                        self.pixseq_show_aa.setText("AA [F4]")
-                        self.pixseq_show_aa.setEnabled(True)
+                        self.gui.pixseq_show_aa.setText("AA [F4]")
+                        self.gui.pixseq_show_aa.setEnabled(True)
                         self.viewer.bind_key(key="F4", func=self.select_channel_aa, overwrite=True)
-                        self.pixseq_show_aa.clicked.connect(partial(self.update_active_image, channel="aa"))
+                        self.gui.pixseq_show_aa.clicked.connect(partial(self.update_active_image, channel="aa"))
                     else:
-                        self.pixseq_show_aa.setText("")
-                        self.pixseq_show_aa.setEnabled(False)
+                        self.gui.pixseq_show_aa.setText("")
+                        self.gui.pixseq_show_aa.setEnabled(False)
 
         except:
             print(traceback.format_exc())
             pass
 
     def update_import_append_options(self):
 
         try:
 
-            if self.pixseq_append.isChecked():
-                self.pixseq_append_dataset.setEnabled(True)
-                self.pixseq_append_dataset_label.setEnabled(True)
-                self.pixseq_append_dataset.setVisible(True)
-                self.pixseq_append_dataset_label.setVisible(True)
+            if self.gui.pixseq_append.isChecked():
+                self.gui.pixseq_append_dataset.setEnabled(True)
+                self.gui.pixseq_append_dataset_label.setEnabled(True)
+                self.gui.pixseq_append_dataset.setVisible(True)
+                self.gui.pixseq_append_dataset_label.setVisible(True)
             else:
-                self.pixseq_append_dataset.setEnabled(False)
-                self.pixseq_append_dataset_label.setEnabled(False)
-                self.pixseq_append_dataset.setVisible(False)
-                self.pixseq_append_dataset_label.setVisible(False)
+                self.gui.pixseq_append_dataset.setEnabled(False)
+                self.gui.pixseq_append_dataset_label.setEnabled(False)
+                self.gui.pixseq_append_dataset.setVisible(False)
+                self.gui.pixseq_append_dataset_label.setVisible(False)
 
         except:
             print(traceback.format_exc())
             pass
 
 
 
@@ -497,56 +573,59 @@
     def update_import_options(self):
 
         if self.verbose:
             print("Updating import options")
 
         def update_channel_layout(self, show = True):
             if show:
-                self.pixseq_channel_layout.setEnabled(True)
-                self.pixseq_channel_layout.clear()
-                self.pixseq_channel_layout.addItems(["Donor-Acceptor", "Acceptor-Donor"])
-                self.pixseq_channel_layout.setHidden(False)
-                self.pixseq_channel_layout_label.setHidden(False)
+                self.gui.pixseq_channel_layout.setEnabled(True)
+                self.gui.pixseq_channel_layout.clear()
+                self.gui.pixseq_channel_layout.addItems(["Donor-Acceptor", "Acceptor-Donor"])
+                self.gui.pixseq_channel_layout.setHidden(False)
+                self.gui.pixseq_channel_layout_label.setHidden(False)
             else:
-                self.pixseq_channel_layout.setEnabled(False)
-                self.pixseq_channel_layout.clear()
-                self.pixseq_channel_layout.setHidden(True)
-                self.pixseq_channel_layout_label.setHidden(True)
+                self.gui.pixseq_channel_layout.setEnabled(False)
+                self.gui.pixseq_channel_layout.clear()
+                self.gui.pixseq_channel_layout.setHidden(True)
+                self.gui.pixseq_channel_layout_label.setHidden(True)
 
         def update_alex_first_frame(self, show = True):
             if show:
-                self.pixseq_alex_first_frame.setEnabled(True)
-                self.pixseq_alex_first_frame.clear()
-                self.pixseq_alex_first_frame.addItems(["Donor", "Acceptor"])
-                self.pixseq_alex_first_frame.setHidden(False)
-                self.pixseq_alex_first_frame_label.setHidden(False)
+                self.gui.pixseq_alex_first_frame.setEnabled(True)
+                self.gui.pixseq_alex_first_frame.clear()
+                self.gui.pixseq_alex_first_frame.addItems(["Donor", "Acceptor"])
+                self.gui.pixseq_alex_first_frame.setHidden(False)
+                self.gui.pixseq_alex_first_frame_label.setHidden(False)
             else:
-                self.pixseq_alex_first_frame.setEnabled(False)
-                self.pixseq_alex_first_frame.clear()
-                self.pixseq_alex_first_frame.setHidden(True)
-                self.pixseq_alex_first_frame_label.setHidden(True)
+                self.gui.pixseq_alex_first_frame.setEnabled(False)
+                self.gui.pixseq_alex_first_frame.clear()
+                self.gui.pixseq_alex_first_frame.setHidden(True)
+                self.gui.pixseq_alex_first_frame_label.setHidden(True)
 
-        import_mode = self.pixseq_import_mode.currentText()
+        import_mode = self.gui.pixseq_import_mode.currentText()
 
         if import_mode in ["Donor", "Acceptor"]:
             update_channel_layout(self, show = False)
             update_alex_first_frame(self, show = False)
 
         elif import_mode == "FRET":
             update_channel_layout(self, show = True)
             update_alex_first_frame(self, show = False)
 
         elif import_mode == "ALEX":
             update_channel_layout(self, show = True)
             update_alex_first_frame(self, show = True)
 
-        elif import_mode in ["DA", "DD", "AA","AD"]:
+        elif import_mode in ["DA", "DD", "AA", "AD"]:
             update_channel_layout(self, show = False)
             update_alex_first_frame(self, show = False)
 
+        elif import_mode == "Single Channel":
+            update_channel_layout(self, show = False)
+            update_alex_first_frame(self, show = False)
 
     def pixseq_progress(self, progress, progress_bar):
 
         progress_bar.setValue(progress)
 
         if progress == 100:
             progress_bar.setValue(0)
@@ -566,15 +645,15 @@
             event_pos = self.image_layer.world_to_data(event.position)
             image_shape = self.image_layer.data.shape
             modifiers = event.modifiers
 
             if "Shift" in modifiers or "Control" in modifiers:
 
                 if "Shift" in modifiers:
-                    mode = "fiducials"
+                    mode = "localisations"
                 elif "Control" in modifiers:
                     mode = "bounding_box"
 
                 [y,x] = [event_pos[-2], event_pos[-1]]
 
                 if (x >= 0) & (x < image_shape[-1]) & (y >= 0) & (y < image_shape[-2]):
 
@@ -595,17 +674,17 @@
     def update_nucleotide(self):
 
         if self.verbose:
             print("Updating nucleotide")
 
         try:
 
-            dataset_name = self.update_labels_dataset.currentText()
-            gap_label = self.gap_label.currentText()
-            sequence_label = self.sequence_label.currentText()
+            dataset_name = self.gui.update_labels_dataset.currentText()
+            gap_label = self.gui.gap_label.currentText()
+            sequence_label = self.gui.sequence_label.currentText()
 
             if dataset_name in self.dataset_dict.keys():
                 for channel_dict in self.dataset_dict[dataset_name].values():
                     channel_dict["gap_label"] = gap_label
                     channel_dict["sequence_label"] = sequence_label
 
             if hasattr(self, "traces_dict"):
@@ -621,23 +700,23 @@
         except:
             print(traceback.format_exc())
 
     def delete_dataset(self):
 
         try:
 
-            dataset_name = self.delete_dataset_name.currentText()
+            dataset_name = self.gui.delete_dataset_name.currentText()
 
             if dataset_name in self.dataset_dict.keys():
 
                 if self.verbose:
                     print("Deleting dataset {dataset_name}")
 
                 self.dataset_dict.pop(dataset_name)
-                self.localisation_dict["fiducials"].pop(dataset_name)
+                self.localisation_dict["localisations"].pop(dataset_name)
 
                 if hasattr(self, "traces_dict"):
                     if dataset_name in self.traces_dict.keys():
                         self.traces_dict.pop(dataset_name)
 
                 self.populate_dataset_combos()
                 self.update_channel_select_buttons()
@@ -652,16 +731,16 @@
             pass
 
 
     def update_dataset_name(self):
 
         try:
 
-            old_name = self.pixseq_old_dataset_name.currentText()
-            new_name = self.pixseq_new_dataset_name.text()
+            old_name = self.gui.pixseq_old_dataset_name.currentText()
+            new_name = self.gui.pixseq_new_dataset_name.text()
 
             if old_name != "":
 
                 if new_name == "":
                     raise ValueError("New dataset name cannot be blank")
                 elif new_name in self.dataset_dict.keys():
                     raise ValueError("New dataset name must be unique")
@@ -669,16 +748,16 @@
 
                     if self.verbose:
                         print("Updating dataset name from {old_name} to {new_name}")
 
                     dataset_data = self.dataset_dict.pop(old_name)
                     self.dataset_dict[new_name] = dataset_data
 
-                    localisation_data = self.localisation_dict["fiducials"].pop(old_name)
-                    self.localisation_dict["fiducials"][new_name] = localisation_data
+                    localisation_data = self.localisation_dict["localisations"].pop(old_name)
+                    self.localisation_dict["localisations"][new_name] = localisation_data
 
                     if hasattr(self, "traces_dict"):
                         if old_name in self.traces_dict.keys():
                             print("Updating traces dict")
                             traces_data = self.traces_dict.pop(old_name)
                             self.traces_dict[new_name] = traces_data
 
@@ -696,20 +775,32 @@
 
 
     def update_slider_label(self, slider_name):
 
         label_name = slider_name + "_label"
 
         self.slider = self.findChild(QSlider, slider_name)
-        self.label = self.findChild(QLabel, label_name)
+        self.gui.label = self.findChild(QLabel, label_name)
 
         slider_value = self.slider.value()
-        self.label.setText(str(slider_value))
+        self.gui.label.setText(str(slider_value))
 
     def update_picasso_options(self):
 
-        if self.picasso_detect_mode.currentText() == "Fiducials":
-            self.picasso_frame_mode.clear()
-            self.picasso_frame_mode.addItems(["Active", "All"])
+        if self.gui.picasso_detect_mode.currentText() == "Localisations":
+            self.gui.picasso_frame_mode.clear()
+            self.gui.picasso_frame_mode.addItems(["Active", "All"])
+        else:
+            self.gui.picasso_frame_mode.clear()
+            self.gui.picasso_frame_mode.addItem("Active")
+
+    def update_cellpose_sliders(self, slider_name, label_name):
+
+        slider = getattr(self.gui, slider_name)
+        label = getattr(self.gui, label_name)
+
+        slider_value = slider.value()
+
+        if (slider_name == "cellpose_flowthresh" or slider_name == "cellpose_maskthresh"):
+            label.setText(str(slider_value / 100))
         else:
-            self.picasso_frame_mode.clear()
-            self.picasso_frame_mode.addItem("Active")
+            label.setText(str(slider_value))
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_export_images_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_images_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         return list(common_set)
 
     def update_export_options(self):
 
         if self.dataset_dict != {}:
 
-            dataset_name = self.export_dataset.currentText()
+            dataset_name = self.gui.export_dataset.currentText()
 
             export_channel_list = []
 
             if dataset_name == "All Datasets":
                 dataset_list = list(self.dataset_dict.keys())
             else:
                 dataset_list = [dataset_name]
@@ -37,28 +37,28 @@
 
                 dataset_channel_list = []
 
                 for channel_name, channel_data in self.dataset_dict[dataset_name].items():
 
                     import_mode_list.append(channel_data["import_mode"])
 
-                    if channel_name.lower() in ["donor", "acceptor"]:
+                    if channel_name.lower() in ["donor", "acceptor", "data"]:
                         channel_name = channel_name.capitalize()
                     else:
                         channel_name = channel_name.upper()
 
                     dataset_channel_list.append(channel_name)
                 export_channel_list.append(dataset_channel_list)
 
             export_channel_list = self.common_elements(export_channel_list)
 
             export_channel_list.insert(0, "Import Channel(s)")
 
-            self.export_channel.clear()
-            self.export_channel.addItems(export_channel_list)
+            self.gui.export_channel.clear()
+            self.gui.export_channel.addItems(export_channel_list)
 
     def get_free_RAM(self):
 
             try:
 
                 memory_info = psutil.virtual_memory()
                 available_memory = memory_info.available
@@ -71,16 +71,16 @@
 
     def get_export_path(self,dialog=False):
 
         export_path = None
 
         try:
 
-            dataset_name = self.export_dataset.currentText()
-            export_channel = self.export_channel.currentText()
+            dataset_name = self.gui.export_dataset.currentText()
+            export_channel = self.gui.export_channel.currentText()
 
             dataset_dict = self.dataset_dict[dataset_name]
 
             if export_channel.lower() not in ["alex", "fret"]:
 
                 channel_dict = dataset_dict[export_channel.lower()]
                 image_path = channel_dict["path"]
@@ -124,39 +124,46 @@
 
         return export_path
 
 
 
     def get_export_jobs(self):
 
-        dataset_name = self.export_dataset.currentText()
-        export_channel = self.export_channel.currentText()
+        dataset_name = self.gui.export_dataset.currentText()
+        export_channel = self.gui.export_channel.currentText()
 
         export_jobs = []
         total_frames = 0
 
         if dataset_name == "All Datasets":
 
             for dataset_name in list(self.dataset_dict.keys()):
                 dataset_dict = self.dataset_dict[dataset_name]
 
                 if export_channel != "Import Channel(s)":
+
                     path = dataset_dict[export_channel.lower()]["path"]
-                    export_jobs.append({"dataset_name": dataset_name, "export_channel": export_channel, "import_path": path})
+
+                    export_jobs.append({"dataset_name": dataset_name,
+                                        "export_channel": export_channel,
+                                        "import_path": path})
 
                     n_frames = dataset_dict[export_channel.lower()]["data"].shape[0]
                     total_frames += n_frames
 
                 else:
                     import_modes = np.unique([channel_dict["import_mode"] for channel_dict in dataset_dict.values()])
                     channel_names = np.unique([channel_name for channel_name in dataset_dict.keys()])
                     import_paths = np.unique([channel_dict["path"] for channel_dict in dataset_dict.values()])
 
                     for path, mode, channel in zip(import_paths, import_modes, channel_names):
-                        export_jobs.append({"dataset_name": dataset_name, "export_channel": mode.upper(), "import_path": path})
+
+                        export_jobs.append({"dataset_name": dataset_name,
+                                            "export_channel": mode.upper(),
+                                            "import_path": path})
 
                         n_frames = dataset_dict[channel]["data"].shape[0]
                         total_frames += n_frames
 
         else:
 
             dataset_dict = self.dataset_dict[dataset_name]
@@ -167,14 +174,15 @@
 
                 export_jobs.append({"dataset_name": dataset_name,
                                     "export_channel": export_channel,
                                     "import_path": path})
 
                 n_frames = dataset_dict[export_channel.lower()]["data"].shape[0]
                 total_frames += n_frames
+
             else:
                 import_modes = np.unique([channel_dict["import_mode"] for channel_dict in dataset_dict.values()])
                 channel_names = np.unique([channel_name for channel_name in dataset_dict.keys()])
                 import_paths = np.unique([channel_dict["path"] for channel_dict in dataset_dict.values()])
 
                 for path, mode, channel in zip(import_paths, import_modes, channel_names):
 
@@ -193,15 +201,15 @@
             export_path = os.path.normpath(import_path)
             export_dir = os.path.dirname(export_path)
             file_name = os.path.basename(export_path)
             file_name = os.path.splitext(file_name)[0]
             file_name, file_extension = os.path.splitext(file_name)
             file_name = file_name.replace("_pixseq_processed", "")
 
-            if export_channel.lower() not in ["alex", "fret"]:
+            if export_channel.lower() not in ["alex", "fret", "single channel"]:
                 name_modifier = f"_{export_channel}_pixseq_processed.tif"
                 if name_modifier not in file_name:
                     export_path = os.path.join(export_dir, file_name + name_modifier)
                 else:
                     export_path = os.path.join(export_dir, file_name, ".tif")
             else:
                 name_modifier = "_pixseq_processed.tif"
@@ -229,29 +237,31 @@
 
             if self.dataset_dict != {}:
 
                 export_jobs, total_frames = self.get_export_jobs()
 
                 progress_dict = {}
 
+                self.pixseq_notification(f"Exporting image data...")
+
                 for job_index, export_jobs in enumerate(export_jobs):
 
                     if job_index not in progress_dict.keys():
                         progress_dict[job_index] = 0
 
                     dataset_name = export_jobs["dataset_name"]
                     export_channel = export_jobs["export_channel"]
                     export_path = export_jobs["export_path"]
 
                     self.update_ui(init=True)
 
                     def export_progress(progress, job_index=None):
                         progress_dict[job_index] = progress
                         total_progress = int(np.sum(list(progress_dict.values()))/len(progress_dict))
-                        self.pixseq_progress(total_progress, self.export_progressbar)
+                        self.pixseq_progress(total_progress, self.gui.export_progressbar)
 
                     if export_channel.lower() == "alex":
                         self.worker = Worker(self.export_alex_data,
                             dataset_name=dataset_name,
                             export_path=export_path)
                         self.worker.signals.progress.connect(partial(export_progress, job_index=job_index))
                         self.worker.signals.finished.connect(self.export_data_finished)
@@ -263,14 +273,24 @@
                             dataset_name=dataset_name,
                             export_path=export_path)
                         self.worker.signals.progress.connect(partial(export_progress, job_index=job_index))
                         self.worker.signals.finished.connect(self.export_data_finished)
                         self.worker.signals.error.connect(self.update_ui)
                         self.threadpool.start(self.worker)
 
+                    elif export_channel.lower() == "single channel":
+                        self.worker = Worker(self.export_channel_data,
+                            dataset_name=dataset_name,
+                            export_channel="Data",
+                            export_path=export_path)
+                        self.worker.signals.progress.connect(partial(export_progress, job_index=job_index))
+                        self.worker.signals.finished.connect(self.export_data_finished)
+                        self.worker.signals.error.connect(self.update_ui)
+                        self.threadpool.start(self.worker)
+
                     else:
                         self.worker = Worker(self.export_channel_data,
                             dataset_name=dataset_name,
                             export_channel=export_channel,
                             export_path=export_path)
                         self.worker.signals.progress.connect(partial(export_progress, job_index=job_index))
                         self.worker.signals.finished.connect(self.export_data_finished)
@@ -287,15 +307,15 @@
 
             channel_dict = self.dataset_dict[dataset_name][export_channel.lower()]
 
             image = channel_dict["data"]
 
             tifffile.imwrite(export_path, image)
 
-            print(f"Exported {export_channel} data to {export_path}")
+            self.pixseq_notification(f"Exported {export_channel} data to {export_path}")
 
         except:
             print(traceback.format_exc())
             pass
 
     def export_fret_data(self, progress_callback = None, dataset_name="", export_path=""):
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_export_traces_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_export_traces_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from qtpy.QtWidgets import QFileDialog
 from napari_pixseq.funcs.pixseq_utils_compute import Worker
 from functools import partial
 import numpy as np
 import json
 import pandas as pd
 import originpro as op
+import random
+import string
 
 class npEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.int32):
             return int(obj)
         return json.JSONEncoder.default(self, obj)
 
@@ -18,21 +20,23 @@
 class _export_traces_utils:
 
 
     def get_export_traces_path(self, dialog=True):
 
         if self.traces_dict != {}:
 
-            dataset_name = self.traces_export_dataset.currentText()
-            export_channel = self.traces_export_channel.currentText()
-            export_mode = self.traces_export_mode.currentText()
+            dataset_name = self.gui.traces_export_dataset.currentText()
+            export_channel = self.gui.traces_export_channel.currentText()
+            export_mode = self.gui.traces_export_mode.currentText()
 
             if dataset_name == "All Datasets":
                 dataset_name = list(self.traces_dict.keys())[0]
-            if export_channel == "All Channels":
+            if export_channel in ["All Channels",
+                                  "FRET Efficiency", "ALEX Efficiency",
+                                  "FRET Data", "ALEX Data"]:
                 export_channel = list(self.traces_dict[dataset_name].keys())[0]
 
             import_path = self.dataset_dict[dataset_name][export_channel.lower()]["path"]
 
             import_directory = os.path.dirname(import_path)
             file_name = os.path.basename(import_path)
             file_name, file_extension = os.path.splitext(file_name)
@@ -41,20 +45,24 @@
                 file_extension = ".json"
             elif export_mode == "Dat (.dat)":
                 file_extension = ".dat"
             elif export_mode == "Text (.txt)":
                 file_extension = ".txt"
             elif export_mode == "CSV (.csv)":
                 file_extension = ".csv"
+            elif export_mode == "Nero (.dat)":
+                file_extension = ".dat"
+            elif export_mode == "ebFRET SMD (.mat)":
+                file_extension = ".mat"
             elif export_mode == "Excel":
                 file_extension = ".xlsx"
             elif export_mode == "OriginLab":
                 file_extension = ".opju"
             else:
-                print(f"Export mode {export_mode} not recognized.")
+                self.pixseq_notification(f"Export mode {export_mode} not recognized.")
 
             export_path = os.path.join(import_directory, file_name + file_extension)
             export_path = os.path.normpath(export_path)
 
             if dialog:
                 export_path = QFileDialog.getSaveFileName(self, "Save File", export_path, "All Files (*)")[0]
 
@@ -188,16 +196,14 @@
             if op.oext:
                 op.exit()
 
         except:
             print(traceback.format_exc())
 
 
-
-
     def json_dict_report(self, json_dataset):
 
         try:
 
             if json_dataset != {}:
 
                 json_report = {}
@@ -243,18 +249,18 @@
                 print(f" Size: {json_dataset_size_mb} MB")
 
         except:
             print(traceback.format_exc())
 
     def populate_json_dict(self, progress_callback=None):
 
-        dataset_name = self.traces_export_dataset.currentText()
-        channel_name = self.traces_export_channel.currentText()
-        metric_name = self.traces_export_metric.currentText()
-        background_mode = self.traces_export_background.currentText()
+        dataset_name = self.gui.traces_export_dataset.currentText()
+        channel_name = self.gui.traces_export_channel.currentText()
+        metric_name = self.gui.traces_export_metric.currentText()
+        background_mode = self.gui.traces_export_background.currentText()
 
         metric_key = self.get_dict_key(self.metric_dict, metric_name)
 
         if background_mode not in ["None", None,""] and type(metric_key) == str:
             key_modifier = self.get_dict_key(self.background_dict, background_mode)
             background_metric_key = metric_key + key_modifier
         else:
@@ -272,20 +278,20 @@
             channel_list = [channel for channel in channel_list if "efficiency" not in channel.lower()]
             iteration_channel = channel_list[0]
             if set(["dd", "da"]).issubset(channel_list):
                 channel_list.append("alex_efficiency")
             if set(["donor", "acceptor"]).issubset(channel_list):
                 channel_list.append("fret_efficiency")
 
-        elif channel_name.lower() == "fret":
+        elif channel_name.lower() == "fret data":
             channel_list = ["donor", "acceptor"]
-        elif channel_name.lower() == "alex":
+        elif channel_name.lower() == "alex data":
             channel_list = ["dd", "da", "ad", "aa"]
         else:
-            channel_list = [channel_name]
+            channel_list = [channel_name.lower()]
 
         json_dict = {"metadata": {}, "data": {}}
 
         n_traces = 0
         for dataset in dataset_list:
             if dataset in self.traces_dict:
                 for channel in channel_list:
@@ -394,18 +400,18 @@
         return json_dict
 
     def populate_export_dict(self):
 
         export_dict = {}
 
         try:
-            dataset_name = self.traces_export_dataset.currentText()
-            channel_name = self.traces_export_channel.currentText()
-            metric_name = self.traces_export_metric.currentText()
-            background_mode = self.traces_export_background.currentText()
+            dataset_name = self.gui.traces_export_dataset.currentText()
+            channel_name = self.gui.traces_export_channel.currentText()
+            metric_name = self.gui.traces_export_metric.currentText()
+            background_mode = self.gui.traces_export_background.currentText()
 
             metric_key = self.get_dict_key(self.metric_dict, metric_name)
 
             if background_mode not in ["None", None, ""] and type(metric_key) == str:
                 key_modifier = self.get_dict_key(self.background_dict, background_mode)
                 background_metric_key = metric_key + key_modifier
             else:
@@ -414,42 +420,62 @@
             if dataset_name == "All Datasets":
                 dataset_list = list(self.traces_dict.keys())
             else:
                 dataset_list = [dataset_name]
 
             if channel_name == "All Channels":
                 channel_list = list(self.traces_dict[dataset_list[0]].keys())
-            elif channel_name.lower() == "fret":
+            elif channel_name.lower() == "fret data":
                 channel_list = ["donor", "acceptor"]
-            elif channel_name.lower() == "alex":
+            elif channel_name.lower() == "alex data":
                 channel_list = ["dd", "da", "ad", "aa"]
+            elif channel_name.lower() == "alex efficiency":
+                channel_list = ["alex_efficiency"]
+            elif channel_name.lower() == "fret efficiency":
+                channel_list = ["fret_efficiency"]
             else:
-                channel_list = [channel_name]
-
-            channel_list = [chan for chan in channel_list if "efficiency" not in chan.lower()]
+                channel_list = [channel_name.lower()]
 
             dataset_name_list = []
             channel_name_list = []
             index_list = []
             data_list = []
 
             n_traces = 0
 
             n_traces = len(self.traces_dict[dataset_list[0]][channel_list[0]].keys())
 
-
             for dataset in dataset_list:
+
+                if channel_name == "All Channels" or "efficiency" in channel_name.lower():
+
+                    if set(["dd", "da"]).issubset(channel_list):
+
+                        self.compute_alex_efficiency(dataset, metric_key,
+                            background_metric_key, progress_callback=None,
+                            clip_data=True)
+
+                    elif set(["donor", "acceptor"]).issubset(channel_list):
+
+                        self.compute_fret_efficiency(dataset, metric_key,
+                            background_metric_key, progress_callback=None,
+                            clip_data=True)
+
                 for trace_index in range(n_traces):
                     for channel in channel_list:
 
                         if trace_index in self.traces_dict[dataset][channel].keys():
                             trace_dict = self.traces_dict[dataset][channel][trace_index].copy()
 
                             if channel.lower() in ["dd", "da", "ad", "aa"]:
                                 channel_name = channel.upper()
+                            elif channel.lower() == "alex_efficiency":
+                                channel_name = "ALEX Efficiency"
+                            elif channel.lower() == "fret_efficiency":
+                                channel_name = "FRET Efficiency"
                             else:
                                 channel_name = channel.capitalize()
 
                             if dataset not in export_dict.keys():
                                 export_dict[dataset] = []
 
                             data = np.array(trace_dict[metric_key].copy())
@@ -483,85 +509,104 @@
         self.update_ui()
 
     def export_traces_error(self, error_message):
 
         self.update_ui()
 
 
-
     def export_traces(self):
 
         try:
 
-            self.pixseq_export_traces.setEnabled(False)
+            self.gui.pixseq_export_traces.setEnabled(False)
 
             export_path, export_directory = self.get_export_traces_path(dialog=True)
 
             if export_path != "" and os.path.isdir(export_directory):
 
                 self.update_ui(init=True)
 
-                export_mode = self.traces_export_mode.currentText()
+                export_mode = self.gui.traces_export_mode.currentText()
 
                 if export_mode == "JSON Dataset":
 
                     self.worker = Worker(self.export_traces_json, export_path=export_path)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.export_progressbar))
+                        progress_bar=self.gui.export_progressbar))
                     self.worker.signals.finished.connect(partial(self.export_traces_finished,
                         export_path=export_path))
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
                 elif export_mode == "Dat (.dat)":
 
                     self.worker = Worker(self.export_traces_dat, export_path=export_path)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.export_progressbar))
+                        progress_bar=self.gui.export_progressbar))
                     self.worker.signals.finished.connect(partial(self.export_traces_finished,
                         export_path=export_path))
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
                 elif export_mode == "Text (.txt)":
 
                     self.worker = Worker(self.export_traces_txt, export_path=export_path)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.export_progressbar))
+                        progress_bar=self.gui.export_progressbar))
                     self.worker.signals.finished.connect(partial(self.export_traces_finished,
                         export_path=export_path))
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
                 elif export_mode == "CSV (.csv)":
 
                     self.worker = Worker(self.export_traces_csv, export_path=export_path)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.export_progressbar))
+                        progress_bar=self.gui.export_progressbar))
                     self.worker.signals.finished.connect(partial(self.export_traces_finished,
                         export_path=export_path))
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
                 elif export_mode == "Excel":
 
                     self.worker = Worker(self.export_traces_excel, export_path=export_path)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.export_progressbar))
+                        progress_bar=self.gui.export_progressbar))
                     self.worker.signals.finished.connect(partial(self.export_traces_finished,
                         export_path=export_path))
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
 
                 elif export_mode == "OriginLab":
 
                     self.worker = Worker(self.export_traces_originlab, export_path=export_path)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.export_progressbar))
+                        progress_bar=self.gui.export_progressbar))
+                    self.worker.signals.finished.connect(partial(self.export_traces_finished,
+                        export_path=export_path))
+                    self.worker.signals.error.connect(self.update_ui)
+                    self.threadpool.start(self.worker)
+
+                elif export_mode == "Nero (.dat)":
+
+                    self.worker = Worker(self.export_traces_nero, export_path=export_path)
+                    self.worker.signals.progress.connect(partial(self.pixseq_progress,
+                        progress_bar=self.gui.export_progressbar))
+                    self.worker.signals.finished.connect(partial(self.export_traces_finished,
+                        export_path=export_path))
+                    self.worker.signals.error.connect(self.update_ui)
+                    self.threadpool.start(self.worker)
+
+                elif export_mode == "ebFRET SMD (.mat)":
+
+                    self.worker = Worker(self.export_traces_ebfret_smd, export_path=export_path)
+                    self.worker.signals.progress.connect(partial(self.pixseq_progress,
+                        progress_bar=self.gui.export_progressbar))
                     self.worker.signals.finished.connect(partial(self.export_traces_finished,
                         export_path=export_path))
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
                 else:
                     self.update_ui()
@@ -569,21 +614,147 @@
             else:
                 self.update_ui()
 
         except:
             print(traceback.format_exc())
             self.update_ui()
 
+    def export_traces_nero(self, export_path, progress_callback=None):
+
+        try:
+            export_dict = self.populate_export_dict()
+
+            export_data = np.stack(export_dict["data"], axis=0).T
+
+            export_indices = np.array(export_dict["index"]).astype(int)
+            export_indices += 1
+
+            export_data = pd.DataFrame(export_data)
+            export_data.columns = export_indices
+
+            export_data.to_csv(export_path, index=False, sep=" ")
+
+        except:
+            print(traceback.format_exc())
+
+    def populate_smd_dict(self):
+
+        try:
+
+            dataset_name = self.gui.traces_export_dataset.currentText()
+            channel_name = self.gui.traces_export_channel.currentText()
+            metric_name = self.gui.traces_export_metric.currentText()
+            background_mode = self.gui.traces_export_background.currentText()
+
+            metric_key = self.get_dict_key(self.metric_dict, metric_name)
+
+            if background_mode not in ["None", None, ""] and type(metric_key) == str:
+                key_modifier = self.get_dict_key(self.background_dict, background_mode)
+                background_metric_key = metric_key + key_modifier
+            else:
+                background_metric_key = None
+
+            if dataset_name == "All Datasets":
+                dataset_list = list(self.traces_dict.keys())
+            else:
+                dataset_list = [dataset_name]
+
+            if channel_name == "All Channels":
+                channel_list = list(self.traces_dict[dataset_list[0]].keys())
+            elif channel_name.lower() == "fret data":
+                channel_list = ["donor", "acceptor"]
+            elif channel_name.lower() == "alex data":
+                channel_list = ["dd", "da", "ad", "aa"]
+            elif channel_name.lower() == "alex efficiency":
+                channel_list = ["alex_efficiency"]
+            elif channel_name.lower() == "fret efficiency":
+                channel_list = ["fret_efficiency"]
+            else:
+                channel_list = [channel_name.lower()]
+
+            smd_dict = {"attr": {"data_package": "TraceAnalyser"},
+                        "columns": channel_list,
+                        "data": {"attr": [], "id": [], "index": [], "values": []},
+                        "id": ''.join(random.choices(string.ascii_lowercase + string.digits, k=32)),
+                        "type": "TraceAnalyser",
+                        }
+
+            n_traces = len(self.traces_dict[dataset_list[0]][channel_list[0]].keys())
+
+
+
+            for dataset in dataset_list:
+
+                export_channel = list(self.traces_dict[dataset].keys())[0]
+                file_path = self.dataset_dict[dataset_name][export_channel.lower()]["path"]
+
+                for trace_index in range(n_traces):
+
+                    smd_values = []
+
+                    for channel in channel_list:
+
+                        if trace_index in self.traces_dict[dataset][channel].keys():
+                            trace_dict = self.traces_dict[dataset][channel][trace_index].copy()
+
+                            data = np.array(trace_dict[metric_key].copy())
+
+                            if "efficiency" not in channel and background_mode != "None":
+                                background = np.array(trace_dict[background_metric_key].copy())
+                                data = data - background
+
+                            smd_values.append(data)
+
+                    smd_index = np.expand_dims(np.arange(1, len(smd_values[0])+1), -1).astype(float).tolist()
+                    smd_values = np.stack(smd_values, axis=1).tolist()
+
+                    lowerbound = np.min(smd_values)
+
+                    smd_id = ''.join(random.choices(string.ascii_lowercase + string.digits, k=32))
+                    smd_attr = {
+                        "file": os.path.basename(file_path),
+                        "layer": channel,
+                        "localisation_number": trace_index,
+                        "lowerbound": lowerbound,
+                        "group": "group 1",
+                        "restart":0,
+                        "crop_min": 0,
+                        "crop_max": len(data),
+                    }
+
+                    smd_dict["data"]["attr"].append(smd_attr)
+                    smd_dict["data"]["id"].append(smd_id)
+                    smd_dict["data"]["index"].append(smd_index)
+                    smd_dict["data"]["values"].append(smd_values)
+
+        except:
+            print(traceback.format_exc())
+            smd_dict = {}
+
+        return smd_dict
+
+    def export_traces_ebfret_smd(self, export_path, progress_callback=None):
+
+            try:
+
+                smd_dict = self.populate_smd_dict()
+
+                import mat4py
+                mat4py.savemat(export_path, smd_dict)
+
+            except:
+                print(traceback.format_exc())
 
     def populate_export_combos(self):
 
         try:
             export_channel_list = []
 
-            export_dataset = self.traces_export_dataset.currentText()
+            export_mode = self.gui.traces_export_mode.currentText()
+            export_dataset = self.gui.traces_export_dataset.currentText()
 
             if export_dataset != "":
 
                 if export_dataset == "All Datasets":
 
                     for dataset_name, dataset_dict in self.dataset_dict.items():
                         for channel_name in dataset_dict.keys():
@@ -597,37 +768,43 @@
                             export_channel_list = list(set(export_channel_list))
 
                 else:
 
                     if export_dataset in self.dataset_dict.keys():
                         for channel_name in self.dataset_dict[export_dataset].keys():
 
-                            if channel_name.lower() in ["donor", "acceptor"]:
+                            if channel_name.lower() in ["donor", "acceptor", "data"]:
                                 channel_name = channel_name.capitalize()
                             else:
                                 channel_name = channel_name.upper()
 
                             export_channel_list.append(channel_name)
 
                 if set(["Donor", "Acceptor"]).issubset(set(export_channel_list)):
-                    export_channel_list.insert(0, "FRET")
+                    export_channel_list.insert(0, "FRET Data")
+                    export_channel_list.insert(0, "FRET Efficiency")
                 if set(["DD","DA","AA","AD"]).issubset(set(export_channel_list)):
-                    export_channel_list.insert(0, "ALEX")
+                    export_channel_list.insert(0, "ALEX Data")
+                    export_channel_list.insert(0, "ALEX Efficiency")
 
                 export_channel_list.insert(0, "All Channels")
 
-                self.traces_export_channel.blockSignals(True)
-                self.traces_export_channel.clear()
-                self.traces_export_channel.addItems(export_channel_list)
-                self.traces_export_channel.blockSignals(True)
+                if export_mode == "Nero (.dat)":
+                    multi_channel_list = ["All Channels", "FRET Data", "ALEX Data"]
+                    export_channel_list = [chan for chan in export_channel_list if chan not in multi_channel_list]
+
+                self.gui.traces_export_channel.blockSignals(True)
+                self.gui.traces_export_channel.clear()
+                self.gui.traces_export_channel.addItems(export_channel_list)
+                self.gui.traces_export_channel.blockSignals(True)
 
                 # if hasattr(self, "traces_dict"):
                 #
-                #     dataset_name = self.traces_export_dataset.currentText()
-                #     channel_name = self.traces_export_channel.currentText()
+                #     dataset_name = self.gui.traces_export_dataset.currentText()
+                #     channel_name = self.gui.traces_export_channel.currentText()
                 #
                 #     if dataset_name in self.traces_dict.keys():
                 #
                 #         if dataset_name == "All Datasets":
                 #             dataset_names = list(self.traces_dict.keys())
                 #             dataset_name = dataset_names[0]
                 #
@@ -643,20 +820,20 @@
                 #
                 #         if dataset_name in self.traces_dict.keys():
                 #             if channel_name.lower() in self.traces_dict[dataset_name].keys():
                 #
                 #                 traces_channel_dict = self.traces_dict[dataset_name][channel_name.lower()]
                 #                 metric_names = traces_channel_dict[0].keys()
                 #
-                #                 # self.traces_export_metric.blockSignals(True)
+                #                 # self.gui.traces_export_metric.blockSignals(True)
                 #                 #
-                #                 # self.traces_export_metric.clear()
+                #                 # self.gui.traces_export_metric.clear()
                 #                 #
                 #                 # for metric in metric_names:
                 #                 #     if metric in self.metric_dict.keys():
-                #                 #         self.traces_export_metric.addItem(self.metric_dict[metric])
+                #                 #         self.gui.traces_export_metric.addItem(self.metric_dict[metric])
                 #                 #
-                #                 # self.traces_export_metric.blockSignals(False)
+                #                 # self.gui.traces_export_metric.blockSignals(False)
 
         except:
             print(traceback.format_exc())
             pass
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_import_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_import_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,98 +6,156 @@
 from napari_pixseq.funcs.pixseq_utils_compute import Worker
 import time
 import multiprocessing
 from multiprocessing import shared_memory, Manager
 from functools import partial
 import tifffile
 import concurrent.futures
-
+from astropy.io import fits
 
 def import_image_data(dat, progress_dict={}, index=0):
 
     try:
 
         path = dat["path"]
         frame_list = dat["frame_list"]
         channel_list = dat["channel_list"]
         channel_frame_list = dat["channel_frame_list"]
         channel_images = dat["channel_images"]
 
+        base, ext = os.path.splitext(path)
+
         n_frames = len(frame_list)
 
-        for (frame_index, channels, channel_frame) in zip(frame_list, channel_list, channel_frame_list):
+        if ext.lower() == ".tif":
 
-            image_shape = dat["image_shape"]
-            stop_event = dat["stop_event"]
+            with Image.open(path) as image:
 
-            if not stop_event.is_set():
+                for (frame_index, channels, channel_frame) in zip(frame_list, channel_list, channel_frame_list):
 
-                img_frame = tifffile.imread(path, key=frame_index)
+                    image_shape = dat["image_shape"]
+                    stop_event = dat["stop_event"]
 
-                if len(channels) == 1:
-                    img_frames = [img_frame]
-                else:
-                    img_frames = np.array_split(img_frame, 2, axis=-1)
+                    if not stop_event.is_set():
+
+                        image.seek(frame_index)
+                        img_frame = np.array(image)
+
+                        if len(channels) == 1:
+                            img_frames = [img_frame]
+                        else:
+                            img_frames = np.array_split(img_frame, 2, axis=-1)
+
+                        for channel, channel_img in zip(channels, img_frames):
+
+                            shared_mem = channel_images[channel]
+                            np_array = np.ndarray(image_shape, dtype=dat["dtype"], buffer=shared_mem.buf)
+                            np_array[channel_frame] = channel_img
+
+                    progress = int(((frame_index + 1) / n_frames)*100)
+                    progress_dict[index] = progress
+
+        elif ext.lower() == ".fits":
+
+            with fits.open(path) as hdul:
 
-                for channel, channel_img in zip(channels, img_frames):
+                for (frame_index, channels, channel_frame) in zip(frame_list, channel_list, channel_frame_list):
 
-                    shared_mem = channel_images[channel]
-                    np_array = np.ndarray(image_shape, dtype=dat["dtype"], buffer=shared_mem.buf)
-                    np_array[channel_frame] = channel_img
+                    image_shape = dat["image_shape"]
+                    stop_event = dat["stop_event"]
 
-            progress = int(((frame_index + 1) / n_frames)*100)
-            progress_dict[index] = progress
+                    if not stop_event.is_set():
+
+                        img_frame = hdul[0].data[frame_index]
+
+                        if len(channels) == 1:
+                            img_frames = [img_frame]
+                        else:
+                            img_frames = np.array_split(img_frame, 2, axis=-1)
+
+                        for channel, channel_img in zip(channels, img_frames):
+
+                            shared_mem = channel_images[channel]
+                            np_array = np.ndarray(image_shape, dtype=dat["dtype"], buffer=shared_mem.buf)
+                            np_array[channel_frame] = channel_img
+
+                    progress = int(((frame_index + 1) / n_frames)*100)
+                    progress_dict[index] = progress
 
     except:
         print(traceback.format_exc())
         pass
 
 
 
 class _import_utils:
 
-    def create_import_shared_image(self, image_shape, image_dtype):
+    def create_import_shared_image(self, image_size):
 
         shared_mem = None
 
         try:
 
             if self.verbose:
                 print("Creating shared image...")
 
-            image_shape = tuple(np.array(image_shape).astype(int))
-
-            image_size = np.prod(image_shape) * (image_dtype.itemsize)
-            image_size = int(image_size)
-
-            image_size_gb = image_size / 1000000000
-
             shared_mem = shared_memory.SharedMemory(create=True, size=image_size)
-            shared_memory_name = shared_mem.name
-            shared_image = np.ndarray(image_shape, dtype=image_dtype, buffer=shared_mem.buf)
 
         except:
             print(traceback.format_exc())
             pass
 
         return shared_mem
 
     def get_image_info(self, path):
 
-        with Image.open(path) as img:
-            n_frames = img.n_frames
-            page_shape = img.size
+        if self.verbose:
+            print(f"Getting image info for {path}")
 
-            img.seek(0)
-            np_img = np.array(img)
-            dtype = np_img.dtype
+        base, ext = os.path.splitext(path)
 
-        image_shape = (n_frames, page_shape[1], page_shape[0])
+        if ext.lower() == ".tif":
 
-        return n_frames, image_shape, dtype
+            image_size = os.path.getsize(path)  # Get file size directly
+
+            with tifffile.TiffFile(path) as tif:
+                n_frames = len(tif.pages)  # Number of pages (frames)
+                page_shape = tif.pages[0].shape  # Dimensions of the first page
+                dtype = tif.pages[0].dtype  # Data type of the first page
+
+            image_shape = (n_frames, page_shape[0], page_shape[1])
+
+        elif ext.lower() == ".fits":
+
+            image_size = os.path.getsize(path)
+
+            with fits.open(path, mode='readonly', ignore_missing_end=True) as hdul:
+
+                header = hdul[0].header
+
+                # Extract shape information from the header
+                if header['NAXIS'] == 3:
+                    image_shape = (header['NAXIS3'], header['NAXIS2'], header['NAXIS1'])
+                else:
+                    image_shape = (header['NAXIS2'], header['NAXIS1'])
+
+                n_frames = image_shape[0] if len(image_shape) == 3 else 1
+                page_shape = image_shape[1:] if len(image_shape) == 3 else image_shape
+
+                # Determine the data type from BITPIX
+                bitpix_to_dtype = {8: np.dtype('uint8'),
+                                   16: np.dtype('uint16'),
+                                   32: np.dtype('uint32'),
+                                   -32: np.dtype('float32'),
+                                   -64: np.dtype('float64'),
+                                   }
+
+                dtype = bitpix_to_dtype[header['BITPIX']]
+
+        return n_frames, image_shape, dtype, image_size
 
     def format_import_path(self, path):
 
         try:
 
             path = os.path.normpath(path)
 
@@ -127,38 +185,38 @@
         shared_images = {}
 
         try:
 
             if self.verbose:
                 print("Populating import lists/metadata...")
 
-            import_mode = self.pixseq_import_mode.currentText()
-            import_limit_combo = self.pixseq_import_limt.currentText()
-            channel_layout = self.pixseq_channel_layout.currentText()
-            alex_first_frame = self.pixseq_alex_first_frame.currentText()
+            import_mode = self.gui.pixseq_import_mode.currentText()
+            import_limit_combo = self.gui.pixseq_import_limt.currentText()
+            channel_layout = self.gui.pixseq_channel_layout.currentText()
+            alex_first_frame = self.gui.pixseq_alex_first_frame.currentText()
 
             for path_index, path in enumerate(paths):
 
                 path = self.format_import_path(path)
                 file_name = os.path.basename(path)
 
-                if self.pixseq_append.isChecked():
-                    dataset_name = self.pixseq_append_dataset.currentText()
+                if self.gui.pixseq_append.isChecked():
+                    dataset_name = self.gui.pixseq_append_dataset.currentText()
                 else:
                     dataset_name = file_name
 
                 if dataset_name not in shared_images.keys():
                     shared_images[dataset_name] = {}
 
-                n_frames, image_shape, dtype = self.get_image_info(path)
+                n_frames, image_shape, dtype, image_size = self.get_image_info(path)
 
                 if import_mode.lower() in ["donor", "acceptor", "dd", "da", "ad", "aa"]:
 
                     if import_limit_combo != "None":
-                        import_limit = int(self.pixseq_import_limt.currentText())
+                        import_limit = int(self.gui.pixseq_import_limt.currentText())
                     else:
                         import_limit = n_frames
 
                     image_shape = (import_limit, image_shape[1], image_shape[2])
 
                     frame_list = list(range(n_frames))[:import_limit]
 
@@ -170,15 +228,57 @@
 
                     channel_images = {}
                     for channel in channel_names:
 
                         if self.verbose:
                             print(f"Creating image memory for {dataset_name} {channel}...")
 
-                        shared_image = self.create_import_shared_image(image_shape, dtype)
+                        shared_image = self.create_import_shared_image(image_size)
+                        channel_images[channel] = shared_image
+                        shared_images[dataset_name][channel] = shared_image
+
+                    image_dict = {"path": path,
+                                  "dataset_name": dataset_name,
+                                  "n_frames": n_frames,
+                                  "channel_names": channel_names,
+                                  "channel_list": channel_list,
+                                  "frame_list": frame_list,
+                                  "channel_frame_list": frame_list,
+                                  "channel_images": channel_images,
+                                  "image_shape": image_shape,
+                                  "channel_layout": channel_layout,
+                                  "alex_first_frame": alex_first_frame,
+                                  "dtype": dtype,
+                                  "import_mode": import_mode.lower()}
+
+                    image_list.append(image_dict)
+
+                elif import_mode.lower() == "single channel":
+
+                    if import_limit_combo != "None":
+                        import_limit = int(self.gui.pixseq_import_limt.currentText())
+                    else:
+                        import_limit = n_frames
+
+                    image_shape = (import_limit, image_shape[1], image_shape[2])
+
+                    frame_list = list(range(n_frames))[:import_limit]
+
+                    unique_frames = np.unique(frame_list)
+                    n_frames = len(unique_frames)
+
+                    channel_names = ["data"]
+                    channel_list = [channel_names] * n_frames
+
+                    channel_images = {}
+                    for channel in channel_names:
+                        if self.verbose:
+                            print(f"Creating image memory for {dataset_name} {channel}...")
+
+                        shared_image = self.create_import_shared_image(image_size)
                         channel_images[channel] = shared_image
                         shared_images[dataset_name][channel] = shared_image
 
                     image_dict = {"path": path,
                                   "dataset_name": dataset_name,
                                   "n_frames": n_frames,
                                   "channel_names": channel_names,
@@ -193,15 +293,15 @@
                                   "import_mode": import_mode.lower()}
 
                     image_list.append(image_dict)
 
                 elif import_mode.lower() == "fret":
 
                     if import_limit_combo != "None":
-                        import_limit = int(self.pixseq_import_limt.currentText())
+                        import_limit = int(self.gui.pixseq_import_limt.currentText())
                     else:
                         import_limit = n_frames
 
                     frame_list = list(range(n_frames))[:import_limit]
 
                     if channel_layout.lower() == "donor-acceptor":
                         channel_names = ["donor", "acceptor"]
@@ -217,15 +317,15 @@
 
                     channel_images = {}
                     for channel in channel_names:
 
                         if self.verbose:
                             print(f"Creating shared image for {dataset_name} {channel}...")
 
-                        shared_image = self.create_import_shared_image(image_shape, dtype)
+                        shared_image = self.create_import_shared_image(image_size//2)
                         channel_images[channel] = shared_image
                         shared_images[dataset_name][channel] = shared_image
 
                     image_dict = {"path": path,
                                   "dataset_name": dataset_name,
                                   "n_frames": n_frames,
                                   "channel_names": channel_names,
@@ -240,15 +340,15 @@
                                   "import_mode": import_mode.lower()}
 
                     image_list.append(image_dict)
 
                 elif import_mode.lower() == "alex":
 
                     if import_limit_combo != "None":
-                        import_limit = int(self.pixseq_import_limt.currentText())
+                        import_limit = int(self.gui.pixseq_import_limt.currentText())
                     else:
                         import_limit = n_frames
 
                     frame_list = list(range(n_frames))
 
                     even_frames = frame_list[::2][:import_limit]
                     odd_frames = frame_list[1::2][:import_limit]
@@ -285,15 +385,15 @@
 
                     channel_images = {}
                     for channel in channel_names:
 
                         if self.verbose:
                             print(f"Creating shared memory for {dataset_name} {channel}...")
 
-                        shared_image = self.create_import_shared_image(image_shape, dtype)
+                        shared_image = self.create_import_shared_image(image_size//4)
                         channel_images[channel] = shared_image
                         shared_images[dataset_name][channel] = shared_image
 
                     image_dict = {"path": path,
                                   "dataset_name": dataset_name,
                                   "n_frames": n_frames,
                                   "channel_names": channel_names,
@@ -305,16 +405,16 @@
                                   "channel_layout": channel_layout,
                                   "alex_first_frame": alex_first_frame,
                                   "dtype": dtype,
                                   "import_mode": import_mode.lower()}
 
                     image_list.append(image_dict)
 
-                channel_layout = self.pixseq_channel_layout.currentText()
-                alex_first_frame = self.pixseq_alex_first_frame.currentText()
+                channel_layout = self.gui.pixseq_channel_layout.currentText()
+                alex_first_frame = self.gui.pixseq_alex_first_frame.currentText()
 
                 if dataset_name not in import_dict.keys():
                     import_dict[dataset_name] = {"path":path,
                                                  "import_mode": import_mode.lower(),
                                                  "import_limit": import_limit,
                                                  "channel_layout": channel_layout,
                                                  "alex_first_frame": alex_first_frame,
@@ -380,14 +480,16 @@
         if self.verbose:
             print("Finished processing compute jobs.")
 
     def populate_import_dataset_dict(self, import_dict):
 
         try:
 
+            concat_images = self.gui.pixseq_concatenate.isChecked()
+
             if self.verbose:
                 print("Populating dataset dict")
 
             for dataset_name, dataset_dict in import_dict.items():
 
                 image_dict = {}
 
@@ -443,21 +545,43 @@
                     image_dict[channel_name]["channel_layout"] = channel_layout
                     image_dict[channel_name]["alex_first_frame"] = alex_first_frame
                     image_dict[channel_name]["FRET"] = fret
                     image_dict[channel_name]["import_mode"] = import_mode
                     image_dict[channel_name]["gap_label"] = None
                     image_dict[channel_name]["sequence_label"] = None
 
-                if dataset_name not in self.dataset_dict.keys():
-                    self.dataset_dict[dataset_name] = image_dict
+                if concat_images == False:
+
+                    if dataset_name not in self.dataset_dict.keys():
+                        self.dataset_dict[dataset_name] = image_dict
+                    else:
+                        for channel_name, channel_dict in image_dict.items():
+                            self.dataset_dict[dataset_name][channel_name] = channel_dict
+
                 else:
-                    for channel_name, channel_dict in image_dict.items():
-                        self.dataset_dict[dataset_name][channel_name] = channel_dict
+                    dataset_name = list(import_dict.keys())[0]
+
+                    if dataset_name not in self.dataset_dict.keys():
+                        self.dataset_dict[dataset_name] = image_dict
+                    else:
+                        for channel_name, channel_dict in image_dict.items():
+                            if channel_name not in self.dataset_dict[dataset_name].keys():
+                                self.dataset_dict[dataset_name][channel_name] = channel_dict
+                            else:
+                                dataset_image = self.dataset_dict[dataset_name][channel_name]["data"]
+                                new_image = image_dict[channel_name]["data"]
+
+                                if dataset_image.shape[1:] == new_image.shape[1:]:
+
+                                    dataset_image = np.concatenate([dataset_image, new_image], axis=0)
+
+                                    self.dataset_dict[dataset_name][channel_name]["data"] = dataset_image
 
         except:
+            print(traceback.format_exc())
             pass
 
     def closed_import_shared_images(self):
 
         if hasattr(self, "shared_images"):
 
             if self.verbose:
@@ -491,122 +615,147 @@
         try:
 
             if self.verbose:
                 print("Populating all dataset combos.")
 
             dataset_names = list(self.dataset_dict.keys())
 
-            self.pixseq_dataset_selector.blockSignals(True)
-            self.pixseq_dataset_selector.clear()
-            self.pixseq_dataset_selector.addItems(dataset_names)
-            self.pixseq_dataset_selector.blockSignals(False)
-
-            self.cluster_dataset.blockSignals(True)
-            self.cluster_dataset.clear()
-            self.cluster_dataset.addItems(dataset_names)
-            self.cluster_dataset.blockSignals(False)
-
-            self.tform_compute_dataset.blockSignals(True)
-            self.tform_compute_dataset.clear()
-            self.tform_compute_dataset.addItems(dataset_names)
-            self.tform_compute_dataset.blockSignals(False)
-
-            self.pixseq_old_dataset_name.blockSignals(True)
-            self.pixseq_old_dataset_name.clear()
-            self.pixseq_old_dataset_name.addItems(dataset_names)
-            self.pixseq_old_dataset_name.blockSignals(False)
-
-            self.align_reference_dataset.blockSignals(True)
-            self.align_reference_dataset.clear()
-            self.align_reference_dataset.addItems(dataset_names)
-            self.align_reference_dataset.blockSignals(False)
-
-            self.colo_dataset.blockSignals(True)
-            self.colo_dataset.clear()
-            self.colo_dataset.addItems(dataset_names)
-            self.colo_dataset.blockSignals(False)
-
-            self.pixseq_append_dataset.blockSignals(True)
-            self.pixseq_append_dataset.clear()
-            self.pixseq_append_dataset.addItems(dataset_names)
-            self.pixseq_append_dataset.blockSignals(False)
-
-            self.delete_dataset_name.blockSignals(True)
-            self.delete_dataset_name.clear()
-            self.delete_dataset_name.addItems(dataset_names)
-            self.delete_dataset_name.blockSignals(False)
-
-            self.update_labels_dataset.blockSignals(True)
-            self.update_labels_dataset.clear()
-            self.update_labels_dataset.addItems(dataset_names)
-            self.update_labels_dataset.blockSignals(False)
-
-            self.import_picasso_dataset.blockSignals(True)
-            self.import_picasso_dataset.clear()
-            self.import_picasso_dataset.addItems(dataset_names)
-            self.import_picasso_dataset.blockSignals(False)
+            self.gui.pixseq_dataset_selector.blockSignals(True)
+            self.gui.pixseq_dataset_selector.clear()
+            self.gui.pixseq_dataset_selector.addItems(dataset_names)
+            self.gui.pixseq_dataset_selector.blockSignals(False)
+
+            self.gui.cluster_dataset.blockSignals(True)
+            self.gui.cluster_dataset.clear()
+            self.gui.cluster_dataset.addItems(dataset_names)
+            self.gui.cluster_dataset.blockSignals(False)
+
+            self.gui.tform_compute_dataset.blockSignals(True)
+            self.gui.tform_compute_dataset.clear()
+            self.gui.tform_compute_dataset.addItems(dataset_names)
+            self.gui.tform_compute_dataset.blockSignals(False)
+
+            self.gui.pixseq_old_dataset_name.blockSignals(True)
+            self.gui.pixseq_old_dataset_name.clear()
+            self.gui.pixseq_old_dataset_name.addItems(dataset_names)
+            self.gui.pixseq_old_dataset_name.blockSignals(False)
+
+            self.gui.align_reference_dataset.blockSignals(True)
+            self.gui.align_reference_dataset.clear()
+            self.gui.align_reference_dataset.addItems(dataset_names)
+            self.gui.align_reference_dataset.blockSignals(False)
+
+            self.gui.colo_dataset.blockSignals(True)
+            self.gui.colo_dataset.clear()
+            self.gui.colo_dataset.addItems(dataset_names)
+            self.gui.colo_dataset.blockSignals(False)
+
+            self.gui.pixseq_append_dataset.blockSignals(True)
+            self.gui.pixseq_append_dataset.clear()
+            self.gui.pixseq_append_dataset.addItems(dataset_names)
+            self.gui.pixseq_append_dataset.blockSignals(False)
+
+            self.gui.delete_dataset_name.blockSignals(True)
+            self.gui.delete_dataset_name.clear()
+            self.gui.delete_dataset_name.addItems(dataset_names)
+            self.gui.delete_dataset_name.blockSignals(False)
+
+            self.gui.update_labels_dataset.blockSignals(True)
+            self.gui.update_labels_dataset.clear()
+            self.gui.update_labels_dataset.addItems(dataset_names)
+            self.gui.update_labels_dataset.blockSignals(False)
+
+            self.gui.import_picasso_dataset.blockSignals(True)
+            self.gui.import_picasso_dataset.clear()
+            self.gui.import_picasso_dataset.addItems(dataset_names)
+            self.gui.import_picasso_dataset.blockSignals(False)
+
+            self.gui.picasso_filter_dataset.blockSignals(True)
+            self.gui.picasso_filter_dataset.clear()
+            self.gui.picasso_filter_dataset.addItems(dataset_names)
+            self.gui.picasso_filter_dataset.blockSignals(False)
+
+            self.gui.tracking_dataset.blockSignals(True)
+            self.gui.tracking_dataset.clear()
+            self.gui.tracking_dataset.addItems(dataset_names)
+            self.gui.tracking_dataset.blockSignals(False)
+
+            self.gui.cellpose_dataset.blockSignals(True)
+            self.gui.cellpose_dataset.clear()
+            self.gui.cellpose_dataset.addItems(dataset_names)
+            self.gui.cellpose_dataset.blockSignals(False)
 
             if len(dataset_names) > 1:
                 dataset_names.insert(0, "All Datasets")
 
-            self.traces_export_dataset.blockSignals(True)
-            self.traces_export_dataset.clear()
-            self.traces_export_dataset.addItems(dataset_names)
-            self.traces_export_dataset.blockSignals(False)
-
-            self.filtering_datasets.blockSignals(True)
-            self.filtering_datasets.clear()
-            self.filtering_datasets.addItems(dataset_names)
-            self.filtering_datasets.blockSignals(False)
-
-            self.picasso_dataset.blockSignals(True)
-            self.picasso_dataset.clear()
-            self.picasso_dataset.addItems(dataset_names)
-            self.picasso_dataset.blockSignals(False)
-
-            self.undrift_dataset_selector.blockSignals(True)
-            self.undrift_dataset_selector.clear()
-            self.undrift_dataset_selector.addItems(dataset_names)
-            self.undrift_dataset_selector.blockSignals(False)
-
-            self.export_dataset.blockSignals(True)
-            self.export_dataset.clear()
-            self.export_dataset.addItems(dataset_names)
-            self.export_dataset.blockSignals(False)
-
-            self.locs_export_dataset.blockSignals(True)
-            self.locs_export_dataset.clear()
-            self.locs_export_dataset.addItems(dataset_names)
-            self.locs_export_dataset.blockSignals(False)
+            self.gui.traces_export_dataset.blockSignals(True)
+            self.gui.traces_export_dataset.clear()
+            self.gui.traces_export_dataset.addItems(dataset_names)
+            self.gui.traces_export_dataset.blockSignals(False)
+
+            self.gui.filtering_datasets.blockSignals(True)
+            self.gui.filtering_datasets.clear()
+            self.gui.filtering_datasets.addItems(dataset_names)
+            self.gui.filtering_datasets.blockSignals(False)
+
+            self.gui.picasso_dataset.blockSignals(True)
+            self.gui.picasso_dataset.clear()
+            self.gui.picasso_dataset.addItems(dataset_names)
+            self.gui.picasso_dataset.blockSignals(False)
+
+            self.gui.undrift_dataset_selector.blockSignals(True)
+            self.gui.undrift_dataset_selector.clear()
+            self.gui.undrift_dataset_selector.addItems(dataset_names)
+            self.gui.undrift_dataset_selector.blockSignals(False)
+
+            self.gui.export_dataset.blockSignals(True)
+            self.gui.export_dataset.clear()
+            self.gui.export_dataset.addItems(dataset_names)
+            self.gui.export_dataset.blockSignals(False)
+
+            self.gui.locs_export_dataset.blockSignals(True)
+            self.gui.locs_export_dataset.clear()
+            self.gui.locs_export_dataset.addItems(dataset_names)
+            self.gui.locs_export_dataset.blockSignals(False)
+
+            self.gui.simple_plot_dataset.blockSignals(True)
+            self.gui.simple_plot_dataset.clear()
+            self.gui.simple_plot_dataset.addItems(dataset_names)
+            self.gui.simple_plot_dataset.blockSignals(False)
+
+            self.gui.picasso_render_dataset.blockSignals(True)
+            self.gui.picasso_render_dataset.clear()
+            self.gui.picasso_render_dataset.addItems(dataset_names)
+            self.gui.picasso_render_dataset.blockSignals(False)
 
         except:
             print(traceback.format_exc())
 
     def initialise_localisation_dict(self):
 
         if hasattr(self, "localisation_dict"):
-            self.localisation_dict = {"bounding_boxes": {}, "fiducials": {}}
+            self.localisation_dict = {"bounding_boxes": {}, "localisations": {}}
 
         if hasattr(self, "dataset_dict"):
 
             if self.verbose:
                 print("Initialising localisation dict.")
 
             for dataset_name, dataset_dict in self.dataset_dict.items():
 
                 if dataset_name not in self.localisation_dict.keys():
-                    self.localisation_dict["fiducials"][dataset_name] = {}
+                    self.localisation_dict["localisations"][dataset_name] = {}
 
-                fiducial_dict = self.localisation_dict["fiducials"][dataset_name]
+                fiducial_dict = self.localisation_dict["localisations"][dataset_name]
 
                 for channel_name, channel_dict in dataset_dict.items():
                     if channel_name not in fiducial_dict.keys():
                         fiducial_dict[channel_name.lower()] = {}
 
-                self.localisation_dict["fiducials"][dataset_name] = fiducial_dict
+                self.localisation_dict["localisations"][dataset_name] = fiducial_dict
 
     def _pixseq_import_data_finished(self):
 
         if self.verbose:
             print("Finished importing data, executing post import functions")
 
         self.initialise_localisation_dict()
@@ -624,32 +773,32 @@
 
         self.update_ui()
 
     def pixseq_import_data(self):
 
         try:
 
-            append_dataset = self.pixseq_append_dataset.currentText()
+            append_dataset = self.gui.pixseq_append_dataset.currentText()
 
-            if self.pixseq_append.isChecked() and append_dataset not in self.dataset_dict.keys():
+            if self.gui.pixseq_append.isChecked() and append_dataset not in self.dataset_dict.keys():
                 print("Please select a dataset to append to")
             else:
 
                 desktop = os.path.expanduser("~/Desktop")
-                paths = QFileDialog.getOpenFileNames(self, 'Open file', desktop, "Image files (*.tif *.tiff)")[0]
+                paths = QFileDialog.getOpenFileNames(self, 'Open file', desktop, "Image files (*.tif *.fits)")[0]
 
                 paths = [path for path in paths if path != ""]
 
                 if paths != []:
 
                     self.update_ui(init=True)
 
                     self.worker = Worker(self._pixseq_import_data, paths=paths)
                     self.worker.signals.progress.connect(partial(self.pixseq_progress,
-                        progress_bar=self.pixseq_import_progressbar))
+                        progress_bar=self.gui.pixseq_import_progressbar))
                     self.worker.signals.finished.connect(self._pixseq_import_data_finished)
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
             pass
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_loc_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_loc_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import yaml
 import tempfile
 import shutil
 from pathlib import Path
 import traceback
 import numpy as np
 from qtpy.QtWidgets import QFileDialog
+import pandas as pd
 
 class picasso_loc_utils():
 
     def __init__(self, locs: np.recarray = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.locs = locs
@@ -123,16 +124,14 @@
                     self.locs = np.delete(self.locs, loc_index, axis=0)
                     self.locs = self.locs.view(self.dtype)
                     self.locs = np.squeeze(self.locs, axis=1)
 
                 self.remove_duplicate_locs()
 
         except:
-            print(loc_index)
-            print(self.locs, self.locs.dtype)
             print(traceback.format_exc())
             pass
 
         return self.locs
 
     def create_locs(self, new_loc, fitted = False):
 
@@ -168,14 +167,69 @@
 
     if os.name == "nt":
         if path.startswith("\\\\"):
             path = '\\\\?\\UNC\\' + path[2:]
 
     return Path(path)
 
+
+def initialise_localisation_export(loc_data):
+
+    try:
+
+        export_mode = loc_data["export_mode"]
+
+        if export_mode == "Picasso HDF5":
+            export_picasso_localisation(loc_data)
+        else:
+            export_localisation_data(loc_data)
+
+    except:
+        print(traceback.format_exc())
+        pass
+
+
+def export_localisation_data(loc_data):
+
+    try:
+
+        export_mode = loc_data["export_mode"]
+        export_path = loc_data["export_path"]
+        locs = loc_data["locs"]
+
+        if export_mode == "CSV":
+
+            df = pd.DataFrame(locs)
+
+            df.to_csv(export_path, index=False)
+
+        elif export_mode == "POS.OUT":
+
+            localisation_data = pd.DataFrame(locs)
+
+            pos_locs = localisation_data[["frame", "x", "y", "photons", "bg", "sx", "sy", ]].copy()
+
+            pos_locs.dropna(axis=0, inplace=True)
+
+            pos_locs.columns = ["FRAME", "XCENTER", "YCENTER", "BRIGHTNESS", "BG", "S_X", "S_Y", ]
+
+            pos_locs.loc[:, "I0"] = 0
+            pos_locs.loc[:, "THETA"] = 0
+            pos_locs.loc[:, "ECC"] = (pos_locs["S_X"] / pos_locs["S_Y"])
+            pos_locs.loc[:, "FRAME"] = pos_locs["FRAME"] + 1
+
+            pos_locs = pos_locs[["FRAME", "XCENTER", "YCENTER", "BRIGHTNESS", "BG", "I0", "S_X", "S_Y", "THETA", "ECC", ]]
+
+            pos_locs.to_csv(export_path, sep="\t", index=False)
+
+    except:
+        print(traceback.format_exc())
+
+
+
 def export_picasso_localisation(loc_data):
 
     try:
         locs = loc_data["locs"]
         h5py_path = loc_data["hdf5_path"]
         yaml_path = loc_data["info_path"]
         info = loc_data["picasso_info"]
@@ -220,35 +274,35 @@
 
 
     def _import_picasso_localisations_finished(self):
 
         try:
             self.update_ui()
 
-            self.draw_fiducials(update_vis=True)
+            self.draw_localisations(update_vis=True)
             self.draw_bounding_boxes(update_vis=True)
 
         except:
             print(traceback.format_exc())
             pass
 
 
     def _import_picasso_localisations(self, progress_callback = None, path=""):
 
         try:
 
-            dataset = self.import_picasso_dataset.currentText()
-            channel = self.import_picasso_channel.currentText()
-            type = self.import_picasso_type.currentText()
-
-            if type == "Fiducials":
-                if dataset not in self.localisation_dict["fiducials"].keys():
-                    self.localisation_dict["fiducials"][dataset] = {}
-                if channel.lower() not in self.localisation_dict["fiducials"][dataset].keys():
-                    self.localisation_dict["fiducials"][dataset][channel.lower()] = {}
+            dataset = self.gui.import_picasso_dataset.currentText()
+            channel = self.gui.import_picasso_channel.currentText()
+            type = self.gui.import_picasso_type.currentText()
+
+            if type == "Localisations":
+                if dataset not in self.localisation_dict["localisations"].keys():
+                    self.localisation_dict["localisations"][dataset] = {}
+                if channel.lower() not in self.localisation_dict["localisations"][dataset].keys():
+                    self.localisation_dict["localisations"][dataset][channel.lower()] = {}
 
             yaml_path = path.replace(".hdf5", ".yaml")
 
             dtype = [('frame', '<u4'), ('x', '<f4'), ('y', '<f4'),
                      ('photons', '<f4'), ('sx', '<f4'), ('sy', '<f4'),
                      ('bg', '<f4'), ('lpx', '<f4'), ('lpy', '<f4'),
                      ('ellipticity', '<f4'),('net_gradient', '<f4')]
@@ -257,47 +311,47 @@
                 print("Loading localisations from hdf5")
 
             with h5py.File(path, "r") as f:
                 locs = np.array(f["locs"], dtype=dtype).view(np.recarray)
                 # print(locs.dtype.descr)
                 # print(len(locs[0]))
 
-            box_size = self.picasso_box_size.currentText()
+            box_size = self.gui.picasso_box_size.currentText()
 
 
             if self.verbose:
                 print("Loading localisations from yaml")
 
             if os.path.exists(yaml_path):
                 with open(yaml_path, "r") as info_file:
                     info = list(yaml.load_all(info_file, Loader=yaml.UnsafeLoader))
 
                 if "Box Size" in info[1].keys():
                     box_size = info[1]["Box Size"]
 
-            if type == "Fiducials":
+            if type == "Localisations":
 
                 if self.verbose:
                     print("Creating render locs")
 
                 render_locs = {}
                 for frame in np.unique(locs.frame):
                     frame_locs = locs[locs.frame == frame].copy()
                     render_locs[frame] = np.vstack((frame_locs.y, frame_locs.x)).T.tolist()
 
                 loc_centres = self.get_localisation_centres(locs)
 
                 if self.verbose:
                     print("Updating localisation dict")
 
-                self.localisation_dict["fiducials"][dataset][channel.lower()]["localisations"] = locs.copy()
-                self.localisation_dict["fiducials"][dataset][channel.lower()]["localisation_centres"] = loc_centres.copy()
-                self.localisation_dict["fiducials"][dataset][channel.lower()]["render_locs"] = render_locs
-                self.localisation_dict["fiducials"][dataset][channel.lower()]["fitted"] = True
-                self.localisation_dict["fiducials"][dataset][channel.lower()]["box_size"] = box_size
+                self.localisation_dict["localisations"][dataset][channel.lower()]["localisations"] = locs.copy()
+                self.localisation_dict["localisations"][dataset][channel.lower()]["localisation_centres"] = loc_centres.copy()
+                self.localisation_dict["localisations"][dataset][channel.lower()]["render_locs"] = render_locs
+                self.localisation_dict["localisations"][dataset][channel.lower()]["fitted"] = True
+                self.localisation_dict["localisations"][dataset][channel.lower()]["box_size"] = box_size
 
             else:
                 unique_frames = np.unique(locs.frame)
                 locs = locs[locs.frame == unique_frames[0]]
 
                 loc_centres = self.get_localisation_centres(locs)
 
@@ -315,17 +369,17 @@
             pass
 
 
     def import_picaaso_localisations(self):
 
         try:
 
-            dataset = self.import_picasso_dataset.currentText()
-            channel = self.import_picasso_channel.currentText()
-            type = self.import_picasso_type.currentText()
+            dataset = self.gui.import_picasso_dataset.currentText()
+            channel = self.gui.import_picasso_channel.currentText()
+            type = self.gui.import_picasso_type.currentText()
 
             if dataset in self.dataset_dict.keys():
                 if channel.lower() in self.dataset_dict[dataset].keys():
 
                     dataset_path = self.dataset_dict[dataset][channel.lower()]["path"]
 
                     dataset_dir = os.path.dirname(dataset_path)
@@ -351,88 +405,90 @@
             print(traceback.format_exc())
             pass
 
     def update_loc_export_options(self):
 
         try:
 
-            dataset_name  = self.locs_export_dataset.currentText()
+            dataset_name  = self.gui.locs_export_dataset.currentText()
 
             if dataset_name in self.dataset_dict.keys() or dataset_name == "All Datasets":
 
                 if dataset_name == "All Datasets":
                     channel_names = ["All Channels"]
                 else:
                     channel_names = list(self.dataset_dict[dataset_name].keys())
                     channel_names = [name for name in channel_names if "efficiency" not in name.lower()]
 
                     for channel_index, channel_name in enumerate(channel_names):
-                        if channel_name in ["donor", "acceptor"]:
+                        if channel_name in ["donor", "acceptor","data"]:
                             channel_names[channel_index] = channel_name.capitalize()
                         else:
                             channel_names[channel_index] = channel_name.upper()
 
                     channel_names.insert(0, "All Channels")
 
-                self.locs_export_channel.blockSignals(True)
-                self.locs_export_channel.clear()
-                self.locs_export_channel.addItems(channel_names)
-                self.locs_export_channel.blockSignals(False)
+                self.gui.locs_export_channel.blockSignals(True)
+                self.gui.locs_export_channel.clear()
+                self.gui.locs_export_channel.addItems(channel_names)
+                self.gui.locs_export_channel.blockSignals(False)
 
         except:
             print(traceback.format_exc())
             pass
 
 
     def export_locs(self, progress_callback = None, export_dataset = "", export_channel = ""):
 
         try:
 
-            export_loc_mode = self.locs_export_mode.currentText()
+            export_loc_type = self.gui.locs_export_type.currentText()
+            export_loc_mode = self.gui.locs_export_mode.currentText()
+
             export_loc_jobs = []
 
             if export_dataset == "All Datasets":
                 dataset_list = list(self.dataset_dict.keys())
             else:
                 dataset_list = [export_dataset]
 
-            if export_loc_mode == "Fiducials":
-                loc_type_list = ["Fiducials"]
-            elif export_loc_mode == "Bounding Boxes":
+            if export_loc_type == "Localisations":
+                loc_type_list = ["Localisations"]
+            elif export_loc_type == "Bounding Boxes":
                 loc_type_list = ["Bounding Boxes"]
             else:
-                loc_type_list = ["Fiducials", "Bounding Boxes"]
+                loc_type_list = ["Localisations", "Bounding Boxes"]
 
             for dataset_name in dataset_list:
 
                 if export_channel == "All Channels":
                     channel_list = list(self.dataset_dict[dataset_name].keys())
                 else:
                     channel_list = [export_channel]
 
                 channel_list = [channel.lower() for channel in channel_list if "efficiency" not in channel.lower()]
 
                 for channel_name in channel_list:
 
                     for loc_type in loc_type_list:
 
-                        if loc_type == "Fiducials":
-                            loc_dict, n_locs, fitted = self.get_loc_dict(dataset_name, channel_name, type="fiducials")
+                        if loc_type == "Localisations":
+                            loc_dict, n_locs, fitted = self.get_loc_dict(dataset_name, channel_name, type="localisations")
                         elif loc_type == "Bounding Boxes":
                             loc_dict, n_locs, fitted = self.get_loc_dict(dataset_name, channel_name, type="bounding_boxes")
 
                         if n_locs > 0 and fitted == True:
 
                             locs = loc_dict["localisations"]
                             box_size = loc_dict["box_size"]
 
                             if "min_net_gradient" in loc_dict.keys():
                                 min_net_gradient = loc_dict["min_net_gradient"]
                             else:
-                                min_net_gradient = int(self.picasso_min_net_gradient.text())
+                                min_net_gradient = int(self.gui.picasso_min_net_gradient.text())
 
                             if channel_name in self.dataset_dict[dataset_name].keys():
 
                                 import_path = self.dataset_dict[dataset_name][channel_name]["path"]
                                 image_shape = self.dataset_dict[dataset_name][channel_name]["data"].shape
 
                                 base, ext = os.path.splitext(import_path)
@@ -441,55 +497,72 @@
                                     export_channel_name = channel_name.capitalize()
                                 else:
                                     export_channel_name = channel_name.upper()
 
                                 if loc_type == "Bounding Boxes":
                                     hdf5_path = base + f"_picasso_bboxes.hdf5"
                                     info_path = base + f"_picasso_bboxes.yaml"
+
+                                    if export_loc_mode == "CSV":
+                                        export_path = base + f"_picasso_bboxes.csv"
+                                    elif export_loc_mode == "POS.OUT":
+                                        export_path = base + f"_picasso_bboxes.pos.out"
+                                    else:
+                                        export_path = ""
+
                                 else:
-                                    hdf5_path = base + f"_picasso_{export_channel_name}_fiducials.hdf5"
-                                    info_path = base + f"_picasso_{export_channel_name}_fiducials.yaml"
+                                    hdf5_path = base + f"_picasso_{export_channel_name}_localisations.hdf5"
+                                    info_path = base + f"_picasso_{export_channel_name}_localisations.yaml"
+
+                                    if export_loc_mode == "CSV":
+                                        export_path = base + f"_picasso_{export_channel_name}_localisations.csv"
+                                    elif export_loc_mode == "POS.OUT":
+                                        export_path = base + f"_picasso_{export_channel_name}_localisations.pos.out"
+
+                                    else:
+                                        export_path = ""
 
                                 picasso_info = [{"Byte Order": "<", "Data Type": "uint16", "File": import_path,
                                                  "Frames": image_shape[0], "Height": image_shape[1],
                                                  "Micro-Manager Acquisiton Comments": "", "Width":image_shape[2],},
                                                 {"Box Size": box_size, "Fit method": "LQ, Gaussian", "Generated by": "Picasso Localize",
                                                  "Min. Net Gradient": min_net_gradient, "Pixelsize": 130, "ROI": None, }]
 
                                 export_loc_job = { "dataset_name": dataset_name,
                                                    "channel_name": channel_name,
                                                    "loc_type": loc_type,
                                                    "locs": locs,
                                                    "fitted": fitted,
+                                                   "export_mode": export_loc_mode,
                                                    "hdf5_path": hdf5_path,
                                                    "info_path": info_path,
+                                                   "export_path": export_path,
                                                    "picasso_info": picasso_info,
                                                   }
+
                             export_loc_jobs.append(export_loc_job)
 
             if len(export_loc_jobs) > 0:
 
                 with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
-                    futures = [executor.submit(export_picasso_localisation, job) for job in export_loc_jobs]
+                    futures = [executor.submit(initialise_localisation_export, job) for job in export_loc_jobs]
 
                     for future in concurrent.futures.as_completed(futures):
                         try:
                             future.result()
                         except:
                             print(traceback.format_exc())
                             pass
 
                         progress = int(100 * (len(export_loc_jobs) - len(futures)) / len(export_loc_jobs))
 
                         if progress_callback is not None:
                             progress_callback.emit(progress)
 
 
-
-
         except:
             self.update_ui()
             print(traceback.format_exc())
             pass
 
 
     def export_locs_finished(self):
@@ -505,46 +578,46 @@
             pass
 
     def initialise_export_locs(self, event=None, export_dataset = "", export_channel = ""):
 
         try:
 
             if export_dataset == "" or export_dataset not in self.dataset_dict.keys():
-                export_dataset = self.locs_export_dataset.currentText()
+                export_dataset = self.gui.locs_export_dataset.currentText()
             if export_channel == "":
-                export_channel = self.locs_export_channel.currentText()
+                export_channel = self.gui.locs_export_channel.currentText()
 
             self.update_ui(init = True)
 
             self.worker = Worker(self.export_locs, export_dataset = export_dataset, export_channel = export_channel)
-            self.worker.signals.progress.connect(partial(self.pixseq_progress,progress_bar=self.export_progressbar))
+            self.worker.signals.progress.connect(partial(self.pixseq_progress,progress_bar=self.gui.export_progressbar))
             self.worker.signals.finished.connect(self.export_locs_finished)
             self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
             pass
 
-    def get_loc_dict(self, dataset_name="", channel_name="", type = "fiducials"):
+    def get_loc_dict(self, dataset_name="", channel_name="", type = "localisations"):
 
         loc_dict = {}
         n_localisations = 0
         fitted = False
 
         try:
 
-            if type.lower() == "fiducials":
+            if type.lower() == "localisations":
 
-                if dataset_name not in self.localisation_dict["fiducials"].keys():
-                    self.localisation_dict["fiducials"][dataset_name] = {}
+                if dataset_name not in self.localisation_dict["localisations"].keys():
+                    self.localisation_dict["localisations"][dataset_name] = {}
                 else:
-                    if channel_name not in self.localisation_dict["fiducials"][dataset_name].keys():
-                        self.localisation_dict["fiducials"][dataset_name][channel_name] = {}
+                    if channel_name not in self.localisation_dict["localisations"][dataset_name].keys():
+                        self.localisation_dict["localisations"][dataset_name][channel_name] = {}
                     else:
-                        loc_dict = self.localisation_dict["fiducials"][dataset_name][channel_name].copy()
+                        loc_dict = self.localisation_dict["localisations"][dataset_name][channel_name].copy()
 
             else:
 
                 if "bounding_boxes" not in self.localisation_dict.keys():
                     self.localisation_dict["bounding_boxes"] = {}
 
                 loc_dict = self.localisation_dict["bounding_boxes"].copy()
@@ -558,20 +631,20 @@
         except:
             print(traceback.format_exc())
             pass
 
         return loc_dict, n_localisations, fitted
 
 
-    def update_loc_dict(self, dataset_name="", channel_name="", type = "fiducials", loc_dict = {}):
+    def update_loc_dict(self, dataset_name="", channel_name="", type = "localisations", loc_dict = {}):
 
         try:
 
-            if type == "fiducials":
-                self.localisation_dict["fiducials"][dataset_name][channel_name] = loc_dict
+            if type == "localisations":
+                self.localisation_dict["localisations"][dataset_name][channel_name] = loc_dict
             else:
                 self.localisation_dict["bounding_boxes"] = loc_dict
 
         except:
             print(traceback.format_exc())
             pass
 
@@ -586,20 +659,20 @@
 
     def compute_net_gradient(self, position, box_size = None):
 
         net_gradient = 0
 
         try:
 
-            dataset = self.pixseq_dataset_selector.currentText()
+            dataset = self.gui.pixseq_dataset_selector.currentText()
             channel = self.active_channel
             frame = self.viewer.dims.current_step[0]
 
             if box_size is None:
-                box_size = self.picasso_box_size.currentText()
+                box_size = self.gui.picasso_box_size.currentText()
 
             loc_mask, _, loc_bg_mask = self.generate_localisation_mask(
                 box_size, spot_shape = "square")
 
             box_size = len(loc_mask[0])
 
             x, y = position[0], position[1]
@@ -635,24 +708,24 @@
 
 
 
     def add_manual_localisation(self, position, mode):
 
         try:
 
-            active_dataset = self.pixseq_dataset_selector.currentText()
+            active_dataset = self.gui.pixseq_dataset_selector.currentText()
             active_channel = self.active_channel
-            box_size = int(self.picasso_box_size.currentText())
+            box_size = int(self.gui.picasso_box_size.currentText())
             frame = self.viewer.dims.current_step[0]
             net_gradient = self.compute_net_gradient(position, box_size=box_size)
 
-            if mode == "fiducials":
+            if mode == "localisations":
 
                 loc_dict, n_locs, _ = self.get_loc_dict(active_dataset, active_channel,
-                    type = "fiducials")
+                    type = "localisations")
 
 
                 if n_locs > 0:
                     locs = loc_dict["localisations"].copy()
                     render_locs = loc_dict["render_locs"].copy()
                     loc_centers = loc_dict["localisation_centres"].copy()
                     box_size = int(loc_dict["box_size"])
@@ -689,16 +762,16 @@
                             render_frame_locs.pop(min_index)
                             render_locs[frame] = render_frame_locs
 
                             loc_dict["localisations"] = locs
                             loc_dict["localisation_centres"] = loc_centers
                             loc_dict["render_locs"] = render_locs
 
-                            self.update_loc_dict(active_dataset, active_channel, "fiducials", loc_dict)
-                            self.draw_fiducials(update_vis=True)
+                            self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
+                            self.draw_localisations(update_vis=True)
 
                         else:
 
                             locs = loc_utils.add_loc(new_loc = [frame, x, y, net_gradient])
 
                             loc_centers = np.append(loc_centers, np.array([[frame,y,x]], dtype=int), axis=0)
                             loc_centers = loc_centers.tolist()
@@ -708,16 +781,16 @@
                             else:
                                 render_locs[frame].append([round(y),round(x)])
 
                             loc_dict["localisations"] = locs
                             loc_dict["localisation_centres"] = loc_centers
                             loc_dict["render_locs"] = render_locs
 
-                            self.update_loc_dict(active_dataset, active_channel, "fiducials", loc_dict)
-                            self.draw_fiducials(update_vis=True)
+                            self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
+                            self.draw_localisations(update_vis=True)
 
                     else:
 
                         locs = loc_utils.add_loc(new_loc=[frame, x, y, net_gradient])
 
                         loc_centers = np.append(loc_centers, np.array([[frame, y, x]], dtype=int), axis=0)
                         loc_centers = loc_centers.tolist()
@@ -730,21 +803,21 @@
                         else:
                             render_locs[frame] = [[round(y), round(x)]]
 
                         loc_dict["localisations"] = locs
                         loc_dict["localisation_centres"] = loc_centers
                         loc_dict["render_locs"] = render_locs
 
-                        self.update_loc_dict(active_dataset, active_channel, "fiducials", loc_dict)
-                        self.draw_fiducials(update_vis=True)
+                        self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
+                        self.draw_localisations(update_vis=True)
 
                 else:
                     x, y = position
 
-                    box_size = int(self.picasso_box_size.currentText())
+                    box_size = int(self.gui.picasso_box_size.currentText())
 
                     new_loc = [frame, position[0], position[1], net_gradient]
 
                     loc_utils = picasso_loc_utils()
                     locs = loc_utils.create_locs(new_loc=new_loc)
 
                     loc_centers = [[frame, y, x]]
@@ -752,16 +825,16 @@
 
                     loc_dict["localisations"] = locs
                     loc_dict["localisation_centres"] = loc_centers
                     loc_dict["render_locs"] = render_locs
                     loc_dict["fitted"] = False
                     loc_dict["box_size"] = box_size
 
-                    self.update_loc_dict(active_dataset, active_channel, "fiducials", loc_dict)
-                    self.draw_fiducials(update_vis=True)
+                    self.update_loc_dict(active_dataset, active_channel, "localisations", loc_dict)
+                    self.draw_localisations(update_vis=True)
 
             elif mode == "bounding_box":
 
                 loc_dict, n_locs,_ = self.get_loc_dict(active_dataset, active_channel,
                     type = "bounding_box")
 
                 if n_locs > 0:
@@ -822,15 +895,15 @@
                         self.update_loc_dict(active_dataset, active_channel, "bounding_boxes", loc_dict)
                         self.draw_bounding_boxes()
 
                 else:
 
                     x, y = position
 
-                    box_size = int(self.picasso_box_size.currentText())
+                    box_size = int(self.gui.picasso_box_size.currentText())
 
                     new_loc = [frame, position[0], position[1], net_gradient]
 
                     loc_utils = picasso_loc_utils()
                     locs = loc_utils.create_locs(new_loc=new_loc)
 
                     loc_centers = [[y, x]]
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_picasso_detect.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_picasso_detect.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import numpy as np
 import traceback
+
+import pandas as pd
+
 from napari_pixseq.funcs.pixseq_utils_compute import Worker
 import time
 import os
 from multiprocessing import shared_memory
 from picasso import localize
 from picasso.localize import get_spots, identify_frame
 from picasso.gaussmle import gaussmle
 from functools import partial
 import concurrent.futures
 import multiprocessing
-
+from picasso.render import render
+from shapely.geometry import Point, Polygon
+from multiprocessing import Manager
 
 def remove_overlapping_locs(locs, box_size):
 
     try:
 
         coordinates = np.vstack((locs.y, locs.x)).T
 
@@ -52,15 +57,15 @@
     spots = np.zeros((n_spots, box, box), dtype=movie.dtype)
     for id, (frame, xc, yc) in enumerate(zip(ids_frame, ids_x, ids_y)):
         spots[id] = movie[frame, yc - r : yc + r + 1, xc - r : xc + r + 1]
 
     return spots
 
 
-def picasso_detect(dat):
+def picasso_detect(dat, progress_list):
 
     result = None
 
     try:
 
         frame_index = dat["frame_index"]
         min_net_gradient = dat["min_net_gradient"]
@@ -68,23 +73,24 @@
         roi = dat["roi"]
         dataset = dat["dataset"]
         channel = dat["channel"]
         detect = dat["detect"]
         fit = dat["fit"]
         remove_overlapping = dat["remove_overlapping"]
         stop_event = dat["stop_event"]
+        polygon_filter = dat["polygon_filter"]
+        polygons = dat["polygons"]
 
         if not stop_event.is_set():
 
             # Access the shared memory
             shared_mem = shared_memory.SharedMemory(name=dat["shared_memory_name"])
             np_array = np.ndarray(dat["shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
 
-            # Perform preprocessing steps and overwrite original image
-            frame = np_array[frame_index].copy()
+            frame = np_array.copy()
 
             if detect:
                 locs = identify_frame(frame, min_net_gradient, box_size, 0, roi=roi)
 
                 if remove_overlapping:
                     # overlapping removed prior to fitting to increase speed
                     locs = remove_overlapping_locs(locs, box_size)
@@ -97,18 +103,14 @@
             if fit:
                 expected_loc_length = 12
                 try:
                     image = np.expand_dims(frame, axis=0)
                     camera_info = {"baseline": 100.0, "gain": 1, "sensitivity": 1.0, "qe": 0.9, }
                     spot_data = get_spots(image, locs, box_size, camera_info)
 
-                    # frame = np.expand_dims(frame, axis=0)
-                    # locs.frame = 0
-                    # spot_data = cut_spots(frame, locs.frame, locs.x, locs.y, box_size)
-
                     theta, CRLBs, likelihoods, iterations = gaussmle(spot_data, eps=0.001, max_it=1000, method="sigma")
                     locs = localize.locs_from_fits(locs.copy(), theta, CRLBs, likelihoods, iterations, box_size)
 
                     locs.frame = frame_index
 
                     if remove_overlapping:
                         # sometimes locs can overlap after fitting
@@ -117,140 +119,178 @@
                 except:
                     # print(traceback.format_exc())
                     pass
 
             for loc in locs:
                 loc.frame = frame_index
 
-            render_locs= {}
-            render_locs[frame_index] = np.vstack((locs.y, locs.x)).T.tolist()
+            if polygon_filter:
+
+                if len(polygons) > 0 and len(locs) > 0:
 
-            locs = [loc for loc in locs if len(loc) == expected_loc_length]
-            locs = np.array(locs).view(np.recarray)
+                    expected_loc_length += 1
+
+                    loclist = pd.DataFrame(locs).to_dict(orient="records")
+
+                    filtered_locs = []
+
+                    for loc in loclist:
+                        point = Point(loc["x"], loc["y"])
+
+                        for polygon_index, polygon in enumerate(polygons):
+                            if polygon.contains(point):
+                                loc["segmentation"] = polygon_index
+                                filtered_locs.append(loc)
+
+                    if len(filtered_locs):
+                        locs = pd.DataFrame(filtered_locs).to_records(index=False)
+                    else:
+                        locs = []
+
+                else:
+                    locs = []
+
+            render_locs = {frame_index: []}
+
+            if len(locs) > 0:
+                render_locs[frame_index] = np.vstack((locs.y, locs.x)).T.tolist()
+
+                locs = [loc for loc in locs if len(loc) == expected_loc_length]
+                locs = np.array(locs).view(np.recarray)
 
             result = {"dataset": dataset, "channel": channel, "frame_index": frame_index,
                       "locs": locs,"render_locs": render_locs}
 
     except:
         print(traceback.format_exc())
         pass
 
+    progress_list.append(dat["frame_index"])
+
     return result
 
 
 class _picasso_detect_utils:
 
-
-
-    def populate_localisation_dict(self, loc_dict, render_loc_dict, detect_mode, image_channel, box_size, fitted=False):
+    def populate_localisation_dict(self, loc_dict, render_loc_dict, detect_mode,
+            image_channel, box_size, fitted=False):
 
         if self.verbose:
             print("Populating localisation dictionary...")
 
         detect_mode = detect_mode.lower()
 
         try:
 
             for dataset_name, locs in loc_dict.items():
 
-                render_locs = render_loc_dict[dataset_name]
+                if detect_mode == "localisations":
 
-                if detect_mode == "fiducials":
+                    if dataset_name not in self.localisation_dict["localisations"].keys():
+                        self.localisation_dict["localisations"][dataset_name] = {}
+                    if image_channel not in self.localisation_dict["localisations"][dataset_name].keys():
+                        self.localisation_dict["localisations"][dataset_name][image_channel.lower()] = {}
+
+                    render_locs = render_loc_dict[dataset_name]
 
                     loc_centres = self.get_localisation_centres(locs)
 
                     fiducial_dict = {"localisations": [], "localisation_centres": [], "render_locs": {}}
 
                     fiducial_dict["localisations"] = locs.copy()
                     fiducial_dict["localisation_centres"] = loc_centres.copy()
                     fiducial_dict["render_locs"] = render_locs
 
                     fiducial_dict["fitted"] = fitted
                     fiducial_dict["box_size"] = box_size
 
-                    if dataset_name not in self.localisation_dict["fiducials"].keys():
-                        self.localisation_dict["fiducials"][dataset_name] = {}
-                    if image_channel not in self.localisation_dict["fiducials"][dataset_name].keys():
-                        self.localisation_dict["fiducials"][dataset_name][image_channel.lower()] = {}
-
-                    self.localisation_dict["fiducials"][dataset_name][image_channel.lower()] = fiducial_dict.copy()
+                    self.localisation_dict["localisations"][dataset_name][image_channel.lower()] = fiducial_dict.copy()
 
                 else:
 
                     loc_centres = self.get_localisation_centres(locs)
 
                     self.localisation_dict["bounding_boxes"]["localisations"] = locs.copy()
                     self.localisation_dict["bounding_boxes"]["localisation_centres"] = loc_centres.copy()
                     self.localisation_dict["bounding_boxes"]["fitted"] = fitted
                     self.localisation_dict["bounding_boxes"]["box_size"] = box_size
 
 
         except:
             print(traceback.format_exc())
-            self.picasso_progressbar.setValue(0)
-            self.picasso_detect.setEnabled(True)
-            self.picasso_fit.setEnabled(True)
-            self.picasso_detectfit.setEnabled(True)
+            self.gui.picasso_progressbar.setValue(0)
+            self.gui.picasso_detect.setEnabled(True)
+            self.gui.picasso_fit.setEnabled(True)
+            self.gui.picasso_detectfit.setEnabled(True)
 
     def _picasso_wrapper_result(self, result):
 
         try:
 
             if self.verbose:
                 print("Picasso wrapper result received")
 
             fitted, loc_dict, render_loc_dict, total_locs = result
 
-            detect_mode = self.picasso_detect_mode.currentText()
-            image_channel = self.picasso_channel.currentText()
-            box_size = int(self.picasso_box_size.currentText())
+            detect_mode = self.gui.picasso_detect_mode.currentText()
+            image_channel = self.gui.picasso_channel.currentText()
+            box_size = int(self.gui.picasso_box_size.currentText())
 
             dataset_names = list(loc_dict.keys())
 
             if len(dataset_names) > 0:
 
                 self.populate_localisation_dict(loc_dict, render_loc_dict, detect_mode,
                     image_channel, box_size, fitted)
 
                 if fitted:
-                    print("Fitted {} localisations".format(total_locs))
+                    self.pixseq_notification("Fitted {} {}".format(total_locs, detect_mode))
                 else:
-                    print("Detected {} localisations".format(total_locs))
+                    self.pixseq_notification("Detected {} {}".format(total_locs, detect_mode))
 
         except:
             print(traceback.format_exc())
 
     def _picasso_wrapper_finished(self):
 
         try:
 
-            image_channel = self.picasso_channel.currentText()
-            dataset_name = self.picasso_dataset.currentText()
+            image_channel = self.gui.picasso_channel.currentText()
+            dataset_name = self.gui.picasso_dataset.currentText()
 
             if dataset_name == "All Datasets":
                 dataset_name = self.active_dataset
 
             self.update_active_image(channel=image_channel.lower(), dataset=dataset_name)
 
             self.draw_bounding_boxes()
+            self.draw_localisations()
+
+            self.update_filter_criterion()
+            self.update_criterion_ranges()
 
             self.update_ui()
 
         except:
             print(traceback.format_exc())
 
+
+
+
     def get_frame_locs(self, dataset_name, image_channel, frame_index):
 
         try:
 
             loc_dict, n_locs, _ = self.get_loc_dict(dataset_name,
-                image_channel.lower(), type = "fiducials")
+                image_channel.lower(), type = "localisations")
 
             if "localisations" not in loc_dict.keys():
                 return None
+            elif len(loc_dict["localisations"]) == 0:
+                return None
             else:
                 locs = loc_dict["localisations"]
                 locs = locs[locs.frame == frame_index]
 
                 return locs.copy()
 
         except:
@@ -260,85 +300,107 @@
     def _picasso_wrapper(self, progress_callback, detect, fit, min_net_gradient, image_channel):
 
         loc_dict = {}
         render_loc_dict = {}
         total_locs = 0
         try:
 
-            box_size = int(self.picasso_box_size.currentText())
-            dataset_name = self.picasso_dataset.currentText()
-            frame_mode = self.picasso_frame_mode.currentText()
-            remove_overlapping = self.picasso_remove_overlapping.isChecked()
+            box_size = int(self.gui.picasso_box_size.currentText())
+            dataset_name = self.gui.picasso_dataset.currentText()
+            frame_mode = self.gui.picasso_frame_mode.currentText()
+            remove_overlapping = self.gui.picasso_remove_overlapping.isChecked()
+            polygon_filter = self.gui.picasso_segmentation_filtering.isChecked()
             roi = self.generate_roi()
 
             if dataset_name == "All Datasets":
                 dataset_list = list(self.dataset_dict.keys())
             else:
                 dataset_list = [dataset_name]
 
             channel_list = [image_channel.lower()]
 
-            self.shared_images = self.create_shared_images(dataset_list=dataset_list, channel_list=channel_list)
+            if frame_mode.lower() == "active":
+                frame_index = self.viewer.dims.current_step[0]
+            else:
+                frame_index = None
+
+            self.shared_frames = self.create_shared_frames(
+                dataset_list=dataset_list,
+                channel_list=channel_list,
+                frame_index=frame_index,
+            )
+
+            segmentation_polygons = self.get_segmentation_polygons()
 
             compute_jobs = []
 
             if self.verbose:
                 print("Creating Picasso compute jobs...")
 
             if self.verbose:
-                print("Creating compute jobs for {} datasets...".format(len(self.shared_images)))
-
-            for image_dict in self.shared_images:
+                print(f"Creating compute jobs for {len(self.shared_images)} datasets...")
 
+            for image_dict in self.shared_frames:
                 image_dict = image_dict.copy()
 
                 if frame_mode.lower() == "active":
                     frame_list = [self.viewer.dims.current_step[0]]
                 else:
-                    n_frames = image_dict['shape'][0]
+                    n_frames = image_dict["shape"][0]
                     frame_list = list(range(n_frames))
 
                 for frame_index in frame_list:
 
+                    polygons = []
+                    if type(segmentation_polygons) == dict:
+                        if frame_index in segmentation_polygons.keys():
+                            polygons = segmentation_polygons[frame_index]
+                    if type(segmentation_polygons) == list:
+                        polygons = segmentation_polygons
+
+                    frame_dict = image_dict["frame_dict"][frame_index]
+
                     time_start = time.time()
 
                     if self.verbose:
-                        print("Creating compute job for frame {}".format(frame_index))
+                        print(f"Creating compute job for frame {frame_index}")
 
-                    frame_locs = self.get_frame_locs(image_dict["dataset"],
-                        image_channel, frame_index)
+                    frame_locs = self.get_frame_locs(image_dict["dataset"], image_channel, frame_index)
 
                     if detect == False and frame_locs is None:
                         continue
+                    # elif polygon_filter is True and len(polygons) == 0:
+                    #     continue
                     else:
-                        compute_job = {"dataset": image_dict["dataset"],
-                                       "channel": image_dict["channel"],
+                        compute_job = {"dataset": frame_dict["dataset"],
+                                       "channel": frame_dict["channel"],
                                        "frame_index": frame_index,
-                                       "shared_memory_name": image_dict['shared_memory_name'],
-                                       "shape": image_dict['shape'],
-                                       "dtype": image_dict['dtype'],
+                                       "shared_memory_name": frame_dict["shared_memory_name"],
+                                       "shape": frame_dict["shape"],
+                                       "dtype": frame_dict["dtype"],
                                        "detect": detect,
                                        "fit": fit,
                                        "min_net_gradient": int(min_net_gradient),
                                        "box_size": int(box_size),
                                        "roi": roi,
                                        "frame_locs": frame_locs,
                                        "remove_overlapping": remove_overlapping,
-                                       "stop_event": self.stop_event,
-                                       }
+                                       "polygon_filter":polygon_filter,
+                                       "polygons": polygons,
+                                       "stop_event": self.stop_event, }
 
                     compute_jobs.append(compute_job)
 
                     if self.verbose:
                         time_end = time.time()
                         time_duration = time_end - time_start
-                        print("Compute job created in {} seconds".format(time_duration))
+                        print(f"Compute job created in {time_duration} seconds")
 
-            if len(compute_jobs) > 0:
 
+            if len(compute_jobs) > 0:
                 if self.verbose:
                     print(f"Starting Picasso {len(compute_jobs)} compute jobs...")
 
                 timeout_duration = 10  # Timeout in seconds
 
                 loc_dict = {}
                 render_loc_dict = {}
@@ -346,100 +408,117 @@
                 if frame_mode.lower() == "active":
                     executor_class = concurrent.futures.ThreadPoolExecutor
                     cpu_count = 1
                 else:
                     executor_class = concurrent.futures.ProcessPoolExecutor
                     cpu_count = int(multiprocessing.cpu_count() * 0.9)
 
-                with executor_class(max_workers=cpu_count) as executor:
-                    futures = {executor.submit(picasso_detect, job): job for job in compute_jobs}
+                with Manager() as manager:
+                    progress_list = manager.list()
 
-                iter = 0
-                for future in concurrent.futures.as_completed(futures):
-                    if self.stop_event.is_set():
-                        future.cancel()
-                    else:
-                        job = futures[future]
-                        try:
-                            result = future.result(timeout=timeout_duration)  # Process result here
-
-                            if result is not None:
-                                dataset_name = result["dataset"]
-
-                                if dataset_name not in loc_dict:
-                                    loc_dict[dataset_name] = []
-                                    render_loc_dict[dataset_name] = {}
-
-                                locs = result["locs"]
-                                render_locs = result["render_locs"]
-
-                                loc_dict[dataset_name].extend(locs)
-                                render_loc_dict[dataset_name] = {**render_loc_dict[dataset_name], **render_locs}
-
-                            iter += 1
-                            progress = int((iter / len(compute_jobs)) * 100)
-                            progress_callback.emit(progress)  # Emit the signal
-
-                        except concurrent.futures.TimeoutError:
-                            # print(f"Task {job} timed out after {timeout_duration} seconds.")
-                            pass
-                        except Exception as e:
-                            print(f"Error occurred in task {job}: {e}")  # Handle other exceptions
-                            pass
+                    with executor_class(max_workers=cpu_count) as executor:
+                        futures = {executor.submit(picasso_detect, job, progress_list): job for job in compute_jobs}
+
+                        # Calculate and emit progress
+                        while any(not future.done() for future in futures):
+                            progress = (len(progress_list)/len(compute_jobs)) * 100
+                            if progress_callback is not None:
+                                progress_callback.emit(progress)
+
+                        for future in concurrent.futures.as_completed(futures):
+
+                            if self.stop_event.is_set():
+                                future.cancel()
+                            else:
+                                job = futures[future]
+                                try:
+                                    result = future.result(timeout=timeout_duration)  # Process result here
+
+                                    if result is not None:
+                                        dataset_name = result["dataset"]
+
+                                        if dataset_name not in loc_dict:
+                                            loc_dict[dataset_name] = []
+                                            render_loc_dict[dataset_name] = {}
+
+                                        locs = result["locs"]
+                                        render_locs = result["render_locs"]
+
+                                        if len(locs) > 0:
+                                            loc_dict[dataset_name].extend(locs)
+
+                                        render_loc_dict[dataset_name] = {**render_loc_dict[dataset_name], **render_locs, }
+
+                                except concurrent.futures.TimeoutError:
+                                    # print(f"Task {job} timed out after {timeout_duration} seconds.")
+                                    pass
+                                except Exception as e:
+                                    print(f"Error occurred in task {job}: {e}")  # Handle other exceptions
 
                 if self.verbose:
                     print("Finished Picasso compute jobs...")
                     print("Compiling Picasso results...")
 
                 total_locs = 0
                 for dataset, locs in loc_dict.items():
-                    locs = np.hstack(locs).view(np.recarray).copy()
-                    locs.sort(kind="mergesort", order="frame")
-                    locs = np.array(locs).view(np.recarray)
-                    loc_dict[dataset] = locs
+                    if len(locs) > 0:
+                        locs = np.hstack(locs).view(np.recarray).copy()
+                        locs.sort(kind="mergesort", order="frame")
+                        locs = np.array(locs).view(np.recarray)
+                        loc_dict[dataset] = locs
                     total_locs += len(locs)
 
-            self.restore_shared_images()
+
+            self.restore_shared_frames()
+
             self.update_ui()
 
         except:
             print(traceback.format_exc())
-            self.restore_shared_images()
+
+            self.restore_shared_frames()
 
             self.update_ui()
 
             loc_dict = {}
             render_loc_dict = {}
             total_locs = 0
 
         return fit, loc_dict, render_loc_dict, total_locs
 
     def pixseq_picasso(self, detect = False, fit = False):
 
         try:
             if self.dataset_dict != {}:
 
-                min_net_gradient = self.picasso_min_net_gradient.text()
-                image_channel = self.picasso_channel.currentText()
+                min_net_gradient = self.gui.picasso_min_net_gradient.text()
+                image_channel = self.gui.picasso_channel.currentText()
+                frame_mode = self.gui.picasso_frame_mode.currentText()
+                minimise_ram = self.gui.picasso_minimise_ram.isChecked()
 
                 if min_net_gradient.isdigit() and image_channel != "":
 
-                    self.picasso_progressbar.setValue(0)
-                    self.picasso_detect.setEnabled(False)
-                    self.picasso_fit.setEnabled(False)
-                    self.picasso_detectfit.setEnabled(False)
+                    self.gui.picasso_progressbar.setValue(0)
+                    self.gui.picasso_detect.setEnabled(False)
+                    self.gui.picasso_fit.setEnabled(False)
+                    self.gui.picasso_detectfit.setEnabled(False)
 
                     self.update_ui(init=True)
 
+                    if minimise_ram == True and frame_mode.lower() != "active":
+                        self.clear_live_images()
+
                     self.worker = Worker(self._picasso_wrapper,
                         detect=detect, fit=fit,
                         min_net_gradient=min_net_gradient,
                         image_channel=image_channel,)
 
-                    self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.picasso_progressbar))
+                    self.worker.signals.progress.connect(partial(self.pixseq_progress,
+                        progress_bar=self.gui.picasso_progressbar))
+
                     self.worker.signals.result.connect(self._picasso_wrapper_result)
                     self.worker.signals.finished.connect(self._picasso_wrapper_finished)
                     self.worker.signals.error.connect(self.update_ui)
                     self.threadpool.start(self.worker)
 
 
         except:
@@ -449,25 +528,25 @@
 
 
     def generate_roi(self):
 
         if self.verbose:
             print("Generating ROI")
 
-        border_width = self.picasso_roi_border_width.text()
-        window_cropping = self.picasso_window_cropping.isChecked()
+        border_width = self.gui.picasso_roi_border_width.text()
+        window_cropping = self.gui.picasso_window_cropping .isChecked()
 
         roi = None
 
         try:
 
             generate_roi = False
 
             if window_cropping:
-                layers_names = [layer.name for layer in self.viewer.layers if layer.name not in ["bounding_boxes", "fiducials"]]
+                layers_names = [layer.name for layer in self.viewer.layers if layer.name not in ["bounding_boxes", "localisations"]]
 
                 crop = self.viewer.layers[layers_names[0]].corner_pixels[:, -2:]
                 [[y1, x1], [y2, x2]] = crop
 
                 generate_roi = True
 
             else:
@@ -478,16 +557,16 @@
                         generate_roi = True
                 elif type(border_width) == int:
                     if border_width > 0:
                         generate_roi = True
 
             if generate_roi:
 
-                dataset = self.picasso_dataset.currentText()
-                channel = self.picasso_channel.currentText()
+                dataset = self.gui.picasso_dataset.currentText()
+                channel = self.gui.picasso_channel.currentText()
 
                 if dataset == "All Datasets":
                     dataset = list(self.dataset_dict.keys())[0]
 
                 image_shape = self.dataset_dict[dataset][channel.lower()]["data"].shape
 
                 frame_shape = image_shape[1:]
@@ -521,18 +600,18 @@
     def export_picasso_locs(self, locs):
 
         if self.verbos:
             print("Exporting Picasso locs")
 
         try:
 
-            dataset_name = self.picasso_dataset.currentText()
-            image_channel = self.picasso_channel.currentText()
-            min_net_gradient = int(self.picasso_min_net_gradient.text())
-            box_size = int(self.picasso_box_size.currentText())
+            dataset_name = self.gui.picasso_dataset.currentText()
+            image_channel = self.gui.picasso_channel.currentText()
+            min_net_gradient = int(self.gui.picasso_min_net_gradient.text())
+            box_size = int(self.gui.picasso_box_size.currentText())
 
             path = self.dataset_dict[dataset_name][image_channel.lower()]["path"]
             image_shape = self.dataset_dict[dataset_name][image_channel.lower()]["data"].shape
 
             base, ext = os.path.splitext(path)
             path = base + f"_{image_channel}_picasso_locs.hdf5"
 
@@ -545,7 +624,90 @@
 
             from picasso.io import save_locs
             # save_locs(path, locs, info)
 
         except:
             print(traceback.format_exc())
             pass
+
+    def render_picasso_locs(self, locs, image_shape, blur_method=None, min_blur_width=1,
+            pixel_size=1, progress_callback=None, oversampling=20, ):
+        try:
+            h, w = image_shape[-2:]
+
+            viewport = [(0, 0), (h, w)]
+
+            n_rendered_locs, image = render(locs, viewport=viewport,
+                blur_method=blur_method, min_blur_width=min_blur_width, oversampling=oversampling, )
+
+        except:
+            image = np.zeros(image_shape[-2:], dtype=np.int8)
+
+        return image, pixel_size, oversampling
+
+    def picasso_render_finished(self):
+
+        self.update_filter_criterion()
+        self.update_criterion_ranges()
+
+        self.update_ui(init=False)
+
+
+
+    def draw_picasso_render(self, data):
+
+        try:
+            image, pixel_size, oversampling = data
+
+            scale = [pixel_size / oversampling, pixel_size / oversampling]
+
+            layer_names = [layer.name for layer in self.viewer.layers]
+
+            if "SMLM Render" not in layer_names:
+                self.viewer.add_image(image, name="SMLM Render", colormap="viridis", scale=scale, )
+            else:
+                self.viewer.layers["SMLM Render"].data = image
+                self.viewer.layers["SMLM Render"].scale = scale
+
+        except:
+            print(traceback.format_exc())
+
+    def initialise_picasso_render(self):
+
+        try:
+
+            dataset_name = self.gui.picasso_render_dataset.currentText()
+            image_channel = self.gui.picasso_render_channel.currentText()
+            blur_method = self.gui.picasso_render_blur_method.currentText()
+            min_blur_width = float(self.gui.picasso_render_min_blur.text())
+
+            if (image_channel.lower() in self.localisation_dict["localisations"][dataset_name].keys()):
+                localisation_dict = self.localisation_dict["localisations"][dataset_name][image_channel.lower()].copy()
+
+                if localisation_dict["fitted"] == True:
+                    locs = localisation_dict["localisations"]
+
+                    image_shape = list(self.dataset_dict[dataset_name][image_channel.lower()]["data"].shape)
+                    pixel_size = 1
+
+                    if blur_method == "One-Pixel-Blur":
+                        blur_method = "smooth"
+                    elif blur_method == "Global Localisation Precision":
+                        blur_method = "convolve"
+                    elif (blur_method == "Individual Localisation Precision, iso"):
+                        blur_method = "gaussian_iso"
+                    elif blur_method == "Individual Localisation Precision":
+                        blur_method = "gaussian"
+                    else:
+                        blur_method = None
+
+                    self.update_ui(init=True)
+
+                    worker = Worker(self.render_picasso_locs, locs=locs, image_shape=image_shape,
+                        blur_method=blur_method, min_blur_width=min_blur_width, pixel_size=pixel_size, )
+                    worker.signals.result.connect(self.draw_picasso_render)
+                    worker.signals.finished.connect(self.picasso_render_finished)
+                    self.threadpool.start(worker)
+
+        except:
+            print(traceback.format_exc())
+            self.update_ui()
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_plot_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_plot_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,46 +32,46 @@
 
             if hasattr(self, "traces_dict"):
 
                 if self.traces_dict != {}:
 
                     self.updating_plot_combos = True
 
-                    self.plot_data.blockSignals(True)
-                    self.plot_data.clear()
+                    self.gui.plot_data.blockSignals(True)
+                    self.gui.plot_data.clear()
 
                     dataset_names = list(self.traces_dict.keys())
 
                     if len(dataset_names) > 0:
                         dataset_names.insert(0, "All Datasets")
 
-                    self.plot_data.addItems(dataset_names)
-                    self.plot_data.blockSignals(False)
+                    self.gui.plot_data.addItems(dataset_names)
+                    self.gui.plot_data.blockSignals(False)
 
                     self.updating_plot_combos = False
 
         except:
             print(traceback.format_exc())
 
     def update_plot_channel_combo(self):
 
         try:
 
             if hasattr(self, "traces_dict"):
 
                 if self.traces_dict != {}:
 
-                    dataset_name = self.plot_data.currentText()
+                    dataset_name = self.gui.plot_data.currentText()
 
                     if dataset_name != "":
 
                         self.updating_plot_combos = True
 
-                        self.plot_channel.blockSignals(True)
-                        self.plot_channel.clear()
+                        self.gui.plot_channel.blockSignals(True)
+                        self.gui.plot_channel.clear()
 
                         if dataset_name == "All Datasets":
                             channel_names = []
                             for dataset in self.traces_dict.keys():
                                 channel_names.extend(list(self.traces_dict[dataset].keys()))
                             channel_names = list(set(channel_names))
                         else:
@@ -87,22 +87,22 @@
                             plot_channel_list.insert(1, "FRET Data")
                             plot_channel_list.insert(2, "FRET Efficiency")
                             plot_channel_list.insert(3, "FRET Data + Efficiency")
 
                         for channel_index, channel_name in enumerate(channel_names):
                             if channel_name.lower() in ["dd","da","ad","aa"]:
                                 plot_channel_list.append(channel_name.upper())
-                            elif channel_name.lower() in ["donor","acceptor"]:
+                            elif channel_name.lower() in ["donor","acceptor","data"]:
                                 plot_channel_list.append(channel_name.capitalize())
                             else:
                                 pass
 
-                        self.update_qcombo_items(self.plot_channel, plot_channel_list)
+                        self.update_qcombo_items(self.gui.plot_channel, plot_channel_list)
 
-                        self.plot_channel.blockSignals(False)
+                        self.gui.plot_channel.blockSignals(False)
                         self.updating_plot_combos = False
 
         except:
             print(traceback.format_exc())
 
     def update_plot_metrics_combos(self):
 
@@ -119,20 +119,21 @@
 
                     channel = channel_names[0]
                     dataset = dataset_names[0]
 
                     if dataset != "" and channel != "":
 
                         channel_dict = self.traces_dict[dataset][channel]
+                        trace_indeces = list(channel_dict.keys())
 
                         n_traces = len(channel_dict)
 
                         if n_traces > 0:
 
-                            metric_names = channel_dict[0].keys()
+                            metric_names = channel_dict[trace_indeces[0]].keys()
 
                             plot_metric_items = []
                             background_metric_items = []
 
                             for metric in metric_names:
                                 if "_local_bg" in metric:
                                     background_metric_items.append("Local Background")
@@ -147,18 +148,18 @@
 
                             plot_metric_items = list(set(plot_metric_items))
                             background_metric_items = list(set(background_metric_items))
 
                             background_metric_items.insert(0, "None")
 
                             self.updating_plot_combos = True
-                            self.update_qcombo_items(self.plot_metric, plot_metric_items)
-                            self.update_qcombo_items(self.plot_background_mode, background_metric_items)
-                            self.update_qcombo_items(self.traces_export_metric, plot_metric_items)
-                            self.update_qcombo_items(self.traces_export_background, background_metric_items)
+                            self.update_qcombo_items(self.gui.plot_metric, plot_metric_items)
+                            self.update_qcombo_items(self.gui.plot_background_mode, background_metric_items)
+                            self.update_qcombo_items(self.gui.traces_export_metric, plot_metric_items)
+                            self.update_qcombo_items(self.gui.traces_export_background, background_metric_items)
                             self.updating_plot_combos = False
 
         except:
             print(traceback.format_exc())
 
 
     def update_qcombo_items(self, qcombo, items):
@@ -195,22 +196,23 @@
 
     def compute_fret_efficiency(self,  dataset_name, metric_key, background_metric_key,
             progress_callback=None, gamma_correction=1, clip_data=False, efficiency_offset=False):
 
         try:
 
             dataset_dict = self.traces_dict[dataset_name].copy()
-            n_traces = len(dataset_dict["donor"])
+            trace_indices = list(dataset_dict["donor"].keys())
+            n_traces = len(trace_indices)
 
             dataset_dict["fret_efficiency"] = {}
-            for trace_index in range(n_traces):
+            for trace_index in trace_indices:
                 if trace_index not in dataset_dict["fret_efficiency"]:
                     dataset_dict["fret_efficiency"][trace_index] = {metric_key: []}
 
-            for trace_index in range(n_traces):
+            for trace_index in trace_indices:
 
                 donor = copy.deepcopy(dataset_dict["donor"][trace_index][metric_key])
                 acceptor = copy.deepcopy(dataset_dict["acceptor"][trace_index][metric_key])
 
                 if background_metric_key != None:
 
                     donor_bg = copy.deepcopy(dataset_dict["donor"][trace_index][background_metric_key])
@@ -313,18 +315,18 @@
 
         return sorted_list
 
     def populate_plot_dict(self, progress_callback=None):
 
         try:
 
-            dataset_name = self.plot_data.currentText()
-            channel_name = self.plot_channel.currentText()
-            metric_name = self.plot_metric.currentText()
-            background_mode = self.plot_background_mode.currentText()
+            dataset_name = self.gui.plot_data.currentText()
+            channel_name = self.gui.plot_channel.currentText()
+            metric_name = self.gui.plot_metric.currentText()
+            background_mode = self.gui.plot_background_mode.currentText()
 
             if hasattr(self, "plot_show_dict") == False:
                 self.plot_show_dict = {}
 
             metric_key = self.get_dict_key(self.metric_dict, metric_name)
 
             if background_mode != "None":
@@ -383,22 +385,21 @@
 
             plot_dict = {}
 
             for dataset_name in plot_datasets:
 
                 if channel_name == "All Channels" or "efficiency" in channel_name.lower():
                     dataset_channels = self.traces_dict[dataset_name].keys()
-                    if set(["dd", "da"]).issubset(dataset_channels):
 
+                    if set(["dd", "da"]).issubset(dataset_channels):
                         self.compute_alex_efficiency(dataset_name, metric_key,
                             background_metric_key, progress_callback,
                             clip_data=True)
 
                     elif set(["donor", "acceptor"]).issubset(dataset_channels):
-
                         self.compute_fret_efficiency(dataset_name, metric_key,
                             background_metric_key, progress_callback,
                             clip_data=True)
 
                 for channel_index, channel in enumerate(plot_channels):
 
                     if channel in self.traces_dict[dataset_name].keys():
@@ -466,72 +467,74 @@
     def initialize_plot(self):
 
         try:
             if hasattr(self, "traces_dict"):
 
                 if self.traces_dict != {}:
 
-                    dataset_name = self.plot_data.currentText()
-                    channel_name = self.plot_channel.currentText()
-                    metric_name = self.plot_metric.currentText()
+                    dataset_name = self.gui.plot_data.currentText()
+                    channel_name = self.gui.plot_channel.currentText()
+                    metric_name = self.gui.plot_metric.currentText()
 
                     if dataset_name != "" and channel_name != "" and metric_name != "":
 
                         if self.updating_plot_combos == False:
 
-                            self.plot_localisation_number.setEnabled(False)
-                            self.plot_data.setEnabled(False)
-                            self.plot_channel.setEnabled(False)
-                            self.plot_metric.setEnabled(False)
-                            self.split_plots.setEnabled(False)
-                            self.normalise_plots.setEnabled(False)
+                            self.gui.plot_localisation_number.setEnabled(False)
+                            self.gui.plot_data.setEnabled(False)
+                            self.gui.plot_channel.setEnabled(False)
+                            self.gui.plot_metric.setEnabled(False)
+                            self.gui.split_plots.setEnabled(False)
+                            self.gui.normalise_plots.setEnabled(False)
 
                             self.populate_plot_dict()
                             self.create_plot_checkboxes()
                             self.update_plot_layout()
                             self.plot_traces()
 
-                            self.plot_localisation_number.setEnabled(True)
-                            self.plot_data.setEnabled(True)
-                            self.plot_channel.setEnabled(True)
-                            self.plot_metric.setEnabled(True)
-                            self.split_plots.setEnabled(True)
-                            self.normalise_plots.setEnabled(True)
+                            self.gui.plot_localisation_number.setEnabled(True)
+                            self.gui.plot_data.setEnabled(True)
+                            self.gui.plot_channel.setEnabled(True)
+                            self.gui.plot_metric.setEnabled(True)
+                            self.gui.split_plots.setEnabled(True)
+                            self.gui.normalise_plots.setEnabled(True)
 
         except:
             print(traceback.format_exc())
             pass
 
 
     def create_plot_checkboxes(self):
 
         try:
 
-            grid_layout = self.traces_channel_selection_layout
+            grid_layout = self.gui.traces_channel_selection_layout
 
             channel_list = []
             label_list = []
 
             for dataset_name, dataset_dict in self.plot_dict.items():
-                for label in dataset_dict[0]["labels"]:
+
+                first_index = list(dataset_dict.keys())[0]
+
+                for label in dataset_dict[first_index]["labels"]:
                     label_list.append(label)
-                for channel in dataset_dict[0]["channels"]:
+                for channel in dataset_dict[first_index]["channels"]:
                     channel_list.append(channel)
 
             for i in range(grid_layout.count()):
                 item = grid_layout.itemAt(i)
                 if item is not None:
                     checkbox = item.widget()
                     checkbox_label = checkbox.text()
                     if isinstance(checkbox, QCheckBox):
                         if checkbox_label not in label_list:
                             checkbox.hide()
 
             self.repaint()
-            self.pixseq_ui.repaint()
 
             if len(channel_list) > 1:
                 for col_index, (channel, label) in enumerate(zip(channel_list,label_list)):
                     check_box_name = f"plot_show_{channel}"
                     check_box_label = f"{label}"
 
                     check_box_label = check_box_label.replace("Show: ","")
@@ -548,25 +551,25 @@
 
                         check_box.blockSignals(True)
                         check_box.setChecked(True)
                         check_box.blockSignals(False)
 
                         check_box.stateChanged.connect(self.plot_checkbox_event)
 
-                        self.traces_channel_selection_layout.addWidget(check_box, 0, col_index)
+                        self.gui.traces_channel_selection_layout.addWidget(check_box, 0, col_index)
 
         except:
             print(traceback.format_exc())
             pass
 
     def plot_checkbox_event(self, event):
 
         try:
 
-            grid_layout = self.traces_channel_selection_layout
+            grid_layout = self.gui.traces_channel_selection_layout
 
             for i in range(grid_layout.count()):
                 item = grid_layout.itemAt(i)
                 widget = item.widget()
                 if isinstance(widget, QCheckBox):
                     label = widget.text()
                     state = widget.isChecked()
@@ -592,16 +595,16 @@
 
         try:
 
             self.plot_grid = {}
 
             self.graph_canvas.clear()
 
-            split = self.split_plots.isChecked()
-            plot_mode = self.plot_channel.currentText()
+            split = self.gui.split_plots.isChecked()
+            plot_mode = self.gui.plot_channel.currentText()
 
             efficiency_plot = False
 
             n_traces = []
 
             for plot_index, (dataset_name, dataset_dict) in enumerate(self.plot_dict.items()):
 
@@ -712,16 +715,16 @@
                             "plot_lines_labels": plot_lines_labels,
                             "efficiency_plot": efficiency_plot,
                             }
 
             if len(n_traces) > 0:
 
                 n_traces = max(n_traces)
-                self.plot_localisation_number = self.findChild(QSlider, 'plot_localisation_number')
-                self.plot_localisation_number.setMaximum(n_traces-1)
+                self.gui.plot_localisation_number = self.gui.plot_localisation_number
+                self.gui.plot_localisation_number.setMaximum(n_traces-1)
 
                 plot_list = []
                 for plot_index, grid in enumerate(self.plot_grid.values()):
                     sub_axes = grid["sub_axes"]
                     sub_plots = []
                     for plot in sub_axes:
                         sub_plots.append(plot)
@@ -771,17 +774,17 @@
         try:
 
             if hasattr(self, "plot_grid") == False:
                 self.update_plot_layout()
 
             if self.plot_grid != {}:
 
-                localisation_number = self.plot_localisation_number.value()
+                localisation_number = self.gui.plot_localisation_number.value()
 
-                if self.focus_on_bbox.isChecked() == True:
+                if self.gui.focus_on_bbox.isChecked() == True:
                     self.get_loc_coords(localisation_number)
 
                 for plot_index, grid in enumerate(self.plot_grid.values()):
 
                     plot_dataset = grid["plot_dataset"]
                     sub_axes = grid["sub_axes"]
                     plot_lines = grid["plot_lines"]
@@ -794,15 +797,15 @@
 
                         if line_index == 0:
                             plot.setTitle(plot_details)
 
                         data_index = self.plot_dict[plot_dataset][localisation_number]["labels"].index(plot_label)
                         data = self.plot_dict[plot_dataset][localisation_number]["data"][data_index]
 
-                        if self.normalise_plots.isChecked() and "efficiency" not in plot_label.lower():
+                        if self.gui.normalise_plots.isChecked() and "efficiency" not in plot_label.lower():
                             data = (data - np.min(data)) / (np.max(data) - np.min(data))
 
                         plot_line = plot_lines[line_index]
                         plot_line.setData(data)
 
                         if plot_ranges["xRange"][1] < len(data):
                             plot_ranges["xRange"][1] = len(data)
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_temporal_filtering.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_temporal_filtering.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def update_filtering_channels(self):
 
         try:
 
             if self.dataset_dict != {}:
 
-                filtering_datasets = self.filtering_datasets.currentText()
+                filtering_datasets = self.gui.filtering_datasets.currentText()
 
                 if filtering_datasets == "All Datasets":
                     dataset_names = list(self.dataset_dict.keys())
                     channel_names = list(self.dataset_dict[dataset_names[0]].keys())
                 else:
                     dataset_names = [filtering_datasets]
                     channel_names = list(self.dataset_dict[dataset_names[0]].keys())
@@ -93,16 +93,16 @@
                         channel_name = channel_name.capitalize()
 
                     channel_names[channel_index] = channel_name
 
                 if len(channel_names) > 0:
                     channel_names.insert(0, "All Channels")
 
-                self.filtering_channels.clear()
-                self.filtering_channels.addItems(channel_names)
+                self.gui.filtering_channels.clear()
+                self.gui.filtering_channels.addItems(channel_names)
 
         except:
             print(traceback.format_exc())
             pass
 
     def calculate_image_chunks(self, total_height, num_chunks):
 
@@ -115,16 +115,16 @@
             end_height = total_height if i == num_chunks - 1 else start_height + chunk_size
             height_ranges.append((start_height, end_height))
 
         return height_ranges
 
     def _populate_temport_compute_jobs(self):
 
-        filter_size = int(self.filtering_filter_size.currentText())
-        filter_mode = self.filtering_mode.currentText()
+        filter_size = int(self.gui.filtering_filter_size.currentText())
+        filter_mode = self.gui.filtering_mode.currentText()
 
         compute_jobs = []
 
         try:
             for image_dict in self.shared_images:
 
                 h = image_dict['shape'][1]
@@ -150,16 +150,16 @@
 
         return compute_jobs
 
     def _pixseq_temporal_filtering(self, progress_callback = True):
 
         try:
 
-            filtering_datasets = self.filtering_datasets.currentText()
-            filtering_channels = self.filtering_channels.currentText()
+            filtering_datasets = self.gui.filtering_datasets.currentText()
+            filtering_channels = self.gui.filtering_channels.currentText()
 
             if filtering_datasets == "All Datasets":
                 dataset_names = list(self.dataset_dict.keys())
             else:
                 dataset_names = [filtering_datasets]
 
             if filtering_channels == "All Channels":
@@ -167,15 +167,15 @@
             else:
                 channel_names = [filtering_channels.lower()]
 
             self.shared_images = self.create_shared_images(dataset_names, channel_names)
 
             compute_jobs = self._populate_temport_compute_jobs()
 
-            print("Starting temporal filtering on {} images".format(len(self.shared_images)))
+            self.pixseq_notification("Starting temporal filtering on {} images".format(len(self.shared_images)))
 
             start_time = time.time()
 
             if len(compute_jobs) == 0:
                 pass
             elif len(compute_jobs) == 1:
                 temporal_filtering(compute_jobs[0])
@@ -215,20 +215,22 @@
             self.update_ui()
             print(traceback.format_exc())
             pass
 
     def pixseq_temporal_filtering(self, viewer=None):
 
         try:
-            self.filtering_start.setEnabled(False)
+            self.pixseq_notification("Starting temporal filtering...")
+
+            self.gui.filtering_start.setEnabled(False)
 
             self.update_ui(init=True)
 
             self.worker = Worker(self._pixseq_temporal_filtering)
-            self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.filtering_progressbar))
+            self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.gui.filtering_progressbar))
             self.worker.signals.finished.connect(self._pixseq_temporal_filtering_finished)
             self.worker.signals.error.connect(self.update_ui)
             self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
             print(traceback.format_exc())
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_trace_compute_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -304,28 +304,33 @@
         shared_mem = dat["shared_mem"]
         np_array = np.ndarray(dat["shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
         spot_size = dat["spot_size"]
         spot_center = dat["spot_center"]
         stop_event = dat["stop_event"]
         spot_index = dat["spot_index"]
         channel = dat["channel"]
+        frame_shape = np_array.shape[1:]
 
         if not stop_event.is_set():
 
             spot_metrics = {}
 
             spot_cx, spot_cy = spot_center
 
             n_pixels = spot_size**2
 
-            [x1,x2,y1,y2] = dat["spot_bound"]  #
+            bounds = dat["spot_bound"]
+
             spot_mask = dat["spot_mask"]
             spot_mask = spot_mask.astype(np.uint8)
-
             spot_background_mask = dat["spot_background_mask"]
+
+            [x1, x2, y1, y2], spot_mask, spot_background_mask = crop_spot_data(frame_shape,
+                bounds, spot_mask,spot_background_mask)
+
             spot_overlap = dat["background_overlap_mask"][y1:y2, x1:x2]
 
             if spot_overlap.shape == spot_background_mask.shape:
                 spot_background_mask = spot_background_mask & spot_overlap
 
             spot_mask = np.logical_not(spot_mask).astype(int)
             spot_background_mask = np.logical_not(spot_background_mask).astype(int)
@@ -408,14 +413,59 @@
         print(traceback.format_exc())
         spot_metrics = None
         pass
 
     return spot_metrics
 
 
+def crop_spot_data(image_shape, spot_bounds, spot_mask, background_mask=None):
+
+    try:
+        x1, x2, y1, y2 = spot_bounds
+        crop = [0, spot_mask.shape[1], 0, spot_mask.shape[0]]
+
+        if x1 < 0:
+            crop[0] = abs(x1)
+            x1 = 0
+        if x2 > image_shape[1]:
+            crop[1] = spot_mask.shape[1] - (x2 - image_shape[1])
+            x2 = image_shape[1]
+        if y1 < 0:
+            crop[2] = abs(y1)
+            y1 = 0
+        if y2 > image_shape[0]:
+            crop[3] = spot_mask.shape[0] - (y2 - image_shape[0])
+            y2 = image_shape[0]
+
+        corrected_bounds = [x1, x2, y1, y2]
+
+        if spot_mask is not None:
+            loc_mask = spot_mask.copy()
+            loc_mask = loc_mask[crop[2]:crop[3], crop[0]:crop[1]]
+        else:
+            loc_mask = None
+
+        if background_mask is not None:
+            loc_bg_mask = background_mask.copy()
+            loc_bg_mask = loc_bg_mask[crop[2]:crop[3], crop[0]:crop[1]]
+        else:
+            loc_bg_mask = None
+
+    except:
+        loc_mask = spot_mask
+        loc_bg_mask = background_mask
+        corrected_bounds = spot_bounds
+        print(traceback.format_exc())
+
+    return corrected_bounds, loc_mask, loc_bg_mask
+
+
+
+
+
 class _trace_compute_utils:
 
     def generate_spot_bounds(self, locs, box_size):
 
         spot_bounds = []
 
         for loc_index, loc in enumerate(locs):
@@ -440,15 +490,15 @@
 
             spot_bounds.append([x1,x2,y1,y2])
 
         return spot_bounds
 
     def _pixseq_compute_traces_finished(self):
 
-        self.compute_traces.setEnabled(True)
+        self.gui.compute_traces.setEnabled(True)
 
         self.populate_plot_combos()
         self.populate_export_combos()
         self.initialize_plot()
 
         self.update_ui()
 
@@ -554,25 +604,25 @@
 
     def generate_background_overlap_mask(self, locs, spot_mask, spot_background_mask, image_mask_shape):
 
         global_spot_mask = np.zeros(image_mask_shape, dtype=np.uint8)
         global_background_mask = np.zeros(image_mask_shape, dtype=np.uint8)
 
         spot_mask = spot_mask.astype(np.uint16)
-        spot_background_mask = spot_background_mask
+        spot_background_mask = spot_background_mask.astype(np.uint16)
 
         spot_bounds = self.generate_spot_bounds(locs,  len(spot_mask[0]))
 
-        for loc_index, [x1,x2,y1,y2] in enumerate(spot_bounds):
+        for loc_index, bounds in enumerate(spot_bounds):
 
-            x1, y1 = max(0, x1), max(0, y1)
-            x2, y2 = min(global_spot_mask.shape[1], x2), min(global_spot_mask.shape[0], y2)
+            [x1, x2, y1, y2], loc_mask, log_bg_mask = crop_spot_data(image_mask_shape,
+                bounds, spot_mask,spot_background_mask)
 
-            global_spot_mask[y1:y2, x1:x2] += spot_mask[:y2-y1, :x2-x1]
-            global_background_mask[y1:y2, x1:x2] += spot_background_mask[:y2-y1, :x2-x1]
+            global_spot_mask[y1:y2, x1:x2] += loc_mask
+            global_background_mask[y1:y2, x1:x2] += log_bg_mask
 
         global_spot_mask[global_spot_mask > 0] = 1
         global_background_mask[global_background_mask > 0] = 1
 
         intersection_mask = global_spot_mask & global_background_mask
 
         global_background_mask = global_background_mask - intersection_mask
@@ -612,22 +662,22 @@
         compute_jobs = {"spot_metrics": [],
                         "background_metrics": [],
                         "picasso_metrics": [],
                         }
 
         try:
 
-            self.traces_spot_size = self.findChild(QComboBox, "traces_spot_size")
+            self.gui.traces_spot_size = self.gui.traces_spot_size
 
-            spot_size = int(self.traces_spot_size.currentText())
-            spot_shape = self.traces_spot_shape.currentText()
-            buffer_size = int(self.traces_background_buffer.currentText())
-            bg_width = int(self.traces_background_width.currentText())
-            compute_global_background = self.compute_global_background.isChecked()
-            compute_picasso = self.compute_with_picasso.isChecked()
+            spot_size = int(self.gui.traces_spot_size.currentText())
+            spot_shape = self.gui.traces_spot_shape.currentText()
+            buffer_size = int(self.gui.traces_background_buffer.currentText())
+            bg_width = int(self.gui.traces_background_width.currentText())
+            compute_global_background = self.gui.compute_global_background.isChecked()
+            compute_picasso = self.gui.compute_with_picasso.isChecked()
 
             localisation_dict = copy.deepcopy(self.localisation_dict["bounding_boxes"])
             locs = localisation_dict["localisations"].copy()
             box_size = localisation_dict["box_size"]
 
             spot_mask, buffer_mask, spot_background_mask = self.generate_localisation_mask(spot_size,
                 spot_shape, buffer_size, bg_width, plot=False)
@@ -642,15 +692,15 @@
             for image_dict in self.shared_images:
 
                 mask_shape = image_dict["shape"][1:]
                 n_frames = image_dict["shape"][0]
                 n_locs = len(locs)
                 channel = image_dict["channel"]
                 dataset = image_dict["dataset"]
-                n_pixels = int(self.traces_spot_size.currentText()) ** 2
+                n_pixels = int(self.gui.traces_spot_size.currentText()) ** 2
 
                 background_overlap_mask, global_spot_mask = self.generate_background_overlap_mask(locs,
                     buffer_mask, spot_background_mask, mask_shape)
 
                 for spot_index, (spot_loc, spot_bound, spot_center) in enumerate(zip(locs, spot_bounds, spot_centers)):
                     spot_compute_task = {"compute_task":"spot_metrics",
                                          "spot_index": spot_index,
@@ -715,29 +765,27 @@
 
 
 
     def extract_spot_metrics_wrapper(self, progress_callback):
 
         try:
 
-            compute_global_background = self.compute_global_background.isChecked()
-            compute_picasso = self.compute_with_picasso.isChecked()
+            compute_global_background = self.gui.compute_global_background.isChecked()
+            compute_picasso = self.gui.compute_with_picasso.isChecked()
 
             compute_jobs = self.populate_spot_metric_compute_jobs()
 
             spot_metrics_jobs = compute_jobs["spot_metrics"]
             background_metrics_jobs = compute_jobs["background_metrics"]
             picasso_metrics_jobs = compute_jobs["picasso_metrics"]
 
             spot_metrics = []
             background_metrics = []
             picasso_metrics = []
 
-            extract_spot_metrics(spot_metrics_jobs[0])
-
             cpu_count = int(multiprocessing.cpu_count() * 0.9)
 
             total_jobs = len(spot_metrics_jobs) + len(background_metrics_jobs) + len(picasso_metrics_jobs)
 
             with concurrent.futures.ProcessPoolExecutor(max_workers=cpu_count) as executor:
                 # Combine both job types into a single dictionary
 
@@ -754,19 +802,22 @@
                     else:
                         job = futures[future]
                         job_type = job["compute_task"]
                         try:
                             result = future.result()  # Process result here
                             # Append result to the appropriate list based on job type
                             if job_type == "spot_metrics":
-                                spot_metrics.append(result)
+                                if result is not None:
+                                    spot_metrics.append(result)
                             elif job_type == "picasso_metrics":
-                                picasso_metrics.append(result)
+                                if result is not None:
+                                    picasso_metrics.append(result)
                             else:
-                                background_metrics.append(result)
+                                if result is not None:
+                                    background_metrics.append(result)
                         except concurrent.futures.TimeoutError:
                             # Handle timeout
                             pass
                         except Exception as e:
                             print(e)
                             # Handle other exceptions
                             pass
@@ -944,14 +995,28 @@
                             bleach_index= -1
 
 
                         for channel in dataset_dict.keys():
                             self.traces_dict[dataset_name][channel][spot_index]["bleach_index"] = bleach_index
                             self.traces_dict[dataset_name][channel][spot_index]["donor_bleach_index"] = donor_bleach_index
                             self.traces_dict[dataset_name][channel][spot_index]["acceptor_bleach_index"] = acceptor_bleach_index
+                else:
+
+                    for spot_index in dataset_dict[channel_list[0]].keys():
+
+                        data = dataset_dict[channel_list[0]][spot_index][spot_metric].copy()
+                        background_data = dataset_dict[channel_list[0]][spot_index][background_metric].copy()
+
+                        bleach_index = self.find_bleach_indices(data, background_data, mode=mode)
+
+                        for channel in dataset_dict.keys():
+                            self.traces_dict[dataset_name][channel][spot_index]["bleach_index"] = bleach_index
+                            self.traces_dict[dataset_name][channel][spot_index]["donor_bleach_index"] = bleach_index
+                            self.traces_dict[dataset_name][channel][spot_index]["acceptor_bleach_index"] = bleach_index
+
 
         except:
             print(traceback.format_exc())
             pass
 
 
     def _pixseq_compute_traces(self, progress_callback=None, picasso=False):
@@ -967,62 +1032,72 @@
             self.extract_spot_metrics_wrapper(progress_callback)
 
             self.restore_shared_images()
 
             self.populatate_traces_dict()
 
             self.compute_photo_bleaching()
-            self.compute_traces.setEnabled(True)
+            self.gui.compute_traces.setEnabled(True)
 
         except:
             self.update_ui()
             self.restore_shared_images()
             print(traceback.format_exc())
             pass
 
     def pixseq_compute_traces(self):
 
         try:
 
-            if self.localisation_dict != {}:
-
-                layer_names = [layer.name for layer in self.viewer.layers]
+            compute_traces = False
 
+            if self.localisation_dict != {}:
                 if "bounding_boxes" in self.localisation_dict.keys():
                     if "localisations" in self.localisation_dict["bounding_boxes"].keys():
-                        if len(self.localisation_dict["bounding_boxes"]["localisations"]):
+                        n_bboxes = len(self.localisation_dict["bounding_boxes"]["localisations"])
+
+                        if n_bboxes > 0:
+                            compute_traces = True
+
+            if compute_traces == True:
+
+                self.pixseq_notification(f"Computing traces for {n_bboxes} bounding boxes.")
 
-                            self.update_ui(init=True)
+                self.update_ui(init=True)
+
+                self.worker = Worker(self._pixseq_compute_traces)
+                self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.gui.compute_traces_progressbar))
+                self.worker.signals.finished.connect(self._pixseq_compute_traces_finished)
+                self.worker.signals.error.connect(self._pixseq_compute_traces_finished)
+                self.threadpool.start(self.worker)
+
+            else:
+                self.pixseq_notification("Bounding Boxes required for trace computation.")
 
-                            self.worker = Worker(self._pixseq_compute_traces)
-                            self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.compute_traces_progressbar))
-                            self.worker.signals.finished.connect(self._pixseq_compute_traces_finished)
-                            self.worker.signals.error.connect(self._pixseq_compute_traces_finished)
-                            self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
             self.restore_shared_images()
             print(traceback.format_exc())
 
     def visualise_background_masks(self):
 
-        self.compute_traces.setEnabled(True)
+        self.gui.compute_traces.setEnabled(True)
 
         try:
 
             import cv2
 
             if "bounding_boxes" in self.localisation_dict.keys():
                 if "localisations" in self.localisation_dict["bounding_boxes"].keys():
 
-                    spot_size = int(self.traces_spot_size.currentText())
-                    spot_shape = self.traces_spot_shape.currentText()
-                    buffer_size = int(self.traces_background_buffer.currentText())
-                    bg_width = int(self.traces_background_width.currentText())
+                    spot_size = int(self.gui.traces_spot_size.currentText())
+                    spot_shape = self.gui.traces_spot_shape.currentText()
+                    buffer_size = int(self.gui.traces_background_buffer.currentText())
+                    bg_width = int(self.gui.traces_background_width.currentText())
 
                     localisation_dict = copy.deepcopy(self.localisation_dict["bounding_boxes"])
                     locs = localisation_dict["localisations"]
 
                     spot_mask, buffer_mask, bg_mask = self.generate_localisation_mask(spot_size, spot_shape, buffer_size, bg_width)
 
                     mask_shape = self.dataset_dict[self.active_dataset][self.active_channel]["data"].shape[-2:]
@@ -1033,23 +1108,22 @@
 
                     bg_mask = bg_mask.astype(np.uint8)
 
                     mask_shape = self.dataset_dict[self.active_dataset][self.active_channel]["data"].shape[-2:]
 
                     global_spot_mask = np.zeros(mask_shape, dtype=np.uint16)
 
-                    for loc_index, [x1, x2, y1, y2] in enumerate(spot_bounds):
-                        temp_mask = np.zeros(mask_shape, dtype=np.uint8)
+                    for loc_index, bounds in enumerate(spot_bounds):
 
-                        x1, y1 = max(0, x1), max(0, y1)
-                        x2, y2 = min(global_spot_mask.shape[1], x2), min(global_spot_mask.shape[0], y2)
+                        [x1, x2, y1, y2], loc_bg_mask, _ = crop_spot_data(mask_shape, bounds, bg_mask)
 
-                        temp_mask[y1:y2, x1:x2] += bg_mask
-                        global_spot_mask[temp_mask > 0] = loc_index + 1
+                        temp_mask = np.zeros(mask_shape, dtype=np.uint8)
+                        temp_mask[y1:y2, x1:x2] += loc_bg_mask
 
+                        global_spot_mask[temp_mask > 0] = loc_index + 1
 
                     binary_spot_mask = global_spot_mask > 0
                     overlap_mask = binary_spot_mask & background_overlap_mask
                     inverse_overlap_mask = np.logical_not(overlap_mask)
 
                     global_spot_mask[inverse_overlap_mask] = 0
 
@@ -1065,40 +1139,38 @@
 
         try:
             import cv2
 
             if "bounding_boxes" in self.localisation_dict.keys():
                 if "fitted" in self.localisation_dict["bounding_boxes"].keys():
 
-                    spot_size = int(self.traces_spot_size.currentText())
-                    spot_shape = self.traces_spot_shape.currentText()
-                    buffer_size = int(self.traces_background_buffer.currentText())
-                    bg_width = int(self.traces_background_width.currentText())
+                    spot_size = int(self.gui.traces_spot_size.currentText())
+                    spot_shape = self.gui.traces_spot_shape.currentText()
+                    buffer_size = int(self.gui.traces_background_buffer.currentText())
+                    bg_width = int(self.gui.traces_background_width.currentText())
 
                     localisation_dict = copy.deepcopy(self.localisation_dict["bounding_boxes"])
                     locs = localisation_dict["localisations"]
 
                     spot_mask, buffer_mask, spot_background_mask = self.generate_localisation_mask(spot_size, spot_shape, buffer_size, bg_width)
 
                     spot_bounds = self.generate_spot_bounds(locs, len(spot_mask[0]))
 
                     spot_mask = spot_mask.astype(np.uint8)
 
                     mask_shape = self.dataset_dict[self.active_dataset][self.active_channel]["data"].shape[-2:]
 
                     global_spot_mask = np.zeros(mask_shape, dtype=np.uint16)
 
-                    for loc_index, [x1,x2,y1,y2] in enumerate(spot_bounds):
+                    for loc_index, bounds in enumerate(spot_bounds):
 
-                        temp_mask = np.zeros(mask_shape, dtype=np.uint8)
+                        [x1, x2, y1, y2], loc_mask, _ = crop_spot_data(mask_shape, bounds, spot_mask)
 
-                        x1, y1 = max(0, x1), max(0, y1)
-                        x2, y2 = min(global_spot_mask.shape[1], x2), min(global_spot_mask.shape[0], y2)
-
-                        temp_mask[y1:y2, x1:x2] += spot_mask
+                        temp_mask = np.zeros(mask_shape, dtype=np.uint8)
+                        temp_mask[y1:y2, x1:x2] += loc_mask
                         global_spot_mask[temp_mask > 0] = loc_index + 1
 
                     if "Spot Mask" in self.viewer.layers:
                         self.viewer.layers.remove("Spot Mask")
                     self.viewer.add_labels(
                         global_spot_mask,
                         opacity=0.8,
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_transform_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_transform_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,37 @@
 from napari_pixseq.funcs.pixseq_utils_compute import Worker
 from qtpy.QtWidgets import QFileDialog
 import math
 import json
 from datetime import datetime
 
 
-def transform_image(img, transform_matrix, progress_callback=None):
+def transform_image(img, transform_matrix,
+        transform_mode = "homography", progress_callback=None):
 
     w, h = img.shape[-2:]
 
     n_frames = img.shape[0]
     n_segments = math.ceil(n_frames / 100)
     image_splits = np.array_split(img, n_segments)
 
     transformed_image = []
 
     iter = 0
 
     for index, image in enumerate(image_splits):
+
         image = np.moveaxis(image, 0, -1)
-        image = cv2.warpPerspective(image, transform_matrix, (h, w), borderMode=cv2.BORDER_CONSTANT, borderValue=(0, 0, 0, 0))
-        # image = np.moveaxis(image, -1, 0)
+
+        if transform_mode == "homography":
+            image = cv2.warpPerspective(image, transform_matrix, (h, w),
+                borderMode=cv2.BORDER_CONSTANT, borderValue=(0, 0, 0, 0))
+        elif transform_mode == "affine":
+            image = cv2.warpAffine(image, transform_matrix, (h, w),
+                borderMode=cv2.BORDER_CONSTANT, borderValue=(0, 0, 0, 0))
 
         transformed_image.append(image)
         iter += 250
         progress = int((iter / n_frames) * 100)
 
         if progress_callback is not None:
             progress_callback(progress)
@@ -55,24 +62,24 @@
 
 
     def compute_transform_matrix(self):
 
         try:
             if self.dataset_dict != {}:
 
-                dataset_name = self.tform_compute_dataset.currentText()
-                target_channel = self.tform_compute_target_channel.currentText()
-                reference_channel = self.tform_compute_ref_channel.currentText()
+                dataset_name = self.gui.tform_compute_dataset.currentText()
+                target_channel = self.gui.tform_compute_target_channel.currentText()
+                reference_channel = self.gui.tform_compute_ref_channel.currentText()
 
                 target_locs = None
                 reference_locs = None
 
-                if dataset_name in self.localisation_dict["fiducials"].keys():
+                if dataset_name in self.localisation_dict["localisations"].keys():
 
-                    fiducial_dict = self.localisation_dict["fiducials"][dataset_name]
+                    fiducial_dict = self.localisation_dict["localisations"][dataset_name]
 
                     if target_channel.lower() in fiducial_dict.keys():
                         target_locs = fiducial_dict[target_channel.lower()]["localisations"]
 
                     if reference_channel.lower() in fiducial_dict.keys():
                         reference_locs = fiducial_dict[reference_channel.lower()]["localisations"]
 
@@ -92,15 +99,15 @@
                     reference_points = np.float32([reference_points[m.queryIdx] for m in matches]).reshape(-1, 2)
                     target_points = np.float32([target_points[m.trainIdx] for m in matches]).reshape(-1, 2)
 
                     self.transform_matrix, _ = cv2.findHomography(target_points, reference_points, cv2.RANSAC)
 
                     print(f"Transform Matrix\n: {self.transform_matrix}")
 
-                    if self.save_tform.isChecked():
+                    if self.gui.save_tform.isChecked():
                         self.save_transform_matrix()
 
         except:
             print(traceback.format_exc())
             pass
 
 
@@ -110,26 +117,26 @@
 
             if self.transform_matrix is not None:
 
                 # get save file name and path
                 date = datetime.now().strftime("%y%m%d")
                 file_name = f'pixseq_transform_matrix-{date}.txt'
 
-                dataset_name = self.tform_compute_dataset.currentText()
-                channel_name = self.tform_compute_target_channel.currentText()
+                dataset_name = self.gui.tform_compute_dataset.currentText()
+                channel_name = self.gui.tform_compute_target_channel.currentText()
 
                 path = self.dataset_dict[dataset_name][channel_name.lower()]["path"]
                 path_directory = os.path.dirname(path)
 
                 tform_path = os.path.join(path_directory, file_name)
 
                 tform_path = QFileDialog.getSaveFileName(self, 'Save transform matrix', tform_path, 'Text files (*.txt)')[0]
 
                 if tform_path != "":
-                    print(f"Saving transform matrix to {tform_path}")
+                    self.pixseq_notification(f"Saving transform matrix to {tform_path}")
 
                     with open(tform_path, 'w') as filehandle:
                         json.dump(self.transform_matrix.tolist(), filehandle)
 
         except:
             print(traceback.format_exc())
             pass
@@ -145,24 +152,21 @@
 
         except:
             print(traceback.format_exc())
             pass
 
     def _apply_transform_matrix(self, progress_callback=None):
 
-        print("Applying transform matrix...")
+        self.pixseq_notification("Applying transform matrix...")
 
         try:
 
             if self.dataset_dict != {}:
 
-                from qtpy.QtWidgets import QComboBox
-                self.tform_apply_target = self.findChild(QComboBox, 'tform_apply_target')
-
-                apply_channel = self.tform_apply_target.currentText()
+                apply_channel = self.gui.tform_apply_target.currentText()
 
                 if "donor" in apply_channel.lower():
                     ref_emission = "d"
                 else:
                     ref_emission = "a"
 
                 target_images = []
@@ -203,28 +207,28 @@
 
         try:
 
             if self.dataset_dict != {}:
 
                 if hasattr(self, "transform_matrix") == False:
 
-                    print("No transform matrix loaded.")
+                    self.pixseq_notification("No transform matrix loaded.")
 
                 else:
 
                     if self.transform_matrix is None:
 
-                        print("No transform matrix loaded.")
+                        self.pixseq_notification("No transform matrix loaded.")
 
                     else:
 
                         self.update_ui(init=True)
 
                         self.worker = Worker(self._apply_transform_matrix)
-                        self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.tform_apply_progressbar))
+                        self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.gui.tform_apply_progressbar))
                         self.worker.signals.finished.connect(self._apply_transform_matrix_finished)
                         self.worker.signals.error.connect(self.update_ui)
                         self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_undrift_utils.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_undrift_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,50 +72,46 @@
         def undrift_callback(progress):
             compute_progress["undrift"] = (progress/n_pairs)*100
             total_progress()
 
         if type(segmentation) == int:
             if n_frames > segmentation:
 
-                drift, _ = picasso_undrift(undrift_locs,
+                drift, undrifted_locs = picasso_undrift(undrift_locs,
                     picasso_info,
                     segmentation=segmentation,
                     display=False,
                     segmentation_callback=segmentation_callback,
                     rcc_callback=undrift_callback,
                     )
 
                 dataset_dict["drift"] = drift
+                dataset_dict["undrifted_locs"] = undrifted_locs
 
             else:
                 progress_dict[index] = 100
         else:
             progress_dict[index] = 100
 
     except:
         print(traceback.format_exc())
         pass
 
     return dataset_dict
 
 
-
-
-
-
-
 class _undrift_utils:
 
     def undrift_localisations(self):
 
         try:
 
             for dataset_name, dataset_data in self.dataset_dict.items():
                 for channel_name, channel_data in self.dataset_dict[dataset_name].items():
-                    fiducial_dict = self.localisation_dict["fiducials"][dataset_name][channel_name.lower()].copy()
+                    fiducial_dict = self.localisation_dict["localisations"][dataset_name][channel_name.lower()].copy()
 
                     if "drift" in channel_data.keys() and "localisations" in fiducial_dict.keys():
                         locs = fiducial_dict["localisations"]
 
                         drift = channel_data["drift"]
 
                         render_locs = {}
@@ -128,30 +124,30 @@
                             if frame not in render_locs.keys():
                                 render_locs[frame] = []
 
                             render_locs[frame].append([loc.y, loc.x])
 
                         localisation_centres = self.get_localisation_centres(locs)
 
-                        self.localisation_dict["fiducials"][dataset_name][channel_name.lower()]["localisations"] = locs
-                        self.localisation_dict["fiducials"][dataset_name][channel_name.lower()]["localisation_centres"] = localisation_centres
-                        self.localisation_dict["fiducials"][dataset_name][channel_name.lower()]["render_locs"] = render_locs
+                        self.localisation_dict["localisations"][dataset_name][channel_name.lower()]["localisations"] = locs
+                        self.localisation_dict["localisations"][dataset_name][channel_name.lower()]["localisation_centres"] = localisation_centres
+                        self.localisation_dict["localisations"][dataset_name][channel_name.lower()]["render_locs"] = render_locs
 
         except:
             print(traceback.format_exc())
             pass
 
     def _undrift_images_finished(self):
 
         try:
 
             self.image_layer.data = self.dataset_dict[self.active_dataset][self.active_channel]["data"]
 
             self.undrift_localisations()
-            self.draw_fiducials(update_vis=True)
+            self.draw_localisations(update_vis=True)
 
             for layer in self.viewer.layers:
                 layer.refresh()
 
             self.update_ui()
 
         except:
@@ -291,16 +287,16 @@
             pass
 
 
     def undrift_images(self, segmentation=20):
 
         try:
 
-            dataset = self.undrift_dataset_selector.currentText()
-            channel = self.undrift_channel_selector.currentText()
+            dataset = self.gui.undrift_dataset_selector.currentText()
+            channel = self.gui.undrift_channel_selector.currentText()
 
             if dataset == "All Datasets":
                 dataset_list = list(self.dataset_dict.keys())
             else:
                 dataset_list = [dataset]
 
             undrift_dict = {}
@@ -312,22 +308,22 @@
                     n_frames,height,width = self.dataset_dict[dataset][channel.lower()]["data"].shape
                     picasso_info = [{'Frames': n_frames, 'Height': height, 'Width': width}, {}]
 
                     undrift_dict[dataset] = {"loc_dict": loc_dict, "n_locs": n_locs,
                                              "picasso_info": picasso_info,
                                              "channel": channel.lower(), "dataset": dataset}
                 else:
-                    print("No fitted localizations found for dataset: " + dataset)
+                    self.pixseq_notification("No fitted localizations found for dataset: " + dataset)
 
             if undrift_dict != {}:
 
                 self.update_ui(init=True)
 
                 self.worker = Worker(self._undrift_images, undrift_dict=undrift_dict, segmentation=20)
-                self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.undrift_progressbar))
+                self.worker.signals.progress.connect(partial(self.pixseq_progress, progress_bar=self.gui.undrift_progressbar))
                 self.worker.signals.finished.connect(self._undrift_images_finished)
                 self.threadpool.start(self.worker)
 
         except:
             self.update_ui()
             print(traceback.format_exc())
             pass
```

### Comparing `napari-PixSeq-1.0.0/src/napari_pixseq/funcs/pixseq_utils_compute.py` & `napari_pixseq-1.0.2/src/napari_pixseq/funcs/pixseq_utils_compute.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from qtpy.QtCore import QObject
 from qtpy.QtCore import QRunnable
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
 import traceback
 import sys
 from multiprocessing import Process, shared_memory, Pool
 import numpy as np
-
+import napari
 
 class _utils_compute:
 
     def create_shared_images(self, dataset_list = None, channel_list = None):
 
         if self.verbose:
             print("Creating shared images")
@@ -73,53 +73,102 @@
                     shared_mem.close()
                     shared_mem.unlink()
 
                 except:
                     print(traceback.format_exc())
                     pass
 
-    def create_shared_frames(self):
+    def create_shared_frames(self, dataset_list = None, channel_list = None, frame_index = None):
 
         if self.verbose:
             print("Creating shared frames")
 
+        if dataset_list is None:
+            dataset_list = list(self.dataset_dict.keys())
+        else:
+            dataset_list = [dataset for dataset in dataset_list if dataset in self.dataset_dict.keys()]
+
         self.shared_frames = []
 
-        for dataset_name, dataset_dict in self.dataset_dict.items():
-            for channel_name, channel_dict in dataset_dict.items():
+        for dataset_name in dataset_list:
+
+            if channel_list is None:
+                channel_names = list(self.dataset_dict[dataset_name].keys())
+            else:
+                channel_names = [channel for channel in channel_list if channel in self.dataset_dict[dataset_name].keys()]
+
+            for channel_name in channel_names:
+
+                if channel_name in self.dataset_dict[dataset_name].keys():
+
+                    channel_dict = self.dataset_dict[dataset_name][channel_name]
 
-                image = channel_dict.pop("data")
+                    if type(frame_index) == int:
 
-                image_dict = {"dataset": dataset_name,
-                              "channel": channel_name,
-                              "gap_label": channel_dict["gap_label"],
-                              "sequence_label": channel_dict["sequence_label"],
-                              "n_frames": image.shape[0],
-                              "shape": image.shape,
-                              "dtype": image.dtype,
-                              "frame_dict":{},
-                              }
-
-                for frame_index, frame in enumerate(image):
-
-                    if frame_index not in image_dict["frame_dict"]:
-                        image_dict["frame_dict"][frame_index] = {}
-
-                    shared_mem = shared_memory.SharedMemory(create=True, size=frame.nbytes)
-                    shared_frame = np.ndarray(frame.shape, dtype=frame.dtype, buffer=shared_mem.buf)
-                    shared_frame[:] = frame[:]
+                        image = channel_dict["data"]
 
-                    image_dict["frame_dict"][frame_index] = {"frame_index": frame_index,
-                                                             "dataset": dataset_name,
+                        image_dict = {"dataset": dataset_name,
+                                      "channel": channel_name,
+                                      "gap_label": channel_dict["gap_label"],
+                                      "sequence_label": channel_dict["sequence_label"],
+                                      "n_frames": image.shape[0],
+                                      "shape": image.shape,
+                                      "dtype": image.dtype,
+                                      "frame_dict":{},
+                                      }
+
+                        frame = image[frame_index]
+
+                        shared_mem = shared_memory.SharedMemory(create=True, size=frame.nbytes)
+                        shared_memory_name = shared_mem.name
+                        shared_frame = np.ndarray(frame.shape, dtype=frame.dtype, buffer=shared_mem.buf)
+                        shared_frame[:] = frame[:]
+
+                        image_dict["frame_dict"][frame_index] = {"frame_index": frame_index,
+                                                                "dataset": dataset_name,
                                                                 "channel": channel_name,
                                                                 "shared_mem": shared_mem,
+                                                                "shared_memory_name": shared_memory_name,
                                                                 "shape": frame.shape,
                                                                 "dtype": frame.dtype,
                                                                 }
 
+                    else:
+
+                        image = channel_dict.pop("data")
+
+                        image_dict = {"dataset": dataset_name,
+                                      "channel": channel_name,
+                                      "gap_label": channel_dict["gap_label"],
+                                      "sequence_label": channel_dict["sequence_label"],
+                                      "n_frames": image.shape[0],
+                                      "shape": image.shape,
+                                      "dtype": image.dtype,
+                                      "frame_dict":{},
+                                      }
+
+                        for frame_index, frame in enumerate(image):
+
+                            if frame_index not in image_dict["frame_dict"]:
+                                image_dict["frame_dict"][frame_index] = {}
+
+                            shared_mem = shared_memory.SharedMemory(create=True, size=frame.nbytes)
+                            shared_memory_name = shared_mem.name
+                            shared_frame = np.ndarray(frame.shape, dtype=frame.dtype, buffer=shared_mem.buf)
+                            shared_frame[:] = frame[:]
+
+                            image_dict["frame_dict"][frame_index] = {"frame_index": frame_index,
+                                                                     "dataset": dataset_name,
+                                                                     "channel": channel_name,
+                                                                     "shared_mem": shared_mem,
+                                                                     "shared_memory_name": shared_memory_name,
+                                                                     "shape": frame.shape,
+                                                                     "dtype": frame.dtype,
+                                                                     }
+
                 self.shared_frames.append(image_dict)
 
         return self.shared_frames
 
     def restore_shared_frames(self):
 
         if self.verbose:
@@ -127,40 +176,69 @@
 
         if hasattr(self, "shared_frames"):
 
             for image_dict in self.shared_frames:
 
                 try:
 
-                    frame_dict = image_dict["frame_dict"]
+                    dataset = image_dict["dataset"]
+                    channel = image_dict["channel"]
 
-                    image = []
+                    dataset_dict = self.dataset_dict[dataset][channel]
 
-                    for frame_index, frame_dict in frame_dict.items():
+                    if "data" not in dataset_dict.keys():
 
-                        shared_mem = frame_dict["shared_mem"]
+                        frame_dict = image_dict["frame_dict"]
 
-                        frame = np.ndarray(frame_dict["shape"], dtype=frame_dict["dtype"], buffer=shared_mem.buf)
+                        image = []
 
-                        image.append(frame.copy())
+                        for frame_index, frame_dict in frame_dict.items():
 
-                        shared_mem.close()
-                        shared_mem.unlink()
+                            shared_mem = frame_dict["shared_mem"]
 
-                    image = np.stack(image, axis=0)
+                            frame = np.ndarray(frame_dict["shape"],
+                                dtype=frame_dict["dtype"],
+                                buffer=shared_mem.buf)
 
-                    self.dataset_dict[image_dict["dataset"]][image_dict["channel"]]["data"] = image
+                            image.append(frame.copy())
 
-                    shared_mem.close()
-                    shared_mem.unlink()
+                            shared_mem.close()
+                            shared_mem.unlink()
+
+                        image = np.stack(image, axis=0)
+
+                        self.dataset_dict[dataset][channel]["data"] = image
+
+                        shared_mem.close()
+                        shared_mem.unlink()
 
                 except:
                     print(traceback.format_exc())
                     pass
 
+    def clear_live_images(self):
+
+        try:
+
+            if self.verbose:
+                print("Clearing live images")
+
+            image_layers = [layer for layer in self.viewer.layers if isinstance(layer, napari.layers.Image)]
+
+            for layer in image_layers:
+
+                frame_shape = layer.data.shape[1:]
+                empty_frame = np.zeros(frame_shape, dtype=layer.data.dtype)
+                layer.data = empty_frame
+
+        except:
+            print(traceback.format_exc())
+            pass
+
+
 
 class WorkerSignals(QObject):
     """
     Defines the signals available from a running worker thread.
 
     Supported signals are:
```

