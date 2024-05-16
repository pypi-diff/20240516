# Comparing `tmp/nemos-0.1.1.tar.gz` & `tmp/nemos-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemos-0.1.1.tar", last modified: Tue Apr 16 19:53:26 2024, max compression
+gzip compressed data, was "nemos-0.1.2.tar", last modified: Tue Apr 16 21:06:50 2024, max compression
```

## Comparing `nemos-0.1.1.tar` & `nemos-0.1.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.458010 nemos-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.438010 nemos-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.438010 nemos-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.438010 nemos-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/workflows/connect.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-16 19:53:22.000000 nemos-0.1.1/.github/workflows/deploy-pure-python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 19:53:22.000000 nemos-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 19:53:22.000000 nemos-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    45579 2024-04-16 19:53:22.000000 nemos-0.1.1/CCN-letterFoot.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-16 19:53:22.000000 nemos-0.1.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-16 19:53:22.000000 nemos-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 19:53:22.000000 nemos-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:53:22.000000 nemos-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-16 19:53:26.458010 nemos-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-16 19:53:22.000000 nemos-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.442010 nemos-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    57441 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/CCN-logo-wText.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.442010 nemos-0.1.1/docs/api_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_01_basis_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_04_pynapple_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_05_sklearn_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/_plot_06_magic_designer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/plot_02_glm_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/plot_03_glm_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/api_guide/plot_04_population_glm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   101811 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data.png
--rw-r--r--   0 runner    (1001) docker     (127)   141981 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-epochs.svg
--rw-r--r--   0 runner    (1001) docker     (127)   141785 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-response.svg
--rw-r--r--   0 runner    (1001) docker     (127)   141744 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-stimulus.svg
--rw-r--r--   0 runner    (1001) docker     (127)   142136 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated-units.svg
--rw-r--r--   0 runner    (1001) docker     (127)    85629 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/allen_data_annotated.gif
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)   130022 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/glm_features_scheme.svg
--rw-r--r--   0 runner    (1001) docker     (127)    62970 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/glm_population_scheme.svg
--rw-r--r--   0 runner    (1001) docker     (127)   133950 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/glm_scheme.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/assets/lnp_model.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/background/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/_plot_04_modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/background/background_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/background_utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_00_conceptual_intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_01_1D_basis_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_02_ND_basis_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/background/plot_03_1D_convolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.446009 nemos-0.1.1/docs/developers_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/01-basis_module.md
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/02-base_class.md
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/03-observation_models.md
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/04-regularizer.md
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/05-glm.md
--rw-r--r--   0 runner    (1001) docker     (127)   294441 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/GLM_scheme.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/developers_notes/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/gallery_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)   100847 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/head_dir_tuning.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.450010 nemos-0.1.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/javascripts/katex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.450010 nemos-0.1.1/docs/neural_modeling/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.450010 nemos-0.1.1/docs/neural_modeling/examples_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/nemos.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    31660 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/examples_utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    28528 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_01_current_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_02_head_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_03_grid_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_04_v1_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/neural_modeling/plot_05_place_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-16 19:53:22.000000 nemos-0.1.1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-16 19:53:22.000000 nemos-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-16 19:53:22.000000 nemos-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:53:26.458010 nemos-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.434010 nemos-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.454010 nemos-0.1.1/src/nemos/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    61643 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    41490 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20962 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/observation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/proximal_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/pytrees.py
--rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/regularizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/type_casting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-16 19:53:22.000000 nemos-0.1.1/src/nemos/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.458010 nemos-0.1.1/src/nemos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 19:53:26.000000 nemos-0.1.1/src/nemos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:53:26.458010 nemos-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)   103841 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/simulate_coupled_neurons_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)   162098 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    74427 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_observation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_proximal_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_pytrees.py
--rw-r--r--   0 runner    (1001) docker     (127)    34407 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_regularizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19890 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_type_casting.py
--rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/test_vallidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-16 19:53:22.000000 nemos-0.1.1/tests/utils_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 19:53:22.000000 nemos-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.266739 nemos-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.246739 nemos-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 21:06:43.000000 nemos-0.1.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.246739 nemos-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-16 21:06:43.000000 nemos-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 21:06:43.000000 nemos-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.246739 nemos-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-16 21:06:43.000000 nemos-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-16 21:06:43.000000 nemos-0.1.2/.github/workflows/connect.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-16 21:06:43.000000 nemos-0.1.2/.github/workflows/deploy-pure-python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 21:06:43.000000 nemos-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 21:06:43.000000 nemos-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    45579 2024-04-16 21:06:43.000000 nemos-0.1.2/CCN-letterFoot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-16 21:06:43.000000 nemos-0.1.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-16 21:06:43.000000 nemos-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 21:06:43.000000 nemos-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 21:06:43.000000 nemos-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-16 21:06:50.266739 nemos-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-16 21:06:43.000000 nemos-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.246739 nemos-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    57441 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/CCN-logo-wText.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.250739 nemos-0.1.2/docs/api_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/_plot_01_basis_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/_plot_04_pynapple_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/_plot_05_sklearn_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/_plot_06_magic_designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/plot_02_glm_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/plot_03_glm_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/api_guide/plot_04_population_glm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.254739 nemos-0.1.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   101811 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/allen_data.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141981 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/allen_data_annotated-epochs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   141785 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/allen_data_annotated-response.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   141744 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/allen_data_annotated-stimulus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   142136 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/allen_data_annotated-units.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    85629 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/allen_data_annotated.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)   130022 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/glm_features_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    62970 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/glm_population_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   133950 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/glm_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24604 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/assets/lnp_model.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.254739 nemos-0.1.2/docs/background/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/_plot_04_modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.254739 nemos-0.1.2/docs/background/background_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/background_utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/plot_00_conceptual_intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/plot_01_1D_basis_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/plot_02_ND_basis_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/background/plot_03_1D_convolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.254739 nemos-0.1.2/docs/developers_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/01-basis_module.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/02-base_class.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/03-observation_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/04-regularizer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/05-glm.md
+-rw-r--r--   0 runner    (1001) docker     (127)   294441 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/GLM_scheme.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/developers_notes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/gallery_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100847 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/head_dir_tuning.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.258739 nemos-0.1.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/javascripts/katex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.258739 nemos-0.1.2/docs/neural_modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.258739 nemos-0.1.2/docs/neural_modeling/examples_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/examples_utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/examples_utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/examples_utils/nemos.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    31660 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/examples_utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28528 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/plot_01_current_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/plot_02_head_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/plot_03_grid_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/plot_04_v1_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/neural_modeling/plot_05_place_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-16 21:06:43.000000 nemos-0.1.2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-16 21:06:43.000000 nemos-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-16 21:06:43.000000 nemos-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:06:50.266739 nemos-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.242739 nemos-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.262739 nemos-0.1.2/src/nemos/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61643 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41490 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20962 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/observation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/proximal_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/pytrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/regularizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/type_casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15524 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-16 21:06:43.000000 nemos-0.1.2/src/nemos/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.266739 nemos-0.1.2/src/nemos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-16 21:06:50.000000 nemos-0.1.2/src/nemos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-16 21:06:50.000000 nemos-0.1.2/src/nemos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:06:50.000000 nemos-0.1.2/src/nemos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 21:06:50.000000 nemos-0.1.2/src/nemos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 21:06:50.000000 nemos-0.1.2/src/nemos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:06:50.266739 nemos-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14454 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103841 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/simulate_coupled_neurons_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162098 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74427 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_observation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_proximal_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_pytrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34407 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_regularizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19890 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_type_casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/test_vallidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-16 21:06:43.000000 nemos-0.1.2/tests/utils_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-16 21:06:43.000000 nemos-0.1.2/tox.ini
```

### Comparing `nemos-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `nemos-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `nemos-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/.github/workflows/ci.yml` & `nemos-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/.github/workflows/connect.yml` & `nemos-0.1.2/.github/workflows/connect.yml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/.github/workflows/deploy-pure-python.yml` & `nemos-0.1.2/.github/workflows/deploy-pure-python.yml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/.gitignore` & `nemos-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/.readthedocs.yaml` & `nemos-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/CCN-letterFoot.png` & `nemos-0.1.2/CCN-letterFoot.png`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/CITATION.cff` & `nemos-0.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/CODE_OF_CONDUCT.md` & `nemos-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/CONTRIBUTING.md` & `nemos-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/LICENSE` & `nemos-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/PKG-INFO` & `nemos-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemos
-Version: 0.1.1
+Version: 0.1.2
 Summary: NEural MOdelS, a statistical modeling framework for neuroscience.
 Author: nemos authors
 License: MIT License
         
         Copyright (c) 2023 nemos authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,18 +25,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: neuroscience,Poisson-GLM
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.4
 Requires-Dist: jaxopt>=0.6
 Requires-Dist: numpy>1.20
 Requires-Dist: scipy>=1.10
 Requires-Dist: typing_extensions>=4.6
@@ -64,15 +64,15 @@
 Requires-Dist: dandi; extra == "docs"
 Requires-Dist: ipython; extra == "docs"
 Requires-Dist: matplotlib>=3.7; extra == "docs"
 
 # nemos 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/flatironinstitute/nemos/blob/main/LICENSE)
-![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.9%7C3.10%7C3.11-blue.svg)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![codecov](https://codecov.io/gh/flatironinstitute/nemos/graph/badge.svg?token=vvtrcTFNeu)](https://codecov.io/gh/flatironinstitute/nemos)
 [![Documentation Status](https://readthedocs.org/projects/nemos/badge/?version=latest)](https://nemos.readthedocs.io/en/latest/?badge=latest)
 [![nemos CI](https://github.com/flatironinstitute/nemos/actions/workflows/ci.yml/badge.svg)](https://github.com/flatironinstitute/nemos/actions/workflows/ci.yml)
 
 
 `nemos` (NEural MOdelS) is a statistical modeling framework optimized for systems neuroscience and powered by [JAX](https://jax.readthedocs.io/en/latest/). 
@@ -201,20 +201,20 @@
 
 
 ## Installation
 Run the following `pip` command in your virtual environment.
 
 **For macOS/Linux users:**
  ```bash
- pip install git+https://github.com/flatironinstitute/nemos.git
+ pip install nemos
  ```
 
 **For Windows users:**
  ```
- python -m pip install git+https://github.com/flatironinstitute/nemos.git
+ python -m pip install nemos
  ```
 
 For more details, including specifics for GPU users and developers, refer to `nemos` [docs](https://nemos.readthedocs.io/en/latest/installation/).
 
 
 ## Disclaimer
```

### Comparing `nemos-0.1.1/README.md` & `nemos-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # nemos 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/flatironinstitute/nemos/blob/main/LICENSE)
-![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.9%7C3.10%7C3.11-blue.svg)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![codecov](https://codecov.io/gh/flatironinstitute/nemos/graph/badge.svg?token=vvtrcTFNeu)](https://codecov.io/gh/flatironinstitute/nemos)
 [![Documentation Status](https://readthedocs.org/projects/nemos/badge/?version=latest)](https://nemos.readthedocs.io/en/latest/?badge=latest)
 [![nemos CI](https://github.com/flatironinstitute/nemos/actions/workflows/ci.yml/badge.svg)](https://github.com/flatironinstitute/nemos/actions/workflows/ci.yml)
 
 
 `nemos` (NEural MOdelS) is a statistical modeling framework optimized for systems neuroscience and powered by [JAX](https://jax.readthedocs.io/en/latest/). 
@@ -134,20 +134,20 @@
 
 
 ## Installation
 Run the following `pip` command in your virtual environment.
 
 **For macOS/Linux users:**
  ```bash
- pip install git+https://github.com/flatironinstitute/nemos.git
+ pip install nemos
  ```
 
 **For Windows users:**
  ```
- python -m pip install git+https://github.com/flatironinstitute/nemos.git
+ python -m pip install nemos
  ```
 
 For more details, including specifics for GPU users and developers, refer to `nemos` [docs](https://nemos.readthedocs.io/en/latest/installation/).
 
 
 ## Disclaimer
```

### Comparing `nemos-0.1.1/docs/CCN-logo-wText.png` & `nemos-0.1.2/docs/CCN-logo-wText.png`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/api_guide/plot_02_glm_demo.py` & `nemos-0.1.2/docs/api_guide/plot_02_glm_demo.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/api_guide/plot_03_glm_pytree.py` & `nemos-0.1.2/docs/api_guide/plot_03_glm_pytree.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/api_guide/plot_04_population_glm.py` & `nemos-0.1.2/docs/api_guide/plot_04_population_glm.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/allen_data.png` & `nemos-0.1.2/docs/assets/allen_data.png`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/allen_data_annotated-epochs.svg` & `nemos-0.1.2/docs/assets/allen_data_annotated-epochs.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/allen_data_annotated-response.svg` & `nemos-0.1.2/docs/assets/allen_data_annotated-response.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/allen_data_annotated-stimulus.svg` & `nemos-0.1.2/docs/assets/allen_data_annotated-stimulus.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/allen_data_annotated-units.svg` & `nemos-0.1.2/docs/assets/allen_data_annotated-units.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/allen_data_annotated.gif` & `nemos-0.1.2/docs/assets/allen_data_annotated.gif`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/glm_features_scheme.svg` & `nemos-0.1.2/docs/assets/glm_features_scheme.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/glm_population_scheme.svg` & `nemos-0.1.2/docs/assets/glm_population_scheme.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/glm_scheme.svg` & `nemos-0.1.2/docs/assets/glm_scheme.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/assets/lnp_model.svg` & `nemos-0.1.2/docs/assets/lnp_model.svg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/background/background_utils/plotting.py` & `nemos-0.1.2/docs/background/background_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/background/plot_00_conceptual_intro.py` & `nemos-0.1.2/docs/background/plot_00_conceptual_intro.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/background/plot_01_1D_basis_function.py` & `nemos-0.1.2/docs/background/plot_01_1D_basis_function.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/background/plot_02_ND_basis_function.py` & `nemos-0.1.2/docs/background/plot_02_ND_basis_function.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/background/plot_03_1D_convolution.py` & `nemos-0.1.2/docs/background/plot_03_1D_convolution.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/01-basis_module.md` & `nemos-0.1.2/docs/developers_notes/01-basis_module.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/02-base_class.md` & `nemos-0.1.2/docs/developers_notes/02-base_class.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/03-observation_models.md` & `nemos-0.1.2/docs/developers_notes/03-observation_models.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/04-regularizer.md` & `nemos-0.1.2/docs/developers_notes/04-regularizer.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/05-glm.md` & `nemos-0.1.2/docs/developers_notes/05-glm.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/GLM_scheme.jpg` & `nemos-0.1.2/docs/developers_notes/GLM_scheme.jpg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/developers_notes/README.md` & `nemos-0.1.2/docs/developers_notes/README.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/gallery_conf.py` & `nemos-0.1.2/docs/gallery_conf.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/gen_ref_pages.py` & `nemos-0.1.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/head_dir_tuning.jpg` & `nemos-0.1.2/docs/head_dir_tuning.jpg`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/index.md` & `nemos-0.1.2/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,20 +132,20 @@
     executed epoch-by-epoch, avoiding the risk of introducing artifacts from gaps in your time-series.
 
 ## Installation
 Run the following `pip` command in your virtual environment.
 
 **For macOS/Linux users:**
  ```bash
- pip install git+https://github.com/flatironinstitute/nemos.git
+ pip install nemos
  ```
 
 **For Windows users:**
  ```
- python -m pip install git+https://github.com/flatironinstitute/nemos.git
+ python -m pip install nemos
  ```
 
 For more details, including specifics for GPU users and developers, refer to `nemos` [docs](https://nemos.readthedocs.io/en/latest/installation/).
 
 
 ## Disclaimer
```

### Comparing `nemos-0.1.1/docs/installation.md` & `nemos-0.1.2/docs/installation.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,20 +41,20 @@
 After creating you virtual environment, follow one of the following sections below, depending on whether you need GPU support or not:
 ### CPU Installation
 
 To install `nemos` on a system without a GPU, run this command from within your activated environment, 
 
 **For macOS/Linux users:**
  ```bash
-  pip install git+https://github.com/flatironinstitute/nemos.git
+  pip install nemos
  ```
 
 **For Windows users:**
  ```
- python -m pip install git+https://github.com/flatironinstitute/nemos.git
+ python -m pip install nemos
  ```
 
 ### GPU Installation
 
 !!! warning
     JAX does not guarantee GPU support for Windows, see [here](https://jax.readthedocs.io/en/latest/installation.html#supported-platforms) for updates.
 
@@ -82,8 +82,8 @@
     cd nemos
     ```
 
 2. **Install in editable mode:** Install the package in editable mode (using the `-e` option) and include the developer dependencies (using `[dev]`):
 
     ```bash
     pip install -e .[dev]
-    ```
+    ```
```

### Comparing `nemos-0.1.1/docs/neural_modeling/examples_utils/data.py` & `nemos-0.1.2/docs/neural_modeling/examples_utils/data.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/examples_utils/model.py` & `nemos-0.1.2/docs/neural_modeling/examples_utils/model.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/examples_utils/plotting.py` & `nemos-0.1.2/docs/neural_modeling/examples_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/plot_01_current_injection.py` & `nemos-0.1.2/docs/neural_modeling/plot_01_current_injection.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/plot_02_head_direction.py` & `nemos-0.1.2/docs/neural_modeling/plot_02_head_direction.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/plot_03_grid_cells.py` & `nemos-0.1.2/docs/neural_modeling/plot_03_grid_cells.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/plot_04_v1_cells.py` & `nemos-0.1.2/docs/neural_modeling/plot_04_v1_cells.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/neural_modeling/plot_05_place_cells.py` & `nemos-0.1.2/docs/neural_modeling/plot_05_place_cells.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/docs/quickstart.md` & `nemos-0.1.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/mkdocs.yml` & `nemos-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/pyproject.toml` & `nemos-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nemos"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{name = "nemos authors"}]
 description = "NEural MOdelS, a statistical modeling framework for neuroscience."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = ["neuroscience", "Poisson-GLM"]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 
 # Define dependencies for the project
 dependencies = [
     "jax>=0.4",                     # Numerical computing library
     "jaxopt>=0.6",                  # Optimization library built on JAX
     "numpy>1.20",                   # Numerical computing library
```

### Comparing `nemos-0.1.1/src/nemos/base_class.py` & `nemos-0.1.2/src/nemos/base_class.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/basis.py` & `nemos-0.1.2/src/nemos/basis.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/convolve.py` & `nemos-0.1.2/src/nemos/convolve.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/exceptions.py` & `nemos-0.1.2/src/nemos/exceptions.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/glm.py` & `nemos-0.1.2/src/nemos/glm.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/observation_models.py` & `nemos-0.1.2/src/nemos/observation_models.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/proximal_operator.py` & `nemos-0.1.2/src/nemos/proximal_operator.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/pytrees.py` & `nemos-0.1.2/src/nemos/pytrees.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/regularizer.py` & `nemos-0.1.2/src/nemos/regularizer.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/simulation.py` & `nemos-0.1.2/src/nemos/simulation.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/tree_utils.py` & `nemos-0.1.2/src/nemos/tree_utils.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/type_casting.py` & `nemos-0.1.2/src/nemos/type_casting.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos/utils.py` & `nemos-0.1.2/src/nemos/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,49 +66,14 @@
 
     if pytree_map_and_reduce(lambda x: x.ndim <= axis, any, tree):
         raise ValueError(
             "'axis' must be smaller than the number of dimensions of any array in 'tree'."
         )
 
 
-def check_convolve_input_dims(basis_matrix: jnp.ndarray, time_series: Any):
-    """
-    Check the dimensions of inputs for convolution operation.
-
-    This function validates that the `basis_matrix` is 2-dimensional and the `time_series`
-    is either a pytree of 2-dimensional arrays or a single 3-dimensional array.
-
-    Parameters
-    ----------
-    basis_matrix :
-        A 2-dimensional array representing the basis matrix.
-    time_series :
-        A pytree of 2-dimensional arrays or a single 3-dimensional array representing the time series.
-
-    Raises
-    ------
-    ValueError
-        If `basis_matrix` is not a 2-dimensional array or if `time_series` is not a pytree of
-        2-dimensional arrays or a single 3-dimensional array.
-    """
-    # check input size
-    if not check_dimensionality(basis_matrix, expected_dim=2):
-        raise ValueError("basis_matrix must be a 2 dimensional array-like object.")
-
-    try:
-        if time_series.ndim != 3:
-            raise AttributeError
-    except AttributeError:
-        if not check_dimensionality(time_series, 2):
-            raise ValueError(
-                "time_series must be a pytree of 2 dimensional array-like objects or a"
-                " 3 dimensional array-like object."
-            )
-
-
 def check_non_empty(pytree: Any, pytree_name: str):
     """
     Check if any array in the pytree is empty.
 
     Parameters
     ----------
     pytree :
```

### Comparing `nemos-0.1.1/src/nemos/validation.py` & `nemos-0.1.2/src/nemos/validation.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/src/nemos.egg-info/PKG-INFO` & `nemos-0.1.2/src/nemos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemos
-Version: 0.1.1
+Version: 0.1.2
 Summary: NEural MOdelS, a statistical modeling framework for neuroscience.
 Author: nemos authors
 License: MIT License
         
         Copyright (c) 2023 nemos authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,18 +25,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: neuroscience,Poisson-GLM
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.4
 Requires-Dist: jaxopt>=0.6
 Requires-Dist: numpy>1.20
 Requires-Dist: scipy>=1.10
 Requires-Dist: typing_extensions>=4.6
@@ -64,15 +64,15 @@
 Requires-Dist: dandi; extra == "docs"
 Requires-Dist: ipython; extra == "docs"
 Requires-Dist: matplotlib>=3.7; extra == "docs"
 
 # nemos 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/flatironinstitute/nemos/blob/main/LICENSE)
-![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.9%7C3.10%7C3.11-blue.svg)
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![codecov](https://codecov.io/gh/flatironinstitute/nemos/graph/badge.svg?token=vvtrcTFNeu)](https://codecov.io/gh/flatironinstitute/nemos)
 [![Documentation Status](https://readthedocs.org/projects/nemos/badge/?version=latest)](https://nemos.readthedocs.io/en/latest/?badge=latest)
 [![nemos CI](https://github.com/flatironinstitute/nemos/actions/workflows/ci.yml/badge.svg)](https://github.com/flatironinstitute/nemos/actions/workflows/ci.yml)
 
 
 `nemos` (NEural MOdelS) is a statistical modeling framework optimized for systems neuroscience and powered by [JAX](https://jax.readthedocs.io/en/latest/). 
@@ -201,20 +201,20 @@
 
 
 ## Installation
 Run the following `pip` command in your virtual environment.
 
 **For macOS/Linux users:**
  ```bash
- pip install git+https://github.com/flatironinstitute/nemos.git
+ pip install nemos
  ```
 
 **For Windows users:**
  ```
- python -m pip install git+https://github.com/flatironinstitute/nemos.git
+ python -m pip install nemos
  ```
 
 For more details, including specifics for GPU users and developers, refer to `nemos` [docs](https://nemos.readthedocs.io/en/latest/installation/).
 
 
 ## Disclaimer
```

### Comparing `nemos-0.1.1/src/nemos.egg-info/SOURCES.txt` & `nemos-0.1.2/src/nemos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/conftest.py` & `nemos-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/simulate_coupled_neurons_params.json` & `nemos-0.1.2/tests/simulate_coupled_neurons_params.json`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_base_class.py` & `nemos-0.1.2/tests/test_base_class.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_basis.py` & `nemos-0.1.2/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_convolution.py` & `nemos-0.1.2/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_glm.py` & `nemos-0.1.2/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_observation_models.py` & `nemos-0.1.2/tests/test_observation_models.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_proximal_operator.py` & `nemos-0.1.2/tests/test_proximal_operator.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_pytrees.py` & `nemos-0.1.2/tests/test_pytrees.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_regularizer.py` & `nemos-0.1.2/tests/test_regularizer.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_simulation.py` & `nemos-0.1.2/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_tree_utils.py` & `nemos-0.1.2/tests/test_tree_utils.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_type_casting.py` & `nemos-0.1.2/tests/test_type_casting.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/test_utils.py` & `nemos-0.1.2/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from contextlib import nullcontext as does_not_raise
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pynapple as nap
 import pytest
+from scipy.interpolate import splev
 
 from nemos import utils
 
 
 @pytest.mark.parametrize(
     "arrays, expected_out",
     [
@@ -475,7 +476,85 @@
 
         assert np.isnan(
             shifted_series[0, -1]
         ).all(), "Last time bin should be NaN for anti-causal shift"
         assert np.array_equal(
             shifted_series[0, :-1], time_series[0, 1:]
         ), "Anti-causal shift did not work as expected"
+
+
+# Sample functions to test
+def correct_function(x):
+    return jnp.sin(x)  # Returns a jax.numpy.ndarray and is differentiable
+
+
+def non_ndarray_function(x):
+    return [x, x]  # Not returning a jax.numpy.ndarray
+
+
+def nondifferentiable_function(x):
+    knots = np.linspace(0, 1, 10)
+    tck = np.zeros(10)
+    tck[0] = 1
+    return splev(x, (knots, tck, 3), 0)  # Not differentiable
+
+
+def non_preserving_shape_function(x):
+    return jnp.sum(x)  # Does not preserve input shape, returns scalar
+
+
+def scalar_function(x):
+    return jnp.sum(x)  # Returns a scalar
+
+
+# Test cases with the match parameter
+def test_assert_returns_ndarray():
+    # Should pass
+    utils.assert_returns_ndarray(
+        correct_function, [jnp.array([1.0])], "correct_function"
+    )
+
+    # Should fail and match the error message
+    with pytest.raises(TypeError, match="must return a jax.numpy.ndarray"):
+        utils.assert_returns_ndarray(
+            non_ndarray_function, [jnp.array([1.0])], "non_ndarray_function"
+        )
+
+
+def test_assert_differentiable():
+    # Should pass
+    utils.assert_differentiable(correct_function, "correct_function")
+
+    # Should fail and match the error message
+    with pytest.raises(TypeError, match="is not differentiable"):
+        utils.assert_differentiable(
+            nondifferentiable_function, "nondifferentiable_function"
+        )
+
+
+def test_assert_preserve_shape():
+    # Should pass
+    utils.assert_preserve_shape(
+        correct_function, [jnp.array([1.0, 2.0])], "correct_function", 0
+    )
+
+    # Should fail and match the error message
+    with pytest.raises(ValueError, match="must preserve the input array shape"):
+        utils.assert_preserve_shape(
+            non_preserving_shape_function,
+            [jnp.array([1.0, 2.0])],
+            "non_preserving_shape_function",
+            0,
+        )
+
+
+def test_assert_scalar_func():
+    # Should pass
+    utils.assert_scalar_func(
+        scalar_function, [jnp.array([1.0, 2.0])], "scalar_function"
+    )
+
+    # Should fail and match the error message
+    with pytest.raises(TypeError, match="should return a scalar"):
+        utils.assert_scalar_func(
+            correct_function, [jnp.array([1.0])], "correct_function"
+        )
```

### Comparing `nemos-0.1.1/tests/test_vallidation.py` & `nemos-0.1.2/tests/test_vallidation.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tests/utils_testing.py` & `nemos-0.1.2/tests/utils_testing.py`

 * *Files identical despite different names*

### Comparing `nemos-0.1.1/tox.ini` & `nemos-0.1.2/tox.ini`

 * *Files identical despite different names*

