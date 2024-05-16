# Comparing `tmp/mlops_ods-0.1.202405121821.tar.gz` & `tmp/mlops_ods-0.1.202405161324.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_ods-0.1.202405121821.tar", max compression
+gzip compressed data, was "mlops_ods-0.1.202405161324.tar", max compression
```

## Comparing `mlops_ods-0.1.202405121821.tar` & `mlops_ods-0.1.202405161324.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1015 2024-05-12 18:21:01.370671 mlops_ods-0.1.202405121821/README.md
--rw-r--r--   0        0        0      899 2024-05-12 18:21:33.678687 mlops_ods-0.1.202405121821/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/app/__init__.py
--rw-r--r--   0        0        0       50 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/app/example.py
--rw-r--r--   0        0        0       69 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/conf/config.yaml
--rw-r--r--   0        0        0      287 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/conf/features/features.yaml
--rw-r--r--   0        0        0      103 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/conf/model/fast.yaml
--rw-r--r--   0        0        0      103 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/conf/model/slow.yaml
--rw-r--r--   0        0        0      146 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/conf/settings/predict.yaml
--rw-r--r--   0        0        0      183 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/conf/settings/train.yaml
--rw-r--r--   0        0        0      702 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/config.py
--rw-r--r--   0        0        0      113 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dataset/.gitignore
--rw-r--r--   0        0        0      122 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dataset/2015-street-tree-census-tree-data.csv.dvc
--rw-r--r--   0        0        0       21 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dataset/features/.gitignore
--rw-r--r--   0        0        0       74 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dataset/prepared/.gitignore
--rw-r--r--   0        0        0       11 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dataset/processed/.gitignore
--rw-r--r--   0        0        0       47 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/__init__.py
--rw-r--r--   0        0        0      127 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/__main__.py
--rw-r--r--   0        0        0       50 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/cli.py
--rw-r--r--   0        0        0     1845 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/dvc-research.md
--rw-r--r--   0        0        0     2585 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/models.py
--rw-r--r--   0        0        0      500 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/preprocessing.py
--rw-r--r--   0        0        0     2013 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/scaler.py
--rw-r--r--   0        0        0       49 2024-05-12 18:21:01.406671 mlops_ods-0.1.202405121821/src/mlops_ods/models/.gitignore
--rw-r--r--   0        0        0  9730898 2024-05-12 18:21:01.430671 mlops_ods-0.1.202405121821/src/mlops_ods/notebooks/eda.ipynb
--rw-r--r--   0        0        0    51114 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/notebooks/model.ipynb
--rw-r--r--   0        0        0     7740 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/dag.svg
--rw-r--r--   0        0        0      647 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/model_fit.py
--rw-r--r--   0        0        0      624 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
--rw-r--r--   0        0        0      268 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
--rw-r--r--   0        0        0     1046 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
--rw-r--r--   0        0        0      628 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/snakemake_steps.md
--rw-r--r--   0        0        0     2364 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/train_predict.py
--rw-r--r--   0        0        0        0 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/utils/__init__.py
--rw-r--r--   0        0        0     2262 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/utils/utils_etl.py
--rw-r--r--   0        0        0     2138 2024-05-12 18:21:01.434671 mlops_ods-0.1.202405121821/src/mlops_ods/utils/utils_model.py
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 mlops_ods-0.1.202405121821/PKG-INFO
+-rw-r--r--   0        0        0     1015 2024-05-16 13:23:42.767181 mlops_ods-0.1.202405161324/README.md
+-rw-r--r--   0        0        0      944 2024-05-16 13:24:12.195270 mlops_ods-0.1.202405161324/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/app/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/app/example.py
+-rw-r--r--   0        0        0       69 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/config.yaml
+-rw-r--r--   0        0        0      287 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/features/features.yaml
+-rw-r--r--   0        0        0      103 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/model/fast.yaml
+-rw-r--r--   0        0        0      103 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/model/slow.yaml
+-rw-r--r--   0        0        0      146 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/settings/predict.yaml
+-rw-r--r--   0        0        0      183 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/settings/train.yaml
+-rw-r--r--   0        0        0      702 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/config.py
+-rw-r--r--   0        0        0      113 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/.gitignore
+-rw-r--r--   0        0        0      122 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/2015-street-tree-census-tree-data.csv.dvc
+-rw-r--r--   0        0        0       21 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/features/.gitignore
+-rw-r--r--   0        0        0       74 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/prepared/.gitignore
+-rw-r--r--   0        0        0       11 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/processed/.gitignore
+-rw-r--r--   0        0        0       47 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/__main__.py
+-rw-r--r--   0        0        0       50 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/cli.py
+-rw-r--r--   0        0        0     1845 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/dvc-research.md
+-rw-r--r--   0        0        0     2585 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/models.py
+-rw-r--r--   0        0        0      500 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/preprocessing.py
+-rw-r--r--   0        0        0     2013 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/scaler.py
+-rw-r--r--   0        0        0       49 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/models/.gitignore
+-rw-r--r--   0        0        0  9730898 2024-05-16 13:23:42.831181 mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/eda.ipynb
+-rw-r--r--   0        0        0    51114 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/model.ipynb
+-rw-r--r--   0        0        0     7740 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/dag.svg
+-rw-r--r--   0        0        0      647 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit.py
+-rw-r--r--   0        0        0      624 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
+-rw-r--r--   0        0        0      268 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
+-rw-r--r--   0        0        0     1046 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
+-rw-r--r--   0        0        0      628 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/snakemake_steps.md
+-rw-r--r--   0        0        0     2364 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/train_predict.py
+-rw-r--r--   0        0        0        0 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/utils/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_etl.py
+-rw-r--r--   0        0        0     2138 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_model.py
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlops_ods-0.1.202405161324/PKG-INFO
```

### Comparing `mlops_ods-0.1.202405121821/README.md` & `mlops_ods-0.1.202405161324/README.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/pyproject.toml` & `mlops_ods-0.1.202405161324/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops_ods"
-version = "0.1.202405121821"
+version = "0.1.202405161324"
 description = ""
 authors = ["Iuliia Fokina"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
@@ -19,14 +19,16 @@
 hydra-core = "^1.3.2"
 dvc = "^3.50.1"
 dvc-gdrive = "^3.0.1"
 click = "^8.1.7"
 lakefs-spec = "^0.9.0"
 minio = "^7.2.7"
 mlflow = "^2.12.2"
+clearml = "^1.15.1"
+clearml-agent = "^1.8.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.3.0"
 isort = "^5.13.2"
 mypy = "^1.9.0"
```

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/config.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/config.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/dvc-research.md` & `mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/dvc-research.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/models.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/models.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/dvc_functions/scaler.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/scaler.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/notebooks/eda.ipynb` & `mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/eda.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/notebooks/model.ipynb` & `mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/model.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/dag.svg` & `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/dag.svg`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/model_fit.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/model_fit_bigger.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit_bigger.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/preprocess_data_research.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/preprocess_data_research.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/snakemake_scripts/snakemake_steps.md` & `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/snakemake_steps.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/train_predict.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/train_predict.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/utils/utils_etl.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_etl.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/src/mlops_ods/utils/utils_model.py` & `mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405121821/PKG-INFO` & `mlops_ods-0.1.202405161324/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: mlops_ods
-Version: 0.1.202405121821
+Version: 0.1.202405161324
 Summary: 
 Author: Iuliia Fokina
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: catboost (>=1.2.5,<2.0.0)
+Requires-Dist: clearml (>=1.15.1,<2.0.0)
+Requires-Dist: clearml-agent (>=1.8.0,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: dvc (>=3.50.1,<4.0.0)
 Requires-Dist: dvc-gdrive (>=3.0.1,<4.0.0)
 Requires-Dist: folium (>=0.16.0,<0.17.0)
 Requires-Dist: geodatasets (>=2023.12.0,<2024.0.0)
 Requires-Dist: geopandas (>=0.14.3,<0.15.0)
```

