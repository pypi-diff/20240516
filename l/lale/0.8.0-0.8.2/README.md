# Comparing `tmp/lale-0.8.0.tar.gz` & `tmp/lale-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lale-0.8.0.tar", last modified: Wed Feb 21 13:17:24 2024, max compression
+gzip compressed data, was "lale-0.8.2.tar", last modified: Thu May 16 18:20:20 2024, max compression
```

## Comparing `lale-0.8.0.tar` & `lale-0.8.2.tar`

### file list

```diff
@@ -1,362 +1,363 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-02-21 13:17:24.000000 lale-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-02-21 13:17:15.000000 lale-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-21 13:17:15.000000 lale-0.8.0/lale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24607 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/data_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/movie_review.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/datasets/multitable/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/multitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/multitable/fetch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/multitable/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/datasets/openml/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/openml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/openml/openml_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/sklearn_to_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/datasets/uci/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/uci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/uci/uci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-21 13:17:15.000000 lale-0.8.0/lale/datasets/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-02-21 13:17:15.000000 lale-0.8.0/lale/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-02-21 13:17:15.000000 lale-0.8.0/lale/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-02-21 13:17:15.000000 lale-0.8.0/lale/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)    47546 2024-02-21 13:17:15.000000 lale-0.8.0/lale/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22625 2024-02-21 13:17:15.000000 lale-0.8.0/lale/json_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/_common_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/aif360/
--rw-r--r--   0 runner    (1001) docker     (127)    14239 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/_mystic_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/_suppress_aif360_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/adversarial_debiasing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/bagging_orbis_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/calibrated_eq_odds_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    62291 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/disparate_impact_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/eq_odds_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/gerry_fair_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/lfr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/meta_fair_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/optim_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/orbis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/prejudice_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/protected_attributes_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/redacting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/reject_option_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/reweighing.py
--rw-r--r--   0 runner    (1001) docker     (127)    84991 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/aif360/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/autogen/
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/additive_chi2_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/ard_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/bayesian_ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/bernoulli_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/bernoulli_rbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/birch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/calibrated_classifier_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/cca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/complement_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/dictionary_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/elastic_net.py
--rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/elastic_net_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/factor_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/gaussian_process_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/gaussian_process_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/gaussian_random_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/huber_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/k_bins_discretizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/kernel_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/kernel_ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/label_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/label_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/label_spreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lars_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lasso_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lasso_lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lasso_lars_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/lasso_lars_ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/latent_dirichlet_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/linear_discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/locally_linear_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/logistic_regression_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/max_abs_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/mini_batch_dictionary_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/mini_batch_k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/mini_batch_sparse_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/mlp_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/multi_label_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/multi_task_elastic_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/multi_task_elastic_net_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/multi_task_lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/multi_task_lasso_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/nearest_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/nu_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/nu_svr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/orthogonal_matching_pursuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/orthogonal_matching_pursuit_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/passive_aggressive_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/pls_canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/plssvd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/power_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/radius_neighbors_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/radius_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/random_trees_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/ransac_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/rbf_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/ridge_classifier_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/ridge_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/skewed_chi2_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/sparse_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/sparse_random_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/theil_sen_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/transformed_target_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/autogen/truncated_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/category_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/category_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/category_encoders/hashing_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/category_encoders/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/imblearn/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/adasyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/all_knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/base_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/borderline_smote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/condensed_nearest_neighbour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/edited_nearest_neighbours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/instance_hardness_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/random_over_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/random_under_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/repeated_edited_nearest_neighbours.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/smote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/smoteenn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/smoten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/smotenc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/imblearn/svm_smote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/lale/
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/auto_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/both.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/concat_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/grid_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    18211 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/halving_grid_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/identity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/no_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/observing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/optimize_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/optimize_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/sample_based_voting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/smac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/tee.py
--rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/time_series_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lale/topk_voting_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/lightgbm/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lightgbm/lgbm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/lightgbm/lgbm_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/rasl/
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/_eval_pandas_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/_eval_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/batched_bagging_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/concat_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/hashing_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/min_max_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/monoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/orderby.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/ordinal_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17822 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/select_k_best.py
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/simple_imputer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/sort_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/spark_explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/split_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    57980 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/rasl/task_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12339 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/ada_boost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/ada_boost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/bagging_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/bagging_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/decision_tree_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/dummy_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/dummy_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/extra_trees_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/extra_trees_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/feature_agglomeration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/fit_spec_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/gaussian_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/gradient_boosting_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/isolation_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/isomap.py
--rw-r--r--   0 runner    (1001) docker     (127)    14041 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/k_means.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/k_neighbors_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/k_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13033 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/linear_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/linear_svr.py
--rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/min_max_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/missing_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/mlp_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/multi_output_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/multinomial_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/nmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/nystroem.py
--rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/ordinal_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/passive_aggressive_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/polynomial_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/quadratic_discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/quantile_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20568 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/random_forest_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/rfe.py
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/ridge_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/robust_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/select_k_best.py
--rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/sgd_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/sgd_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/simple_imputer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/stacking_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/stacking_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/stacking_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/svr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/target_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/tfidf_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/variance_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/voting_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/sklearn/voting_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/snapml/
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/batched_tree_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/batched_tree_ensemble_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_boosting_machine_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_boosting_machine_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_decision_tree_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_random_forest_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/snapml/snap_svm_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/lib/xgboost/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/xgboost/_common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    36460 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/xgboost/xgb_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    33671 2024-02-21 13:17:15.000000 lale-0.8.0/lale/lib/xgboost/xgb_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-21 13:17:15.000000 lale-0.8.0/lale/operator_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)   214694 2024-02-21 13:17:15.000000 lale-0.8.0/lale/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29239 2024-02-21 13:17:15.000000 lale-0.8.0/lale/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:15.000000 lale-0.8.0/lale/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-02-21 13:17:15.000000 lale-0.8.0/lale/schema2enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-02-21 13:17:15.000000 lale-0.8.0/lale/schema_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)    43950 2024-02-21 13:17:15.000000 lale-0.8.0/lale/schema_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-02-21 13:17:15.000000 lale-0.8.0/lale/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-21 13:17:15.000000 lale-0.8.0/lale/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/search/
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/PGO.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/lale_grid_search_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    19805 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/lale_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/lale_smac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/op2hp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23863 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/schema2search_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/search_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-02-21 13:17:15.000000 lale-0.8.0/lale/search/search_space_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-21 13:17:15.000000 lale-0.8.0/lale/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-21 13:17:15.000000 lale-0.8.0/lale/sklearn_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-02-21 13:17:15.000000 lale-0.8.0/lale/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/Visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/VisitorMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/VisitorPathError.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/batch_data_dictionary_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/hdf5_to_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/numpy_to_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/numpy_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/pandas_to_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-21 13:17:15.000000 lale-0.8.0/lale/util/pandas_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-02-21 13:17:15.000000 lale-0.8.0/lale/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/lale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-02-21 13:17:24.000000 lale-0.8.0/lale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-02-21 13:17:24.000000 lale-0.8.0/lale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 13:17:24.000000 lale-0.8.0/lale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-21 13:17:24.000000 lale-0.8.0/lale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-21 13:17:24.000000 lale-0.8.0/lale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 13:17:24.000000 lale-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-02-21 13:17:15.000000 lale-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:17:24.000000 lale-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-21 13:17:15.000000 lale-0.8.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-21 13:17:15.000000 lale-0.8.0/test/mock_custom_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-21 13:17:15.000000 lale-0.8.0/test/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    69121 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_aif360.py
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_aif360_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_autogen_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    27541 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_core_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    49416 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_core_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    48983 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_core_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_core_regressors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_core_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27885 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_custom_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_halving_gridsearchcv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_interoperability.py
--rw-r--r--   0 runner    (1001) docker     (127)    45993 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_json_pretty_viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_nlp_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    44900 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_pgo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)   110832 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_relational.py
--rw-r--r--   0 runner    (1001) docker     (127)    18521 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_relational_from_sklearn_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)   104153 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_relational_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_sklearn_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_snapml.py
--rw-r--r--   0 runner    (1001) docker     (127)    58716 2024-02-21 13:17:15.000000 lale-0.8.0/test/test_type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.186519 lale-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-16 18:20:12.000000 lale-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-16 18:20:20.186519 lale-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-16 18:20:12.000000 lale-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.134518 lale-0.8.2/lale/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 18:20:12.000000 lale-0.8.2/lale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.134518 lale-0.8.2/lale/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24607 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/data_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/movie_review.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.134518 lale-0.8.2/lale/datasets/multitable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/multitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/multitable/fetch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/multitable/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.138518 lale-0.8.2/lale/datasets/openml/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/openml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/openml/openml_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/sklearn_to_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.138518 lale-0.8.2/lale/datasets/uci/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/uci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/uci/uci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-16 18:20:12.000000 lale-0.8.2/lale/datasets/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-05-16 18:20:12.000000 lale-0.8.2/lale/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-05-16 18:20:12.000000 lale-0.8.2/lale/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-16 18:20:12.000000 lale-0.8.2/lale/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47546 2024-05-16 18:20:12.000000 lale-0.8.2/lale/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22625 2024-05-16 18:20:12.000000 lale-0.8.2/lale/json_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.138518 lale-0.8.2/lale/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/_common_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.142518 lale-0.8.2/lale/lib/aif360/
+-rw-r--r--   0 runner    (1001) docker     (127)    14239 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/_mystic_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/_suppress_aif360_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/adversarial_debiasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/bagging_orbis_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/calibrated_eq_odds_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62291 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/disparate_impact_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/eq_odds_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/gerry_fair_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/lfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/meta_fair_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/optim_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/orbis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/prejudice_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/protected_attributes_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/redacting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/reject_option_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/reweighing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84991 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/aif360/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.150518 lale-0.8.2/lale/lib/autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/additive_chi2_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/ard_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/bayesian_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/bernoulli_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/bernoulli_rbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/birch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/calibrated_classifier_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/complement_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/dictionary_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/elastic_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/elastic_net_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/factor_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/gaussian_process_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/gaussian_process_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/gaussian_random_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/huber_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/k_bins_discretizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/kernel_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/kernel_ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/label_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/label_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/label_spreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lars_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lasso_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lasso_lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lasso_lars_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/lasso_lars_ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/latent_dirichlet_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12053 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/linear_discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/locally_linear_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/logistic_regression_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/max_abs_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/mini_batch_dictionary_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/mini_batch_k_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/mini_batch_sparse_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/mlp_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/multi_label_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/multi_task_elastic_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/multi_task_elastic_net_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/multi_task_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/multi_task_lasso_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/nearest_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/nu_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/nu_svr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/orthogonal_matching_pursuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/orthogonal_matching_pursuit_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/passive_aggressive_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/pls_canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/plssvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/power_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/radius_neighbors_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/radius_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/random_trees_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/ransac_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/rbf_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/ridge_classifier_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/ridge_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/skewed_chi2_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/sparse_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/sparse_random_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/theil_sen_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/transformed_target_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/autogen/truncated_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.154518 lale-0.8.2/lale/lib/category_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/category_encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/category_encoders/hashing_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/category_encoders/target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.154518 lale-0.8.2/lale/lib/imblearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/adasyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/all_knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/base_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/borderline_smote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/condensed_nearest_neighbour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/edited_nearest_neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/instance_hardness_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/random_over_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/random_under_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/repeated_edited_nearest_neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/smote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/smoteenn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/smoten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/smotenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/imblearn/svm_smote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.158518 lale-0.8.2/lale/lib/lale/
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/auto_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/both.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/concat_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12734 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/grid_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18211 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/halving_grid_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/identity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/no_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/observing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/optimize_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/optimize_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/sample_based_voting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/smac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/tee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/time_series_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lale/topk_voting_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.158518 lale-0.8.2/lale/lib/lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lightgbm/lgbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/lightgbm/lgbm_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.162518 lale-0.8.2/lale/lib/rasl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/_eval_pandas_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/_eval_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/batched_bagging_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/concat_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/hashing_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/min_max_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/monoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/orderby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/ordinal_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17822 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/select_k_best.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/simple_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/sort_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/spark_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/split_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57980 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/rasl/task_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.174519 lale-0.8.2/lale/lib/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12339 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/ada_boost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/ada_boost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/bagging_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/bagging_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/decision_tree_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/dummy_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/dummy_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/extra_trees_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/extra_trees_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/feature_agglomeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/fit_spec_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/gaussian_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/gradient_boosting_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/isolation_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/isomap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14041 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/k_neighbors_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/k_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/linear_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/linear_svr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/min_max_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/missing_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/mlp_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/multi_output_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/multinomial_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/nystroem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/ordinal_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/passive_aggressive_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/polynomial_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/quadratic_discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/quantile_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20568 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/random_forest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/rfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/ridge_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/robust_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/select_k_best.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/sgd_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/sgd_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/simple_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/stacking_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/stacking_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/stacking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/svr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/target_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/tfidf_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/variance_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/voting_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/sklearn/voting_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.174519 lale-0.8.2/lale/lib/snapml/
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/batched_tree_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/batched_tree_ensemble_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_boosting_machine_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_boosting_machine_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_decision_tree_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_random_forest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/snapml/snap_svm_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.178519 lale-0.8.2/lale/lib/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/xgboost/_common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/xgboost/xgb_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33671 2024-05-16 18:20:12.000000 lale-0.8.2/lale/lib/xgboost/xgb_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-16 18:20:12.000000 lale-0.8.2/lale/operator_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   214694 2024-05-16 18:20:12.000000 lale-0.8.2/lale/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29239 2024-05-16 18:20:12.000000 lale-0.8.2/lale/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:12.000000 lale-0.8.2/lale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-16 18:20:12.000000 lale-0.8.2/lale/schema2enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-05-16 18:20:12.000000 lale-0.8.2/lale/schema_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43950 2024-05-16 18:20:12.000000 lale-0.8.2/lale/schema_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-16 18:20:12.000000 lale-0.8.2/lale/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-16 18:20:12.000000 lale-0.8.2/lale/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.178519 lale-0.8.2/lale/search/
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/PGO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/lale_grid_search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19805 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/lale_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/lale_smac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/op2hp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23863 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/schema2search_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-16 18:20:12.000000 lale-0.8.2/lale/search/search_space_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-16 18:20:12.000000 lale-0.8.2/lale/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-16 18:20:12.000000 lale-0.8.2/lale/sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-05-16 18:20:12.000000 lale-0.8.2/lale/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.178519 lale-0.8.2/lale/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/VisitorMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/VisitorPathError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/batch_data_dictionary_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/hdf5_to_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/numpy_to_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/numpy_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/pandas_to_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-16 18:20:12.000000 lale-0.8.2/lale/util/pandas_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-16 18:20:12.000000 lale-0.8.2/lale/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.134518 lale-0.8.2/lale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-16 18:20:19.000000 lale-0.8.2/lale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11257 2024-05-16 18:20:20.000000 lale-0.8.2/lale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:20:19.000000 lale-0.8.2/lale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 18:20:19.000000 lale-0.8.2/lale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 18:20:19.000000 lale-0.8.2/lale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:20:20.186519 lale-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-16 18:20:12.000000 lale-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:20:20.186519 lale-0.8.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-16 18:20:12.000000 lale-0.8.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-16 18:20:12.000000 lale-0.8.2/test/mock_custom_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-16 18:20:12.000000 lale-0.8.2/test/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69121 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_aif360.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_aif360_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_autogen_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27541 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_core_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49416 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_core_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48983 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_core_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_core_regressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_core_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27885 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_custom_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_halving_gridsearchcv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_interoperability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46419 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_json_pretty_viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_nlp_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44900 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_pgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110832 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18521 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_relational_from_sklearn_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104153 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_relational_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_sklearn_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_snapml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58716 2024-05-16 18:20:12.000000 lale-0.8.2/test/test_type_checking.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lale-0.8.0/PKG-INFO` & `lale-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lale
-Version: 0.8.0
+Version: 0.8.2
 Summary: Library for Semi-Automated Data Science
 Home-page: https://github.com/IBM/lale
 Author: Guillaume Baudart, Martin Hirzel, Kiran Kate, Parikshit Ram, Avraham Shinnar
 License: Apache License 2.0
 Description: # Lale
         
         [![Tests](https://github.com/IBM/lale/workflows/Tests/badge.svg?branch=master)](https://github.com/IBM/lale/actions?query=workflow%3ATests+branch%3Amaster)
```

### Comparing `lale-0.8.0/README.md` & `lale-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/__init__.py` & `lale-0.8.2/lale/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
-__version__ = "0.8.0"
+__version__ = "0.8.2"
 
 try:
     # This variable is injected in the __builtins__ by the build
     # process. It is used to not try to import rest of the lale packages when
     # it is being installed.
     __LALE_SETUP__  # type: ignore  # pylint:disable=used-before-assignment
 except NameError:
```

### Comparing `lale-0.8.0/lale/datasets/__init__.py` & `lale-0.8.2/lale/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/data_schemas.py` & `lale-0.8.2/lale/datasets/data_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/movie_review.py` & `lale-0.8.2/lale/datasets/movie_review.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/multitable/__init__.py` & `lale-0.8.2/lale/datasets/multitable/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/multitable/fetch_datasets.py` & `lale-0.8.2/lale/datasets/multitable/fetch_datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/multitable/util.py` & `lale-0.8.2/lale/datasets/multitable/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/openml/__init__.py` & `lale-0.8.2/lale/datasets/openml/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/openml/openml_datasets.py` & `lale-0.8.2/lale/datasets/openml/openml_datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/sklearn_to_pandas.py` & `lale-0.8.2/lale/datasets/sklearn_to_pandas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/uci/uci_datasets.py` & `lale-0.8.2/lale/datasets/uci/uci_datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/datasets/util.py` & `lale-0.8.2/lale/datasets/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/docstrings.py` & `lale-0.8.2/lale/docstrings.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/expressions.py` & `lale-0.8.2/lale/expressions.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/grammar.py` & `lale-0.8.2/lale/grammar.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/helpers.py` & `lale-0.8.2/lale/helpers.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/json_operator.py` & `lale-0.8.2/lale/json_operator.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/__init__.py` & `lale-0.8.2/lale/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/_common_schemas.py` & `lale-0.8.2/lale/lib/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/__init__.py` & `lale-0.8.2/lale/lib/aif360/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/_mystic_util.py` & `lale-0.8.2/lale/lib/aif360/_mystic_util.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/_suppress_aif360_warnings.py` & `lale-0.8.2/lale/lib/aif360/_suppress_aif360_warnings.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/adversarial_debiasing.py` & `lale-0.8.2/lale/lib/aif360/adversarial_debiasing.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/bagging_orbis_classifier.py` & `lale-0.8.2/lale/lib/aif360/bagging_orbis_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/calibrated_eq_odds_postprocessing.py` & `lale-0.8.2/lale/lib/aif360/calibrated_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/datasets.py` & `lale-0.8.2/lale/lib/aif360/datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/disparate_impact_remover.py` & `lale-0.8.2/lale/lib/aif360/disparate_impact_remover.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/eq_odds_postprocessing.py` & `lale-0.8.2/lale/lib/aif360/eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/gerry_fair_classifier.py` & `lale-0.8.2/lale/lib/aif360/gerry_fair_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/lfr.py` & `lale-0.8.2/lale/lib/aif360/lfr.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/meta_fair_classifier.py` & `lale-0.8.2/lale/lib/aif360/meta_fair_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/optim_preproc.py` & `lale-0.8.2/lale/lib/aif360/optim_preproc.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/orbis.py` & `lale-0.8.2/lale/lib/aif360/orbis.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/prejudice_remover.py` & `lale-0.8.2/lale/lib/aif360/prejudice_remover.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/protected_attributes_encoder.py` & `lale-0.8.2/lale/lib/aif360/protected_attributes_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/redacting.py` & `lale-0.8.2/lale/lib/aif360/redacting.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/reject_option_classification.py` & `lale-0.8.2/lale/lib/aif360/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/reweighing.py` & `lale-0.8.2/lale/lib/aif360/reweighing.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/aif360/util.py` & `lale-0.8.2/lale/lib/aif360/util.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/__init__.py` & `lale-0.8.2/lale/lib/autogen/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/additive_chi2_sampler.py` & `lale-0.8.2/lale/lib/autogen/additive_chi2_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/ard_regression.py` & `lale-0.8.2/lale/lib/autogen/ard_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/bayesian_ridge.py` & `lale-0.8.2/lale/lib/autogen/bayesian_ridge.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/bernoulli_nb.py` & `lale-0.8.2/lale/lib/autogen/bernoulli_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/bernoulli_rbm.py` & `lale-0.8.2/lale/lib/autogen/bernoulli_rbm.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/binarizer.py` & `lale-0.8.2/lale/lib/autogen/binarizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/birch.py` & `lale-0.8.2/lale/lib/autogen/birch.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/calibrated_classifier_cv.py` & `lale-0.8.2/lale/lib/autogen/calibrated_classifier_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/cca.py` & `lale-0.8.2/lale/lib/autogen/cca.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/complement_nb.py` & `lale-0.8.2/lale/lib/autogen/complement_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/dictionary_learning.py` & `lale-0.8.2/lale/lib/autogen/dictionary_learning.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/elastic_net.py` & `lale-0.8.2/lale/lib/autogen/elastic_net.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/elastic_net_cv.py` & `lale-0.8.2/lale/lib/autogen/elastic_net_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/factor_analysis.py` & `lale-0.8.2/lale/lib/autogen/factor_analysis.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/fast_ica.py` & `lale-0.8.2/lale/lib/autogen/fast_ica.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/gaussian_process_classifier.py` & `lale-0.8.2/lale/lib/autogen/gaussian_process_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/gaussian_process_regressor.py` & `lale-0.8.2/lale/lib/autogen/gaussian_process_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/gaussian_random_projection.py` & `lale-0.8.2/lale/lib/autogen/gaussian_random_projection.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/huber_regressor.py` & `lale-0.8.2/lale/lib/autogen/huber_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/incremental_pca.py` & `lale-0.8.2/lale/lib/autogen/incremental_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/k_bins_discretizer.py` & `lale-0.8.2/lale/lib/autogen/k_bins_discretizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/kernel_pca.py` & `lale-0.8.2/lale/lib/autogen/kernel_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/kernel_ridge.py` & `lale-0.8.2/lale/lib/autogen/kernel_ridge.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/label_binarizer.py` & `lale-0.8.2/lale/lib/autogen/label_binarizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/label_encoder.py` & `lale-0.8.2/lale/lib/autogen/label_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/label_propagation.py` & `lale-0.8.2/lale/lib/autogen/label_propagation.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/label_spreading.py` & `lale-0.8.2/lale/lib/autogen/label_spreading.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lars.py` & `lale-0.8.2/lale/lib/autogen/lars.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lars_cv.py` & `lale-0.8.2/lale/lib/autogen/lars_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lasso.py` & `lale-0.8.2/lale/lib/autogen/lasso.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lasso_cv.py` & `lale-0.8.2/lale/lib/autogen/lasso_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lasso_lars.py` & `lale-0.8.2/lale/lib/autogen/lasso_lars.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lasso_lars_cv.py` & `lale-0.8.2/lale/lib/autogen/lasso_lars_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/lasso_lars_ic.py` & `lale-0.8.2/lale/lib/autogen/lasso_lars_ic.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/latent_dirichlet_allocation.py` & `lale-0.8.2/lale/lib/autogen/latent_dirichlet_allocation.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/linear_discriminant_analysis.py` & `lale-0.8.2/lale/lib/autogen/linear_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/locally_linear_embedding.py` & `lale-0.8.2/lale/lib/autogen/locally_linear_embedding.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/logistic_regression_cv.py` & `lale-0.8.2/lale/lib/autogen/logistic_regression_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/max_abs_scaler.py` & `lale-0.8.2/lale/lib/autogen/max_abs_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/mini_batch_dictionary_learning.py` & `lale-0.8.2/lale/lib/autogen/mini_batch_dictionary_learning.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/mini_batch_k_means.py` & `lale-0.8.2/lale/lib/autogen/mini_batch_k_means.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/mini_batch_sparse_pca.py` & `lale-0.8.2/lale/lib/autogen/mini_batch_sparse_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/mlp_regressor.py` & `lale-0.8.2/lale/lib/autogen/mlp_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/multi_label_binarizer.py` & `lale-0.8.2/lale/lib/autogen/multi_label_binarizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/multi_task_elastic_net.py` & `lale-0.8.2/lale/lib/autogen/multi_task_elastic_net.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/multi_task_elastic_net_cv.py` & `lale-0.8.2/lale/lib/autogen/multi_task_elastic_net_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/multi_task_lasso.py` & `lale-0.8.2/lale/lib/autogen/multi_task_lasso.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/multi_task_lasso_cv.py` & `lale-0.8.2/lale/lib/autogen/multi_task_lasso_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/nearest_centroid.py` & `lale-0.8.2/lale/lib/autogen/nearest_centroid.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/nu_svc.py` & `lale-0.8.2/lale/lib/autogen/nu_svc.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/nu_svr.py` & `lale-0.8.2/lale/lib/autogen/nu_svr.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/orthogonal_matching_pursuit.py` & `lale-0.8.2/lale/lib/autogen/orthogonal_matching_pursuit.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/orthogonal_matching_pursuit_cv.py` & `lale-0.8.2/lale/lib/autogen/orthogonal_matching_pursuit_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/passive_aggressive_regressor.py` & `lale-0.8.2/lale/lib/autogen/passive_aggressive_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/perceptron.py` & `lale-0.8.2/lale/lib/autogen/perceptron.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/pls_canonical.py` & `lale-0.8.2/lale/lib/autogen/pls_canonical.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/pls_regression.py` & `lale-0.8.2/lale/lib/autogen/pls_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/plssvd.py` & `lale-0.8.2/lale/lib/autogen/plssvd.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/power_transformer.py` & `lale-0.8.2/lale/lib/autogen/power_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/radius_neighbors_classifier.py` & `lale-0.8.2/lale/lib/autogen/radius_neighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/radius_neighbors_regressor.py` & `lale-0.8.2/lale/lib/autogen/radius_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/random_trees_embedding.py` & `lale-0.8.2/lale/lib/autogen/random_trees_embedding.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/ransac_regressor.py` & `lale-0.8.2/lale/lib/autogen/ransac_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/rbf_sampler.py` & `lale-0.8.2/lale/lib/autogen/rbf_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/ridge_classifier_cv.py` & `lale-0.8.2/lale/lib/autogen/ridge_classifier_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/ridge_cv.py` & `lale-0.8.2/lale/lib/autogen/ridge_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/skewed_chi2_sampler.py` & `lale-0.8.2/lale/lib/autogen/skewed_chi2_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/sparse_pca.py` & `lale-0.8.2/lale/lib/autogen/sparse_pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/sparse_random_projection.py` & `lale-0.8.2/lale/lib/autogen/sparse_random_projection.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/theil_sen_regressor.py` & `lale-0.8.2/lale/lib/autogen/theil_sen_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/transformed_target_regressor.py` & `lale-0.8.2/lale/lib/autogen/transformed_target_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/autogen/truncated_svd.py` & `lale-0.8.2/lale/lib/autogen/truncated_svd.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/category_encoders/__init__.py` & `lale-0.8.2/lale/lib/category_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/category_encoders/hashing_encoder.py` & `lale-0.8.2/lale/lib/category_encoders/hashing_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/category_encoders/target_encoder.py` & `lale-0.8.2/lale/lib/category_encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/dataframe.py` & `lale-0.8.2/lale/lib/dataframe.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/__init__.py` & `lale-0.8.2/lale/lib/imblearn/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/_common_schemas.py` & `lale-0.8.2/lale/lib/imblearn/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/adasyn.py` & `lale-0.8.2/lale/lib/imblearn/adasyn.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/all_knn.py` & `lale-0.8.2/lale/lib/imblearn/all_knn.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/base_resampler.py` & `lale-0.8.2/lale/lib/imblearn/base_resampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/borderline_smote.py` & `lale-0.8.2/lale/lib/imblearn/borderline_smote.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/condensed_nearest_neighbour.py` & `lale-0.8.2/lale/lib/imblearn/condensed_nearest_neighbour.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/edited_nearest_neighbours.py` & `lale-0.8.2/lale/lib/imblearn/edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/instance_hardness_threshold.py` & `lale-0.8.2/lale/lib/imblearn/instance_hardness_threshold.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/random_over_sampler.py` & `lale-0.8.2/lale/lib/imblearn/random_over_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/random_under_sampler.py` & `lale-0.8.2/lale/lib/imblearn/random_under_sampler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/repeated_edited_nearest_neighbours.py` & `lale-0.8.2/lale/lib/imblearn/repeated_edited_nearest_neighbours.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/smote.py` & `lale-0.8.2/lale/lib/imblearn/smote.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/smoteenn.py` & `lale-0.8.2/lale/lib/imblearn/smoteenn.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/smoten.py` & `lale-0.8.2/lale/lib/imblearn/smoten.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/smotenc.py` & `lale-0.8.2/lale/lib/imblearn/smotenc.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/imblearn/svm_smote.py` & `lale-0.8.2/lale/lib/imblearn/svm_smote.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/__init__.py` & `lale-0.8.2/lale/lib/lale/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/auto_pipeline.py` & `lale-0.8.2/lale/lib/lale/auto_pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/both.py` & `lale-0.8.2/lale/lib/lale/both.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/concat_features.py` & `lale-0.8.2/lale/lib/lale/concat_features.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/grid_search_cv.py` & `lale-0.8.2/lale/lib/lale/grid_search_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/halving_grid_search_cv.py` & `lale-0.8.2/lale/lib/lale/halving_grid_search_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/hyperopt.py` & `lale-0.8.2/lale/lib/lale/hyperopt.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/identity_wrapper.py` & `lale-0.8.2/lale/lib/lale/identity_wrapper.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/no_op.py` & `lale-0.8.2/lale/lib/lale/no_op.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/observing.py` & `lale-0.8.2/lale/lib/lale/observing.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/optimize_last.py` & `lale-0.8.2/lale/lib/lale/optimize_last.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/optimize_suffix.py` & `lale-0.8.2/lale/lib/lale/optimize_suffix.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/sample_based_voting.py` & `lale-0.8.2/lale/lib/lale/sample_based_voting.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/smac.py` & `lale-0.8.2/lale/lib/lale/smac.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/tee.py` & `lale-0.8.2/lale/lib/lale/tee.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/time_series_transformer.py` & `lale-0.8.2/lale/lib/lale/time_series_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lale/topk_voting_classifier.py` & `lale-0.8.2/lale/lib/lale/topk_voting_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lightgbm/__init__.py` & `lale-0.8.2/lale/lib/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lightgbm/lgbm_classifier.py` & `lale-0.8.2/lale/lib/lightgbm/lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/lightgbm/lgbm_regressor.py` & `lale-0.8.2/lale/lib/lightgbm/lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/__init__.py` & `lale-0.8.2/lale/lib/rasl/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/_eval_pandas_df.py` & `lale-0.8.2/lale/lib/rasl/_eval_pandas_df.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/_eval_spark_df.py` & `lale-0.8.2/lale/lib/rasl/_eval_spark_df.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/_util.py` & `lale-0.8.2/lale/lib/rasl/_util.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/aggregate.py` & `lale-0.8.2/lale/lib/rasl/aggregate.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/alias.py` & `lale-0.8.2/lale/lib/rasl/alias.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/batched_bagging_classifier.py` & `lale-0.8.2/lale/lib/rasl/batched_bagging_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/batching.py` & `lale-0.8.2/lale/lib/rasl/batching.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/concat_features.py` & `lale-0.8.2/lale/lib/rasl/concat_features.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/convert.py` & `lale-0.8.2/lale/lib/rasl/convert.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/datasets.py` & `lale-0.8.2/lale/lib/rasl/datasets.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/filter.py` & `lale-0.8.2/lale/lib/rasl/filter.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/functions.py` & `lale-0.8.2/lale/lib/rasl/functions.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/group_by.py` & `lale-0.8.2/lale/lib/rasl/group_by.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/hashing_encoder.py` & `lale-0.8.2/lale/lib/rasl/hashing_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/join.py` & `lale-0.8.2/lale/lib/rasl/join.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/map.py` & `lale-0.8.2/lale/lib/rasl/map.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/metrics.py` & `lale-0.8.2/lale/lib/rasl/metrics.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/min_max_scaler.py` & `lale-0.8.2/lale/lib/rasl/min_max_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/monoid.py` & `lale-0.8.2/lale/lib/rasl/monoid.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/one_hot_encoder.py` & `lale-0.8.2/lale/lib/rasl/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/orderby.py` & `lale-0.8.2/lale/lib/rasl/orderby.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/ordinal_encoder.py` & `lale-0.8.2/lale/lib/rasl/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/project.py` & `lale-0.8.2/lale/lib/rasl/project.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/relational.py` & `lale-0.8.2/lale/lib/rasl/relational.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/scan.py` & `lale-0.8.2/lale/lib/rasl/scan.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/scores.py` & `lale-0.8.2/lale/lib/rasl/scores.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/select_k_best.py` & `lale-0.8.2/lale/lib/rasl/select_k_best.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/simple_imputer.py` & `lale-0.8.2/lale/lib/rasl/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/sort_index.py` & `lale-0.8.2/lale/lib/rasl/sort_index.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/spark_explainer.py` & `lale-0.8.2/lale/lib/rasl/spark_explainer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/split_xy.py` & `lale-0.8.2/lale/lib/rasl/split_xy.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/standard_scaler.py` & `lale-0.8.2/lale/lib/rasl/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/target_encoder.py` & `lale-0.8.2/lale/lib/rasl/target_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/rasl/task_graphs.py` & `lale-0.8.2/lale/lib/rasl/task_graphs.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/__init__.py` & `lale-0.8.2/lale/lib/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/_common_schemas.py` & `lale-0.8.2/lale/lib/sklearn/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/ada_boost_classifier.py` & `lale-0.8.2/lale/lib/sklearn/ada_boost_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/ada_boost_regressor.py` & `lale-0.8.2/lale/lib/sklearn/ada_boost_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/bagging_classifier.py` & `lale-0.8.2/lale/lib/sklearn/bagging_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/bagging_regressor.py` & `lale-0.8.2/lale/lib/sklearn/bagging_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/column_transformer.py` & `lale-0.8.2/lale/lib/sklearn/column_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/decision_tree_classifier.py` & `lale-0.8.2/lale/lib/sklearn/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/decision_tree_regressor.py` & `lale-0.8.2/lale/lib/sklearn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/dummy_classifier.py` & `lale-0.8.2/lale/lib/sklearn/dummy_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/dummy_regressor.py` & `lale-0.8.2/lale/lib/sklearn/dummy_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/extra_trees_classifier.py` & `lale-0.8.2/lale/lib/sklearn/extra_trees_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/extra_trees_regressor.py` & `lale-0.8.2/lale/lib/sklearn/extra_trees_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/feature_agglomeration.py` & `lale-0.8.2/lale/lib/sklearn/feature_agglomeration.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/fit_spec_proxy.py` & `lale-0.8.2/lale/lib/sklearn/fit_spec_proxy.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/function_transformer.py` & `lale-0.8.2/lale/lib/sklearn/function_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/gaussian_nb.py` & `lale-0.8.2/lale/lib/sklearn/gaussian_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/gradient_boosting_classifier.py` & `lale-0.8.2/lale/lib/sklearn/gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/gradient_boosting_regressor.py` & `lale-0.8.2/lale/lib/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/isolation_forest.py` & `lale-0.8.2/lale/lib/sklearn/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/isomap.py` & `lale-0.8.2/lale/lib/sklearn/isomap.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/k_means.py` & `lale-0.8.2/lale/lib/sklearn/k_means.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/k_neighbors_classifier.py` & `lale-0.8.2/lale/lib/sklearn/k_neighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/k_neighbors_regressor.py` & `lale-0.8.2/lale/lib/sklearn/k_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/linear_regression.py` & `lale-0.8.2/lale/lib/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/linear_svc.py` & `lale-0.8.2/lale/lib/sklearn/linear_svc.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/linear_svr.py` & `lale-0.8.2/lale/lib/sklearn/linear_svr.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/logistic_regression.py` & `lale-0.8.2/lale/lib/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/min_max_scaler.py` & `lale-0.8.2/lale/lib/sklearn/min_max_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/missing_indicator.py` & `lale-0.8.2/lale/lib/sklearn/missing_indicator.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/mlp_classifier.py` & `lale-0.8.2/lale/lib/sklearn/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/multi_output_regressor.py` & `lale-0.8.2/lale/lib/sklearn/multi_output_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/multinomial_nb.py` & `lale-0.8.2/lale/lib/sklearn/multinomial_nb.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/nmf.py` & `lale-0.8.2/lale/lib/sklearn/nmf.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/normalizer.py` & `lale-0.8.2/lale/lib/sklearn/normalizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/nystroem.py` & `lale-0.8.2/lale/lib/sklearn/nystroem.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/one_hot_encoder.py` & `lale-0.8.2/lale/lib/sklearn/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/ordinal_encoder.py` & `lale-0.8.2/lale/lib/sklearn/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/passive_aggressive_classifier.py` & `lale-0.8.2/lale/lib/sklearn/passive_aggressive_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/pca.py` & `lale-0.8.2/lale/lib/sklearn/pca.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/perceptron.py` & `lale-0.8.2/lale/lib/sklearn/perceptron.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/pipeline.py` & `lale-0.8.2/lale/lib/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/polynomial_features.py` & `lale-0.8.2/lale/lib/sklearn/polynomial_features.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/quadratic_discriminant_analysis.py` & `lale-0.8.2/lale/lib/sklearn/quadratic_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/quantile_transformer.py` & `lale-0.8.2/lale/lib/sklearn/quantile_transformer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/random_forest_classifier.py` & `lale-0.8.2/lale/lib/sklearn/random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/random_forest_regressor.py` & `lale-0.8.2/lale/lib/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/rfe.py` & `lale-0.8.2/lale/lib/sklearn/rfe.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/ridge.py` & `lale-0.8.2/lale/lib/sklearn/ridge.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/ridge_classifier.py` & `lale-0.8.2/lale/lib/sklearn/ridge_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/robust_scaler.py` & `lale-0.8.2/lale/lib/sklearn/robust_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/select_k_best.py` & `lale-0.8.2/lale/lib/sklearn/select_k_best.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/sgd_classifier.py` & `lale-0.8.2/lale/lib/sklearn/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/sgd_regressor.py` & `lale-0.8.2/lale/lib/sklearn/sgd_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/simple_imputer.py` & `lale-0.8.2/lale/lib/sklearn/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/stacking_classifier.py` & `lale-0.8.2/lale/lib/sklearn/stacking_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/stacking_regressor.py` & `lale-0.8.2/lale/lib/sklearn/stacking_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/stacking_utils.py` & `lale-0.8.2/lale/lib/sklearn/stacking_utils.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/standard_scaler.py` & `lale-0.8.2/lale/lib/sklearn/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/svc.py` & `lale-0.8.2/lale/lib/sklearn/svc.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/svr.py` & `lale-0.8.2/lale/lib/sklearn/svr.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/target_encoder.py` & `lale-0.8.2/lale/lib/sklearn/target_encoder.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/tfidf_vectorizer.py` & `lale-0.8.2/lale/lib/sklearn/tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/variance_threshold.py` & `lale-0.8.2/lale/lib/sklearn/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/voting_classifier.py` & `lale-0.8.2/lale/lib/sklearn/voting_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/sklearn/voting_regressor.py` & `lale-0.8.2/lale/lib/sklearn/voting_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/__init__.py` & `lale-0.8.2/lale/lib/snapml/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/batched_tree_ensemble_classifier.py` & `lale-0.8.2/lale/lib/snapml/batched_tree_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/batched_tree_ensemble_regressor.py` & `lale-0.8.2/lale/lib/snapml/batched_tree_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_boosting_machine_classifier.py` & `lale-0.8.2/lale/lib/snapml/snap_boosting_machine_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_boosting_machine_regressor.py` & `lale-0.8.2/lale/lib/snapml/snap_boosting_machine_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_decision_tree_classifier.py` & `lale-0.8.2/lale/lib/snapml/snap_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_decision_tree_regressor.py` & `lale-0.8.2/lale/lib/snapml/snap_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_linear_regression.py` & `lale-0.8.2/lale/lib/snapml/snap_linear_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_logistic_regression.py` & `lale-0.8.2/lale/lib/snapml/snap_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_random_forest_classifier.py` & `lale-0.8.2/lale/lib/snapml/snap_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_random_forest_regressor.py` & `lale-0.8.2/lale/lib/snapml/snap_random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/snapml/snap_svm_classifier.py` & `lale-0.8.2/lale/lib/snapml/snap_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/xgboost/__init__.py` & `lale-0.8.2/lale/lib/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/xgboost/_common_schemas.py` & `lale-0.8.2/lale/lib/xgboost/_common_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/lib/xgboost/xgb_classifier.py` & `lale-0.8.2/lale/lib/xgboost/xgb_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
             pip install xgboost
         or with
             pip install 'lale[full]'"""
 
     def __init__(self, **hyperparams):
         self.validate_hyperparams(**hyperparams)
         self._wrapped_model = xgboost.XGBClassifier(**hyperparams)
+        self._label_encoder = None
 
     def fit(self, X, y, **fit_params):
         renamed_X = _rename_all_features(X)
         assert xgboost_version is not None
         if (
             xgboost_version >= version.Version("1.3.0")
             and "eval_metric" not in fit_params
@@ -89,15 +90,18 @@
             warnings.filterwarnings("ignore", category=FutureWarning)
 
             if "xgb_model" not in fit_params:
                 trainable_le = LabelEncoder()
                 trained_le = trainable_le.fit(y)
                 self._label_encoder = trained_le
 
-            numeric_y = self._label_encoder.transform(y)
+            if self._label_encoder is not None:
+                numeric_y = self._label_encoder.transform(y)
+            else:
+                numeric_y = y
             self._wrapped_model.fit(renamed_X, numeric_y, **fit_params)
         return self
 
     def partial_fit(self, X, y, **fit_params):
         fit_params = lale.helpers.dict_without(fit_params, "classes")
         if self._wrapped_model.__sklearn_is_fitted__():
             booster = self._wrapped_model.get_booster()
@@ -105,16 +109,18 @@
         return self.fit(X, y, **fit_params)
 
     def predict(self, X, **predict_params):
         renamed_X = _rename_all_features(X)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=FutureWarning)
             numeric_result = self._wrapped_model.predict(renamed_X, **predict_params)
-        result = self._label_encoder.inverse_transform(numeric_result)
-        return result
+        if self._label_encoder is not None:
+            return self._label_encoder.inverse_transform(numeric_result)
+        else:
+            return numeric_result
 
     def predict_proba(self, X):
         return self._wrapped_model.predict_proba(X)
 
     def score(self, X, y):
         from sklearn.metrics import accuracy_score
```

### Comparing `lale-0.8.0/lale/lib/xgboost/xgb_regressor.py` & `lale-0.8.2/lale/lib/xgboost/xgb_regressor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/operator_wrapper.py` & `lale-0.8.2/lale/operator_wrapper.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/operators.py` & `lale-0.8.2/lale/operators.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/pretty_print.py` & `lale-0.8.2/lale/pretty_print.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/schema2enums.py` & `lale-0.8.2/lale/schema2enums.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/schema_ranges.py` & `lale-0.8.2/lale/schema_ranges.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/schema_simplifier.py` & `lale-0.8.2/lale/schema_simplifier.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/schema_utils.py` & `lale-0.8.2/lale/schema_utils.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/schemas.py` & `lale-0.8.2/lale/schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/PGO.py` & `lale-0.8.2/lale/search/PGO.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/__init__.py` & `lale-0.8.2/lale/search/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/lale_grid_search_cv.py` & `lale-0.8.2/lale/search/lale_grid_search_cv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/lale_hyperopt.py` & `lale-0.8.2/lale/search/lale_hyperopt.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/lale_smac.py` & `lale-0.8.2/lale/search/lale_smac.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/op2hp.py` & `lale-0.8.2/lale/search/op2hp.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/schema2search_space.py` & `lale-0.8.2/lale/search/schema2search_space.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/search_space.py` & `lale-0.8.2/lale/search/search_space.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/search/search_space_grid.py` & `lale-0.8.2/lale/search/search_space_grid.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/settings.py` & `lale-0.8.2/lale/settings.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/sklearn_compat.py` & `lale-0.8.2/lale/sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/type_checking.py` & `lale-0.8.2/lale/type_checking.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/Visitor.py` & `lale-0.8.2/lale/util/Visitor.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/VisitorMeta.py` & `lale-0.8.2/lale/util/VisitorMeta.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/VisitorPathError.py` & `lale-0.8.2/lale/util/VisitorPathError.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/__init__.py` & `lale-0.8.2/lale/util/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/batch_data_dictionary_dataset.py` & `lale-0.8.2/lale/util/batch_data_dictionary_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/hdf5_to_torch_dataset.py` & `lale-0.8.2/lale/util/hdf5_to_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/numpy_to_torch_dataset.py` & `lale-0.8.2/lale/util/numpy_to_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/numpy_torch_dataset.py` & `lale-0.8.2/lale/util/numpy_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/pandas_to_torch_dataset.py` & `lale-0.8.2/lale/util/pandas_to_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/util/pandas_torch_dataset.py` & `lale-0.8.2/lale/util/pandas_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/lale/visualize.py` & `lale-0.8.2/lale/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                 "graph",
                 label=jsn.get("viz_label", jsn["label"]),
                 style="filled",
                 fillcolor=_STATE2COLOR[jsn["state"]],
                 tooltip=_indiv_op_tooltip(uid, jsn),
             )
             if "documentation_url" in jsn:
-                dot.attr("graph", URL=jsn["documentation_url"])
+                dot.attr("graph", URL=jsn["documentation_url"], target="_blank")
             nodes = jsn["steps"]
             if jsn["class"] == _LALE_SKL_PIPELINE:
                 names = list(nodes.keys())
                 edges = [[names[i], names[i + 1]] for i in range(len(names) - 1)]
             else:
                 edges = []
     for step_uid, step_jsn in nodes.items():
@@ -188,14 +188,15 @@
         else:
             assert node_kind == "IndividualOp"
             tooltip = _indiv_op_tooltip(step_uid, step_jsn)
             attrs = {
                 "style": "filled",
                 "fillcolor": _STATE2COLOR[step_jsn["state"]],
                 "tooltip": tooltip,
+                "target": "_blank",
             }
             if "documentation_url" in step_jsn:
                 attrs["URL"] = step_jsn["documentation_url"]
             label0 = step_jsn.get("viz_label", step_jsn["label"])
             if "\n" in label0:
                 label3 = label0
             else:
```

### Comparing `lale-0.8.0/lale.egg-info/PKG-INFO` & `lale-0.8.2/lale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lale
-Version: 0.8.0
+Version: 0.8.2
 Summary: Library for Semi-Automated Data Science
 Home-page: https://github.com/IBM/lale
 Author: Guillaume Baudart, Martin Hirzel, Kiran Kate, Parikshit Ram, Avraham Shinnar
 License: Apache License 2.0
 Description: # Lale
         
         [![Tests](https://github.com/IBM/lale/workflows/Tests/badge.svg?branch=master)](https://github.com/IBM/lale/actions?query=workflow%3ATests+branch%3Amaster)
```

### Comparing `lale-0.8.0/lale.egg-info/SOURCES.txt` & `lale-0.8.2/lale.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 lale/__init__.py
 lale/docstrings.py
 lale/expressions.py
 lale/grammar.py
 lale/helpers.py
```

### Comparing `lale-0.8.0/lale.egg-info/requires.txt` & `lale-0.8.2/lale.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,40 +14,41 @@
 
 [dev]
 pre-commit
 
 [fairness]
 mystic
 liac-arff>=2.4.0
-aif360<0.6.0
+aif360>=0.5.0
 imbalanced-learn
 BlackBoxAuditing
 
 [full]
 mystic
 xgboost<2.1.0
 lightgbm<4.4.0
 snapml<1.16.0,>=1.7.0rc3
 liac-arff>=2.4.0
 tensorflow<=2.16.0,>=2.4.0
 smac<=0.10.0
 numba
-aif360>=0.4.0
+aif360>=0.5.0
 torch>=1.0
 BlackBoxAuditing
 imbalanced-learn
 cvxpy>=1.0
 fairlearn
 h5py
 
 [test]
 mystic
 joblib
 ipython<8.8.0
 jupyter
+lxml<5.2.0
 sphinx>=5.0.0
 sphinx_rtd_theme>=0.5.2
 docutils<0.17
 m2r2
 sphinxcontrib.apidoc
 sphinxcontrib-svg2pdfconverter
 pytest
@@ -58,11 +59,11 @@
 
 [tutorial]
 ipython<8.8.0
 jupyter
 xgboost<=1.5.1
 imbalanced-learn
 liac-arff>=2.4.0
-aif360==0.5.0
+aif360>=0.5.0
 BlackBoxAuditing
 typing-extensions
 pandas<2.0.0
```

### Comparing `lale-0.8.0/setup.py` & `lale-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,29 @@
         "xgboost<2.1.0",
         "lightgbm<4.4.0",
         "snapml>=1.7.0rc3,<1.16.0",
         "liac-arff>=2.4.0",
         "tensorflow>=2.4.0,<=2.16.0",
         "smac<=0.10.0",
         "numba",
-        "aif360>=0.4.0",
+        "aif360>=0.5.0",
         "torch>=1.0",
         "BlackBoxAuditing",
         "imbalanced-learn",
         "cvxpy>=1.0",
         "fairlearn",
         "h5py",
     ],
     "dev": ["pre-commit"],
     "test": [
         "mystic",
         "joblib",
         "ipython<8.8.0",
         "jupyter",
+        "lxml<5.2.0",
         "sphinx>=5.0.0",
         "sphinx_rtd_theme>=0.5.2",
         "docutils<0.17",
         "m2r2",
         "sphinxcontrib.apidoc",
         "sphinxcontrib-svg2pdfconverter",
         "pytest",
@@ -98,25 +99,25 @@
         "func_timeout",
         "category-encoders",
         "pynisher==0.6.4",
     ],
     "fairness": [
         "mystic",
         "liac-arff>=2.4.0",
-        "aif360<0.6.0",
+        "aif360>=0.5.0",
         "imbalanced-learn",
         "BlackBoxAuditing",
     ],
     "tutorial": [
         "ipython<8.8.0",
         "jupyter",
         "xgboost<=1.5.1",
         "imbalanced-learn",
         "liac-arff>=2.4.0",
-        "aif360==0.5.0",
+        "aif360>=0.5.0",
         "BlackBoxAuditing",
         "typing-extensions",
         "pandas<2.0.0",
     ],
 }
 
 classifiers = [
```

### Comparing `lale-0.8.0/test/__init__.py` & `lale-0.8.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/mock_custom_operators.py` & `lale-0.8.2/test/mock_custom_operators.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/mock_module.py` & `lale-0.8.2/test/mock_module.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_aif360.py` & `lale-0.8.2/test/test_aif360.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_aif360_ensembles.py` & `lale-0.8.2/test/test_aif360_ensembles.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_autogen_lib.py` & `lale-0.8.2/test/test_autogen_lib.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_category_encoders.py` & `lale-0.8.2/test/test_category_encoders.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_core_classifiers.py` & `lale-0.8.2/test/test_core_classifiers.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_core_misc.py` & `lale-0.8.2/test/test_core_misc.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_core_pipeline.py` & `lale-0.8.2/test/test_core_pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_core_regressors.py` & `lale-0.8.2/test/test_core_regressors.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_core_transformers.py` & `lale-0.8.2/test/test_core_transformers.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_custom_schemas.py` & `lale-0.8.2/test/test_custom_schemas.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_grammar.py` & `lale-0.8.2/test/test_grammar.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_halving_gridsearchcv.py` & `lale-0.8.2/test/test_halving_gridsearchcv.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_interoperability.py` & `lale-0.8.2/test/test_interoperability.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_json_pretty_viz.py` & `lale-0.8.2/test/test_json_pretty_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,27 @@
         kernel_tfm_or_not = NoOp | Nystroem
         tfm = PCA
         clf = make_choice(LogisticRegression, KNeighborsClassifier)
         clf.visualize(ipython_display=False)
         optimizable = kernel_tfm_or_not >> tfm >> clf
         optimizable.visualize(ipython_display=False)
 
+    def test_url_generation(self):
+        from graphviz import Source
+
+        from lale.lib.lale import NoOp
+        from lale.lib.sklearn import PCA, LogisticRegression
+
+        sample = NoOp >> PCA >> LogisticRegression
+        result = Source(str(sample.visualize(ipython_display=False)))
+        for i in result:
+            if "URL" in i:
+                print(i)
+                self.assertTrue("target=_blank" in i)
+
     def test_invalid_input(self):
         from sklearn.linear_model import LogisticRegression as SklearnLR
 
         scikit_lr = SklearnLR()
         from lale.helpers import to_graphviz
 
         with self.assertRaises(TypeError):
```

### Comparing `lale-0.8.0/test/test_nlp_operators.py` & `lale-0.8.2/test/test_nlp_operators.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_notebooks.py` & `lale-0.8.2/test/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_optimizers.py` & `lale-0.8.2/test/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_pgo.py` & `lale-0.8.2/test/test_pgo.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_pipeline.py` & `lale-0.8.2/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_relational.py` & `lale-0.8.2/test/test_relational.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_relational_from_sklearn_manual.py` & `lale-0.8.2/test/test_relational_from_sklearn_manual.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_relational_sklearn.py` & `lale-0.8.2/test/test_relational_sklearn.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_replace.py` & `lale-0.8.2/test/test_replace.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_sklearn_compat.py` & `lale-0.8.2/test/test_sklearn_compat.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_snapml.py` & `lale-0.8.2/test/test_snapml.py`

 * *Files identical despite different names*

### Comparing `lale-0.8.0/test/test_type_checking.py` & `lale-0.8.2/test/test_type_checking.py`

 * *Files identical despite different names*

