# Comparing `tmp/spox-0.9.2.tar.gz` & `tmp/spox-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spox-0.9.2.tar", last modified: Fri Oct 20 19:11:04 2023, max compression
+gzip compressed data, was "spox-0.9.3.tar", last modified: Mon Oct 23 14:42:30 2023, max compression
```

## Comparing `spox-0.9.2.tar` & `spox-0.9.3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.133710 spox-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-10-20 19:10:56.000000 spox-0.9.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-20 19:10:56.000000 spox-0.9.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.105709 spox-0.9.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-20 19:10:56.000000 spox-0.9.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-20 19:10:56.000000 spox-0.9.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-20 19:10:56.000000 spox-0.9.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.105709 spox-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-20 19:10:56.000000 spox-0.9.2/.github/workflows/build_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-20 19:10:56.000000 spox-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-10-20 19:10:56.000000 spox-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-10-20 19:10:56.000000 spox-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-20 19:10:56.000000 spox-0.9.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-20 19:10:56.000000 spox-0.9.2/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-20 19:10:56.000000 spox-0.9.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2023-10-20 19:10:56.000000 spox-0.9.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-10-20 19:10:56.000000 spox-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-20 19:11:04.133710 spox-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2023-10-20 19:10:56.000000 spox-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.105709 spox-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-20 19:10:56.000000 spox-0.9.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2023-10-20 19:10:56.000000 spox-0.9.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.109709 spox-0.9.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2023-10-20 19:10:56.000000 spox-0.9.2/docs/guides/advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2023-10-20 19:10:56.000000 spox-0.9.2/docs/guides/converter.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    38133 2023-10-20 19:10:56.000000 spox-0.9.2/docs/guides/example-model-netron.png
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2023-10-20 19:10:56.000000 spox-0.9.2/docs/guides/inference.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2023-10-20 19:10:56.000000 spox-0.9.2/docs/guides/inline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    50579 2023-10-20 19:10:56.000000 spox-0.9.2/docs/guides/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-10-20 19:10:56.000000 spox-0.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-20 19:10:56.000000 spox-0.9.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.109709 spox-0.9.2/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-20 19:10:56.000000 spox-0.9.2/docs/manual/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2023-10-20 19:10:56.000000 spox-0.9.2/docs/manual/operators.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-10-20 19:10:56.000000 spox-0.9.2/docs/manual/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2023-10-20 19:10:56.000000 spox-0.9.2/docs/manual/unstable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-20 19:10:56.000000 spox-0.9.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-20 19:10:56.000000 spox-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 19:11:04.133710 spox-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.101709 spox-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.113710 spox-0.9.2/src/spox/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_adapt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20284 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_future.py
--rw-r--r--   0 runner    (1001) docker     (127)    18834 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_internal_op.py
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_traverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_type_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_value_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.101709 spox-0.9.2/src/spox/opset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.101709 spox-0.9.2/src/spox/opset/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.117709 spox-0.9.2/src/spox/opset/ai/onnx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.117709 spox-0.9.2/src/spox/opset/ai/onnx/ml/
--rw-r--r--   0 runner    (1001) docker     (127)    63350 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/opset/ai/onnx/ml/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)   462668 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/opset/ai/onnx/v17.py
--rw-r--r--   0 runner    (1001) docker     (127)    93775 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/opset/ai/onnx/v18.py
--rw-r--r--   0 runner    (1001) docker     (127)    99994 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/opset/ai/onnx/v19.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 19:10:56.000000 spox-0.9.2/src/spox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.117709 spox-0.9.2/src/spox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-20 19:11:04.000000 spox-0.9.2/src/spox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2023-10-20 19:11:04.000000 spox-0.9.2/src/spox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 19:11:04.000000 spox-0.9.2/src/spox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-20 19:11:04.000000 spox-0.9.2/src/spox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-20 19:11:04.000000 spox-0.9.2/src/spox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.121709 spox-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 19:10:56.000000 spox-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-10-20 19:10:56.000000 spox-0.9.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.121709 spox-0.9.2/tests/full/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 19:10:56.000000 spox-0.9.2/tests/full/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2023-10-20 19:10:56.000000 spox-0.9.2/tests/full/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-10-20 19:10:56.000000 spox-0.9.2/tests/full/test_brackets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2023-10-20 19:10:56.000000 spox-0.9.2/tests/full/test_lifting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2023-10-20 19:10:56.000000 spox-0.9.2/tests/full/test_turing_completeness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.125709 spox-0.9.2/tests/future/
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2023-10-20 19:10:56.000000 spox-0.9.2/tests/future/test_var_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_adapt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_custom_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_equiv_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10402 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_opsets.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_standard_op.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_subgraphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_type_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2023-10-20 19:10:56.000000 spox-0.9.2/tests/test_value_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.125709 spox-0.9.2/tests/type_inference/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_array_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_category_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_imputer.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_one_hot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_tree_ensemble_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-20 19:10:56.000000 spox-0.9.2/tests/type_inference/test_tree_ensemble_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.125709 spox-0.9.2/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    26060 2023-10-20 19:10:56.000000 spox-0.9.2/tools/generate_opset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.129710 spox-0.9.2/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/class.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/construct.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/constructor.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/docstring.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.129710 spox-0.9.2/tools/templates/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/extras/const.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/extras/promote.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/extras/xif.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/extras/xloop.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/inherit.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/preamble.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/summary.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.133710 spox-0.9.2/tools/templates/type_inference/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/arrayfeatureextractor1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/binarizer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/categorymapper1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/compress11.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/if16.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/imputer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/linearregressor1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/loop16-fix.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/loop16.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/normalizer1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/onehot11.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/onehotencoder1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/scaler1.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/treeensembleclassifier3.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/type_inference/treeensembleregressor3.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 19:11:04.133710 spox-0.9.2/tools/templates/value_propagation/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-20 19:10:56.000000 spox-0.9.2/tools/templates/value_propagation/constant13.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.017766 spox-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2023-10-23 14:42:20.000000 spox-0.9.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-23 14:42:20.000000 spox-0.9.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.989765 spox-0.9.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-23 14:42:20.000000 spox-0.9.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-23 14:42:20.000000 spox-0.9.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-23 14:42:20.000000 spox-0.9.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.989765 spox-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-23 14:42:20.000000 spox-0.9.3/.github/workflows/build_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-23 14:42:20.000000 spox-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-10-23 14:42:20.000000 spox-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-10-23 14:42:20.000000 spox-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-23 14:42:20.000000 spox-0.9.3/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-23 14:42:20.000000 spox-0.9.3/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-23 14:42:20.000000 spox-0.9.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2023-10-23 14:42:20.000000 spox-0.9.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-10-23 14:42:20.000000 spox-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-23 14:42:30.017766 spox-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2023-10-23 14:42:20.000000 spox-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.989765 spox-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-23 14:42:20.000000 spox-0.9.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2023-10-23 14:42:20.000000 spox-0.9.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.993765 spox-0.9.3/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2023-10-23 14:42:20.000000 spox-0.9.3/docs/guides/advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2023-10-23 14:42:20.000000 spox-0.9.3/docs/guides/converter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    38133 2023-10-23 14:42:20.000000 spox-0.9.3/docs/guides/example-model-netron.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2023-10-23 14:42:20.000000 spox-0.9.3/docs/guides/inference.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2023-10-23 14:42:20.000000 spox-0.9.3/docs/guides/inline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    50579 2023-10-23 14:42:20.000000 spox-0.9.3/docs/guides/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-10-23 14:42:20.000000 spox-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-23 14:42:20.000000 spox-0.9.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.993765 spox-0.9.3/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-23 14:42:20.000000 spox-0.9.3/docs/manual/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2023-10-23 14:42:20.000000 spox-0.9.3/docs/manual/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-10-23 14:42:20.000000 spox-0.9.3/docs/manual/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2023-10-23 14:42:20.000000 spox-0.9.3/docs/manual/unstable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-23 14:42:20.000000 spox-0.9.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-23 14:42:20.000000 spox-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 14:42:30.017766 spox-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.985765 spox-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.997765 spox-0.9.3/src/spox/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20284 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18834 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_internal_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_traverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_type_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_value_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.985765 spox-0.9.3/src/spox/opset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.985765 spox-0.9.3/src/spox/opset/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.001765 spox-0.9.3/src/spox/opset/ai/onnx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.001765 spox-0.9.3/src/spox/opset/ai/onnx/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)    63350 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/opset/ai/onnx/ml/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)   462668 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/opset/ai/onnx/v17.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93775 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/opset/ai/onnx/v18.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99994 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/opset/ai/onnx/v19.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:20.000000 spox-0.9.3/src/spox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:29.997765 spox-0.9.3/src/spox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-23 14:42:29.000000 spox-0.9.3/src/spox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2023-10-23 14:42:29.000000 spox-0.9.3/src/spox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 14:42:29.000000 spox-0.9.3/src/spox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-23 14:42:29.000000 spox-0.9.3/src/spox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-23 14:42:29.000000 spox-0.9.3/src/spox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.005766 spox-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:20.000000 spox-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-10-23 14:42:20.000000 spox-0.9.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.005766 spox-0.9.3/tests/full/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:20.000000 spox-0.9.3/tests/full/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2023-10-23 14:42:20.000000 spox-0.9.3/tests/full/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2023-10-23 14:42:20.000000 spox-0.9.3/tests/full/test_brackets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2023-10-23 14:42:20.000000 spox-0.9.3/tests/full/test_lifting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2023-10-23 14:42:20.000000 spox-0.9.3/tests/full/test_turing_completeness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.005766 spox-0.9.3/tests/future/
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2023-10-23 14:42:20.000000 spox-0.9.3/tests/future/test_var_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_adapt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_custom_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_equiv_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10402 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_opsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_standard_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_subgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_type_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-10-23 14:42:20.000000 spox-0.9.3/tests/test_value_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.009766 spox-0.9.3/tests/type_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_array_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_category_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_imputer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_tree_ensemble_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-23 14:42:20.000000 spox-0.9.3/tests/type_inference/test_tree_ensemble_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.009766 spox-0.9.3/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    26060 2023-10-23 14:42:20.000000 spox-0.9.3/tools/generate_opset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.009766 spox-0.9.3/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/class.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/construct.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/constructor.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/docstring.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.009766 spox-0.9.3/tools/templates/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/extras/const.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/extras/promote.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/extras/xif.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/extras/xloop.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/inherit.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/preamble.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/summary.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.013766 spox-0.9.3/tools/templates/type_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/arrayfeatureextractor1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/binarizer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/categorymapper1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/compress11.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/if16.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/imputer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/linearregressor1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/loop16-fix.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/loop16.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/normalizer1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/onehot11.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/onehotencoder1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/scaler1.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/treeensembleclassifier3.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/type_inference/treeensembleregressor3.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 14:42:30.013766 spox-0.9.3/tools/templates/value_propagation/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-23 14:42:20.000000 spox-0.9.3/tools/templates/value_propagation/constant13.jinja2
```

### Comparing `spox-0.9.2/.github/workflows/build_and_publish.yml` & `spox-0.9.3/.github/workflows/build_and_publish.yml`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/.github/workflows/ci.yml` & `spox-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/.gitignore` & `spox-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/.pre-commit-config.yaml` & `spox-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/CHANGELOG.rst` & `spox-0.9.3/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,34 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Change log
 ==========
 
+0.9.3 (2023-10-23)
+------------------
+
+**Bug fixes**
+
+- Address missing Value Infos when building singleton model for shape inference.
+- Fix issue where Value Propagation failure prevents model creation/inlining.
+
+
 0.9.2 (2023-10-20)
 ------------------
 
 **Other changes**
 
 - Fix a deprecation warning from one of Spox's dependencies.
 
 0.9.1 (2023-10-05)
 ------------------
 
-**Bug fix**
+**Bug fixes**
 
 - The node-adaption no longer fails if faced with a node that has repeating inputs.
 - Forego version adaption of inlined models if no nodes are from the default domain.
 
 
 0.9.0 (2023-06-12)
 ------------------
```

### Comparing `spox-0.9.2/LICENSE` & `spox-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/PKG-INFO` & `spox-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spox
-Version: 0.9.2
+Version: 0.9.3
 Summary: A framework for constructing ONNX computational graphs.
 Author-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Maintainer-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Project-URL: Source, https://github.com/quantco/spox
 Keywords: machine-learning,onnx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `spox-0.9.2/README.md` & `spox-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/Makefile` & `spox-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/conf.py` & `spox-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/guides/advanced.ipynb` & `spox-0.9.3/docs/guides/advanced.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/guides/converter.ipynb` & `spox-0.9.3/docs/guides/converter.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/guides/example-model-netron.png` & `spox-0.9.3/docs/guides/example-model-netron.png`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/guides/inference.ipynb` & `spox-0.9.3/docs/guides/inference.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/guides/inline.ipynb` & `spox-0.9.3/docs/guides/inline.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/guides/tutorial.ipynb` & `spox-0.9.3/docs/guides/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/index.rst` & `spox-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/make.bat` & `spox-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/manual/operators.rst` & `spox-0.9.3/docs/manual/operators.rst`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/manual/overview.rst` & `spox-0.9.3/docs/manual/overview.rst`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/docs/manual/unstable.rst` & `spox-0.9.3/docs/manual/unstable.rst`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/pyproject.toml` & `spox-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_adapt.py` & `spox-0.9.3/src/spox/_adapt.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_attributes.py` & `spox-0.9.3/src/spox/_attributes.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_build.py` & `spox-0.9.3/src/spox/_build.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_debug.py` & `spox-0.9.3/src/spox/_debug.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_exceptions.py` & `spox-0.9.3/src/spox/_exceptions.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_fields.py` & `spox-0.9.3/src/spox/_fields.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_function.py` & `spox-0.9.3/src/spox/_function.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_future.py` & `spox-0.9.3/src/spox/_future.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_graph.py` & `spox-0.9.3/src/spox/_graph.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_inline.py` & `spox-0.9.3/src/spox/_inline.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,15 @@
             i.name: wrap_feed(var._value)
             for i, var in zip(self.model.graph.input, self.inputs.inputs)
         }
         output_feed = run(self.model, input_feed)
         return {
             f"outputs_{k}": unwrap_feed(var.unwrap_type(), output_feed[o.name]).value
             for k, (o, var) in enumerate(zip(self.graph.output, self.outputs.outputs))
+            if o.name in output_feed
         }
 
     def to_onnx(
         self, scope: Scope, doc_string: Optional[str] = None, build_subgraph=None
     ) -> List[onnx.NodeProto]:
         input_names: Dict[str, int] = {
             p.name: i for i, p in enumerate(self.graph.input)
```

### Comparing `spox-0.9.2/src/spox/_internal_op.py` & `spox-0.9.3/src/spox/_internal_op.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_node.py` & `spox-0.9.3/src/spox/_node.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_public.py` & `spox-0.9.3/src/spox/_public.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_schemas.py` & `spox-0.9.3/src/spox/_schemas.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_scope.py` & `spox-0.9.3/src/spox/_scope.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_shape.py` & `spox-0.9.3/src/spox/_shape.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_standard.py` & `spox-0.9.3/src/spox/_standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Module implementing a base for standard ONNX operators, which use the functionality of ONNX node-level inference."""
-import logging
 from typing import TYPE_CHECKING, Callable, Dict, Tuple
 
 import numpy
 import onnx
 import onnx.reference
 import onnx.shape_inference
 from onnx.defs import OpSchema
@@ -171,23 +170,17 @@
         model, scope = self.to_singleton_onnx_model(with_dummy_subgraphs=False)
         wrap_feed, run, unwrap_feed = _value_prop.get_backend_calls()
         input_feed = {
             scope.var[var]: wrap_feed(var._value)
             for var in self.inputs.get_vars().values()
             if var._value
         }
-        try:
-            output_feed = run(model, input_feed)
-        except Exception as e:
-            logging.debug(
-                f"Value propagation in {self.get_op_repr()} on backend "
-                f"{_value_prop._VALUE_PROP_BACKEND} failed with - "
-                f"{type(e).__name__}: {e}"
-            )
-            output_feed = {}
+
+        output_feed = run(model, input_feed)
+
         results = {
             scope.var[str(name)]
             ._which_output: unwrap_feed(scope.var[str(name)].unwrap_type(), result)
             .value
             for name, result in output_feed.items()
         }
         return {k: v for k, v in results.items() if k is not None}
@@ -240,16 +233,20 @@
     """
     if graph.requested_arguments is None:
         raise RuntimeError("Subgraph must have requested_arguments to construct dummy.")
 
     inputs = []
     for i, arr in enumerate(graph.requested_arguments):
         inputs.append(arr.unwrap_type()._to_onnx_value_info(f"__dummy_input{i}"))
+
+    value_infos = []
     nodes = []
     outputs = []
     for i, arr in enumerate(graph.requested_results.values()):
         outer = f"__dummy_outer_output{i}"
+        value_infos.append(arr.unwrap_type()._to_onnx_value_info(outer))
         out = f"__dummy_output{i}"
         outputs.append(arr.unwrap_type()._to_onnx_value_info(out))
         nodes.append(onnx.helper.make_node("Identity", [outer], [out]))
-
-    return onnx.helper.make_graph(nodes, f"__dummy_{key}", inputs, outputs)
+    return onnx.helper.make_graph(
+        nodes, f"__dummy_{key}", inputs, outputs, value_info=value_infos
+    )
```

### Comparing `spox-0.9.2/src/spox/_traverse.py` & `spox-0.9.3/src/spox/_traverse.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_type_system.py` & `spox-0.9.3/src/spox/_type_system.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_utils.py` & `spox-0.9.3/src/spox/_utils.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/_value_prop.py` & `spox-0.9.3/src/spox/_value_prop.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+import logging
 import warnings
 from dataclasses import dataclass
 from typing import Dict, List, Union
 
 import numpy
 import onnx
 import onnx.reference
@@ -151,31 +152,42 @@
 
 def _run_reference_implementation(
     model: onnx.ModelProto, input_feed: Dict[str, RefValue]
 ) -> Dict[str, RefValue]:
     try:
         session = onnx.reference.ReferenceEvaluator(model)
         output_feed = dict(zip(session.output_names, session.run(None, input_feed)))
-    except NotImplementedError:
+    except Exception as e:
         # Give up on value propagation if an implementation is missing.
+        logging.debug(
+            f"Value propagation in {model} on the ONNX reference implementation failed with - "
+            f"{type(e).__name__}: {e}"
+        )
         return {}
     return output_feed
 
 
 def _run_onnxruntime(
     model: onnx.ModelProto, input_feed: Dict[str, ORTValue]
 ) -> Dict[str, ORTValue]:
     import onnxruntime
 
     # Silence possible warnings during execution (especially constant folding)
     options = onnxruntime.SessionOptions()
     options.log_severity_level = 3
-    session = onnxruntime.InferenceSession(model.SerializeToString(), options)
-    output_names = [output.name for output in session.get_outputs()]
-    output_feed = dict(zip(output_names, session.run(None, input_feed)))
+    try:
+        session = onnxruntime.InferenceSession(model.SerializeToString(), options)
+        output_names = [output.name for output in session.get_outputs()]
+        output_feed = dict(zip(output_names, session.run(None, input_feed)))
+    except Exception as e:
+        logging.debug(
+            f"Value propagation in {model} on the onnxruntime failed with - "
+            f"{type(e).__name__}: {e}"
+        )
+        return {}
     return output_feed
 
 
 def get_backend_calls():
     if _VALUE_PROP_BACKEND == ValuePropBackend.REFERENCE:
         wrap_feed = PropValue.to_ref_value
         run = _run_reference_implementation
```

### Comparing `spox-0.9.2/src/spox/_var.py` & `spox-0.9.3/src/spox/_var.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/opset/ai/onnx/ml/v3.py` & `spox-0.9.3/src/spox/opset/ai/onnx/ml/v3.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/opset/ai/onnx/v17.py` & `spox-0.9.3/src/spox/opset/ai/onnx/v17.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/opset/ai/onnx/v18.py` & `spox-0.9.3/src/spox/opset/ai/onnx/v18.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox/opset/ai/onnx/v19.py` & `spox-0.9.3/src/spox/opset/ai/onnx/v19.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/src/spox.egg-info/PKG-INFO` & `spox-0.9.3/src/spox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spox
-Version: 0.9.2
+Version: 0.9.3
 Summary: A framework for constructing ONNX computational graphs.
 Author-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Maintainer-email: Jakub Bachurski <kbachurski@gmail.com>, Christian Bourjau <christian.bourjau@quantco.com>
 Project-URL: Source, https://github.com/quantco/spox
 Keywords: machine-learning,onnx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `spox-0.9.2/src/spox.egg-info/SOURCES.txt` & `spox-0.9.3/src/spox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/conftest.py` & `spox-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/full/conftest.py` & `spox-0.9.3/tests/full/conftest.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/full/test_brackets.py` & `spox-0.9.3/tests/full/test_brackets.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/full/test_lifting.py` & `spox-0.9.3/tests/full/test_lifting.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/full/test_turing_completeness.py` & `spox-0.9.3/tests/full/test_turing_completeness.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/future/test_var_operators.py` & `spox-0.9.3/tests/future/test_var_operators.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_adapt.py` & `spox-0.9.3/tests/test_adapt.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """
 <
  ir_version: 8,
  opset_import: ["" : 12]
 >
 agraph (float[1, N] A) => (float[N] B)
 {
-    B = Squeeze<axes: floats = [0]>(A)
+    B = Squeeze<axes = [0]>(A)
 }
 """
     )
 
 
 @pytest.fixture
 def old_identity() -> onnx.ModelProto:
```

### Comparing `spox-0.9.2/tests/test_attr.py` & `spox-0.9.3/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_broadcast.py` & `spox-0.9.3/tests/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_constructors.py` & `spox-0.9.3/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_custom_operator.py` & `spox-0.9.3/tests/test_custom_operator.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_equiv_types.py` & `spox-0.9.3/tests/test_equiv_types.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_function.py` & `spox-0.9.3/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_graph.py` & `spox-0.9.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_initializer.py` & `spox-0.9.3/tests/test_initializer.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_inline.py` & `spox-0.9.3/tests/test_inline.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_opsets.py` & `spox-0.9.3/tests/test_opsets.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_public.py` & `spox-0.9.3/tests/test_public.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_standard_op.py` & `spox-0.9.3/tests/test_standard_op.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_subgraphs.py` & `spox-0.9.3/tests/test_subgraphs.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_tensor.py` & `spox-0.9.3/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/test_type_translation.py` & `spox-0.9.3/tests/test_type_translation.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_array_feature_extractor.py` & `spox-0.9.3/tests/type_inference/test_array_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_compress.py` & `spox-0.9.3/tests/type_inference/test_compress.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_imputer.py` & `spox-0.9.3/tests/type_inference/test_imputer.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_label_encoder.py` & `spox-0.9.3/tests/type_inference/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_linear_regressor.py` & `spox-0.9.3/tests/type_inference/test_linear_regressor.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_one_hot.py` & `spox-0.9.3/tests/type_inference/test_one_hot.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_one_hot_encoder.py` & `spox-0.9.3/tests/type_inference/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_scaler.py` & `spox-0.9.3/tests/type_inference/test_scaler.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tests/type_inference/test_tree_ensemble_classifier.py` & `spox-0.9.3/tests/type_inference/test_tree_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/generate_opset.py` & `spox-0.9.3/tools/generate_opset.py`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/class.jinja2` & `spox-0.9.3/tools/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/construct.jinja2` & `spox-0.9.3/tools/templates/construct.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/constructor.jinja2` & `spox-0.9.3/tools/templates/constructor.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/docstring.jinja2` & `spox-0.9.3/tools/templates/docstring.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/extras/promote.jinja2` & `spox-0.9.3/tools/templates/extras/promote.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/extras/xif.jinja2` & `spox-0.9.3/tools/templates/extras/xif.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/extras/xloop.jinja2` & `spox-0.9.3/tools/templates/extras/xloop.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/preamble.jinja2` & `spox-0.9.3/tools/templates/preamble.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/arrayfeatureextractor1.jinja2` & `spox-0.9.3/tools/templates/type_inference/arrayfeatureextractor1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/compress11.jinja2` & `spox-0.9.3/tools/templates/type_inference/compress11.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/if16.jinja2` & `spox-0.9.3/tools/templates/type_inference/if16.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/imputer1.jinja2` & `spox-0.9.3/tools/templates/type_inference/imputer1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/loop16.jinja2` & `spox-0.9.3/tools/templates/type_inference/loop16.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/onehot11.jinja2` & `spox-0.9.3/tools/templates/type_inference/onehot11.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/scaler1.jinja2` & `spox-0.9.3/tools/templates/type_inference/scaler1.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/type_inference/treeensembleclassifier3.jinja2` & `spox-0.9.3/tools/templates/type_inference/treeensembleclassifier3.jinja2`

 * *Files identical despite different names*

### Comparing `spox-0.9.2/tools/templates/value_propagation/constant13.jinja2` & `spox-0.9.3/tools/templates/value_propagation/constant13.jinja2`

 * *Files identical despite different names*

