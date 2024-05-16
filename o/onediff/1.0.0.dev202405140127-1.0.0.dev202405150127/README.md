# Comparing `tmp/onediff-1.0.0.dev202405140127.tar.gz` & `tmp/onediff-1.0.0.dev202405150127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.0.0.dev202405140127.tar", last modified: Tue May 14 01:27:35 2024, max compression
+gzip compressed data, was "onediff-1.0.0.dev202405150127.tar", last modified: Wed May 15 01:27:58 2024, max compression
```

## Comparing `onediff-1.0.0.dev202405140127.tar` & `onediff-1.0.0.dev202405150127.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.614687 onediff-1.0.0.dev202405140127/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.614687 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.618687 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.618687 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.618687 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.618687 onediff-1.0.0.dev202405140127/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.618687 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.618687 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/backends/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.622687 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.622687 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.622687 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/with_fx_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/with_fx_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-14 01:27:35.000000 onediff-1.0.0.dev202405140127/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-14 01:27:35.000000 onediff-1.0.0.dev202405140127/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:27:35.000000 onediff-1.0.0.dev202405140127/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 01:27:35.000000 onediff-1.0.0.dev202405140127/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 01:27:35.000000 onediff-1.0.0.dev202405140127/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:27:35.626687 onediff-1.0.0.dev202405140127/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-14 01:27:28.000000 onediff-1.0.0.dev202405140127/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.744598 onediff-1.0.0.dev202405150127/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.744598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.744598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.748598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.752598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.752598 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_fx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_fx_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 01:27:58.000000 onediff-1.0.0.dev202405150127/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:27:58.756599 onediff-1.0.0.dev202405150127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-15 01:27:53.000000 onediff-1.0.0.dev202405150127/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.0.0.dev202405140127/LICENSE` & `onediff-1.0.0.dev202405150127/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/PKG-INFO` & `onediff-1.0.0.dev202405150127/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405140127
+Version: 1.0.0.dev202405150127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,15 @@
 <img src="imgs/onediff_logo.png" height="100">
 </p>
 
 ---
 <p align="center">
   <a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip install"></a>
   <a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Stars&color=green"></a>
+  <a href="https://github.com/siliconflow/onediff?tab=Apache-2.0-1-ov-file#readme" target="_blank"><img src="https://img.shields.io/github/license/siliconflow/onediff"></a>
   <a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community wiki-green"></a>
   <a href="https://twitter.com/search?q=%22onediff%22&src=typed_query&f=live" target="_blank"><img src="https://img.shields.io/badge/Twitter-Discuss-green?logo=twitter&amp"></a>
   <a href="https://discord.gg/RKJTjZMcPQ" target="_blank"><img src="https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square"></a>
 </p>
 
 <p align="center">
   <a href="https://github.com/siliconflow/onediff/milestone/3" target="_blank"><img src="https://img.shields.io/github/milestones/progress/siliconflow/onediff/3"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405140127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405150127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -12,16 +12,17 @@
 Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: transformers>=4.27.1 Requires-Dist:
 diffusers>=0.19.3 Requires-Dist: accelerate Requires-Dist: torch
                             [imgs/onediff_logo.png]
 ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _i_n_s_t_a_l_l_]_[_h_t_t_p_s_:_/
                    _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/
-  _o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_ _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
+ _o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+  _l_i_c_e_n_s_e_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y
+           _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
         _g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_]_[_h_t_t_p_s_:_/_/_d_c_b_a_d_g_e_._v_e_r_c_e_l_._a_p_p_/_a_p_i_/_s_e_r_v_e_r_/
                            _R_K_J_T_j_Z_M_c_P_Q_?_s_t_y_l_e_=_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_m_i_l_e_s_t_o_n_e_s_/_p_r_o_g_r_e_s_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_3_]
       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_c_l_o_s_e_d_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_c_o_l_o_r_=_b_l_u_e_]_[_h_t_t_p_s_:_/_/
   _g_i_t_h_u_b_._c_o_m_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_s_d_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
         _g_i_t_h_u_b_._c_o_m_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_e_x_a_m_p_l_e_s_._y_m_l_/
```

### Comparing `onediff-1.0.0.dev202405140127/README.md` & `onediff-1.0.0.dev202405150127/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 <img src="imgs/onediff_logo.png" height="100">
 </p>
 
 ---
 <p align="center">
   <a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip install"></a>
   <a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Stars&color=green"></a>
+  <a href="https://github.com/siliconflow/onediff?tab=Apache-2.0-1-ov-file#readme" target="_blank"><img src="https://img.shields.io/github/license/siliconflow/onediff"></a>
   <a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community wiki-green"></a>
   <a href="https://twitter.com/search?q=%22onediff%22&src=typed_query&f=live" target="_blank"><img src="https://img.shields.io/badge/Twitter-Discuss-green?logo=twitter&amp"></a>
   <a href="https://discord.gg/RKJTjZMcPQ" target="_blank"><img src="https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square"></a>
 </p>
 
 <p align="center">
   <a href="https://github.com/siliconflow/onediff/milestone/3" target="_blank"><img src="https://img.shields.io/github/milestones/progress/siliconflow/onediff/3"></a>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                             [imgs/onediff_logo.png]
 ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _i_n_s_t_a_l_l_]_[_h_t_t_p_s_:_/
                    _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/
-  _o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_ _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
+ _o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+  _l_i_c_e_n_s_e_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y
+           _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
         _g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_]_[_h_t_t_p_s_:_/_/_d_c_b_a_d_g_e_._v_e_r_c_e_l_._a_p_p_/_a_p_i_/_s_e_r_v_e_r_/
                            _R_K_J_T_j_Z_M_c_P_Q_?_s_t_y_l_e_=_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_m_i_l_e_s_t_o_n_e_s_/_p_r_o_g_r_e_s_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_3_]
       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_c_l_o_s_e_d_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_c_o_l_o_r_=_b_l_u_e_]_[_h_t_t_p_s_:_/_/
   _g_i_t_h_u_b_._c_o_m_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_s_d_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
         _g_i_t_h_u_b_._c_o_m_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_e_x_a_m_p_l_e_s_._y_m_l_/
```

### Comparing `onediff-1.0.0.dev202405140127/setup.py` & `onediff-1.0.0.dev202405150127/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.0.0.dev202405150127/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/__init__.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,19 +141,21 @@
                     *args, **kwargs
                 )
         return output
 
     def __getattr__(self, name):
         return getattr(self._deployable_module_model, name)
 
-    def load_graph(self, file_path, device=None, run_warmup=True):
-        self.get_graph().load_graph(file_path, device, run_warmup)
+    def load_graph(self, file_path, device=None, run_warmup=True, *, state_dict=None):
+        self.get_graph().load_graph(
+            file_path, device, run_warmup, state_dict=state_dict
+        )
 
-    def save_graph(self, file_path):
-        self.get_graph().save_graph(file_path)
+    def save_graph(self, file_path, *, process_state_dict=lambda x: x):
+        self.get_graph().save_graph(file_path, process_state_dict=process_state_dict)
 
     def extra_repr(self) -> str:
         return self._deployable_module_model.extra_repr()
 
     def set_graph_file(self, file_path: str) -> None:
         """ Sets the path of the graph file.
```

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,25 @@
         # self.config.enable_cudnn_conv_heuristic_search_algo(False)
         self.config.allow_fuse_add_to_output(True)
 
     def build(self, *args, **kwargs):
         return self.model(*args, **kwargs)
 
     @cost_cnt(transform_mgr.debug_mode)
-    def load_graph(self, file_path, device=None, run_warmup=True):
-        state_dict = flow.load(file_path)
+    def load_graph(self, file_path, device=None, run_warmup=True, *, state_dict=None):
+        state_dict = state_dict if state_dict is not None else flow.load(file_path)
         self.graph_state_dict = state_dict  # used for OneflowGraph.save_graph
+
         if device is not None:
             state_dict = flow.nn.Graph.runtime_state_dict_to(state_dict, device)
+
         self.load_runtime_state_dict(state_dict, warmup_with_run=run_warmup)
 
     @cost_cnt(transform_mgr.debug_mode)
-    def save_graph(self, file_path):
+    def save_graph(self, file_path, *, process_state_dict: lambda x: x):
         if hasattr(self, "graph_state_dict"):
             flow.save(self.graph_state_dict, file_path)
             return
 
         state_dict = self.runtime_state_dict()
 
         import oneflow.framework.args_tree as args_tree
@@ -55,8 +57,9 @@
             out_tree = args_tree.ArgsTree((output, None), False)
             # dataclass type needs to be reversed to torch type to avoid saving error.
             out = out_tree.map_leaf(reverse_dataclass)
             state_dict[name]["outputs_original"] = out[0]
 
         args_tree._is_dataclass = original_is_dataclass
 
+        state_dict = process_state_dict(state_dict)
         flow.save(state_dict, file_path)
```

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/env_var.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/options.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/options.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if isinstance(submodule, torch.nn.Conv2d) and hasattr(
             submodule, GRAPH_RELATED_TENSOR_ATTR
         ):
             delattr(submodule, GRAPH_RELATED_TENSOR_ATTR)
 
     for weight_name, weight_tensor in constant_folding_info.items():
         submodule = deployable_module._torch_module.get_submodule(
-            weight_name.removesuffix(".weight")
+            removesuffix(weight_name, ".weight")
         )
         object.__setattr__(submodule, GRAPH_RELATED_TENSOR_ATTR, weight_tensor)
 
 
 def generate_constant_folding_info(
     deployable_module, torch_module: torch.nn.Module = None
 ) -> Dict[str, flow.Tensor]:
@@ -181,7 +181,13 @@
     constant_folding_info = getattr(module, CONSTANT_FOLDING_INFO_ATTR, None)
     if constant_folding_info is None:
         return
 
     logger.info(f"state_dict updated, modify the related weight in graph")
     update_graph_with_constant_folding_info(module, constant_folding_info)
     setattr(module._torch_module, STATE_UPDATED_ATTR, False)
+
+def removesuffix(s: str, suffix: str) -> str:
+    if s.endswith(suffix):
+        return s[:len(s) - len(suffix)]
+    else:
+        return s
```

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/with_fx_graph.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_fx_graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/infer_compiler/with_fx_interpreter.py` & `onediff-1.0.0.dev202405150127/src/onediff/infer_compiler/with_fx_interpreter.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/optimization/attention_processor.py` & `onediff-1.0.0.dev202405150127/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/optimization/quant_optimizer.py` & `onediff-1.0.0.dev202405150127/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.0.0.dev202405150127/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/quantization/load_quantized_model.py` & `onediff-1.0.0.dev202405150127/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.0.0.dev202405150127/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff/quantization/quantize_utils.py` & `onediff-1.0.0.dev202405150127/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/src/onediff.egg-info/PKG-INFO` & `onediff-1.0.0.dev202405150127/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405140127
+Version: 1.0.0.dev202405150127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,15 @@
 <img src="imgs/onediff_logo.png" height="100">
 </p>
 
 ---
 <p align="center">
   <a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip install"></a>
   <a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Stars&color=green"></a>
+  <a href="https://github.com/siliconflow/onediff?tab=Apache-2.0-1-ov-file#readme" target="_blank"><img src="https://img.shields.io/github/license/siliconflow/onediff"></a>
   <a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community wiki-green"></a>
   <a href="https://twitter.com/search?q=%22onediff%22&src=typed_query&f=live" target="_blank"><img src="https://img.shields.io/badge/Twitter-Discuss-green?logo=twitter&amp"></a>
   <a href="https://discord.gg/RKJTjZMcPQ" target="_blank"><img src="https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square"></a>
 </p>
 
 <p align="center">
   <a href="https://github.com/siliconflow/onediff/milestone/3" target="_blank"><img src="https://img.shields.io/github/milestones/progress/siliconflow/onediff/3"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405140127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405150127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -12,16 +12,17 @@
 Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: transformers>=4.27.1 Requires-Dist:
 diffusers>=0.19.3 Requires-Dist: accelerate Requires-Dist: torch
                             [imgs/onediff_logo.png]
 ---
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _i_n_s_t_a_l_l_]_[_h_t_t_p_s_:_/
                    _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/
-  _o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_ _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
+ _o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+  _l_i_c_e_n_s_e_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y
+           _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
         _g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_]_[_h_t_t_p_s_:_/_/_d_c_b_a_d_g_e_._v_e_r_c_e_l_._a_p_p_/_a_p_i_/_s_e_r_v_e_r_/
                            _R_K_J_T_j_Z_M_c_P_Q_?_s_t_y_l_e_=_s_q_u_a_r_e_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_m_i_l_e_s_t_o_n_e_s_/_p_r_o_g_r_e_s_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_3_]
       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_c_l_o_s_e_d_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_c_o_l_o_r_=_b_l_u_e_]_[_h_t_t_p_s_:_/_/
   _g_i_t_h_u_b_._c_o_m_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_s_d_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
         _g_i_t_h_u_b_._c_o_m_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_e_x_a_m_p_l_e_s_._y_m_l_/
```

### Comparing `onediff-1.0.0.dev202405140127/src/onediff.egg-info/SOURCES.txt` & `onediff-1.0.0.dev202405150127/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/tests/test_dual_module_list.py` & `onediff-1.0.0.dev202405150127/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.0.0.dev202405150127/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/tests/test_quantitative_quality.py` & `onediff-1.0.0.dev202405150127/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405140127/tests/test_quantize_custom_model.py` & `onediff-1.0.0.dev202405150127/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

