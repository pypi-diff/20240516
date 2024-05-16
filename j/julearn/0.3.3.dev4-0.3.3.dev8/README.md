# Comparing `tmp/julearn-0.3.3.dev4.tar.gz` & `tmp/julearn-0.3.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julearn-0.3.3.dev4.tar", last modified: Mon May  6 09:04:03 2024, max compression
+gzip compressed data, was "julearn-0.3.3.dev8.tar", last modified: Tue May 14 08:21:41 2024, max compression
```

## Comparing `julearn-0.3.3.dev4.tar` & `julearn-0.3.3.dev8.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.097706 julearn-0.3.3.dev4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.049705 julearn-0.3.3.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/documentation_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/feature_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/check-stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.049705 julearn-0.3.3.dev4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.057705 julearn-0.3.3.dev4/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/function_warning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/api/viz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/available_pipeline_steps.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.061705 julearn-0.3.3.dev4/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.065705 julearn-0.3.3.dev4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/corrected_ttest.png
--rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/final_estimator.png
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/iris_X.png
--rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/iris_df.png
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/iris_y.png
--rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_calm.png
--rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_confbias.png
--rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_generalization.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_it.png
--rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_ml.png
--rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/julearn_logo_mlit.png
--rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/multiple_scorers_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/plot_scores.png
--rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/scores_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/scores_run_cv_splitter.png
--rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/images/scores_run_cv_train.png
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/docs/selected_deeper_topics/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/CBPM.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/confound_removal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/cross_validation_splitter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/hyperparameter_tuning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/model_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/stacked_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/selected_deeper_topics/target_transformers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/docs/what_really_need_know/
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/model_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/what_really_need_know/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/00_starting/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/plot_cm_acc_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/plot_example_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/plot_stratified_kfold_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/run_combine_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/run_grouped_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/00_starting/run_simple_binary_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/01_model_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/01_model_comparison/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/01_model_comparison/plot_simple_model_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.069706 julearn-0.3.3.dev4/examples/02_inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/plot_groupcv_inspect_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/plot_inspect_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/plot_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/02_inspection/run_binary_inspect_folds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/03_complex_models/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_apply_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_example_pca_featsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_multiple_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/03_complex_models/run_stacked_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/04_confounds/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/04_confounds/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/04_confounds/plot_confound_removal_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/04_confounds/run_return_confounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/05_customization/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/05_customization/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/05_customization/run_custom_scorers_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/99_docs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_cbpm_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_confound_removal_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_cv_splitters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_data_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_hyperparameters_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_model_comparison_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_model_evaluation_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_model_inspection_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_pipeline_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_stacked_models_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/99_docs/run_target_transformer_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.073706 julearn-0.3.3.dev4/examples/XX_disabled/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/XX_disabled/dis_run_n_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/examples/XX_disabled/dis_run_target_confound_removal.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/base/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/tests/test_base_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/base/tests/test_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.077706 julearn-0.3.3.dev4/julearn/inspect/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/inspect/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/_optuna_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/_skopt_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/continuous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_continous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_optuna_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_skopt_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/model_selection/tests/test_stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/models/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/tests/test_available_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/models/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.081706 julearn-0.3.3.dev4/julearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    36758 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/target_pipeline_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    27718 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/scoring/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/tests/test_available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/scoring/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/stats/corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/stats/tests/test_corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39240 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/tests/test_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.085706 julearn-0.3.3.dev4/julearn/transformers/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/set_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_set_column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/ju_column_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/target/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/target/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/target/tests/test_target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/transformers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_cbpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_confounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/transformers/tests/test_jucolumntransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.089706 julearn-0.3.3.dev4/julearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/julearn/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/viz/_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/julearn/viz/res/
--rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/julearn/viz/res/julearn_logo_generalization.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:03.093706 julearn-0.3.3.dev4/julearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-06 09:04:03.000000 julearn-0.3.3.dev4/julearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 09:04:02.000000 julearn-0.3.3.dev4/julearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:04:03.097706 julearn-0.3.3.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-06 09:03:57.000000 julearn-0.3.3.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.508633 julearn-0.3.3.dev8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.460632 julearn-0.3.3.dev8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.468632 julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/documentation_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/feature_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.468632 julearn-0.3.3.dev8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/check-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-14 08:21:41.508633 julearn-0.3.3.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.472633 julearn-0.3.3.dev8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.460632 julearn-0.3.3.dev8/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.472633 julearn-0.3.3.dev8/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.472633 julearn-0.3.3.dev8/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.472633 julearn-0.3.3.dev8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/_templates/function_warning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.476632 julearn-0.3.3.dev8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/api/viz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/available_pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.476632 julearn-0.3.3.dev8/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.476632 julearn-0.3.3.dev8/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.480632 julearn-0.3.3.dev8/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/corrected_ttest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39468 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/final_estimator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/iris_X.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51228 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/iris_df.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/iris_y.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54482 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74874 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_calm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78884 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_confbias.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61311 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_generalization.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60581 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_it.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66833 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_ml.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60581 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/julearn_logo_mlit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94858 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/multiple_scorers_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84126 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/plot_scores.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43199 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/scores_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/scores_run_cv_splitter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47133 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/images/scores_run_cv_train.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.480632 julearn-0.3.3.dev8/docs/selected_deeper_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/CBPM.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/confound_removal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/cross_validation_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/hyperparameter_tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/model_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/stacked_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/selected_deeper_topics/target_transformers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.480632 julearn-0.3.3.dev8/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/sphinxext/gh_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.484633 julearn-0.3.3.dev8/docs/what_really_need_know/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/what_really_need_know/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/what_really_need_know/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/what_really_need_know/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/what_really_need_know/model_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/what_really_need_know/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/what_really_need_know/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.484633 julearn-0.3.3.dev8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.484633 julearn-0.3.3.dev8/examples/00_starting/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/plot_cm_acc_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/plot_example_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/plot_stratified_kfold_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/run_combine_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/run_grouped_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/00_starting/run_simple_binary_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.484633 julearn-0.3.3.dev8/examples/01_model_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/01_model_comparison/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/01_model_comparison/plot_simple_model_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.484633 julearn-0.3.3.dev8/examples/02_inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/02_inspection/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/02_inspection/plot_groupcv_inspect_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/02_inspection/plot_inspect_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/02_inspection/plot_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/02_inspection/run_binary_inspect_folds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.484633 julearn-0.3.3.dev8/examples/03_complex_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/run_apply_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/run_example_pca_featsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/run_hyperparameter_multiple_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/run_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/03_complex_models/run_stacked_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.488633 julearn-0.3.3.dev8/examples/04_confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/04_confounds/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/04_confounds/plot_confound_removal_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/04_confounds/run_return_confounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.488633 julearn-0.3.3.dev8/examples/05_customization/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/05_customization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/05_customization/run_custom_scorers_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.488633 julearn-0.3.3.dev8/examples/99_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_cbpm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_confound_removal_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_cv_splitters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_data_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23629 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_hyperparameters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_model_comparison_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_model_evaluation_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_model_inspection_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_pipeline_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_stacked_models_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/99_docs/run_target_transformer_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.488633 julearn-0.3.3.dev8/examples/XX_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/XX_disabled/dis_run_n_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/examples/XX_disabled/dis_run_target_confound_removal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.492632 julearn-0.3.3.dev8/julearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 08:21:41.000000 julearn-0.3.3.dev8/julearn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.492632 julearn-0.3.3.dev8/julearn/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/base/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/base/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.492632 julearn-0.3.3.dev8/julearn/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/base/tests/test_base_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/base/tests/test_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.492632 julearn-0.3.3.dev8/julearn/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.492632 julearn-0.3.3.dev8/julearn/inspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/inspect/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.496632 julearn-0.3.3.dev8/julearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/_optuna_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/continuous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.496632 julearn-0.3.3.dev8/julearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/tests/test_available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/tests/test_continous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/tests/test_optuna_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/tests/test_skopt_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/model_selection/tests/test_stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.496632 julearn-0.3.3.dev8/julearn/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/models/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/models/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.496632 julearn-0.3.3.dev8/julearn/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/models/tests/test_available_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/models/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/models/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.496632 julearn-0.3.3.dev8/julearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36758 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/target_pipeline_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.496632 julearn-0.3.3.dev8/julearn/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/tests/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27718 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/tests/test_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/tests/test_target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/pipeline/tests/test_target_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/scoring/available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/scoring/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/scoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/scoring/tests/test_available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/scoring/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/stats/corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/stats/tests/test_corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39190 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24533 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/tests/test_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/transformers/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/set_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.500633 julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_set_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/ju_column_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.504633 julearn-0.3.3.dev8/julearn/transformers/target/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.504633 julearn-0.3.3.dev8/julearn/transformers/target/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/tests/test_available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/tests/test_ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/tests/test_ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/target/tests/test_target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.504633 julearn-0.3.3.dev8/julearn/transformers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/tests/test_available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/tests/test_cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/tests/test_confounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/transformers/tests/test_jucolumntransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.504633 julearn-0.3.3.dev8/julearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.504633 julearn-0.3.3.dev8/julearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.504633 julearn-0.3.3.dev8/julearn/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/viz/_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.508633 julearn-0.3.3.dev8/julearn/viz/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    73031 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/julearn/viz/res/julearn_logo_generalization.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:41.508633 julearn-0.3.3.dev8/julearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-14 08:21:41.000000 julearn-0.3.3.dev8/julearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-14 08:21:41.000000 julearn-0.3.3.dev8/julearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:21:41.000000 julearn-0.3.3.dev8/julearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-14 08:21:41.000000 julearn-0.3.3.dev8/julearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 08:21:41.000000 julearn-0.3.3.dev8/julearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:21:41.508633 julearn-0.3.3.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-14 08:21:33.000000 julearn-0.3.3.dev8/tox.ini
```

### Comparing `julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/bug_report.yaml` & `julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/documentation_request.yaml` & `julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/documentation_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/ISSUE_TEMPLATE/feature_request.yaml` & `julearn-0.3.3.dev8/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/workflows/ci-docs.yml` & `julearn-0.3.3.dev8/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/workflows/ci.yml` & `julearn-0.3.3.dev8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/workflows/docs-preview.yml` & `julearn-0.3.3.dev8/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/workflows/docs.yml` & `julearn-0.3.3.dev8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/workflows/lint.yml` & `julearn-0.3.3.dev8/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.github/workflows/pypi.yml` & `julearn-0.3.3.dev8/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.gitignore` & `julearn-0.3.3.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/.pre-commit-config.yaml` & `julearn-0.3.3.dev8/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 ci:
   autofix_prs: false
   autoupdate_commit_msg: "chore: bump pre-commit repositories"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-ast
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.17
     hooks:
       - id: validate-pyproject
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
+  - repo: https://github.com/psf/black-pre-commit-mirror
+    rev: 24.4.2
     hooks:
       - id: black
         exclude: ^(docs/|examples/)
         args: [--check]
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.4
     hooks:
       - id: ruff
         exclude: ^(__init__.py)
-        args: [--format, grouped, --show-fixes]
+        args: [--output-format, grouped, --show-fixes]
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.6
     hooks:
       - id: codespell
         exclude: ^(.github/|docs/)
-        args: [--config, tox.ini]
+        args: [--toml, pyproject.toml]
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-no-eval
       - id: python-no-log-warn
       - id: rst-backticks
       - id: rst-directive-colons
```

### Comparing `julearn-0.3.3.dev4/LICENSE.md` & `julearn-0.3.3.dev8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/PKG-INFO` & `julearn-0.3.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.3.dev4
+Version: 0.3.3.dev8
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
```

### Comparing `julearn-0.3.3.dev4/README.md` & `julearn-0.3.3.dev8/README.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/codecov.yml` & `julearn-0.3.3.dev8/codecov.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/Makefile` & `julearn-0.3.3.dev8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/_templates/class.rst` & `julearn-0.3.3.dev8/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/_templates/function_warning.rst` & `julearn-0.3.3.dev8/docs/_templates/function_warning.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/_templates/versions.html` & `julearn-0.3.3.dev8/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/base.rst` & `julearn-0.3.3.dev8/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/model_selection.rst` & `julearn-0.3.3.dev8/docs/api/model_selection.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/models.rst` & `julearn-0.3.3.dev8/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/scoring.rst` & `julearn-0.3.3.dev8/docs/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/transformers.rst` & `julearn-0.3.3.dev8/docs/api/transformers.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/utils.rst` & `julearn-0.3.3.dev8/docs/api/utils.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/api/viz.rst` & `julearn-0.3.3.dev8/docs/api/viz.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/available_pipeline_steps.rst` & `julearn-0.3.3.dev8/docs/available_pipeline_steps.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/conf.py` & `julearn-0.3.3.dev8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/configuration.rst` & `julearn-0.3.3.dev8/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/contributing.rst` & `julearn-0.3.3.dev8/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/examples.rst` & `julearn-0.3.3.dev8/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/faq.rst` & `julearn-0.3.3.dev8/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/getting_started.rst` & `julearn-0.3.3.dev8/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/corrected_ttest.png` & `julearn-0.3.3.dev8/docs/images/corrected_ttest.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/final_estimator.png` & `julearn-0.3.3.dev8/docs/images/final_estimator.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/iris_X.png` & `julearn-0.3.3.dev8/docs/images/iris_X.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/iris_df.png` & `julearn-0.3.3.dev8/docs/images/iris_df.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/iris_y.png` & `julearn-0.3.3.dev8/docs/images/iris_y.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_calm.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_calm.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_confbias.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_confbias.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_cv.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_generalization.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_it.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_it.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_ml.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_ml.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/julearn_logo_mlit.png` & `julearn-0.3.3.dev8/docs/images/julearn_logo_mlit.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/multiple_scorers_run_cv.png` & `julearn-0.3.3.dev8/docs/images/multiple_scorers_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/plot_scores.png` & `julearn-0.3.3.dev8/docs/images/plot_scores.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/scores_run_cv.png` & `julearn-0.3.3.dev8/docs/images/scores_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/scores_run_cv_splitter.png` & `julearn-0.3.3.dev8/docs/images/scores_run_cv_splitter.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/images/scores_run_cv_train.png` & `julearn-0.3.3.dev8/docs/images/scores_run_cv_train.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/index.rst` & `julearn-0.3.3.dev8/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,18 @@
 * :ref:`modindex`
 * :ref:`search`
 
 
 Indices and tables
 ==================
 
-If you use julearn in a scientific publication, please use the following 
+If you use julearn in a scientific publication, please use the following
 reference
 
-    Hamdan, Sami, Shammi More, Leonard Sasse, Vera Komeyer, 
-    Kaustubh R. Patil, and Federico Raimondo. ‘Julearn: 
-    An Easy-to-Use Library for Leakage-Free Evaluation and Inspection of 
-    ML Models’. arXiv, 19 October 2023. 
+    Hamdan, Sami, Shammi More, Leonard Sasse, Vera Komeyer,
+    Kaustubh R. Patil, and Federico Raimondo. ‘Julearn:
+    An Easy-to-Use Library for Leakage-Free Evaluation and Inspection of
+    ML Models’. arXiv, 19 October 2023.
     https://doi.org/10.48550/arXiv.2310.12568.
 
-Since julearn is also heavily reliant on scikit-learn, please also cite 
+Since julearn is also heavily reliant on scikit-learn, please also cite
 them: https://scikit-learn.org/stable/about.html#citing-scikit-learn
```

### Comparing `julearn-0.3.3.dev4/docs/links.inc` & `julearn-0.3.3.dev8/docs/links.inc`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/maintaining.rst` & `julearn-0.3.3.dev8/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/sphinxext/gh_substitutions.py` & `julearn-0.3.3.dev8/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/what_really_need_know/cross_validation.rst` & `julearn-0.3.3.dev8/docs/what_really_need_know/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/what_really_need_know/index.rst` & `julearn-0.3.3.dev8/docs/what_really_need_know/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/docs/whats_new.rst` & `julearn-0.3.3.dev8/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/00_starting/plot_cm_acc_multiclass.py` & `julearn-0.3.3.dev8/examples/00_starting/plot_cm_acc_multiclass.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/00_starting/plot_example_regression.py` & `julearn-0.3.3.dev8/examples/00_starting/plot_example_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/00_starting/plot_stratified_kfold_reg.py` & `julearn-0.3.3.dev8/examples/00_starting/plot_stratified_kfold_reg.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/00_starting/run_combine_pandas.py` & `julearn-0.3.3.dev8/examples/00_starting/run_combine_pandas.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/00_starting/run_grouped_cv.py` & `julearn-0.3.3.dev8/examples/00_starting/run_grouped_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/00_starting/run_simple_binary_classification.py` & `julearn-0.3.3.dev8/examples/00_starting/run_simple_binary_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/01_model_comparison/plot_simple_model_comparison.py` & `julearn-0.3.3.dev8/examples/01_model_comparison/plot_simple_model_comparison.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/02_inspection/plot_groupcv_inspect_svm.py` & `julearn-0.3.3.dev8/examples/02_inspection/plot_groupcv_inspect_svm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/02_inspection/plot_inspect_random_forest.py` & `julearn-0.3.3.dev8/examples/02_inspection/plot_inspect_random_forest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/02_inspection/plot_preprocess.py` & `julearn-0.3.3.dev8/examples/02_inspection/plot_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/02_inspection/run_binary_inspect_folds.py` & `julearn-0.3.3.dev8/examples/02_inspection/run_binary_inspect_folds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/03_complex_models/run_apply_to_target.py` & `julearn-0.3.3.dev8/examples/03_complex_models/run_apply_to_target.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/03_complex_models/run_example_pca_featsets.py` & `julearn-0.3.3.dev8/examples/03_complex_models/run_example_pca_featsets.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_multiple_grids.py` & `julearn-0.3.3.dev8/examples/03_complex_models/run_hyperparameter_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning.py` & `julearn-0.3.3.dev8/examples/03_complex_models/run_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py` & `julearn-0.3.3.dev8/examples/03_complex_models/run_hyperparameter_tuning_bayessearch.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/03_complex_models/run_stacked_models.py` & `julearn-0.3.3.dev8/examples/03_complex_models/run_stacked_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/04_confounds/plot_confound_removal_classification.py` & `julearn-0.3.3.dev8/examples/04_confounds/plot_confound_removal_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/04_confounds/run_return_confounds.py` & `julearn-0.3.3.dev8/examples/04_confounds/run_return_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/05_customization/run_custom_scorers_regression.py` & `julearn-0.3.3.dev8/examples/05_customization/run_custom_scorers_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_cbpm_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_cbpm_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_confound_removal_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_confound_removal_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_cv_splitters_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_cv_splitters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_data_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_data_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_hyperparameters_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_hyperparameters_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 # the _grid_ of hyperparameters to try. As we see above, we have 3
 # hyperparameters to tune. So it constructs a 3-dimentional grid with all the
 # possible combinations of the hyperparameters values. The second step is to
 # perform cross-validation on each of the possible combinations of
 # hyperparameters values.
 #
 # Other searchers that ``julearn`` provides are the
-# :class:`~sklearn.model_selection.RandomizedSearchCV`, 
+# :class:`~sklearn.model_selection.RandomizedSearchCV`,
 # :class:`~skopt.BayesSearchCV` and
 # :class:`~optuna_integration.sklearn.OptunaSearchCV`.
 #
 # The randomized searcher
 # (:class:`~sklearn.model_selection.RandomizedSearchCV`) is similar to the
 # :class:`~sklearn.model_selection.GridSearchCV`, but instead
 # of trying all the possible combinations of hyperparameter values, it tries
@@ -379,22 +379,22 @@
 ###############################################################################
 # An example using optuna searcher is shown below. The searcher is specified
 # as ``"optuna"`` and the hyperparameters are specified as a dictionary with
 # the hyperparameters to tune and their distributions as for the bayesian
 # searcher. However, the optuna searcher behaviour is controlled by a
 # :class:`~optuna.study.Study` object. This object can be passed to the
 # searcher using the ``study`` parameter in the ``search_params`` dictionary.
-# 
+#
 # .. important::
 #    The optuna searcher requires that all the hyperparameters are specified
-#    as distributions, even the categorical ones. 
+#    as distributions, even the categorical ones.
 #
 # We first modify the pipeline creator so the ``select_k`` parameter is
 # specified as a distribution. We exemplarily use a categorical distribution
-# for the ``class_weight`` hyperparameter, trying the ``"balanced"`` and 
+# for the ``class_weight`` hyperparameter, trying the ``"balanced"`` and
 # ``None`` values.
 
 creator = PipelineCreator(problem_type="classification")
 creator.add("zscore")
 creator.add("select_k", k=(2, 4, "uniform"))
 creator.add(
     "svm",
@@ -441,20 +441,20 @@
 # Specifying distributions
 # ~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # The hyperparameters can be specified as distributions for the randomized
 # searcher, bayesian searcher and optuna searcher. The distributions are
 # either specified toolbox-specific method or  a tuple convention with the
 # following format: ``(low, high, distribution)`` where the distribution can
-# be either ``"log-uniform"`` or ``"uniform"`` or 
+# be either ``"log-uniform"`` or ``"uniform"`` or
 # ``(a, b, c, d, ..., "categorical")`` where ``a``, ``b``, ``c``, ``d``, etc.
 # are the possible categorical values for the hyperparameter.
 #
-# For example, we can specify the ``C`` and ``gamma`` hyperparameters of the 
-# :class:`~sklearn.svm.SVC` as  log-uniform distributions, while keeping 
+# For example, we can specify the ``C`` and ``gamma`` hyperparameters of the
+# :class:`~sklearn.svm.SVC` as  log-uniform distributions, while keeping
 # the ``with_mean`` parameter of the
 # :class:`~sklearn.preprocessing.StandardScaler` as a categorical parameter
 # with two options.
 
 
 creator = PipelineCreator(problem_type="classification")
 creator.add("zscore", with_mean=(True, False, "categorical"))
@@ -465,15 +465,15 @@
 )
 print(creator)
 
 ###############################################################################
 # While this will work for any of the ``random``, ``bayes`` or ``optuna``
 # searcher options, it is important to note that both ``bayes`` and ``optuna``
 # searchers accept further parameters to specify distributions. For example,
-# the ``bayes`` searcher distributions are defined using the 
+# the ``bayes`` searcher distributions are defined using the
 # :class:`~skopt.space.space.Categorical`, :class:`~skopt.space.space.Integer`
 # and :class:`~skopt.space.space.Real`.
 #
 # For example, we can define a log-uniform distribution with base 2 for the
 # ``C`` hyperparameter of the :class:`~sklearn.svm.SVC` model:
 from skopt.space import Real
 creator = PipelineCreator(problem_type="classification")
@@ -489,15 +489,15 @@
 # For the optuna searcher, the distributions are defined using the
 # :class:`~optuna.distributions.CategoricalDistribution`,
 # :class:`~optuna.distributions.FloatDistribution` and
 # :class:`~optuna.distributions.IntDistribution`.
 #
 #
 # For example, we can define a uniform distribution from 0.5 to 0.9 with a 0.05
-# step for the ``n_components`` of a :class:`~sklearn.decomposition.PCA` 
+# step for the ``n_components`` of a :class:`~sklearn.decomposition.PCA`
 # transformer, while keeping a log-uniform distribution for the ``C`` and
 # ``gamma`` hyperparameters of the :class:`~sklearn.svm.SVC` model.
 from optuna.distributions import FloatDistribution
 creator = PipelineCreator(problem_type="classification")
 creator.add("zscore")
 creator.add(
     "pca",
```

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_model_comparison_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_model_comparison_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_model_evaluation_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_model_evaluation_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_model_inspection_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_model_inspection_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_pipeline_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_pipeline_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_stacked_models_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_stacked_models_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/99_docs/run_target_transformer_docs.py` & `julearn-0.3.3.dev8/examples/99_docs/run_target_transformer_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/XX_disabled/dis_run_n_jobs.py` & `julearn-0.3.3.dev8/examples/XX_disabled/dis_run_n_jobs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/examples/XX_disabled/dis_run_target_confound_removal.py` & `julearn-0.3.3.dev8/examples/XX_disabled/dis_run_target_confound_removal.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/api.py` & `julearn-0.3.3.dev8/julearn/api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/base/column_types.py` & `julearn-0.3.3.dev8/julearn/base/column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/base/estimators.py` & `julearn-0.3.3.dev8/julearn/base/estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/base/tests/test_base_estimators.py` & `julearn-0.3.3.dev8/julearn/base/tests/test_base_estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/base/tests/test_column_types.py` & `julearn-0.3.3.dev8/julearn/base/tests/test_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/config.py` & `julearn-0.3.3.dev8/julearn/config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/conftest.py` & `julearn-0.3.3.dev8/julearn/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,14 +282,15 @@
     dict or None
         A dictionary with the search_params argument.
 
     """
 
     return request.param
 
+
 @fixture(
     params=[
         {"kind": "optuna", "n_trials": 10, "cv": 3},
         {"kind": "optuna", "timeout": 20},
     ],
     scope="function",
 )
@@ -306,14 +307,15 @@
     dict or None
         A dictionary with the search_params argument.
 
     """
 
     return request.param
 
+
 _tuning_params = {
     "zscore": {"with_mean": [True, False]},
     "pca": {"n_components": [0.2, 0.7]},
     "select_univariate": {"mode": ["k_best", "percentile"]},
     "rf": {"n_estimators": [2, 5]},
     "svm": {"C": [1, 2]},
     "ridge": {"alpha": [1, 2]},
```

### Comparing `julearn-0.3.3.dev4/julearn/inspect/_cv.py` & `julearn-0.3.3.dev8/julearn/inspect/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/_pipeline.py` & `julearn-0.3.3.dev8/julearn/inspect/_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/_preprocess.py` & `julearn-0.3.3.dev8/julearn/inspect/_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/inspector.py` & `julearn-0.3.3.dev8/julearn/inspect/inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/tests/test_cv.py` & `julearn-0.3.3.dev8/julearn/inspect/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/tests/test_inspector.py` & `julearn-0.3.3.dev8/julearn/inspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/tests/test_pipeline.py` & `julearn-0.3.3.dev8/julearn/inspect/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/inspect/tests/test_preprocess.py` & `julearn-0.3.3.dev8/julearn/inspect/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/__init__.py` & `julearn-0.3.3.dev8/julearn/model_selection/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,7 @@
 )
 
 from ._skopt_searcher import register_bayes_searcher
 from ._optuna_searcher import register_optuna_searcher
 
 register_bayes_searcher()
 register_optuna_searcher()
-
```

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/_optuna_searcher.py` & `julearn-0.3.3.dev8/julearn/model_selection/_optuna_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,18 @@
                 else:
                     logger.info(
                         f"Hyperparameter {k} is log-uniform float "
                         f"[{v[0]}, {v[1]}]"
                     )
                     out[k] = optd.FloatDistribution(v[0], v[1], log=True)
             elif v[2] == "categorical":
-                logger.info(f"Hyperparameter {k} is categorical with 2 "
-                            f"options: [{v[0]} and {v[1]}]")
+                logger.info(
+                    f"Hyperparameter {k} is categorical with 2 "
+                    f"options: [{v[0]} and {v[1]}]"
+                )
                 out[k] = optd.CategoricalDistribution((v[0], v[1]))
             else:
                 out[k] = v
         elif (
             isinstance(v, tuple)
             and isinstance(v[-1], str)
             and v[-1] == "categorical"
```

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/_skopt_searcher.py` & `julearn-0.3.3.dev8/julearn/model_selection/_skopt_searcher.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/available_searchers.py` & `julearn-0.3.3.dev8/julearn/model_selection/available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/continuous_stratified_kfold.py` & `julearn-0.3.3.dev8/julearn/model_selection/continuous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/stratified_bootstrap.py` & `julearn-0.3.3.dev8/julearn/model_selection/stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/tests/test_available_searchers.py` & `julearn-0.3.3.dev8/julearn/model_selection/tests/test_available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/tests/test_continous_stratified_kfold.py` & `julearn-0.3.3.dev8/julearn/model_selection/tests/test_continous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/tests/test_optuna_searcher.py` & `julearn-0.3.3.dev8/julearn/model_selection/tests/test_optuna_searcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from julearn.model_selection._optuna_searcher import (
     _prepare_optuna_hyperparameters_distributions,
 )
 
 
 optd = pytest.importorskip("optuna.distributions")
 
+
 @pytest.mark.parametrize(
     "params_to_tune,expected_types, expected_dist",
     [
         (
             {
                 "n_components": (0.2, 0.7, "uniform"),
                 "n_neighbors": (1.0, 10.0, "log-uniform"),
```

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/tests/test_skopt_searcher.py` & `julearn-0.3.3.dev8/julearn/model_selection/tests/test_skopt_searcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from julearn.model_selection._skopt_searcher import (
     _prepare_skopt_hyperparameters_distributions,
 )
 
 
 sksp = pytest.importorskip("skopt.space")
 
+
 @pytest.mark.parametrize(
     "params_to_tune,expected_types, expected_dist",
     [
         (
             {
                 "n_components": (0.2, 0.7, "uniform"),
                 "n_neighbors": (1.0, 10.0, "log-uniform"),
```

### Comparing `julearn-0.3.3.dev4/julearn/model_selection/tests/test_stratified_bootstrap.py` & `julearn-0.3.3.dev8/julearn/model_selection/tests/test_stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/models/available_models.py` & `julearn-0.3.3.dev8/julearn/models/available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/models/dynamic.py` & `julearn-0.3.3.dev8/julearn/models/dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/models/tests/test_available_models.py` & `julearn-0.3.3.dev8/julearn/models/tests/test_available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/models/tests/test_dynamic.py` & `julearn-0.3.3.dev8/julearn/models/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/models/tests/test_models.py` & `julearn-0.3.3.dev8/julearn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/merger.py` & `julearn-0.3.3.dev8/julearn/pipeline/merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,15 @@
         # Get the transformer/model of the first element
         t = reference_pipeline.named_steps[t_step_name]  # type: ignore
 
         # Check that all searchers have the same transformer/model.
         # TODO: Fix this comparison, as it always returns False.
         for s in pipelines[1:]:
             if isinstance(s, BaseSearchCV):
-                if (
-                    s.estimator.named_steps[t_step_name]  # type: ignore
-                    != t
-                ):
+                if s.estimator.named_steps[t_step_name] != t:  # type: ignore
                     different_steps.append(t_step_name)
                     break
             else:
                 if s.named_steps[t_step_name] != t:  # type: ignore
                     different_steps.append(t_step_name)
                     break
```

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/pipeline_creator.py` & `julearn-0.3.3.dev8/julearn/pipeline/pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/target_pipeline.py` & `julearn-0.3.3.dev8/julearn/pipeline/target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/target_pipeline_creator.py` & `julearn-0.3.3.dev8/julearn/pipeline/target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/tests/test_merger.py` & `julearn-0.3.3.dev8/julearn/pipeline/tests/test_merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,22 @@
     assert isinstance(merged, RandomizedSearchCV)
     assert isinstance(merged.estimator, Pipeline)  # type: ignore
     assert len(merged.estimator.named_steps) == 3  # type: ignore
     named_steps = list(merged.estimator.named_steps.keys())  # type: ignore
     assert "scaler" == named_steps[1]
     assert "rf" == named_steps[2]
     assert len(merged.param_distributions) == 3  # type: ignore
-    assert (
-        merged.param_distributions[-1]["rf__max_features"]  # type: ignore
-        == [2, 3, 7, 42]
-    )
+    assert merged.param_distributions[-1][
+        "rf__max_features"
+    ] == [  # type: ignore
+        2,
+        3,
+        7,
+        42,
+    ]
 
 
 def test_merger_errors() -> None:
     """Test that the merger raises errors when it should."""
     creator1 = PipelineCreator(problem_type="classification")
     creator1.add("zscore", name="scaler", apply_to="continuous")
     creator1.add("rf")
```

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/tests/test_pipeline_creator.py` & `julearn-0.3.3.dev8/julearn/pipeline/tests/test_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline.py` & `julearn-0.3.3.dev8/julearn/pipeline/tests/test_target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/pipeline/tests/test_target_pipeline_creator.py` & `julearn-0.3.3.dev8/julearn/pipeline/tests/test_target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/prepare.py` & `julearn-0.3.3.dev8/julearn/prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/scoring/available_scorers.py` & `julearn-0.3.3.dev8/julearn/scoring/available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/scoring/metrics.py` & `julearn-0.3.3.dev8/julearn/scoring/metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/scoring/tests/test_available_scorers.py` & `julearn-0.3.3.dev8/julearn/scoring/tests/test_available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/scoring/tests/test_metrics.py` & `julearn-0.3.3.dev8/julearn/scoring/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/stats/corrected_ttest.py` & `julearn-0.3.3.dev8/julearn/stats/corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/stats/tests/test_corrected_ttest.py` & `julearn-0.3.3.dev8/julearn/stats/tests/test_corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/tests/test_api.py` & `julearn-0.3.3.dev8/julearn/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,17 +451,16 @@
         sk_X,
         sk_y,  # type: ignore
         cv=cv_outer,  # type: ignore
         scoring=[scoring],
     )
 
     assert len(actual.columns) == len(expected) + 5  # type: ignore
-    assert (
-        len(actual["test_accuracy"])  # type: ignore
-        == len(expected["test_accuracy"])
+    assert len(actual["test_accuracy"]) == len(  # type: ignore
+        expected["test_accuracy"]
     )
     assert all(
         a == b
         for a, b in zip(
             actual["test_accuracy"],  # type: ignore
             expected["test_accuracy"],
         )
@@ -536,17 +535,16 @@
         cv=cv_outer,
         scoring=[scoring],
         groups=sk_groups,  # type: ignore
         fit_params={"groups": sk_groups},
     )
 
     assert len(actual.columns) == len(expected) + 5  # type: ignore
-    assert (
-        len(actual["test_accuracy"])  # type: ignore
-        == len(expected["test_accuracy"])
+    assert len(actual["test_accuracy"]) == len(  # type: ignore
+        expected["test_accuracy"]
     )
     assert all(
         a == b
         for a, b in zip(
             actual["test_accuracy"],  # type: ignore
             expected["test_accuracy"],
         )
@@ -626,17 +624,16 @@
         sk_X,
         sk_y,  # type: ignore
         cv=cv_outer,  # type: ignore
         scoring=[scoring],
     )
 
     assert len(actual.columns) == len(expected) + 5  # type: ignore
-    assert (
-        len(actual["test_accuracy"])  # type: ignore
-        == len(expected["test_accuracy"])
+    assert len(actual["test_accuracy"]) == len(  # type: ignore
+        expected["test_accuracy"]
     )
     assert all(
         a == b
         for a, b in zip(
             actual["test_accuracy"],  # type: ignore
             expected["test_accuracy"],
         )
@@ -742,21 +739,19 @@
         sk_y,  # type: ignore
         cv=cv_outer,  # type: ignore
         scoring=[scoring],
     )
 
     assert len(actual1.columns) == len(expected) + 5  # type: ignore
     assert len(actual2.columns) == len(expected) + 5  # type: ignore
-    assert (
-        len(actual1["test_accuracy"])  # type: ignore
-        == len(expected["test_accuracy"])
-    )
-    assert (
-        len(actual2["test_accuracy"])  # type: ignore
-        == len(expected["test_accuracy"])
+    assert len(actual1["test_accuracy"]) == len(  # type: ignore
+        expected["test_accuracy"]
+    )
+    assert len(actual2["test_accuracy"]) == len(  # type: ignore
+        expected["test_accuracy"]
     )
     assert all(
         a == b
         for a, b in zip(
             actual1["test_accuracy"],  # type: ignore
             expected["test_accuracy"],
         )
```

### Comparing `julearn-0.3.3.dev4/julearn/tests/test_config.py` & `julearn-0.3.3.dev8/julearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/tests/test_prepare.py` & `julearn-0.3.3.dev8/julearn/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/__init__.py` & `julearn-0.3.3.dev8/julearn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/available_transformers.py` & `julearn-0.3.3.dev8/julearn/transformers/available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/cbpm.py` & `julearn-0.3.3.dev8/julearn/transformers/cbpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,12 +280,14 @@
 
     def get_feature_names_out(self, input_features=None):
         """Get output feature names."""
         check_is_fitted(self)
         cols = (
             ["positive"]
             if self.used_corr_sign_ == "pos"
-            else ["negative"]
-            if self.used_corr_sign_ == "neg"
-            else ["positive", "negative"]
+            else (
+                ["negative"]
+                if self.used_corr_sign_ == "neg"
+                else ["positive", "negative"]
+            )
         )
         return np.array(cols, dtype=object)
```

### Comparing `julearn-0.3.3.dev4/julearn/transformers/confound_remover.py` & `julearn-0.3.3.dev8/julearn/transformers/confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/change_column_types.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/change_column_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,17 @@
         """
         self.feature_names_in_ = X.columns
         to_rename = {}
         for col in self.filter_columns(X).columns.tolist():
             if "__:type:__" in col:
                 name, old_type = col.split("__:type:__")
                 if old_type in self.X_types_renamer:
-                    to_rename[
-                        col
-                    ] = f"{name}__:type:__{self.X_types_renamer[old_type]}"
+                    to_rename[col] = (
+                        f"{name}__:type:__{self.X_types_renamer[old_type]}"
+                    )
         self._renamer = to_rename
         return self
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:  # noqa: N803
         """Change the column types.
 
         Parameters
```

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/drop_columns.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/filter_columns.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/set_column_types.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_change_column_types.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_drop_columns.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_filter_columns.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/dataframe/tests/test_set_column_types.py` & `julearn-0.3.3.dev8/julearn/transformers/dataframe/tests/test_set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/ju_column_transformer.py` & `julearn-0.3.3.dev8/julearn/transformers/ju_column_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/__init__.py` & `julearn-0.3.3.dev8/julearn/transformers/target/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/available_target_transformers.py` & `julearn-0.3.3.dev8/julearn/transformers/target/available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/ju_target_transformer.py` & `julearn-0.3.3.dev8/julearn/transformers/target/ju_target_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/ju_transformed_target_model.py` & `julearn-0.3.3.dev8/julearn/transformers/target/ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/target_confound_remover.py` & `julearn-0.3.3.dev8/julearn/transformers/target/target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/tests/test_available_target_transformers.py` & `julearn-0.3.3.dev8/julearn/transformers/target/tests/test_available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/tests/test_ju_transformed_target_model.py` & `julearn-0.3.3.dev8/julearn/transformers/target/tests/test_ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/target/tests/test_target_confound_remover.py` & `julearn-0.3.3.dev8/julearn/transformers/target/tests/test_target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/tests/test_available_transformers.py` & `julearn-0.3.3.dev8/julearn/transformers/tests/test_available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/tests/test_cbpm.py` & `julearn-0.3.3.dev8/julearn/transformers/tests/test_cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/tests/test_confounds.py` & `julearn-0.3.3.dev8/julearn/transformers/tests/test_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/transformers/tests/test_jucolumntransformers.py` & `julearn-0.3.3.dev8/julearn/transformers/tests/test_jucolumntransformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,17 +152,17 @@
     mean_unhealthy = (
         transformer_unhealthy.fit(X)
         .column_transformer_.transformers_[0][1]  # type: ignore
         .mean_
     )
 
     mean_both = (
-        transformer_both.fit(
-            X
-        ).column_transformer_.transformers_[0][1].mean_  # type: ignore
+        transformer_both.fit(X)
+        .column_transformer_.transformers_[0][1]
+        .mean_  # type: ignore
     )
 
     assert_almost_equal(
         transformer_healthy._select_rows(X, y=None)["X"].index.values, [0, 1]
     )
     assert_almost_equal(
         transformer_unhealthy._select_rows(X, None)["X"].index.values, [2, 3]
```

### Comparing `julearn-0.3.3.dev4/julearn/utils/_cv.py` & `julearn-0.3.3.dev8/julearn/utils/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/utils/checks.py` & `julearn-0.3.3.dev8/julearn/utils/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implement various checks for the input of the functions."""
+
 # Author: Federico Raimondo <f.raimondo@fz-juelich.de>
 # License: BSD 3 clause
 
 from typing import List
 
 import numpy as np
 import pandas as pd
```

### Comparing `julearn-0.3.3.dev4/julearn/utils/logging.py` & `julearn-0.3.3.dev8/julearn/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,17 +218,15 @@
     logger.error(msg)
     if exception is not None:
         raise klass(msg) from exception
     else:
         raise klass(msg)
 
 
-def warn_with_log(
-    msg: str, category: Type[Warning] = RuntimeWarning
-) -> None:
+def warn_with_log(msg: str, category: Type[Warning] = RuntimeWarning) -> None:
     """Warn, but first log it.
 
     Parameters
     ----------
     msg : str
         Warning message.
     category : subclass of Warning, optional
```

### Comparing `julearn-0.3.3.dev4/julearn/utils/testing.py` & `julearn-0.3.3.dev8/julearn/utils/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     y: str,
     data: pd.DataFrame,
     api_params: Dict[str, Any],
     sklearn_model: Union[EstimatorLike, ModelLike, Any],  # TODO: fix
     scorers: List[str],
     groups: Optional[str] = None,
     X_types: Optional[Dict[str, List[str]]] = None,  # noqa: N803
-    cv: Union[int, BaseCrossValidator]  = 5,
+    cv: Union[int, BaseCrossValidator] = 5,
     sk_y: Optional[np.ndarray] = None,
     decimal: int = 5,
 ):
     """Test scoring for a model, using the julearn and sklearn API.
 
     Parameters
     ----------
```

### Comparing `julearn-0.3.3.dev4/julearn/utils/tests/test_logging.py` & `julearn-0.3.3.dev8/julearn/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/utils/tests/test_version.py` & `julearn-0.3.3.dev8/julearn/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/utils/typing.py` & `julearn-0.3.3.dev8/julearn/utils/typing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/utils/versions.py` & `julearn-0.3.3.dev8/julearn/utils/versions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/viz/_scores.py` & `julearn-0.3.3.dev8/julearn/viz/_scores.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn/viz/res/julearn_logo_generalization.png` & `julearn-0.3.3.dev8/julearn/viz/res/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn.egg-info/PKG-INFO` & `julearn-0.3.3.dev8/julearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.3.dev4
+Version: 0.3.3.dev8
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
```

### Comparing `julearn-0.3.3.dev4/julearn.egg-info/SOURCES.txt` & `julearn-0.3.3.dev8/julearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/julearn.egg-info/requires.txt` & `julearn-0.3.3.dev8/julearn.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `julearn-0.3.3.dev4/pyproject.toml` & `julearn-0.3.3.dev8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,21 @@
 quiet-level = 3
 ignore-words = "ignore_words.txt"
 interactive = 0
 builtin = "clear,rare,informal,names,usage,code"
 
 [tool.ruff]
 line-length = 79
+extend-exclude = [
+    "__init__.py",
+    "docs",
+    "examples",
+]
+
+[tool.ruff.lint]
 select = [
     # flake8-bugbear
     "B",
     # flake8-blind-except
     "BLE",
     # flake8-comprehensions
     "C4",
@@ -132,19 +139,14 @@
     # pyupgrade
     "UP",
     # pycodestyle warnings
     "W",
     # flake8-2020
     "YTT",
 ]
-extend-exclude = [
-    "__init__.py",
-    "docs",
-    "examples",
-]
 extend-ignore = [
     # Use of `functools.lru_cache` or `functools.cache` on methods can lead to
     # memory leaks. The cache may retain instance references, preventing garbage
     # collection.
     "B019",
     # abstract class with no abstract methods
     "B024",
@@ -159,30 +161,30 @@
     "N802",
     # variable in function should be lowercase
     "N806",
     # use specific rule codes when ignoring type issues
     "PGH003",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-after-imports = 2
 known-first-party = ["julearn"]
 known-third-party =[
     "numpy",
     "pandas",
     "sklearn",
     "statsmodels",
     "bokeh",
     "panel",
     "param",
     "deslib",
     "pytest",
 ]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 20
 
 [tool.towncrier]
 directory = "docs/changes/newsfragments"
 filename = "docs/whats_new.rst"
 package = "julearn"
 # to use gh_substitutions
```

### Comparing `julearn-0.3.3.dev4/tox.ini` & `julearn-0.3.3.dev8/tox.ini`

 * *Files identical despite different names*

