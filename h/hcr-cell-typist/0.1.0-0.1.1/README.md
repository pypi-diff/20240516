# Comparing `tmp/hcr_cell_typist-0.1.0.tar.gz` & `tmp/hcr_cell_typist-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcr_cell_typist-0.1.0.tar", last modified: Mon May  6 13:51:38 2024, max compression
+gzip compressed data, was "hcr_cell_typist-0.1.1.tar", last modified: Thu May 16 13:18:32 2024, max compression
```

## Comparing `hcr_cell_typist-0.1.0.tar` & `hcr_cell_typist-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/
--rw-r--r--   0 luca      (1000) luca      (1000)     1057 2024-05-03 14:06:12.000000 hcr_cell_typist-0.1.0/LICENSE
--rw-r--r--   0 luca      (1000) luca      (1000)     3185 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)     1378 2024-05-06 13:51:26.000000 hcr_cell_typist-0.1.0/README.md
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/
--rw-r--r--   0 luca      (1000) luca      (1000)      113 2024-05-06 12:57:56.000000 hcr_cell_typist-0.1.0/cell_typist/__init__.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/core/
--rw-r--r--   0 luca      (1000) luca      (1000)      158 2024-02-11 23:13:03.000000 hcr_cell_typist-0.1.0/cell_typist/core/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)    16020 2024-05-06 08:33:15.000000 hcr_cell_typist-0.1.0/cell_typist/core/datatypes.py
--rw-r--r--   0 luca      (1000) luca      (1000)    13554 2024-01-14 13:00:14.000000 hcr_cell_typist-0.1.0/cell_typist/core/experiment.py
--rw-r--r--   0 luca      (1000) luca      (1000)     1177 2024-02-11 23:08:35.000000 hcr_cell_typist-0.1.0/cell_typist/core/merge.py
--rw-r--r--   0 luca      (1000) luca      (1000)     2574 2024-01-14 12:45:26.000000 hcr_cell_typist-0.1.0/cell_typist/core/serializer.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/measure/
--rw-r--r--   0 luca      (1000) luca      (1000)      141 2024-02-19 20:25:17.000000 hcr_cell_typist-0.1.0/cell_typist/measure/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     9709 2024-02-19 20:25:19.000000 hcr_cell_typist-0.1.0/cell_typist/measure/measure.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/preprocess/
--rw-r--r--   0 luca      (1000) luca      (1000)      169 2024-01-23 21:31:40.000000 hcr_cell_typist-0.1.0/cell_typist/preprocess/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)    11741 2024-03-03 11:07:34.000000 hcr_cell_typist-0.1.0/cell_typist/preprocess/feature_extraction.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/tests/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-29 15:32:58.000000 hcr_cell_typist-0.1.0/cell_typist/tests/__init__.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/tests/core/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-29 15:33:45.000000 hcr_cell_typist-0.1.0/cell_typist/tests/core/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)    16899 2024-05-03 13:12:05.000000 hcr_cell_typist-0.1.0/cell_typist/tests/core/test_datatypes.py
--rw-r--r--   0 luca      (1000) luca      (1000)    25735 2024-01-09 21:57:08.000000 hcr_cell_typist-0.1.0/cell_typist/tests/core/test_experiment.py
--rw-r--r--   0 luca      (1000) luca      (1000)     1799 2024-01-14 12:41:58.000000 hcr_cell_typist-0.1.0/cell_typist/tests/core/test_serializer.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/tests/measure/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2024-01-02 15:15:58.000000 hcr_cell_typist-0.1.0/cell_typist/tests/measure/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     9865 2024-02-04 23:08:09.000000 hcr_cell_typist-0.1.0/cell_typist/tests/measure/test_measure.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/tests/preprocess/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-30 10:12:47.000000 hcr_cell_typist-0.1.0/cell_typist/tests/preprocess/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)    16021 2024-01-23 21:31:40.000000 hcr_cell_typist-0.1.0/cell_typist/tests/preprocess/test_feature_extraction.py
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-29 16:21:41.000000 hcr_cell_typist-0.1.0/cell_typist/tests/test_load_experiments.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/tests/view/
--rw-r--r--   0 luca      (1000) luca      (1000)        0 2024-01-04 10:26:36.000000 hcr_cell_typist-0.1.0/cell_typist/tests/view/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)     2683 2024-02-02 13:45:27.000000 hcr_cell_typist-0.1.0/cell_typist/tests/view/test_factories.py
--rw-r--r--   0 luca      (1000) luca      (1000)     4724 2024-02-02 13:45:27.000000 hcr_cell_typist-0.1.0/cell_typist/tests/view/test_plot.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/cell_typist/view/
--rw-r--r--   0 luca      (1000) luca      (1000)       47 2024-01-22 19:15:47.000000 hcr_cell_typist-0.1.0/cell_typist/view/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1000)    11764 2024-05-06 12:26:28.000000 hcr_cell_typist-0.1.0/cell_typist/view/factories.py
--rw-r--r--   0 luca      (1000) luca      (1000)    10449 2024-05-06 12:44:02.000000 hcr_cell_typist-0.1.0/cell_typist/view/plot.py
-drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1000)     3185 2024-05-06 13:51:38.000000 hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1000)     1146 2024-05-06 13:51:38.000000 hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1000)        1 2024-05-06 13:51:38.000000 hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1000)      147 2024-05-06 13:51:38.000000 hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/requires.txt
--rw-r--r--   0 luca      (1000) luca      (1000)       12 2024-05-06 13:51:38.000000 hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/top_level.txt
--rw-r--r--   0 luca      (1000) luca      (1000)      805 2024-05-06 13:50:13.000000 hcr_cell_typist-0.1.0/pyproject.toml
--rw-r--r--   0 luca      (1000) luca      (1000)       38 2024-05-06 13:51:38.826991 hcr_cell_typist-0.1.0/setup.cfg
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/
+-rw-r--r--   0 luca      (1000) luca      (1000)     1057 2024-05-03 14:06:12.000000 hcr_cell_typist-0.1.1/LICENSE
+-rw-r--r--   0 luca      (1000) luca      (1000)     3186 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)     1378 2024-05-06 13:51:26.000000 hcr_cell_typist-0.1.1/README.md
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/
+-rw-r--r--   0 luca      (1000) luca      (1000)      451 2024-05-16 13:18:22.000000 hcr_cell_typist-0.1.1/cell_typist/__init__.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/core/
+-rw-r--r--   0 luca      (1000) luca      (1000)      158 2024-02-11 23:13:03.000000 hcr_cell_typist-0.1.1/cell_typist/core/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    16020 2024-05-06 08:33:15.000000 hcr_cell_typist-0.1.1/cell_typist/core/datatypes.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    13554 2024-01-14 13:00:14.000000 hcr_cell_typist-0.1.1/cell_typist/core/experiment.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     1177 2024-02-11 23:08:35.000000 hcr_cell_typist-0.1.1/cell_typist/core/merge.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     2574 2024-01-14 12:45:26.000000 hcr_cell_typist-0.1.1/cell_typist/core/serializer.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/measure/
+-rw-r--r--   0 luca      (1000) luca      (1000)      141 2024-02-19 20:25:17.000000 hcr_cell_typist-0.1.1/cell_typist/measure/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     9886 2024-05-07 20:58:18.000000 hcr_cell_typist-0.1.1/cell_typist/measure/measure.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/preprocess/
+-rw-r--r--   0 luca      (1000) luca      (1000)      169 2024-01-23 21:31:40.000000 hcr_cell_typist-0.1.1/cell_typist/preprocess/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    11741 2024-03-03 11:07:34.000000 hcr_cell_typist-0.1.1/cell_typist/preprocess/feature_extraction.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/tests/
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-29 15:32:58.000000 hcr_cell_typist-0.1.1/cell_typist/tests/__init__.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/tests/core/
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-29 15:33:45.000000 hcr_cell_typist-0.1.1/cell_typist/tests/core/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    16899 2024-05-03 13:12:05.000000 hcr_cell_typist-0.1.1/cell_typist/tests/core/test_datatypes.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    25735 2024-01-09 21:57:08.000000 hcr_cell_typist-0.1.1/cell_typist/tests/core/test_experiment.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     1799 2024-01-14 12:41:58.000000 hcr_cell_typist-0.1.1/cell_typist/tests/core/test_serializer.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/tests/measure/
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2024-01-02 15:15:58.000000 hcr_cell_typist-0.1.1/cell_typist/tests/measure/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     9865 2024-02-04 23:08:09.000000 hcr_cell_typist-0.1.1/cell_typist/tests/measure/test_measure.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/tests/preprocess/
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-30 10:12:47.000000 hcr_cell_typist-0.1.1/cell_typist/tests/preprocess/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    16021 2024-01-23 21:31:40.000000 hcr_cell_typist-0.1.1/cell_typist/tests/preprocess/test_feature_extraction.py
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2023-12-29 16:21:41.000000 hcr_cell_typist-0.1.1/cell_typist/tests/test_load_experiments.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/tests/view/
+-rw-r--r--   0 luca      (1000) luca      (1000)        0 2024-01-04 10:26:36.000000 hcr_cell_typist-0.1.1/cell_typist/tests/view/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     2683 2024-02-02 13:45:27.000000 hcr_cell_typist-0.1.1/cell_typist/tests/view/test_factories.py
+-rw-r--r--   0 luca      (1000) luca      (1000)     4724 2024-02-02 13:45:27.000000 hcr_cell_typist-0.1.1/cell_typist/tests/view/test_plot.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/cell_typist/view/
+-rw-r--r--   0 luca      (1000) luca      (1000)       47 2024-01-22 19:15:47.000000 hcr_cell_typist-0.1.1/cell_typist/view/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    11764 2024-05-06 12:26:28.000000 hcr_cell_typist-0.1.1/cell_typist/view/factories.py
+-rw-r--r--   0 luca      (1000) luca      (1000)    10449 2024-05-06 12:44:02.000000 hcr_cell_typist-0.1.1/cell_typist/view/plot.py
+drwxr-xr-x   0 luca      (1000) luca      (1000)        0 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/
+-rw-r--r--   0 luca      (1000) luca      (1000)     3186 2024-05-16 13:18:32.000000 hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1000)     1146 2024-05-16 13:18:32.000000 hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)        1 2024-05-16 13:18:32.000000 hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)      147 2024-05-16 13:18:32.000000 hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/requires.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)       12 2024-05-16 13:18:32.000000 hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/top_level.txt
+-rw-r--r--   0 luca      (1000) luca      (1000)      806 2024-05-16 12:03:37.000000 hcr_cell_typist-0.1.1/pyproject.toml
+-rw-r--r--   0 luca      (1000) luca      (1000)       38 2024-05-16 13:18:32.170214 hcr_cell_typist-0.1.1/setup.cfg
```

### Comparing `hcr_cell_typist-0.1.0/LICENSE` & `hcr_cell_typist-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/PKG-INFO` & `hcr_cell_typist-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hcr-cell-typist
-Version: 0.1.0
-Summary: A libray to aid cell type classification in HCR experiments, downstream of QuPath
+Version: 0.1.1
+Summary: A library to aid cell type classification in HCR experiments, downstream of QuPath
 Author-email: Luca Masin <luca.masin@kuleuven.be>
 License: Copyright 2024 Luca Masin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `hcr_cell_typist-0.1.0/README.md` & `hcr_cell_typist-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/core/datatypes.py` & `hcr_cell_typist-0.1.1/cell_typist/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/core/experiment.py` & `hcr_cell_typist-0.1.1/cell_typist/core/experiment.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/core/merge.py` & `hcr_cell_typist-0.1.1/cell_typist/core/merge.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/core/serializer.py` & `hcr_cell_typist-0.1.1/cell_typist/core/serializer.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/measure/measure.py` & `hcr_cell_typist-0.1.1/cell_typist/measure/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,29 +218,32 @@
     df_densities = (
         df.groupby(full_groupby)[full_data_columns].sum(numeric_only=True).reset_index()
     )
     df_densities_metadata = (
         df.groupby(full_groupby)[missing_metadata].first().reset_index()
     )
     df_densities = pd.merge(df_densities, df_densities_metadata, how="left")
+    df_densities["DAPI_pos"] = (
+        df.groupby(full_groupby)["Object ID"].count().reset_index()["Object ID"].values
+    )
+    data_columns.append("DAPI_pos")
 
     grouped_area = experiment.annotations.dataframe.groupby(full_groupby)['area'].sum().reset_index()
     df_densities = df_densities.merge(grouped_area, on='Image', how='left')
 
     rename_dict = {col: col.replace("_x", "") for col in df_densities.columns if col.endswith("_x")}
     df_densities = df_densities.rename(columns=rename_dict)
     df_densities.drop(columns=[col for col in df_densities.columns if col.endswith("_y")], inplace=True)
 
-
     for column in data_columns:
         df_densities[f"{column}_density"] = (
             df_densities[column] / df_densities["area"]
         ).round(decimals=decimals)
 
-    new_data_columns = data_columns + [f"{column}_density" for column in data_columns] + ["area"]
+    new_data_columns = data_columns + [f"{column}_density" for column in data_columns] + ["DAPI_pos"] + ["area"]
     df_densities_grouped = df_densities.groupby(groupby)[new_data_columns].mean().reset_index()
     df_densities_metadata = df_densities.groupby(groupby)[missing_metadata].first().reset_index()
     df_densities = pd.merge(df_densities_grouped, df_densities_metadata, how="left")
 
     df_densities["area"] = df_densities["area"].round(decimals=4)
 
     rename_dict = {}
```

### Comparing `hcr_cell_typist-0.1.0/cell_typist/preprocess/feature_extraction.py` & `hcr_cell_typist-0.1.1/cell_typist/preprocess/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/core/test_datatypes.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/core/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/core/test_experiment.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/core/test_experiment.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/core/test_serializer.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/core/test_serializer.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/measure/test_measure.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/measure/test_measure.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/preprocess/test_feature_extraction.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/preprocess/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/view/test_factories.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/view/test_factories.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/tests/view/test_plot.py` & `hcr_cell_typist-0.1.1/cell_typist/tests/view/test_plot.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/view/factories.py` & `hcr_cell_typist-0.1.1/cell_typist/view/factories.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/cell_typist/view/plot.py` & `hcr_cell_typist-0.1.1/cell_typist/view/plot.py`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/PKG-INFO` & `hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hcr-cell-typist
-Version: 0.1.0
-Summary: A libray to aid cell type classification in HCR experiments, downstream of QuPath
+Version: 0.1.1
+Summary: A library to aid cell type classification in HCR experiments, downstream of QuPath
 Author-email: Luca Masin <luca.masin@kuleuven.be>
 License: Copyright 2024 Luca Masin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `hcr_cell_typist-0.1.0/hcr_cell_typist.egg-info/SOURCES.txt` & `hcr_cell_typist-0.1.1/hcr_cell_typist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcr_cell_typist-0.1.0/pyproject.toml` & `hcr_cell_typist-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hcr-cell-typist"
-version = "0.1.0"
-description = "A libray to aid cell type classification in HCR experiments, downstream of QuPath"
+version = "0.1.1"
+description = "A library to aid cell type classification in HCR experiments, downstream of QuPath"
 readme = "README.md"
 authors = [{name = "Luca Masin", email = "luca.masin@kuleuven.be"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

