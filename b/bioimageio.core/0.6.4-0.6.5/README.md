# Comparing `tmp/bioimageio.core-0.6.4.tar.gz` & `tmp/bioimageio.core-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.6.4.tar", last modified: Wed May 15 11:46:26 2024, max compression
+gzip compressed data, was "bioimageio.core-0.6.5.tar", last modified: Thu May 16 11:54:19 2024, max compression
```

## Comparing `bioimageio.core-0.6.4.tar` & `bioimageio.core-0.6.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-15 11:46:23.000000 bioimageio.core-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.134239 bioimageio.core-0.6.4/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.138239 bioimageio.core-0.6.4/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 11:46:23.000000 bioimageio.core-0.6.4/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_magic_tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_op_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/block_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/model_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/proc_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.134239 bioimageio.core-0.6.4/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-15 11:46:26.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 11:46:25.000000 bioimageio.core-0.6.4/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.142239 bioimageio.core-0.6.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/scripts/setup_dev_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/scripts/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 11:46:23.000000 bioimageio.core-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_any_model_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_bioimageio_spec_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_prediction_pipeline_device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/keras/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/test_add_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:46:26.146239 bioimageio.core-0.6.4/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-15 11:45:52.000000 bioimageio.core-0.6.4/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-16 11:54:17.000000 bioimageio.core-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.644246 bioimageio.core-0.6.5/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 11:54:17.000000 bioimageio.core-0.6.5/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/_magic_tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/_op_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15047 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/block_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/bioimageio/core/model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/proc_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/bioimageio/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/keras/_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.648246 bioimageio.core-0.6.5/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-16 11:54:19.000000 bioimageio.core-0.6.5/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-16 11:54:19.000000 bioimageio.core-0.6.5/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:54:19.000000 bioimageio.core-0.6.5/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 11:54:19.000000 bioimageio.core-0.6.5/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-16 11:54:19.000000 bioimageio.core-0.6.5/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 11:54:19.000000 bioimageio.core-0.6.5/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.652246 bioimageio.core-0.6.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/scripts/setup_dev_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/scripts/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_any_model_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_prediction_pipeline_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/weight_converter/keras/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/weight_converter/test_add_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:54:19.656246 bioimageio.core-0.6.5/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-16 11:53:47.000000 bioimageio.core-0.6.5/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.6.4/LICENSE` & `bioimageio.core-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/PKG-INFO` & `bioimageio.core-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
@@ -129,14 +129,18 @@
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.5
+        
+        * improve adapter error messages
+        
         ### 0.6.4
         
         * add `bioimageio validate-format` command
         * improve error messages and display of command results
         
         ### 0.6.3
```

### Comparing `bioimageio.core-0.6.4/README.md` & `bioimageio.core-0.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,18 @@
 
 ## Model Specification
 
 The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
 
 ## Changelog
 
+### 0.6.5
+
+* improve adapter error messages
+
 ### 0.6.4
 
 * add `bioimageio validate-format` command
 * improve error messages and display of command results
 
 ### 0.6.3
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/__init__.py` & `bioimageio.core-0.6.5/bioimageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/_magic_tensor_ops.py` & `bioimageio.core-0.6.5/bioimageio/core/_magic_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/_op_base.py` & `bioimageio.core-0.6.5/bioimageio/core/_op_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/_prediction_pipeline.py` & `bioimageio.core-0.6.5/bioimageio/core/_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/_resource_tests.py` & `bioimageio.core-0.6.5/bioimageio/core/_resource_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import traceback
 import warnings
 from typing import Dict, Hashable, List, Literal, Optional, Set, Tuple, Union
 
 import numpy as np
+from loguru import logger
 
 from bioimageio.core.sample import Sample
 from bioimageio.spec import (
     InvalidDescr,
     ResourceDescr,
     build_description,
     dump_description,
@@ -113,14 +114,16 @@
 
 def _test_model_inference(
     model: Union[v0_4.ModelDescr, v0_5.ModelDescr],
     weight_format: Optional[WeightsFormat],
     devices: Optional[List[str]],
     decimal: int,
 ) -> None:
+    test_name = "Reproduce test outputs from test inputs"
+    logger.info("starting '{}'", test_name)
     error: Optional[str] = None
     tb: List[str] = []
     try:
         inputs = get_test_inputs(model)
         expected = get_test_outputs(model)
 
         with create_prediction_pipeline(
@@ -146,15 +149,15 @@
                     break
     except Exception as e:
         error = str(e)
         tb = traceback.format_tb(e.__traceback__)
 
     model.validation_summary.add_detail(
         ValidationDetail(
-            name="Reproduce test outputs from test inputs",
+            name=test_name,
             status="passed" if error is None else "failed",
             errors=(
                 []
                 if error is None
                 else [
                     ErrorEntry(
                         loc=(
@@ -182,14 +185,18 @@
         (2, 1),
         (3, 2),
     },
 ) -> None:
     if not test_cases:
         return
 
+    logger.info(
+        "Testing inference with {} different input tensor sizes", len(test_cases)
+    )
+
     if not any(
         isinstance(a.size, v0_5.ParameterizedSize)
         for ipt in model.inputs
         for a in ipt.axes
     ):
         # no parameterized sizes => set n=0
         test_cases = {(0, b) for _n, b in test_cases}
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/axis.py` & `bioimageio.core-0.6.5/bioimageio/core/axis.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/block.py` & `bioimageio.core-0.6.5/bioimageio/core/block.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/block_meta.py` & `bioimageio.core-0.6.5/bioimageio/core/block_meta.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/commands.py` & `bioimageio.core-0.6.5/bioimageio/core/commands.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/common.py` & `bioimageio.core-0.6.5/bioimageio/core/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/digest_spec.py` & `bioimageio.core-0.6.5/bioimageio/core/digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/io.py` & `bioimageio.core-0.6.5/bioimageio/core/io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_keras_model_adapter.py` & `bioimageio.core-0.6.5/bioimageio/core/model_adapters/_keras_model_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,29 +22,33 @@
         keras,  # pyright: ignore[reportUnknownVariableType]
     )
 
     tf_version = Version(tf.__version__)  # pyright: ignore[reportUnknownArgumentType]
 except Exception:
     try:
         import keras  # pyright: ignore[reportMissingImports]
-    except Exception:
+    except Exception as e:
         keras = None
-
+        keras_error = str(e)
+    else:
+        keras_error = None
     tf_version = None
+else:
+    keras_error = None
 
 
 class KerasModelAdapter(ModelAdapter):
     def __init__(
         self,
         *,
         model_description: Union[v0_4.ModelDescr, v0_5.ModelDescr],
         devices: Optional[Sequence[str]] = None,
     ) -> None:
         if keras is None:
-            raise ImportError("keras")
+            raise ImportError(f"failed to import keras: {keras_error}")
 
         super().__init__()
         if model_description.weights.keras_hdf5 is None:
             raise ValueError("model has not keras_hdf5 weights specified")
         model_tf_version = model_description.weights.keras_hdf5.tensorflow_version
 
         if tf_version is None or model_tf_version is None:
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_model_adapter.py` & `bioimageio.core-0.6.5/bioimageio/core/model_adapters/_model_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,45 +73,45 @@
 
                     return PytorchModelAdapter(
                         outputs=model_description.outputs,
                         weights=weights.pytorch_state_dict,
                         devices=devices,
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
+                    errors.append(f"{wf}: {e}")
             elif (
                 wf == "tensorflow_saved_model_bundle"
                 and weights.tensorflow_saved_model_bundle is not None
             ):
                 try:
                     from ._tensorflow_model_adapter import TensorflowModelAdapter
 
                     return TensorflowModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
+                    errors.append(f"{wf}: {e}")
             elif wf == "onnx" and weights.onnx is not None:
                 try:
                     from ._onnx_model_adapter import ONNXModelAdapter
 
                     return ONNXModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
+                    errors.append(f"{wf}: {e}")
             elif wf == "torchscript" and weights.torchscript is not None:
                 try:
                     from ._torchscript_model_adapter import TorchscriptModelAdapter
 
                     return TorchscriptModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
+                    errors.append(f"{wf}: {e}")
             elif wf == "keras_hdf5" and weights.keras_hdf5 is not None:
                 # keras can either be installed as a separate package or used as part of tensorflow
                 # we try to first import the keras model adapter using the separate package and,
                 # if it is not available, try to load the one using tf
                 try:
                     from ._keras_model_adapter import (
                         KerasModelAdapter,
@@ -121,15 +121,15 @@
                     if keras is None:
                         from ._tensorflow_model_adapter import KerasModelAdapter
 
                     return KerasModelAdapter(
                         model_description=model_description, devices=devices
                     )
                 except Exception as e:
-                    errors.append(f"{wf}: {e}\n{traceback.format_stack()}")
+                    errors.append(f"{wf}: {e}")
 
         assert errors
         error_list = "\n - ".join(errors)
         raise ValueError(
             "None of the weight format specific model adapters could be created for"
             + f" '{model_description.id or model_description.name}'"
             + f" in this environment. Errors are:\n\n{error_list}.\n\n"
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.6.5/bioimageio/core/model_adapters/_onnx_model_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 
 from ..digest_spec import get_axes_infos
 from ..tensor import Tensor
 from ._model_adapter import ModelAdapter
 
 try:
     import onnxruntime as rt
-except Exception:
+except Exception as e:
     rt = None
+    rt_error = str(e)
+else:
+    rt_error = None
 
 
 class ONNXModelAdapter(ModelAdapter):
     def __init__(
         self,
         *,
         model_description: Union[v0_4.ModelDescr, v0_5.ModelDescr],
         devices: Optional[Sequence[str]] = None,
     ):
         if rt is None:
-            raise ImportError("onnxruntime")
+            raise ImportError(f"failed to import onnxruntime: {rt_error}")
 
         super().__init__()
         self._internal_output_axes = [
             tuple(a.id for a in get_axes_infos(out))
             for out in model_description.outputs
         ]
         if model_description.weights.onnx is None:
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_pytorch_model_adapter.py` & `bioimageio.core-0.6.5/bioimageio/core/model_adapters/_pytorch_model_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 from ..axis import AxisId
 from ..digest_spec import get_axes_infos, import_callable
 from ..tensor import Tensor
 from ._model_adapter import ModelAdapter
 
 try:
     import torch
-except Exception:
+except Exception as e:
     torch = None
+    torch_error = str(e)
+else:
+    torch_error = None
 
 
 class PytorchModelAdapter(ModelAdapter):
     def __init__(
         self,
         *,
         outputs: Union[
@@ -25,15 +28,16 @@
         ],
         weights: Union[
             v0_4.PytorchStateDictWeightsDescr, v0_5.PytorchStateDictWeightsDescr
         ],
         devices: Optional[Sequence[str]] = None,
     ):
         if torch is None:
-            raise ImportError("failed to import torch")
+            raise ImportError(f"failed to import torch: {torch_error}")
+
         super().__init__()
         self.output_dims = [tuple(a.id for a in get_axes_infos(out)) for out in outputs]
         self._network = self.get_network(weights)
         self._devices = self.get_devices(devices)
         self._network = self._network.to(self._devices[0])
 
         self._primary_device = self._devices[0]
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_tensorflow_model_adapter.py` & `bioimageio.core-0.6.5/bioimageio/core/model_adapters/_tensorflow_model_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 
 from ..digest_spec import get_axes_infos
 from ..tensor import Tensor
 from ._model_adapter import ModelAdapter
 
 try:
     import tensorflow as tf  # pyright: ignore[reportMissingImports]
-except Exception:
+except Exception as e:
     tf = None
+    tf_error = str(e)
+else:
+    tf_error = None
 
 
 class TensorflowModelAdapterBase(ModelAdapter):
     weight_format: Literal["keras_hdf5", "tensorflow_saved_model_bundle"]
 
     def __init__(
         self,
@@ -30,15 +33,15 @@
             v0_4.TensorflowSavedModelBundleWeightsDescr,
             v0_5.KerasHdf5WeightsDescr,
             v0_5.TensorflowSavedModelBundleWeightsDescr,
         ],
         model_description: Union[v0_4.ModelDescr, v0_5.ModelDescr],
     ):
         if tf is None:
-            raise ImportError("tensorflow")
+            raise ImportError(f"failed to import tensorflow: {tf_error}")
 
         super().__init__()
         self.model_description = model_description
         tf_version = v0_5.Version(
             tf.__version__  # pyright: ignore[reportUnknownArgumentType]
         )
         model_tf_version = weights.tensorflow_version
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/model_adapters/_torchscript_model_adapter.py` & `bioimageio.core-0.6.5/bioimageio/core/model_adapters/_torchscript_model_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,30 @@
 
 from ..digest_spec import get_axes_infos
 from ..tensor import Tensor
 from ._model_adapter import ModelAdapter
 
 try:
     import torch
-except Exception:
+except Exception as e:
     torch = None
+    torch_error = str(e)
+else:
+    torch_error = None
 
 
 class TorchscriptModelAdapter(ModelAdapter):
     def __init__(
         self,
         *,
         model_description: Union[v0_4.ModelDescr, v0_5.ModelDescr],
         devices: Optional[Sequence[str]] = None,
     ):
         if torch is None:
-            raise ImportError("torch")
+            raise ImportError(f"failed to import torch: {torch_error}")
 
         super().__init__()
         if model_description.weights.torchscript is None:
             raise ValueError(
                 f"No torchscript weights found for model {model_description.name}"
             )
```

### Comparing `bioimageio.core-0.6.4/bioimageio/core/proc_ops.py` & `bioimageio.core-0.6.5/bioimageio/core/proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/proc_setup.py` & `bioimageio.core-0.6.5/bioimageio/core/proc_setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/sample.py` & `bioimageio.core-0.6.5/bioimageio/core/sample.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/stat_calculators.py` & `bioimageio.core-0.6.5/bioimageio/core/stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/stat_measures.py` & `bioimageio.core-0.6.5/bioimageio/core/stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/tensor.py` & `bioimageio.core-0.6.5/bioimageio/core/tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/utils/testing.py` & `bioimageio.core-0.6.5/bioimageio/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/weight_converter/keras/_tensorflow.py` & `bioimageio.core-0.6.5/bioimageio/core/weight_converter/keras/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_onnx.py` & `bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_torchscript.py` & `bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/_torchscript.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio/core/weight_converter/torch/_utils.py` & `bioimageio.core-0.6.5/bioimageio/core/weight_converter/torch/_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.6.5/bioimageio.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
@@ -129,14 +129,18 @@
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.5
+        
+        * improve adapter error messages
+        
         ### 0.6.4
         
         * add `bioimageio validate-format` command
         * improve error messages and display of command results
         
         ### 0.6.3
```

### Comparing `bioimageio.core-0.6.4/bioimageio.core.egg-info/SOURCES.txt` & `bioimageio.core-0.6.5/bioimageio.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/pyproject.toml` & `bioimageio.core-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/scripts/setup_dev_env.py` & `bioimageio.core-0.6.5/scripts/setup_dev_env.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/scripts/show_diff.py` & `bioimageio.core-0.6.5/scripts/show_diff.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/setup.py` & `bioimageio.core-0.6.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     packages=find_namespace_packages(exclude=["tests"]),
     install_requires=[
-        "bioimageio.spec>=0.5.2.post5,<0.6",
+        "bioimageio.spec == 0.5.2.*",
         "fire",
         "imageio>=2.5",
         "loguru",
         "numpy",
         "pydantic-settings",
         "pydantic",
         "python-dotenv",
```

### Comparing `bioimageio.core-0.6.4/tests/test_bioimageio_spec_version.py` & `bioimageio.core-0.6.5/tests/test_bioimageio_spec_version.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_cli.py` & `bioimageio.core-0.6.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_digest_spec.py` & `bioimageio.core-0.6.5/tests/test_digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_prediction.py` & `bioimageio.core-0.6.5/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_prediction_pipeline.py` & `bioimageio.core-0.6.5/tests/test_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_prediction_pipeline_device_management.py` & `bioimageio.core-0.6.5/tests/test_prediction_pipeline_device_management.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_proc_ops.py` & `bioimageio.core-0.6.5/tests/test_proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_resource_tests.py` & `bioimageio.core-0.6.5/tests/test_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_stat_calculators.py` & `bioimageio.core-0.6.5/tests/test_stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_stat_measures.py` & `bioimageio.core-0.6.5/tests/test_stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/test_tensor.py` & `bioimageio.core-0.6.5/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/weight_converter/keras/test_tensorflow.py` & `bioimageio.core-0.6.5/tests/weight_converter/keras/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/weight_converter/test_add_weights.py` & `bioimageio.core-0.6.5/tests/weight_converter/test_add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/weight_converter/torch/test_onnx.py` & `bioimageio.core-0.6.5/tests/weight_converter/torch/test_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.4/tests/weight_converter/torch/test_torchscript.py` & `bioimageio.core-0.6.5/tests/weight_converter/torch/test_torchscript.py`

 * *Files identical despite different names*

