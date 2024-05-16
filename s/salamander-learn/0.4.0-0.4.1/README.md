# Comparing `tmp/salamander_learn-0.4.0.tar.gz` & `tmp/salamander_learn-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salamander_learn-0.4.0.tar", max compression
+gzip compressed data, was "salamander_learn-0.4.1.tar", max compression
```

## Comparing `salamander_learn-0.4.0.tar` & `salamander_learn-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2023-10-08 04:31:09.634064 salamander_learn-0.4.0/LICENSE
--rw-r--r--   0        0        0     2147 2023-12-21 02:00:44.373048 salamander_learn-0.4.0/README.md
--rw-r--r--   0        0        0     1075 2024-05-01 04:04:13.076830 salamander_learn-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      361 2024-05-01 03:58:25.637316 salamander_learn-0.4.0/src/salamander/__init__.py
--rw-r--r--   0        0        0     3166 2023-10-10 17:36:04.452813 salamander_learn-0.4.0/src/salamander/consts.py
--rw-r--r--   0        0        0        3 2023-09-26 18:20:20.939787 salamander_learn-0.4.0/src/salamander/initialization/__init__.py
--rw-r--r--   0        0        0    15419 2024-04-30 20:56:45.838201 salamander_learn-0.4.0/src/salamander/initialization/initialize.py
--rw-r--r--   0        0        0     4345 2024-04-23 20:18:44.627278 salamander_learn-0.4.0/src/salamander/initialization/methods.py
--rw-r--r--   0        0        0      251 2024-04-29 19:11:36.770386 salamander_learn-0.4.0/src/salamander/models/__init__.py
--rw-r--r--   0        0        0    12338 2024-04-29 21:31:58.001850 salamander_learn-0.4.0/src/salamander/models/_utils_corrnmf.py
--rw-r--r--   0        0        0     9270 2024-04-23 22:15:45.379682 salamander_learn-0.4.0/src/salamander/models/_utils_klnmf.py
--rw-r--r--   0        0        0     7977 2024-05-01 03:11:23.599717 salamander_learn-0.4.0/src/salamander/models/corrnmf.py
--rw-r--r--   0        0        0     6012 2024-04-29 21:55:04.012896 salamander_learn-0.4.0/src/salamander/models/corrnmf_det.py
--rw-r--r--   0        0        0     5005 2024-04-29 19:15:29.940852 salamander_learn-0.4.0/src/salamander/models/klnmf.py
--rw-r--r--   0        0        0    25340 2024-05-01 03:11:23.599717 salamander_learn-0.4.0/src/salamander/models/mmcorrnmf.py
--rw-r--r--   0        0        0     6502 2024-04-29 19:15:29.944852 salamander_learn-0.4.0/src/salamander/models/mvnmf.py
--rw-r--r--   0        0        0    20245 2024-04-30 20:50:17.794896 salamander_learn-0.4.0/src/salamander/models/signature_nmf.py
--rw-r--r--   0        0        0     3073 2024-04-30 20:58:47.519140 salamander_learn-0.4.0/src/salamander/models/standard_nmf.py
--rw-r--r--   0        0        0    23831 2024-04-30 21:10:02.971940 salamander_learn-0.4.0/src/salamander/plot.py
--rw-r--r--   0        0        0     5137 2024-04-30 19:28:21.403318 salamander_learn-0.4.0/src/salamander/tools.py
--rw-r--r--   0        0        0     5788 2024-04-30 19:28:21.403318 salamander_learn-0.4.0/src/salamander/utils.py
--rw-r--r--   0        0        0     3226 1970-01-01 00:00:00.000000 salamander_learn-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-08 04:31:09.634064 salamander_learn-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2171 2024-05-02 20:41:48.946735 salamander_learn-0.4.1/README.md
+-rw-r--r--   0        0        0     1075 2024-05-16 14:37:00.721550 salamander_learn-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      361 2024-05-16 14:37:16.258507 salamander_learn-0.4.1/src/salamander/__init__.py
+-rw-r--r--   0        0        0     3166 2023-10-10 17:36:04.452813 salamander_learn-0.4.1/src/salamander/consts.py
+-rw-r--r--   0        0        0        3 2024-05-02 20:41:48.950735 salamander_learn-0.4.1/src/salamander/initialization/__init__.py
+-rw-r--r--   0        0        0    15419 2024-05-02 20:41:48.950735 salamander_learn-0.4.1/src/salamander/initialization/initialize.py
+-rw-r--r--   0        0        0     4345 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/initialization/methods.py
+-rw-r--r--   0        0        0      251 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/__init__.py
+-rw-r--r--   0        0        0    12338 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/_utils_corrnmf.py
+-rw-r--r--   0        0        0     9270 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/_utils_klnmf.py
+-rw-r--r--   0        0        0     7977 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/corrnmf.py
+-rw-r--r--   0        0        0     6012 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/corrnmf_det.py
+-rw-r--r--   0        0        0     5005 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/klnmf.py
+-rw-r--r--   0        0        0    25340 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/mmcorrnmf.py
+-rw-r--r--   0        0        0     6502 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/mvnmf.py
+-rw-r--r--   0        0        0    20384 2024-05-16 14:35:05.179845 salamander_learn-0.4.1/src/salamander/models/signature_nmf.py
+-rw-r--r--   0        0        0     3073 2024-05-02 20:41:48.954735 salamander_learn-0.4.1/src/salamander/models/standard_nmf.py
+-rw-r--r--   0        0        0    23831 2024-05-02 20:41:48.958735 salamander_learn-0.4.1/src/salamander/plot.py
+-rw-r--r--   0        0        0     5137 2024-05-02 20:41:48.958735 salamander_learn-0.4.1/src/salamander/tools.py
+-rw-r--r--   0        0        0     5788 2024-05-02 20:41:48.958735 salamander_learn-0.4.1/src/salamander/utils.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 salamander_learn-0.4.1/PKG-INFO
```

### Comparing `salamander_learn-0.4.0/LICENSE` & `salamander_learn-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/README.md` & `salamander_learn-0.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 [python-image]: https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue.svg
 [python-url]: https://github.com/parklab/salamander
 [license-image]: https://img.shields.io/badge/License-MIT-yellow.svg
 [license-url]: https://github.com/parklab/salamander/blob/main/LICENSE
 [style-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [style-url]: https://github.com/psf/black
 
-Salamander is a non-negative matrix factorization (NMF) framework for signature analysis.
-It implements multiple NMF algorithms, common visualizations, and can be easily customized & expanded.
+Salamander is a non-negative matrix factorization (NMF) framework for signature analysis build on top of [AnnData](https://anndata.readthedocs.io/en/latest/) and [MuData](https://mudata.readthedocs.io/en/latest/). It implements multiple NMF algorithms, common visualizations, and can be easily customized & expanded.
 
 ---
 
 ## Installation
 
 PyPI:
 ```bash
@@ -24,39 +23,37 @@
 ```
 
 ## Usage
 
 The following example illustrates the basic syntax:
 
 ```python
-import pandas as pd
-import salamander
+import anndata as ad
+import salamander as sal
 
-# samples and features have to be named appropriately
-data_path = "..."
-data = pd.read_csv(data_path, index_col=0)
-
-# NMF with a Poisson noise model
-model = salamander.KLNMF(n_signatures=5)
-model.fit(data)
+# initialize data
+adata = ad.AnnData(...)
+
+# NMF with Poisson noise
+model = sal.models.KLNMF(n_signatures=5)
+model.fit(adata)
 
 # barplot
 model.plot_signatures()
 
 # stacked barplot
 model.plot_exposures()
 
 # signature correlation
 model.plot_correlation()
 
 # sample_correlation
 model.plot_correlation(data="samples")
 
 # dimensionality reduction of the exposures
-# method: umap, pca or tsne
 model.plot_embeddings(method="umap")
 ```
 
 For examples of how to customize any NMF algorithm and the plots, check out [the tutorial](https://github.com/parklab/salamander/blob/main/tutorial.ipynb). The following algorithms are currently available:
 * [NMF with KL-divergence loss](https://proceedings.neurips.cc/paper_files/paper/2000/file/f9d1152547c0bde01830b7e8bd60024c-Paper.pdf)
 * [minimum-volume NMF](https://browse.arxiv.org/pdf/1907.02404.pdf)
 * [a variant of correlated NMF](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=87224164eef14589b137547a3fa81f06eef9bbf4)
```

### Comparing `salamander_learn-0.4.0/pyproject.toml` & `salamander_learn-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salamander-learn"
-version = "0.4.0"
+version = "0.4.1"
 description = "Salamander is a non-negative matrix factorization framework for signature analysis"
 license = "MIT"
 authors = ["Benedikt Geiger"]
 maintainers = [
     "Benedikt Geiger <benedikt_geiger@hms.harvard.edu>",
 ]
 packages = [{ include = "salamander", from = "src" }]
```

### Comparing `salamander_learn-0.4.0/src/salamander/consts.py` & `salamander_learn-0.4.1/src/salamander/consts.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/initialization/initialize.py` & `salamander_learn-0.4.1/src/salamander/initialization/initialize.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/initialization/methods.py` & `salamander_learn-0.4.1/src/salamander/initialization/methods.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/_utils_corrnmf.py` & `salamander_learn-0.4.1/src/salamander/models/_utils_corrnmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/_utils_klnmf.py` & `salamander_learn-0.4.1/src/salamander/models/_utils_klnmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/corrnmf.py` & `salamander_learn-0.4.1/src/salamander/models/corrnmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/corrnmf_det.py` & `salamander_learn-0.4.1/src/salamander/models/corrnmf_det.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/klnmf.py` & `salamander_learn-0.4.1/src/salamander/models/klnmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/mmcorrnmf.py` & `salamander_learn-0.4.1/src/salamander/models/mmcorrnmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/mvnmf.py` & `salamander_learn-0.4.1/src/salamander/models/mvnmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/models/signature_nmf.py` & `salamander_learn-0.4.1/src/salamander/models/signature_nmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,26 +384,30 @@
 
         return self
 
     def reorder(
         self,
         asignatures_other: AnnData,
         metric: str = "cosine",
+        keep_names=False,
     ) -> None:
         """
         Reorder the model parameters to match the order of another
         collection of signatures.
         """
+        names = self.asignatures.obs_names
         reordered_indices = match_signatures_pair(
-            asignatures_other.to_df().T, self.asignatures.to_df().T, metric=metric
+            asignatures_other.to_df(), self.asignatures.to_df(), metric=metric
         )
         self.asignatures = self.asignatures[reordered_indices, :].copy()
         self.adata.obsm["exposures"] = self.adata.obsm["exposures"][
             :, reordered_indices
         ]
+        if not keep_names:
+            self.asignatures.obs_names = names
 
     def plot_history(self, outfile: str | None = None, **kwargs) -> Axes:
         """
         Plot the history of the objective function values. See
         the implemenation of 'history' in the plotting module.
         """
         assert "objective_function" in self.history, (
```

### Comparing `salamander_learn-0.4.0/src/salamander/models/standard_nmf.py` & `salamander_learn-0.4.1/src/salamander/models/standard_nmf.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/plot.py` & `salamander_learn-0.4.1/src/salamander/plot.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/tools.py` & `salamander_learn-0.4.1/src/salamander/tools.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/src/salamander/utils.py` & `salamander_learn-0.4.1/src/salamander/utils.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.4.0/PKG-INFO` & `salamander_learn-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salamander-learn
-Version: 0.4.0
+Version: 0.4.1
 Summary: Salamander is a non-negative matrix factorization framework for signature analysis
 License: MIT
 Author: Benedikt Geiger
 Maintainer: Benedikt Geiger
 Maintainer-email: benedikt_geiger@hms.harvard.edu
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -35,16 +35,15 @@
 [python-image]: https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue.svg
 [python-url]: https://github.com/parklab/salamander
 [license-image]: https://img.shields.io/badge/License-MIT-yellow.svg
 [license-url]: https://github.com/parklab/salamander/blob/main/LICENSE
 [style-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [style-url]: https://github.com/psf/black
 
-Salamander is a non-negative matrix factorization (NMF) framework for signature analysis.
-It implements multiple NMF algorithms, common visualizations, and can be easily customized & expanded.
+Salamander is a non-negative matrix factorization (NMF) framework for signature analysis build on top of [AnnData](https://anndata.readthedocs.io/en/latest/) and [MuData](https://mudata.readthedocs.io/en/latest/). It implements multiple NMF algorithms, common visualizations, and can be easily customized & expanded.
 
 ---
 
 ## Installation
 
 PyPI:
 ```bash
@@ -52,39 +51,37 @@
 ```
 
 ## Usage
 
 The following example illustrates the basic syntax:
 
 ```python
-import pandas as pd
-import salamander
+import anndata as ad
+import salamander as sal
 
-# samples and features have to be named appropriately
-data_path = "..."
-data = pd.read_csv(data_path, index_col=0)
-
-# NMF with a Poisson noise model
-model = salamander.KLNMF(n_signatures=5)
-model.fit(data)
+# initialize data
+adata = ad.AnnData(...)
+
+# NMF with Poisson noise
+model = sal.models.KLNMF(n_signatures=5)
+model.fit(adata)
 
 # barplot
 model.plot_signatures()
 
 # stacked barplot
 model.plot_exposures()
 
 # signature correlation
 model.plot_correlation()
 
 # sample_correlation
 model.plot_correlation(data="samples")
 
 # dimensionality reduction of the exposures
-# method: umap, pca or tsne
 model.plot_embeddings(method="umap")
 ```
 
 For examples of how to customize any NMF algorithm and the plots, check out [the tutorial](https://github.com/parklab/salamander/blob/main/tutorial.ipynb). The following algorithms are currently available:
 * [NMF with KL-divergence loss](https://proceedings.neurips.cc/paper_files/paper/2000/file/f9d1152547c0bde01830b7e8bd60024c-Paper.pdf)
 * [minimum-volume NMF](https://browse.arxiv.org/pdf/1907.02404.pdf)
 * [a variant of correlated NMF](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=87224164eef14589b137547a3fa81f06eef9bbf4)
```

