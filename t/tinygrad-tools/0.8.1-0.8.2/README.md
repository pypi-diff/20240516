# Comparing `tmp/tinygrad_tools-0.8.1.tar.gz` & `tmp/tinygrad_tools-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinygrad_tools-0.8.1.tar", last modified: Sun May  5 18:17:17 2024, max compression
+gzip compressed data, was "tinygrad_tools-0.8.2.tar", last modified: Thu May 16 11:08:12 2024, max compression
```

## Comparing `tinygrad_tools-0.8.1.tar` & `tinygrad_tools-0.8.2.tar`

### file list

```diff
@@ -1,130 +1,128 @@
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.361744 tinygrad_tools-0.8.1/
--rw-r--r--   0 qazal      (501) staff       (20)     1055 2023-12-16 21:47:10.000000 tinygrad_tools-0.8.1/LICENSE
--rw-r--r--   0 qazal      (501) staff       (20)    10385 2024-05-05 18:17:17.361451 tinygrad_tools-0.8.1/PKG-INFO
--rw-r--r--   0 qazal      (501) staff       (20)     8238 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/README.md
--rw-r--r--   0 qazal      (501) staff       (20)       38 2024-05-05 18:17:17.361799 tinygrad_tools-0.8.1/setup.cfg
--rw-r--r--   0 qazal      (501) staff       (20)     2176 2024-05-05 18:16:57.000000 tinygrad_tools-0.8.1/setup.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.348205 tinygrad_tools-0.8.1/test/
--rw-r--r--   0 qazal      (501) staff       (20)      463 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_arange.py
--rw-r--r--   0 qazal      (501) staff       (20)     9474 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_assign.py
--rw-r--r--   0 qazal      (501) staff       (20)     9820 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/test/test_const_folding.py
--rw-r--r--   0 qazal      (501) staff       (20)     4214 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_conv.py
--rw-r--r--   0 qazal      (501) staff       (20)      882 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_conv_shapetracker.py
--rw-r--r--   0 qazal      (501) staff       (20)     2532 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_copy_speed.py
--rw-r--r--   0 qazal      (501) staff       (20)     4714 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_custom_function.py
--rw-r--r--   0 qazal      (501) staff       (20)     1218 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_device_speed.py
--rw-r--r--   0 qazal      (501) staff       (20)    33348 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/test/test_dtype.py
--rw-r--r--   0 qazal      (501) staff       (20)     8248 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_dtype_alu.py
--rw-r--r--   0 qazal      (501) staff       (20)     1668 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_fusion_op.py
--rw-r--r--   0 qazal      (501) staff       (20)     3005 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_fuzz_shape_ops.py
--rw-r--r--   0 qazal      (501) staff       (20)     1071 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_gc.py
--rw-r--r--   0 qazal      (501) staff       (20)     2844 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_image_dtype.py
--rw-r--r--   0 qazal      (501) staff       (20)    10899 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_jit.py
--rw-r--r--   0 qazal      (501) staff       (20)      697 2024-03-10 07:24:31.000000 tinygrad_tools-0.8.1/test/test_kernel_cache.py
--rw-r--r--   0 qazal      (501) staff       (20)     3301 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_lazybuffer.py
--rw-r--r--   0 qazal      (501) staff       (20)     1106 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_lazyop.py
--rw-r--r--   0 qazal      (501) staff       (20)    49817 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_linearizer.py
--rw-r--r--   0 qazal      (501) staff       (20)    68288 2024-04-28 14:54:19.000000 tinygrad_tools-0.8.1/test/test_linearizer_failures.py
--rw-r--r--   0 qazal      (501) staff       (20)    14893 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_linearizer_overflows.py
--rw-r--r--   0 qazal      (501) staff       (20)      912 2023-12-25 10:30:26.000000 tinygrad_tools-0.8.1/test/test_masked_st.py
--rw-r--r--   0 qazal      (501) staff       (20)     1722 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_method_cache.py
--rw-r--r--   0 qazal      (501) staff       (20)    31026 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_multitensor.py
--rw-r--r--   0 qazal      (501) staff       (20)     2529 2024-03-10 07:24:31.000000 tinygrad_tools-0.8.1/test/test_net_speed.py
--rwxr-xr-x   0 qazal      (501) staff       (20)    14254 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_nn.py
--rw-r--r--   0 qazal      (501) staff       (20)    91957 2024-05-02 16:40:18.000000 tinygrad_tools-0.8.1/test/test_ops.py
--rw-r--r--   0 qazal      (501) staff       (20)     5510 2024-04-28 15:40:27.000000 tinygrad_tools-0.8.1/test/test_optim.py
--rw-r--r--   0 qazal      (501) staff       (20)     4281 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_pattern_matcher.py
--rw-r--r--   0 qazal      (501) staff       (20)     1835 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_pickle.py
--rw-r--r--   0 qazal      (501) staff       (20)     9922 2024-05-02 16:40:18.000000 tinygrad_tools-0.8.1/test/test_randomness.py
--rw-r--r--   0 qazal      (501) staff       (20)      658 2023-12-25 10:30:26.000000 tinygrad_tools-0.8.1/test/test_sample.py
--rw-r--r--   0 qazal      (501) staff       (20)    22613 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_schedule.py
--rw-r--r--   0 qazal      (501) staff       (20)     3323 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_search.py
--rw-r--r--   0 qazal      (501) staff       (20)     2841 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_setitem.py
--rw-r--r--   0 qazal      (501) staff       (20)     2324 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_specific_conv.py
--rw-r--r--   0 qazal      (501) staff       (20)    11569 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_speed_v_torch.py
--rw-r--r--   0 qazal      (501) staff       (20)     1854 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_subbuffer.py
--rw-r--r--   0 qazal      (501) staff       (20)     6531 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_symbolic_jit.py
--rw-r--r--   0 qazal      (501) staff       (20)     5610 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_symbolic_ops.py
--rw-r--r--   0 qazal      (501) staff       (20)     7554 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_symbolic_shapetracker.py
--rw-r--r--   0 qazal      (501) staff       (20)    21540 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_tensor.py
--rw-r--r--   0 qazal      (501) staff       (20)     1518 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_tensor_data.py
--rw-r--r--   0 qazal      (501) staff       (20)     1763 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/test/test_tensor_variable.py
--rw-r--r--   0 qazal      (501) staff       (20)      436 2023-12-25 10:30:26.000000 tinygrad_tools-0.8.1/test/test_to_numpy.py
--rw-r--r--   0 qazal      (501) staff       (20)     1821 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/test/test_uop_graph.py
--rw-r--r--   0 qazal      (501) staff       (20)    13647 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/test/test_uops.py
--rw-r--r--   0 qazal      (501) staff       (20)     1739 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_uops_stats.py
--rw-r--r--   0 qazal      (501) staff       (20)     2539 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_winograd.py
--rw-r--r--   0 qazal      (501) staff       (20)      910 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/test/test_zero_copy.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.349846 tinygrad_tools-0.8.1/tinygrad/
--rw-r--r--   0 qazal      (501) staff       (20)      449 2024-04-28 15:40:27.000000 tinygrad_tools-0.8.1/tinygrad/__init__.py
--rw-r--r--   0 qazal      (501) staff       (20)     4861 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/buffer.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.350388 tinygrad_tools-0.8.1/tinygrad/codegen/
--rw-r--r--   0 qazal      (501) staff       (20)    39918 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/codegen/kernel.py
--rw-r--r--   0 qazal      (501) staff       (20)    26778 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/codegen/linearizer.py
--rw-r--r--   0 qazal      (501) staff       (20)    22000 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/codegen/uops.py
--rw-r--r--   0 qazal      (501) staff       (20)    14954 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/device.py
--rw-r--r--   0 qazal      (501) staff       (20)     5960 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/dtype.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.351080 tinygrad_tools-0.8.1/tinygrad/engine/
--rw-r--r--   0 qazal      (501) staff       (20)        0 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/engine/__init__.py
--rw-r--r--   0 qazal      (501) staff       (20)    10681 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/engine/jit.py
--rw-r--r--   0 qazal      (501) staff       (20)     6102 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/engine/realize.py
--rw-r--r--   0 qazal      (501) staff       (20)    15157 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/engine/schedule.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.351892 tinygrad_tools-0.8.1/tinygrad/features/
--rw-r--r--   0 qazal      (501) staff       (20)     5252 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/features/graph.py
--rw-r--r--   0 qazal      (501) staff       (20)     4917 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/features/image.py
--rw-r--r--   0 qazal      (501) staff       (20)    11409 2024-05-05 18:04:51.000000 tinygrad_tools-0.8.1/tinygrad/features/multi.py
--rw-r--r--   0 qazal      (501) staff       (20)    11371 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/features/search.py
--rw-r--r--   0 qazal      (501) staff       (20)     9172 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/tinygrad/function.py
--rw-r--r--   0 qazal      (501) staff       (20)    12311 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/helpers.py
--rw-r--r--   0 qazal      (501) staff       (20)    13666 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/lazy.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.352610 tinygrad_tools-0.8.1/tinygrad/nn/
--rw-r--r--   0 qazal      (501) staff       (20)     7836 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/nn/__init__.py
--rw-r--r--   0 qazal      (501) staff       (20)      458 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/nn/datasets.py
--rw-r--r--   0 qazal      (501) staff       (20)     5182 2024-04-28 15:40:27.000000 tinygrad_tools-0.8.1/tinygrad/nn/optim.py
--rw-r--r--   0 qazal      (501) staff       (20)     8626 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/tinygrad/nn/state.py
--rw-r--r--   0 qazal      (501) staff       (20)     7676 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/ops.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.353121 tinygrad_tools-0.8.1/tinygrad/renderer/
--rw-r--r--   0 qazal      (501) staff       (20)    18317 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/tinygrad/renderer/assembly.py
--rw-r--r--   0 qazal      (501) staff       (20)    22526 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/renderer/cstyle.py
--rw-r--r--   0 qazal      (501) staff       (20)     9987 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/renderer/llvmir.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.355144 tinygrad_tools-0.8.1/tinygrad/runtime/
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.357655 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/
--rw-r--r--   0 qazal      (501) staff       (20)    65022 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/amd_gpu.py
--rw-r--r--   0 qazal      (501) staff       (20)    38495 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/comgr.py
--rw-r--r--   0 qazal      (501) staff       (20)   250380 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/cuda.py
--rw-r--r--   0 qazal      (501) staff       (20)   245532 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/hip.py
--rw-r--r--   0 qazal      (501) staff       (20)   270001 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/hsa.py
--rw-r--r--   0 qazal      (501) staff       (20)    29935 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/kfd.py
--rw-r--r--   0 qazal      (501) staff       (20)  1672024 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/nv_gpu.py
--rw-r--r--   0 qazal      (501) staff       (20)    82654 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/autogen/opencl.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.357980 tinygrad_tools-0.8.1/tinygrad/runtime/driver/
--rw-r--r--   0 qazal      (501) staff       (20)     3376 2024-04-28 16:08:31.000000 tinygrad_tools-0.8.1/tinygrad/runtime/driver/hip_comgr.py
--rw-r--r--   0 qazal      (501) staff       (20)     7218 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/driver/hsa.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.358669 tinygrad_tools-0.8.1/tinygrad/runtime/graph/
--rw-r--r--   0 qazal      (501) staff       (20)     1942 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/graph/clang.py
--rw-r--r--   0 qazal      (501) staff       (20)     5253 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/graph/cuda.py
--rw-r--r--   0 qazal      (501) staff       (20)    10023 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/graph/hsa.py
--rw-r--r--   0 qazal      (501) staff       (20)     4573 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/graph/metal.py
--rw-r--r--   0 qazal      (501) staff       (20)    32276 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_amd.py
--rw-r--r--   0 qazal      (501) staff       (20)     1571 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_clang.py
--rw-r--r--   0 qazal      (501) staff       (20)    11440 2024-05-05 18:04:57.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_cuda.py
--rw-r--r--   0 qazal      (501) staff       (20)     2732 2024-05-05 18:04:57.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_disk.py
--rw-r--r--   0 qazal      (501) staff       (20)     7662 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_gpu.py
--rw-r--r--   0 qazal      (501) staff       (20)    16298 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_hsa.py
--rw-r--r--   0 qazal      (501) staff       (20)     2362 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_llvm.py
--rw-r--r--   0 qazal      (501) staff       (20)     5919 2024-05-05 18:04:57.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_metal.py
--rw-r--r--   0 qazal      (501) staff       (20)      363 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_npy.py
--rw-r--r--   0 qazal      (501) staff       (20)    32851 2024-05-05 18:04:57.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_nv.py
--rw-r--r--   0 qazal      (501) staff       (20)    10621 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_python.py
--rw-r--r--   0 qazal      (501) staff       (20)      802 2024-04-28 16:08:31.000000 tinygrad_tools-0.8.1/tinygrad/runtime/ops_rhip.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.359188 tinygrad_tools-0.8.1/tinygrad/shape/
--rw-r--r--   0 qazal      (501) staff       (20)     6334 2024-05-05 18:04:57.000000 tinygrad_tools-0.8.1/tinygrad/shape/shapetracker.py
--rw-r--r--   0 qazal      (501) staff       (20)    16688 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.1/tinygrad/shape/symbolic.py
--rw-r--r--   0 qazal      (501) staff       (20)    17092 2024-05-02 16:40:18.000000 tinygrad_tools-0.8.1/tinygrad/shape/view.py
--rw-r--r--   0 qazal      (501) staff       (20)    76922 2024-05-05 18:04:57.000000 tinygrad_tools-0.8.1/tinygrad/tensor.py
-drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-05 18:17:17.360092 tinygrad_tools-0.8.1/tinygrad_tools.egg-info/
--rw-r--r--   0 qazal      (501) staff       (20)    10385 2024-05-05 18:17:17.000000 tinygrad_tools-0.8.1/tinygrad_tools.egg-info/PKG-INFO
--rw-r--r--   0 qazal      (501) staff       (20)     2930 2024-05-05 18:17:17.000000 tinygrad_tools-0.8.1/tinygrad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 qazal      (501) staff       (20)        1 2024-05-05 18:17:17.000000 tinygrad_tools-0.8.1/tinygrad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 qazal      (501) staff       (20)      554 2024-05-05 18:17:17.000000 tinygrad_tools-0.8.1/tinygrad_tools.egg-info/requires.txt
--rw-r--r--   0 qazal      (501) staff       (20)        9 2024-05-05 18:17:17.000000 tinygrad_tools-0.8.1/tinygrad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.748149 tinygrad_tools-0.8.2/
+-rw-r--r--   0 qazal      (501) staff       (20)     1058 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/LICENSE
+-rw-r--r--   0 qazal      (501) staff       (20)    10312 2024-05-16 11:08:12.747887 tinygrad_tools-0.8.2/PKG-INFO
+-rw-r--r--   0 qazal      (501) staff       (20)     8127 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/README.md
+-rw-r--r--   0 qazal      (501) staff       (20)       38 2024-05-16 11:08:12.748190 tinygrad_tools-0.8.2/setup.cfg
+-rw-r--r--   0 qazal      (501) staff       (20)     2176 2024-05-16 11:07:58.000000 tinygrad_tools-0.8.2/setup.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.735586 tinygrad_tools-0.8.2/test/
+-rw-r--r--   0 qazal      (501) staff       (20)      463 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.2/test/test_arange.py
+-rw-r--r--   0 qazal      (501) staff       (20)    12797 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_assign.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10385 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_const_folding.py
+-rw-r--r--   0 qazal      (501) staff       (20)     4214 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_conv.py
+-rw-r--r--   0 qazal      (501) staff       (20)      882 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_conv_shapetracker.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2532 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_copy_speed.py
+-rw-r--r--   0 qazal      (501) staff       (20)     4800 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_custom_function.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1218 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_device_speed.py
+-rw-r--r--   0 qazal      (501) staff       (20)    34630 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_dtype.py
+-rw-r--r--   0 qazal      (501) staff       (20)     8303 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_dtype_alu.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1668 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_fusion_op.py
+-rw-r--r--   0 qazal      (501) staff       (20)     3003 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_fuzz_shape_ops.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1071 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_gc.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2848 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_image_dtype.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10912 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_jit.py
+-rw-r--r--   0 qazal      (501) staff       (20)      697 2024-03-10 07:24:31.000000 tinygrad_tools-0.8.2/test/test_kernel_cache.py
+-rw-r--r--   0 qazal      (501) staff       (20)     4029 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_lazybuffer.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1106 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_lazyop.py
+-rw-r--r--   0 qazal      (501) staff       (20)    55902 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_linearizer.py
+-rw-r--r--   0 qazal      (501) staff       (20)    69578 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_linearizer_failures.py
+-rw-r--r--   0 qazal      (501) staff       (20)    14889 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_linearizer_overflows.py
+-rw-r--r--   0 qazal      (501) staff       (20)      912 2023-12-25 10:30:26.000000 tinygrad_tools-0.8.2/test/test_masked_st.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1722 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_method_cache.py
+-rw-r--r--   0 qazal      (501) staff       (20)    31310 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_multitensor.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2537 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_net_speed.py
+-rwxr-xr-x   0 qazal      (501) staff       (20)    15424 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_nn.py
+-rw-r--r--   0 qazal      (501) staff       (20)    94674 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_ops.py
+-rw-r--r--   0 qazal      (501) staff       (20)     6018 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_optim.py
+-rw-r--r--   0 qazal      (501) staff       (20)     4281 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_pattern_matcher.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1835 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.2/test/test_pickle.py
+-rw-r--r--   0 qazal      (501) staff       (20)     9921 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_randomness.py
+-rw-r--r--   0 qazal      (501) staff       (20)      658 2023-12-25 10:30:26.000000 tinygrad_tools-0.8.2/test/test_sample.py
+-rw-r--r--   0 qazal      (501) staff       (20)    26731 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_schedule.py
+-rw-r--r--   0 qazal      (501) staff       (20)     3578 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_search.py
+-rw-r--r--   0 qazal      (501) staff       (20)     4639 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_setitem.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2332 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_specific_conv.py
+-rw-r--r--   0 qazal      (501) staff       (20)    11635 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_speed_v_torch.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1854 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_subbuffer.py
+-rw-r--r--   0 qazal      (501) staff       (20)     8478 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_symbolic_jit.py
+-rw-r--r--   0 qazal      (501) staff       (20)     7163 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_symbolic_ops.py
+-rw-r--r--   0 qazal      (501) staff       (20)     7554 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_symbolic_shapetracker.py
+-rw-r--r--   0 qazal      (501) staff       (20)    21553 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_tensor.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1518 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_tensor_data.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1763 2024-05-02 16:41:56.000000 tinygrad_tools-0.8.2/test/test_tensor_variable.py
+-rw-r--r--   0 qazal      (501) staff       (20)      436 2023-12-25 10:30:26.000000 tinygrad_tools-0.8.2/test/test_to_numpy.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1821 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.2/test/test_uop_graph.py
+-rw-r--r--   0 qazal      (501) staff       (20)    14735 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_uops.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1764 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/test/test_uops_stats.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2539 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_winograd.py
+-rw-r--r--   0 qazal      (501) staff       (20)      910 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/test/test_zero_copy.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.736893 tinygrad_tools-0.8.2/tinygrad/
+-rw-r--r--   0 qazal      (501) staff       (20)      449 2024-04-28 15:40:27.000000 tinygrad_tools-0.8.2/tinygrad/__init__.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.737371 tinygrad_tools-0.8.2/tinygrad/codegen/
+-rw-r--r--   0 qazal      (501) staff       (20)    40172 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/codegen/kernel.py
+-rw-r--r--   0 qazal      (501) staff       (20)    27850 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/codegen/linearizer.py
+-rw-r--r--   0 qazal      (501) staff       (20)    22069 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/codegen/uops.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10323 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/device.py
+-rw-r--r--   0 qazal      (501) staff       (20)     6221 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/dtype.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.738271 tinygrad_tools-0.8.2/tinygrad/engine/
+-rw-r--r--   0 qazal      (501) staff       (20)        0 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/engine/__init__.py
+-rw-r--r--   0 qazal      (501) staff       (20)     5219 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/engine/graph.py
+-rw-r--r--   0 qazal      (501) staff       (20)    11049 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/engine/jit.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10866 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/engine/realize.py
+-rw-r--r--   0 qazal      (501) staff       (20)    18500 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/engine/schedule.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10916 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/engine/search.py
+-rw-r--r--   0 qazal      (501) staff       (20)     9616 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/function.py
+-rw-r--r--   0 qazal      (501) staff       (20)    12773 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/helpers.py
+-rw-r--r--   0 qazal      (501) staff       (20)    13379 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/lazy.py
+-rw-r--r--   0 qazal      (501) staff       (20)    11362 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/multi.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.738921 tinygrad_tools-0.8.2/tinygrad/nn/
+-rw-r--r--   0 qazal      (501) staff       (20)     7836 2024-05-05 18:04:56.000000 tinygrad_tools-0.8.2/tinygrad/nn/__init__.py
+-rw-r--r--   0 qazal      (501) staff       (20)      458 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/nn/datasets.py
+-rw-r--r--   0 qazal      (501) staff       (20)     5493 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/nn/optim.py
+-rw-r--r--   0 qazal      (501) staff       (20)     8759 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/nn/state.py
+-rw-r--r--   0 qazal      (501) staff       (20)     7124 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/ops.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.739595 tinygrad_tools-0.8.2/tinygrad/renderer/
+-rw-r--r--   0 qazal      (501) staff       (20)     1788 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/renderer/__init__.py
+-rw-r--r--   0 qazal      (501) staff       (20)    18121 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/renderer/assembly.py
+-rw-r--r--   0 qazal      (501) staff       (20)    22829 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/renderer/cstyle.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10313 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/renderer/llvmir.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.741243 tinygrad_tools-0.8.2/tinygrad/runtime/
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.743864 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/
+-rw-r--r--   0 qazal      (501) staff       (20)    65022 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/amd_gpu.py
+-rw-r--r--   0 qazal      (501) staff       (20)    38495 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/comgr.py
+-rw-r--r--   0 qazal      (501) staff       (20)   250380 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/cuda.py
+-rw-r--r--   0 qazal      (501) staff       (20)   245532 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/hip.py
+-rw-r--r--   0 qazal      (501) staff       (20)   270001 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/hsa.py
+-rw-r--r--   0 qazal      (501) staff       (20)    29935 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/kfd.py
+-rw-r--r--   0 qazal      (501) staff       (20)  1672024 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/nv_gpu.py
+-rw-r--r--   0 qazal      (501) staff       (20)    82654 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/autogen/opencl.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.744267 tinygrad_tools-0.8.2/tinygrad/runtime/driver/
+-rw-r--r--   0 qazal      (501) staff       (20)     3376 2024-04-28 16:08:31.000000 tinygrad_tools-0.8.2/tinygrad/runtime/driver/hip_comgr.py
+-rw-r--r--   0 qazal      (501) staff       (20)     7218 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/runtime/driver/hsa.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.745101 tinygrad_tools-0.8.2/tinygrad/runtime/graph/
+-rw-r--r--   0 qazal      (501) staff       (20)     1957 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/graph/clang.py
+-rw-r--r--   0 qazal      (501) staff       (20)     5265 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/graph/cuda.py
+-rw-r--r--   0 qazal      (501) staff       (20)     7697 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/graph/hcq.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10035 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/graph/hsa.py
+-rw-r--r--   0 qazal      (501) staff       (20)     4579 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/graph/metal.py
+-rw-r--r--   0 qazal      (501) staff       (20)    31238 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_amd.py
+-rw-r--r--   0 qazal      (501) staff       (20)     1468 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_clang.py
+-rw-r--r--   0 qazal      (501) staff       (20)    11040 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_cuda.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2738 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_disk.py
+-rw-r--r--   0 qazal      (501) staff       (20)     7518 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_gpu.py
+-rw-r--r--   0 qazal      (501) staff       (20)    16113 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_hsa.py
+-rw-r--r--   0 qazal      (501) staff       (20)     2229 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_llvm.py
+-rw-r--r--   0 qazal      (501) staff       (20)     5740 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_metal.py
+-rw-r--r--   0 qazal      (501) staff       (20)      369 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_npy.py
+-rw-r--r--   0 qazal      (501) staff       (20)    36458 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_nv.py
+-rw-r--r--   0 qazal      (501) staff       (20)    10692 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/runtime/ops_python.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.745550 tinygrad_tools-0.8.2/tinygrad/shape/
+-rw-r--r--   0 qazal      (501) staff       (20)     6334 2024-05-14 20:28:27.000000 tinygrad_tools-0.8.2/tinygrad/shape/shapetracker.py
+-rw-r--r--   0 qazal      (501) staff       (20)    16688 2024-04-28 14:45:16.000000 tinygrad_tools-0.8.2/tinygrad/shape/symbolic.py
+-rw-r--r--   0 qazal      (501) staff       (20)    17092 2024-05-11 17:06:40.000000 tinygrad_tools-0.8.2/tinygrad/shape/view.py
+-rw-r--r--   0 qazal      (501) staff       (20)    82686 2024-05-16 11:07:21.000000 tinygrad_tools-0.8.2/tinygrad/tensor.py
+drwxr-xr-x   0 qazal      (501) staff       (20)        0 2024-05-16 11:08:12.746490 tinygrad_tools-0.8.2/tinygrad_tools.egg-info/
+-rw-r--r--   0 qazal      (501) staff       (20)    10312 2024-05-16 11:08:12.000000 tinygrad_tools-0.8.2/tinygrad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 qazal      (501) staff       (20)     2902 2024-05-16 11:08:12.000000 tinygrad_tools-0.8.2/tinygrad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 qazal      (501) staff       (20)        1 2024-05-16 11:08:12.000000 tinygrad_tools-0.8.2/tinygrad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 qazal      (501) staff       (20)      560 2024-05-16 11:08:12.000000 tinygrad_tools-0.8.2/tinygrad_tools.egg-info/requires.txt
+-rw-r--r--   0 qazal      (501) staff       (20)        9 2024-05-16 11:08:12.000000 tinygrad_tools-0.8.2/tinygrad_tools.egg-info/top_level.txt
```

### Comparing `tinygrad_tools-0.8.1/LICENSE` & `tinygrad_tools-0.8.2/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2023 George Hotz
+Copyright (c) 2024, the tiny corp
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `tinygrad_tools-0.8.1/PKG-INFO` & `tinygrad_tools-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinygrad-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: You like pytorch? You like micrograd? You love tinygrad! <3
 Author: George Hotz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -44,24 +44,24 @@
 Requires-Dist: hypothesis; extra == "testing"
 Requires-Dist: nibabel; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: markdown-callouts; extra == "docs"
 Requires-Dist: markdown-exec[ansi]; extra == "docs"
+Requires-Dist: black; extra == "docs"
 Provides-Extra: testing-tf
 Requires-Dist: tensorflow==2.15.1; extra == "testing-tf"
 Requires-Dist: tensorflow_addons; extra == "testing-tf"
 
 <div align="center">
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="/docs-legacy/logo_tiny_dark.svg">
-  <source media="(prefers-color-scheme: light)" srcset="/docs-legacy/logo_tiny_light.svg">
-  <img alt="tiny corp logo" src="/docs-legacy/logo_tiny_light.svg" width="50%" height="50%">
+  <source media="(prefers-color-scheme: light)" srcset="/docs/logo_tiny_light.svg">
+  <img alt="tiny corp logo" src="/docs/logo_tiny_dark.svg" width="50%" height="50%">
 </picture>
 
 tinygrad: For something between [PyTorch](https://github.com/pytorch/pytorch) and [karpathy/micrograd](https://github.com/karpathy/micrograd). Maintained by [tiny corp](https://tinygrad.org).
 
 <h3>
 
 [Homepage](https://github.com/tinygrad/tinygrad) | [Documentation](/docs) | [Examples](/examples) | [Showcase](/docs/showcase.md) | [Discord](https://discord.gg/ZjZadyC7PK)
@@ -138,15 +138,15 @@
 - [x] [C Code (Clang)](tinygrad/runtime/ops_clang.py)
 - [x] [LLVM](tinygrad/runtime/ops_llvm.py)
 - [x] [METAL](tinygrad/runtime/ops_metal.py)
 - [x] [CUDA](tinygrad/runtime/ops_cuda.py)
 - [x] [HSA](tinygrad/runtime/ops_hsa.py)
 
 And it is easy to add more! Your accelerator of choice only needs to support a total of ~25 low level ops.
-More information can be found in the [documentation for adding new accelerators](/docs-legacy/adding_new_accelerators.md).
+More information can be found in the [documentation for adding new accelerators](/docs/adding_new_accelerators.md).
 
 ## Installation
 
 The current recommended way to install tinygrad is from source.
 
 ### From source
```

### Comparing `tinygrad_tools-0.8.1/README.md` & `tinygrad_tools-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <div align="center">
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="/docs-legacy/logo_tiny_dark.svg">
-  <source media="(prefers-color-scheme: light)" srcset="/docs-legacy/logo_tiny_light.svg">
-  <img alt="tiny corp logo" src="/docs-legacy/logo_tiny_light.svg" width="50%" height="50%">
+  <source media="(prefers-color-scheme: light)" srcset="/docs/logo_tiny_light.svg">
+  <img alt="tiny corp logo" src="/docs/logo_tiny_dark.svg" width="50%" height="50%">
 </picture>
 
 tinygrad: For something between [PyTorch](https://github.com/pytorch/pytorch) and [karpathy/micrograd](https://github.com/karpathy/micrograd). Maintained by [tiny corp](https://tinygrad.org).
 
 <h3>
 
 [Homepage](https://github.com/tinygrad/tinygrad) | [Documentation](/docs) | [Examples](/examples) | [Showcase](/docs/showcase.md) | [Discord](https://discord.gg/ZjZadyC7PK)
@@ -84,15 +83,15 @@
 - [x] [C Code (Clang)](tinygrad/runtime/ops_clang.py)
 - [x] [LLVM](tinygrad/runtime/ops_llvm.py)
 - [x] [METAL](tinygrad/runtime/ops_metal.py)
 - [x] [CUDA](tinygrad/runtime/ops_cuda.py)
 - [x] [HSA](tinygrad/runtime/ops_hsa.py)
 
 And it is easy to add more! Your accelerator of choice only needs to support a total of ~25 low level ops.
-More information can be found in the [documentation for adding new accelerators](/docs-legacy/adding_new_accelerators.md).
+More information can be found in the [documentation for adding new accelerators](/docs/adding_new_accelerators.md).
 
 ## Installation
 
 The current recommended way to install tinygrad is from source.
 
 ### From source
```

### Comparing `tinygrad_tools-0.8.1/setup.py` & `tinygrad_tools-0.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from setuptools import setup
 
 directory = Path(__file__).resolve().parent
 with open(directory / 'README.md', encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='tinygrad-tools',
-      version='0.8.1',
+      version='0.8.2',
       description='You like pytorch? You like micrograd? You love tinygrad! <3',
       author='George Hotz',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['tinygrad', 'tinygrad.runtime.autogen', 'tinygrad.codegen', 'tinygrad.nn', 'tinygrad.renderer', 'tinygrad.engine',
-                  'tinygrad.runtime', 'tinygrad.runtime.driver', 'tinygrad.runtime.graph', 'tinygrad.shape', 'tinygrad.features'],
+                  'tinygrad.runtime', 'tinygrad.runtime.driver', 'tinygrad.runtime.graph', 'tinygrad.shape'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
       ],
       install_requires=["numpy", "tqdm",
                         "pyobjc-framework-Metal; platform_system=='Darwin'",
                         "pyobjc-framework-libdispatch; platform_system=='Darwin'"],
@@ -54,15 +54,16 @@
             "hypothesis",
             "nibabel",
         ],
         'docs': [
             "mkdocs-material",
             "mkdocstrings[python]",
             "markdown-callouts",
-            "markdown-exec[ansi]"
+            "markdown-exec[ansi]",
+            "black"
         ],
         'testing_tf': [
             "tensorflow==2.15.1",
             "tensorflow_addons",
         ]
       },
       include_package_data=True)
```

### Comparing `tinygrad_tools-0.8.1/test/test_assign.py` & `tinygrad_tools-0.8.2/test/test_assign.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     b = Tensor.zeros(10,10).contiguous()
     a.realize()
     np.testing.assert_allclose(b.numpy(), 0)
 
   def test_assign_zeros(self):
     a = Tensor.zeros(10,10).contiguous()
     b = Tensor.zeros(10,10).contiguous()
-    #with self.assertRaises(RuntimeError):
     a.assign(Tensor.ones(10,10))
     a.realize()
     np.testing.assert_allclose(b.numpy(), 0)
 
   def test_assign_add(self):
     def f(x):
       x += 1
@@ -113,23 +112,23 @@
     a.assign(Tensor.full((4,), 2.).contiguous())
     # NOTE: old_a is now 2, and this would match the behavior of pytorch
     new = a + old_a
     np.testing.assert_allclose(new.numpy(), 4)
 
   def test_assign_diamond_cycle(self):
     # NOTE: should *not* raise AssertionError from numpy
-    with self.assertRaises(RuntimeError):
+    with self.assertRaisesRegex(RuntimeError, "cycle"):
       a = Tensor.ones(4).contiguous().realize()
       times_a = a*3
       a.assign(Tensor.full((4,), 2.).contiguous())
       new = a + (times_a-1)
       np.testing.assert_allclose(new.numpy(), 4)
 
   def test_assign_diamond_contiguous_cycle(self):
-    with self.assertRaises(RuntimeError):
+    with self.assertRaisesRegex(RuntimeError, "cycle"):
       a = Tensor.ones(4).contiguous().realize()
       times_a = a*3
       a.assign(Tensor.full((4,), 2.))
       new = a.contiguous() + times_a-1
       np.testing.assert_allclose(new.numpy(), 4)
 
   def test_assign_diamond_possible(self):
@@ -198,15 +197,15 @@
     b1.assign(r1 * b1)
     Tensor.realize(b0, b1)
     np.testing.assert_equal(b0.numpy(), 128)
     np.testing.assert_equal(b1.numpy(), 608)
 
   def test_crossunder_assign(self):
     # NOTE: should *not* raise AssertionError from numpy
-    with self.assertRaises(RuntimeError):
+    with self.assertRaisesRegex(RuntimeError, "cycle"):
       a = Tensor.full((4,), 2).contiguous().realize()
       b = Tensor.full((4,), 3).contiguous().realize()
       c = a+9
       a += b
       b += c
       Tensor.realize(a,b)
       np.testing.assert_allclose(a.numpy(), 2+3)
@@ -269,22 +268,103 @@
     a = Tensor(np.arange(N*N, dtype=np.float32)).reshape(N,N)
     b = Tensor(np.arange(N*N, dtype=np.float32)).reshape(N,N)
     a.realize()
     b.realize()
     #GlobalCounters.cache = []
     ba1 = a.lazydata.base.realized # noqa: F841
     bb1 = b.lazydata.base.realized # noqa: F841
-    with self.assertRaises(RuntimeError):
+    with self.assertRaisesRegex(RuntimeError, "contiguous"):
       a.assign(a.permute(1,0) + b)   # this should not work!
       a.realize()
       ba2 = a.lazydata.base.realized # noqa: F841
       # NOTE: don't test that it's assigned
       #assert ba1 == ba2 and ba1 != bb1
       np.testing.assert_allclose(a.numpy(), np.arange(N*N).reshape((N,N)) + np.arange(N*N).reshape((N,N)).transpose(1,0))
 
+  def test_simple_assignment_multioutput(self):
+    a = Tensor.randn(32, 32).realize()
+    b = Tensor.full((32, ), 1.).contiguous().realize()
+    c = Tensor.full((32, ), 2.).contiguous().realize()
+    d = Tensor.full((32, ), 3.).contiguous().realize()
+
+    r = a.sum(axis=1)
+    b.assign(r + b)
+    c.assign(r + c)
+    d.assign(r + d)
+
+    kc = GlobalCounters.kernel_count
+    Tensor.realize(b, c, d)
+    assert GlobalCounters.kernel_count - kc == 1
+    np.testing.assert_allclose(b.numpy(), a.sum(1).numpy()+1)
+    np.testing.assert_allclose(c.numpy(), a.sum(1).numpy()+2)
+    np.testing.assert_allclose(d.numpy(), a.sum(1).numpy()+3)
+
+  # NOTE: if the assign target is read/write in a single kernel, it should be contiguous
+
+  def test_permuted_assignment_correct(self):
+    a = Tensor.arange(4 * 4).reshape(4, 4).contiguous().realize()
+    b = Tensor.arange(4 * 4).reshape(4, 4).contiguous().realize()
+    # TODO: scheduler limitation, should NOT raise AssertionError from numpy.
+    with self.assertRaisesRegex(RuntimeError, "contiguous"):
+      a = a.permute(1, 0)
+      new_val = a + b
+      a.assign(new_val)
+      np.testing.assert_equal(a.numpy(), np.arange(4 * 4).reshape(4, 4).transpose(1, 0) + np.arange(4 * 4).reshape(4, 4))
+
+  def test_permuted_reduceop_child_dual_use(self):
+    a = Tensor.randn(32, 32, 32).realize()
+    b = Tensor.full((32, 32), 1.).contiguous().realize()
+    with self.assertRaisesRegex(RuntimeError, "contiguous"):
+      r = a.sum(axis=1)
+      b.assign(r + b.permute(1, 0))
+      b.realize()
+
+  def test_permuted_reduceop_multioutput_dual_use(self):
+    a = Tensor.randn(32, 32, 32).realize()
+    b = Tensor.full((32, 32), 1.).contiguous().realize()
+    c = Tensor.full((32, 32), 2.).contiguous().realize()
+
+    with self.assertRaisesRegex(RuntimeError, "contiguous"):
+      r = a.sum(axis=1)
+      b_perm = b.permute(1, 0)
+      b.assign(r + b)
+      c.assign(r + b_perm)
+      Tensor.realize(b, c)
+
+  def test_permuted_reduceop_multioutput_dual_use_possible(self):
+    a = Tensor.randn(32, 32, 32, dtype=dtypes.int).realize()
+    b = Tensor.arange(32 * 32).reshape(32, 32).realize()
+    c = Tensor.arange(32 * 32).reshape(32, 32).realize()
+
+    kc = GlobalCounters.kernel_count
+    r = a.sum(axis=1)
+    b_perm = b.permute(1, 0)
+    b.assign(r + b)
+    c.assign(r + b_perm.contiguous())
+    Tensor.realize(b, c)
+    assert GlobalCounters.kernel_count - kc == 2
+    np.testing.assert_equal(b.numpy(), a.numpy().sum(1) + np.arange(32 * 32).reshape(32, 32))
+    np.testing.assert_equal(c.numpy(), a.numpy().sum(1) + np.arange(32 * 32).reshape(32, 32).transpose(1, 0))
+
+  def test_permuted_assignment_masked_view_possible(self):
+    a = Tensor.ones(4, 4).contiguous().realize()
+    b = a.shrink((None, (0, 2))).pad((None, (0, 2)), 2)
+    a.assign(a + b)
+    kc = GlobalCounters.kernel_count
+    a.realize()
+    assert GlobalCounters.kernel_count - kc == 1
+    np.testing.assert_equal(a.numpy(), np.ones((4, 4))+np.pad(np.ones((4, 4))[:, 0:2], ((0, 0), (0, 2)), constant_values=2))
+
+  def test_permuted_assignment_masked_view_not_contiguous(self):
+    a = Tensor.ones(4, 4).contiguous().realize()
+    with self.assertRaisesRegex(RuntimeError, "contiguous"):
+      b = a.shrink((None, (0, 2))).pad((None, (0, 2)), 2).permute(1, 0)
+      a.assign(a + b)
+      a.realize()
+
   # TODO: is there a way to sneak in a permute such that it returns the wrong answer?
 
   @unittest.skip("don't use output buffer, and mismatch dtype no longer supported")
   def test_cast_assignment(self):
     a = Tensor(np.arange(N*N, dtype=np.float32)).reshape(N,N)
     a.realize()
     oba1 = a.lazydata.base.output_buffer
```

### Comparing `tinygrad_tools-0.8.1/test/test_const_folding.py` & `tinygrad_tools-0.8.2/test/test_const_folding.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     _check_ast_count(0, Tensor.ones(4) + Tensor.ones(4))
     _check_ast_count(0, Tensor.ones(4) / Tensor.ones(4))
 
   def test_cast(self):
     _check_ast_count(0, Tensor.ones(4).cast(dtypes.int16))
     _check_ast_count(0, Tensor.full(4, fill_value=-1).cast(dtypes.uint16))
 
+  def test_neg_folding(self):
+    _check_ast_count(0, Tensor([1, 2, 3]).mul(-1).neg())
+    _check_ast_count(0, Tensor([1, 2, 3]).neg().mul(-1))
+    _check_ast_count(0, Tensor([1, 2, 3]).neg().neg())
+
 class TestBinaryOpsConstFolding(unittest.TestCase):
   def test_add_literal_zero(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) + 0)
   def test_add_tensor_zero(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) + Tensor.zeros(4))
   def test_literal_zero_add(self):
     _check_ast_count(0, 0 + Tensor([1.0, 2, 3, 4]))
@@ -52,14 +57,21 @@
   def test_mul_tensor_one(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) * Tensor.ones(4))
   def test_literal_one_mul(self):
     _check_ast_count(0, 1 * Tensor([1.0, 2, 3, 4]))
   def test_tensor_one_mul(self):
     _check_ast_count(0, Tensor.ones(4) * Tensor([1.0, 2, 3, 4]))
 
+  def test_bool_tensor_mul_bool(self):
+    _check_ast_count(0, Tensor([True, False]) * True)
+    _check_ast_count(0, Tensor([True, False]) * False)
+  def test_bool_mul_bool_tensor(self):
+    _check_ast_count(0, True * Tensor([True, False]))
+    _check_ast_count(0, False * Tensor([True, False]))
+
   def test_div_literal_one(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) / 1)
   def test_div_tensor_one(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) / Tensor.ones(4))
 
   def test_pow_literal_zero(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) ** 0)
@@ -102,20 +114,22 @@
   def test_mul_shrunk_one(self):
     _check_ast_count(0, Tensor([1.0, 2, 3, 4]) * Tensor.ones(6).shrink(((1, 5),)))
 
   def test_add_padded_one(self):
     _check_ast_count(1, Tensor([1.0, 2, 3, 4]) * Tensor.ones(2).pad(((1, 1),)))
 
   def test_cast_padded(self):
-    _check_ast_count(1, Tensor.ones(4).pad(((1, 1),)).cast(dtypes.int16))
+    # NOTE: this is folded due to CAST_BEFORE_VIEW
+    _check_ast_count(0, Tensor.ones(4).pad(((1, 1),)).cast(dtypes.int16))
     np.testing.assert_equal(Tensor.ones(4).pad(((1, 1),)).cast(dtypes.int16).numpy(), [0, 1, 1, 1, 1, 0])
+    _check_ast_count(0, Tensor.full(4, fill_value=-1).pad(((1, 1),)).cast(dtypes.uint16))
+    np.testing.assert_equal(Tensor.full(4, fill_value=-1).pad(((1, 1),)).cast(dtypes.uint16).numpy(), [0, 65535, 65535, 65535, 65535, 0])
+    # not folded
     _check_ast_count(1, Tensor.ones(4).pad(((1, 1),)).cast(dtypes.int64))
     np.testing.assert_equal(Tensor.ones(4).pad(((1, 1),)).cast(dtypes.int64).numpy(), [0, 1, 1, 1, 1, 0])
-    _check_ast_count(1, Tensor.full(4, fill_value=-1).pad(((1, 1),)).cast(dtypes.uint16))
-    np.testing.assert_equal(Tensor.full(4, fill_value=-1).pad(((1, 1),)).cast(dtypes.uint16).numpy(), [0, 65535, 65535, 65535, 65535, 0])
 
 class TestReduceOpsConstFolding(unittest.TestCase):
   def test_const_sum(self):
     _check_ast_count(0, Tensor.ones(4, 5, 6).sum())
     np.testing.assert_equal(Tensor.ones(4, 5, 6).sum().numpy(), 4 * 5 * 6)
     _check_ast_count(0, Tensor.ones(4, 5, 6).sum(axis=0))
     np.testing.assert_equal(Tensor.ones(4, 5, 6).sum(axis=0).numpy(), np.full((5, 6), 4))
```

### Comparing `tinygrad_tools-0.8.1/test/test_conv.py` & `tinygrad_tools-0.8.2/test/test_conv.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_conv_shapetracker.py` & `tinygrad_tools-0.8.2/test/test_conv_shapetracker.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_copy_speed.py` & `tinygrad_tools-0.8.2/test/test_copy_speed.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_custom_function.py` & `tinygrad_tools-0.8.2/test/test_custom_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 from typing import Optional, Tuple
 from tinygrad.helpers import prod
 from tinygrad.dtype import dtypes
 
 # *** first, we implement the atan2 op at the lowest level ***
 # `atan2_gpu` for GPUBuffers and `atan2_cpu` for CPUBuffers
 from tinygrad.lazy import Buffer, create_lazybuffer
-from tinygrad.device import CompiledRunner, Device
+from tinygrad.device import Device
 from tinygrad.shape.shapetracker import ShapeTracker
+from tinygrad.engine.realize import CompiledRunner
+from tinygrad.renderer import Program
 
 # we don't always have GPU support, so the type signature is the abstract CompiledBuffer instead of GPUBuffer
 def atan2_gpu(ret:Buffer, a:Buffer, b:Buffer):
   assert a.dtype == b.dtype and a.dtype == dtypes.float32, "gpu function only supports float32"
   src = """
   __kernel void atan2_gpu(global float *c, global float *a, global float *b) {
     int idx = get_global_id(0);
     c[idx] = atan2(a[idx], b[idx]);
   }"""
-  CompiledRunner("atan2_gpu", src, ret.device, global_size=[ret.size]).exec([ret, a, b])
+  CompiledRunner(Program("atan2_gpu", src, ret.device, global_size=[ret.size,1,1])).exec([ret, a, b])
 
 def atan2_cpu(ret:Buffer, a:Buffer, b:Buffer): ret.copyin(np.require(np.arctan2(a._buf, b._buf), requirements='C').data)
 
 # *** second, we write the ATan2 mlop ***
 # NOTE: The derivative of atan2 doesn't need a custom op! https://www.liquisearch.com/atan2/derivative
 # In general, it is also optional to write a backward function, just your backward pass won't work without it
```

### Comparing `tinygrad_tools-0.8.1/test/test_device_speed.py` & `tinygrad_tools-0.8.2/test/test_device_speed.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tinygrad.codegen.uops import UOpGraph
 from tinygrad.helpers import Timing, Profiling
 
 class TestDeviceSpeed(unittest.TestCase):
   @classmethod
   def setUpClass(cls):
     cls.dev = Device[Device.DEFAULT]
-    cls.empty = Device[Device.DEFAULT].compiler.render("test", UOpGraph())
+    cls.empty = Device[Device.DEFAULT].renderer.render("test", UOpGraph())
 
   def test_empty_compile(self):
     with Timing("compiler "):
       self.dev.compiler.compile(self.empty)
 
   def test_empty_compile_twice(self):
     self.dev.compiler.compile(self.empty)
```

### Comparing `tinygrad_tools-0.8.1/test/test_dtype.py` & `tinygrad_tools-0.8.2/test/test_dtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest, operator, subprocess
 import numpy as np
 import torch
 from typing import Any, List
-from tinygrad.helpers import getenv, DEBUG
+from tinygrad.helpers import getenv, DEBUG, CI
 from tinygrad.dtype import DType, DTYPES_DICT, ImageDType, PtrDType, least_upper_float, least_upper_dtype
 from tinygrad import Device, Tensor, dtypes
 from hypothesis import given, settings, strategies as strat
-from test.helpers import is_dtype_supported
+from test.helpers import is_dtype_supported, rand_for_dtype
 
 settings.register_profile("my_profile", max_examples=200, deadline=None)
 settings.load_profile("my_profile")
 
 core_dtypes = list(DTYPES_DICT.values())
 if Device.DEFAULT == "CPU": core_dtypes.remove(dtypes.bfloat16)  # NOTE: this is for teenygrad, don't remove
 dtype_ints = [dt for dt in core_dtypes if dtypes.is_int(dt) and is_dtype_supported(dt)]
@@ -43,35 +43,30 @@
 def _test_cast(a:Tensor, target_dtype:DType):
   if a.is_floating_point() and dtypes.is_unsigned(target_dtype):
     # converting negative float to unsigned integer is undefined
     a = a.abs()
   if target_dtype == dtypes.half and Device.DEFAULT == "PYTHON":
     # TODO: struct.pack cannot pack value > 65504 (max of half) into e format
     a = (a > 65504).where(65504, a)
+  if CI and Device.DEFAULT == "CLANG" and (target_dtype, a.dtype) in [(dtypes.double, dtypes.half), (dtypes.half, dtypes.double)]:
+    # TODO: cast between double and half are broken https://github.com/tinygrad/tinygrad/issues/4084
+    return
 
   _test_op(lambda: a.cast(target_dtype), target_dtype, list(a.numpy().astype(target_dtype.np)))
 def _test_bitcast(a:Tensor, target_dtype:DType, target=None):
   if target_dtype == dtypes.bfloat16: raise unittest.SkipTest("no test for bf16 bitcast yet")
   _test_op(lambda: a.bitcast(target_dtype), target_dtype, target or a.numpy().view(target_dtype.np).tolist())
 
 class TestDType(unittest.TestCase):
   DTYPE: Any = None
   DATA: Any = None
   @classmethod
   def setUpClass(cls):
     if not cls.DTYPE or not is_dtype_supported(cls.DTYPE): raise unittest.SkipTest("dtype not supported")
-    DATA_SIZE = 10
-    if dtypes.is_unsigned(cls.DTYPE):
-      cls.DATA = np.random.randint(0, 100, size=DATA_SIZE, dtype=cls.DTYPE.np)
-    elif dtypes.is_int(cls.DTYPE):
-      cls.DATA = np.random.randint(-100, 100, size=DATA_SIZE, dtype=cls.DTYPE.np)
-    elif cls.DTYPE == dtypes.bool:
-      cls.DATA = np.random.choice([True, False], size=DATA_SIZE)
-    else:
-      cls.DATA = np.random.uniform(-10, 10, size=DATA_SIZE).astype(cls.DTYPE.np)
+    cls.DATA = rand_for_dtype(cls.DTYPE, 10)
   def setUp(self):
     if self.DTYPE is None: raise unittest.SkipTest("base class")
 
   def test_to_np(self): _test_to_np(Tensor(self.DATA, dtype=self.DTYPE), self.DTYPE.np, np.array(self.DATA, dtype=self.DTYPE.np))
 
   def test_casts_to(self): list(map(
     lambda dtype: _test_cast(Tensor(self.DATA, dtype=dtype), self.DTYPE),
@@ -201,15 +196,15 @@
 
   def test_float_to_uint(self):
     _test_op(lambda: Tensor([-0.9, -0.3, 1.2], dtype=dtypes.float32).cast(dtypes.uint32), dtypes.uint32,
              [0, 0, 1])
 
 class TestDoubleDtype(TestDType):
   DTYPE = dtypes.double
-  @unittest.skipIf(getenv("CUDACPU") or getenv("PTX"), "conversion not supported on CUDACPU and PTX")  # TODO: why not?
+  @unittest.skipIf((CI and Device.DEFAULT in {"CUDA", "NV"}) or getenv("PTX"), "conversion not supported on CUDACPU and PTX")  # TODO: why not?
   def test_float64_increased_precision(self):
     for func in [
       lambda t: t.exp(),
       lambda t: t.exp2(),
       lambda t: t.log(),
       lambda t: t.log2(),
       lambda t: t.sqrt(),
@@ -527,14 +522,29 @@
     assert (Tensor([0, 1], dtype=dtypes.uint32)).sum().dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint64)).sum().dtype == dtypes.uint64
     assert (Tensor([0, 1], dtype=dtypes.float16)).sum().dtype == dtypes.float16
     #assert (Tensor([0, 1], dtype=dtypes.bfloat16)).sum().dtype == dtypes.bfloat16
     assert (Tensor([0, 1], dtype=dtypes.float32)).sum().dtype == dtypes.float32
     assert (Tensor([0, 1], dtype=dtypes.float64)).sum().dtype == dtypes.float64
 
+  def test_mean(self):
+    assert (Tensor([0, 1], dtype=dtypes.bool)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int8)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int16)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int32)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int64)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint8)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint16)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint32)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint64)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.float16)).mean().dtype == dtypes.float16
+    #assert (Tensor([0, 1], dtype=dtypes.bfloat16)).mean().dtype == dtypes.bfloat16
+    assert (Tensor([0, 1], dtype=dtypes.float32)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.float64)).mean().dtype == dtypes.float64
+
   def test_cumsum(self):
     assert (Tensor([0, 1], dtype=dtypes.bool)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int8)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int16)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int32)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int64)).cumsum(0).dtype == dtypes.int64
     assert (Tensor([0, 1], dtype=dtypes.uint8)).cumsum(0).dtype == dtypes.uint32
@@ -625,33 +635,40 @@
   @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
   def test_mean_half_precision_underflow(self):
     N = 10000
     x = 0.001
     t = Tensor([[x]], dtype=dtypes.half, requires_grad=True).expand(N, N).contiguous()
     np.testing.assert_allclose(t.mean(axis=1).numpy(), np.array([x] * N, dtype=np.float16), rtol=1e-3)
 
-  @unittest.skip("TODO: fix this")
   @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
   def test_mean_half_precision_overflow(self):
-    t = Tensor([60000, 60000, 60000], dtype=dtypes.half, requires_grad=True)
+    N = 256
+    t = Tensor([60000] * N*N, dtype=dtypes.half, requires_grad=True).reshape(N, N)
     np.testing.assert_allclose(t.mean().numpy(), 60000)
     t.square().mean().backward()
-    np.testing.assert_allclose(t.grad.numpy(), [60000 * 2 / 3] * 3)
+    np.testing.assert_allclose(t.grad.numpy().flatten(), [60000 * 2 / (N*N)] * N*N)
 
 class TestImplicitFunctionTypeChange(unittest.TestCase):
   def test_functions(self):
     result = []
     for func in [
       lambda t: t.exp(),
       lambda t: t.exp2(),
       lambda t: t.log(),
       lambda t: t.log2(),
       lambda t: t.sqrt(),
       lambda t: t.sin(),
     ]:
       t = func(Tensor([4.0, 3.0])).max() == func(Tensor([4.0, 3.0]))
       result.append(t.numpy().sum())
-
     assert all(result)
 
+class TestTensorMethod(unittest.TestCase):
+  @given(strat.sampled_from(core_dtypes))
+  def test_abs_diff(self, dt):
+    if dt == dtypes.bool or not is_dtype_supported(dt): return
+    a, b = Tensor([2], dtype=dt), Tensor([1], dtype=dt)
+    ret = (a - b).abs()
+    np.testing.assert_allclose(ret.numpy(), np.abs(a.numpy()-b.numpy()))
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_dtype_alu.py` & `tinygrad_tools-0.8.2/test/test_dtype_alu.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 #binary_operations.append(operator.mod)
 
 # TODO: (a+b)/2 in tensor.py's maximum can overflow. This requires a new implementation of maximum that can be backpropagated
 #binary_operations += [(Tensor.maximum, np.maximum)]
 
 # TODO: CUDACPU segfaults on sin
 # TODO: METAL sin is flaky for float16
-if getenv("CUDACPU") or Device.DEFAULT == "METAL": unary_operations.remove((Tensor.sin, np.sin))
+if getenv("CUDACPU") or (getenv("MOCKGPU") and Device.DEFAULT == "NV") or Device.DEFAULT == "METAL": unary_operations.remove((Tensor.sin, np.sin))
 
 class ht:
   float64 = strat.floats(width=64, allow_subnormal=False)
   float32 = strat.floats(width=32, allow_subnormal=False)
   float16 = strat.floats(width=16, allow_subnormal=False)
   uint8 = strat.integers(0, 255)
   uint16 = strat.integers(0, 65535)
@@ -141,15 +141,15 @@
   @given(ht.bool, ht.bool, strat.sampled_from(((operator.add, operator.add), (operator.mul, operator.mul))))
   def test_bool(self, a, b, op): universal_test(a, b, dtypes.bool, op)
 
   @given(ht.int32, ht.int32, ht.float32, strat.sampled_from(integer_binary_operations), strat.sampled_from(binary_operations))
   def test_int32_midcast_float(self, a, b, c, op1, op2): universal_test_midcast(a, b, c, op1, op2, dtypes.int32, dtypes.float32)
 
   # Metal and CUDACPU and HIP behave differently than numpy in CI for overflows
-  skip_overflow = CI and (Device.DEFAULT in {"RHIP", "HSA"} or getenv("CUDACPU"))
+  skip_overflow = CI and (Device.DEFAULT in {"HSA", "AMD", "NV"} or getenv("CUDACPU"))
   @given(strat.floats(width=32, min_value=0, max_value=10.0) if skip_overflow else ht.float32,
          strat.floats(width=32, min_value=0, max_value=10.0) if skip_overflow else ht.float32,
          ht.int32, strat.sampled_from(binary_operations), strat.sampled_from(integer_binary_operations))
   def test_float_midcast_int32(self, a, b, c, op1, op2): universal_test_midcast(a, b, c, op1, op2, dtypes.float32, dtypes.int32)
 
   @unittest.skip("broken. TODO: fix it")
   @given(ht.float32, strat.sampled_from(dtypes_float+dtypes_int+dtypes_bool))
```

### Comparing `tinygrad_tools-0.8.1/test/test_fusion_op.py` & `tinygrad_tools-0.8.2/test/test_fusion_op.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import time
 import numpy as np
-from tinygrad import Tensor, dtypes, Device
+from tinygrad import Tensor, dtypes
 from tinygrad.engine.schedule import create_schedule
-from tinygrad.engine.realize import run_schedule
+from tinygrad.engine.realize import lower_schedule_item, run_schedule
 
 class TestFusionOp(unittest.TestCase):
   def test_contiguous_add(self):
     def test(contig=False):
       bt = Tensor(np.arange(16), dtype=dtypes.float32).reshape(4,4)
       x = bt.permute(1,0)
       if contig: x = x.contiguous()
@@ -23,17 +23,17 @@
     assert all(x == 20.0 for x in outd)
 
   def test_recursive_add(self):
     st = time.perf_counter()
     a = Tensor([1,2,3,4])
     for _ in range(24): a = a + a
     sched = create_schedule([a.lazydata], None)
-    ji = Device[Device.DEFAULT].get_runner(*sched[-1].ast)
+    ei = lower_schedule_item(sched[-1])
     self.assertLess(time.perf_counter()-st, 1.0)
-    assert len(ji.prg.splitlines()) < 250
+    assert len(ei.prg.p.src.splitlines()) < 250
 
   def test_recursive_add_cmp(self):
     st = time.perf_counter()
     a = Tensor([1,2,3,4])
     for _ in range(24): a = a + a
     sched1 = create_schedule([a.lazydata], None)
     b = Tensor([1,2,3,4])
```

### Comparing `tinygrad_tools-0.8.1/test/test_fuzz_shape_ops.py` & `tinygrad_tools-0.8.2/test/test_fuzz_shape_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 def st_shape(draw) -> tuple[int, ...]:
   s = draw(stn.array_shapes(min_dims=0, max_dims=6,
                             min_side=0, max_side=512))
   assume(prod(s) <= 1024 ** 2)
   assume(prod([d for d in s if d]) <= 1024 ** 4)
   return s
 
-
 def tensors_for_shape(s:tuple[int, ...]) -> tuple[torch.tensor, Tensor]:
   x = np.arange(prod(s)).reshape(s)
   return torch.from_numpy(x), Tensor(x)
 
 def apply(tor, ten, tor_fn, ten_fn=None):
   ok = True
   try: tor = tor_fn(tor)
@@ -47,15 +46,14 @@
     tor, ten, ok = apply(tor, ten, lambda t: t.split(sizes, dim))
     assert ok
     if tor is None and ten is None: return
 
     assert len(tor) == len(ten)
     assert all([np.array_equal(tor.numpy(), ten.numpy()) for (tor, ten) in zip(tor, ten)])
 
-
   @settings.get_profile(__file__)
   @given(st_shape(), st_int32, st_int32)
   def test_chunk(self, s:tuple[int, ...], dim:int, num:int):
     # chunking on a 0 dim is cloning and leads to OOM if done unbounded.
     assume((0 <= (actual_dim := len(s)-dim if dim < 0 else dim) < len(s) and s[actual_dim] > 0) or
            (num < 32))
```

### Comparing `tinygrad_tools-0.8.1/test/test_gc.py` & `tinygrad_tools-0.8.2/test/test_gc.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_image_dtype.py` & `tinygrad_tools-0.8.2/test/test_image_dtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import numpy as np
 from tinygrad import Device, dtypes, Tensor, Variable
 from tinygrad.dtype import ImageDType
-from tinygrad.features.image import to_image_idx
+from tinygrad.codegen.linearizer import to_image_idx
 
 @unittest.skipIf(Device.DEFAULT != "GPU", "only images on GPU")
 class TestImageDType(unittest.TestCase):
   def test_image_and_back(self):
     data = Tensor.randn(9*27*4).realize()
     tst = data.numpy()
     it = data.cast(dtypes.imagef((9,27,4))).realize()
```

### Comparing `tinygrad_tools-0.8.1/test/test_jit.py` & `tinygrad_tools-0.8.2/test/test_jit.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 
   def test_jit_const_inputs(self):
     @TinyJit
     def g(x,y,z): return (x+y+z).realize()
     for i in range(5):
       np.testing.assert_equal(g(Tensor([i]*3), Tensor.ones(3), Tensor.zeros(3)).numpy(), np.array([i+1]*3))
 
-  @unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL", "HSA"}, "no GPU CI")
+  @unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL", "HSA", "NV", "AMD"}, "no GPU CI")
   def test_jitted_transfers(self):
     d0, d1 = f"{Device.DEFAULT}:0", f"{Device.DEFAULT}:1"
 
     def f(a, b):
       x = a.to(d1)
       y = b.to(d1)
       return x.realize(), y.realize()
```

### Comparing `tinygrad_tools-0.8.1/test/test_kernel_cache.py` & `tinygrad_tools-0.8.2/test/test_kernel_cache.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_lazybuffer.py` & `tinygrad_tools-0.8.2/test/test_lazybuffer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 import numpy as np
 import unittest
 from tinygrad import Tensor, Device, dtypes
-from tinygrad.lazy import LazyBuffer, ReduceOps
+from tinygrad.lazy import LazyBuffer, ReduceOps, LoadOps
 from tinygrad.engine.schedule import create_schedule
 
 class TestLazyBuffer(unittest.TestCase):
   def test_fromcpu_shape_tracker(self):
     def helper(a: np.ndarray):
       print(a.shape, a.strides, a.flags.c_contiguous)
       b = Tensor(a).lazydata
@@ -88,9 +88,30 @@
     a = Tensor.rand(255, 256).realize()
     a = a.sum()
     sched = create_schedule([a.lazydata])
     assert len(sched) == 2
     for s in sched:
       assert s.ast[0].src[0].op is ReduceOps.SUM
 
+class TestView(unittest.TestCase):
+  def test_all_masked_out(self):
+    # start with non CONST LoadOps
+    a = Tensor.rand(10, 10)
+    assert a.lazydata.base.op is not LoadOps.CONST
+
+    # all masked out, degrades to const 0
+    b = a.pad(((0, 10), None))[10:]
+    assert b.shape == (10, 10)
+    assert b.lazydata.base.op is LoadOps.CONST and b.lazydata.base.arg == 0
+
+    # mask out dim = 1 works too
+    b = a.pad((None, (0, 10)))[:, 10:]
+    assert b.shape == (10, 10)
+    assert b.lazydata.base.op is LoadOps.CONST and b.lazydata.base.arg == 0
+
+    # partial masked out does not degrade into CONST
+    b = a.pad(((0, 5), None))[5:]
+    assert b.shape == (10, 10)
+    assert b.lazydata.base.op is not LoadOps.CONST
+
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_lazyop.py` & `tinygrad_tools-0.8.2/test/test_lazyop.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_linearizer.py` & `tinygrad_tools-0.8.2/test/test_linearizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing import List, Tuple
 import numpy as np
 import unittest
+from dataclasses import replace
 
 from tinygrad.codegen.kernel import Opt, OptOps, KernelOptError, tensor_cores
 from tinygrad.codegen.linearizer import Linearizer, UOp, UOps, expand_node, expand_idxs
 from tinygrad.device import Device, Buffer
 from tinygrad.ops import BinaryOps, BufferOps, MemBuffer, ConstBuffer, LazyOp, LoadOps, TernaryOps, ReduceOps, UnaryOps
 from tinygrad.shape.shapetracker import ShapeTracker
 from tinygrad.shape.view import View
 from tinygrad.shape.symbolic import MulNode, Variable, NumNode, Node
 from tinygrad.tensor import Tensor
 from tinygrad.engine.schedule import create_schedule
-from tinygrad.engine.realize import run_schedule, lower_schedule
-from tinygrad.helpers import prod, Context, getenv
+from tinygrad.engine.realize import run_schedule, lower_schedule, CompiledRunner
+from tinygrad.helpers import prod, Context, getenv, CI
 from tinygrad.dtype import DType, dtypes
 from tinygrad.codegen.uops import UOpGraph
 
 def helper_realized_ast(r:Tensor):
   s = create_schedule([r.lazydata])
   run_schedule(s[:-1])  # run all kernels except the last one
   # now all input LazyBuffers buffers in s[-1] should be realized
@@ -82,22 +84,62 @@
   def test_multioutput(self):
     dtype, st = dtypes.int, ShapeTracker.from_shape((8,))
     a = LazyOp(BufferOps.LOAD, arg=MemBuffer(idx=2, dtype=dtype, st=st))
     b = LazyOp(BufferOps.LOAD, arg=MemBuffer(idx=3, dtype=dtype, st=st))
     out0 = LazyOp(BufferOps.STORE, (LazyOp(op=BinaryOps.ADD, src=(a,b)),), MemBuffer(idx=0, dtype=dtype, st=st))
     out1 = LazyOp(BufferOps.STORE, (LazyOp(op=BinaryOps.MUL, src=(a,b)),), MemBuffer(idx=1, dtype=dtype, st=st))
 
-    lin = Linearizer(out0, out1)
-    lin.linearize()
+    a_t = Tensor.full(st.shape, 2).contiguous().realize()
+    b_t = Tensor.full(st.shape, 3).contiguous().realize()
+    lin = helper_linearizer_ast((out0, out1), [a_t, b_t], wanna_output=[a_t.numpy()+b_t.numpy(), a_t.numpy()*b_t.numpy()])[0]
 
     stores = [u for u in lin.uops if u.uop is UOps.STORE]
     mutable_bufs = [u for u in lin.uops if u.uop is UOps.DEFINE_GLOBAL and u.arg[-1]]
     assert len(mutable_bufs) == len(stores) == 2
     assert [u.arg[0] for u in mutable_bufs] == [0, 1]
 
+  def test_end_local(self):
+    if not (opts:=Device[Device.DEFAULT].renderer).has_local or not opts.has_shared: self.skipTest("device does not support locals")
+    load = MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker.from_shape((32,)))
+    store = MemBuffer(idx=0, dtype=dtypes.int, st=ShapeTracker.from_shape((1,)))
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BufferOps.LOAD, arg=load),), arg=(0,)),), arg=store),
+
+    load_t = Tensor.full(load.st.shape, 1).contiguous().realize()
+    k = helper_linearizer_ast(ast, [load_t], wanna_output=[load_t.numpy().sum()])[1]
+    self.assertEqual(k.uops.uops[-1].uop, UOps.ENDIF)
+    self.assertLess(k.uops.uops.index([x for x in k.uops.uops if x.uop is UOps.STORE][-1]), k.uops.uops.index(k.uops.uops[-1]))
+
+  @unittest.expectedFailure
+  def test_early_end_local(self):
+    shape, output_shape = (32,), (1,)
+    load0 = MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker.from_shape(shape))
+    load1 = MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker.from_shape(shape))
+    store = MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker.from_shape(output_shape))
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.ADD, src=(
+      LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BufferOps.LOAD, arg=load0),)),LazyOp(op=BufferOps.LOAD, arg=load1), )),)),), arg=store),
+
+    load0_t = Tensor.randn(shape).realize()
+    load1_t = Tensor.randn(shape).realize()
+    k = helper_linearizer_ast(ast, [load0_t, load1_t], wanna_output=[(load0_t.numpy().sum() + load1_t.numpy()).sum()])[1]
+    self.assertEqual(len(endifs:=[x for x in k.uops.uops if x.uop is UOps.ENDIF]), len(ifs:=[x for x in k.uops.uops if x.uop is UOps.IF]))
+    self.assertEqual(len(barriers:=[x for x in k.uops.uops if x.uop is UOps.BARRIER]), 3)
+    self.assertEqual(k.uops.uops[k.uops.uops.index(endifs[0])-1].uop, UOps.STORE)
+    self.assertEqual(k.uops.uops[k.uops.uops.index(endifs[0])+1], barriers[1])
+    self.assertEqual(k.uops.uops[k.uops.uops.index(endifs[0])+2].uop, UOps.LOAD)
+    self.assertLess(k.uops.uops.index(barriers[0]), k.uops.uops.index(ifs[0]))
+    self.assertLess(k.uops.uops.index(ifs[0]), k.uops.uops.index(endifs[0]))
+    self.assertLess(k.uops.uops.index(barriers[1]), k.uops.uops.index(ifs[1]))
+
+  @unittest.expectedFailure
+  def test_mean_std_multireduce(self):
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=UnaryOps.SQRT, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(15, 25, 35), strides=(875, 35, 1), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(15, 25, 35), strides=(875, 35, 1), offset=0, mask=None, contiguous=True),)))),), arg=(0, 1, 2)), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=7.619047619047618e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(15, 25, 35), strides=(0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None), LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(15, 25, 35), strides=(875, 35, 1), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(15, 25, 35), strides=(875, 35, 1), offset=0, mask=None, contiguous=True),)))),), arg=(0, 1, 2)), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=7.619047619047618e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(15, 25, 35), strides=(0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None)), arg=None),), arg=(0, 1, 2)), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=7.619628162145687e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 1, 1), strides=(0, 0, 0), offset=0, mask=None, contiguous=True),))))), arg=None),), arg=None),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 1, 1), strides=(0, 0, 0), offset=0, mask=None, contiguous=True),)))), # noqa: E501
+
+    x = Tensor.randn(15, 25, 35).realize()
+    helper_linearizer_ast(ast, [x], wanna_output=[x.numpy().std()])
+
   def test_load_dedup(self):
     # for different leaves in the AST, the same loads may occur.
 
     a = Tensor.randn(4).realize()
     # these are of size 3 to avoid float4 coalesce
     r = a[:-1] + a[1:]
 
@@ -137,15 +179,15 @@
     k = Linearizer(*create_schedule([r.lazydata])[-1].ast)
     k.upcast()
     k.linearize()
     num_ops = len([uop for uop in k.uops if uop.uop is UOps.ALU])
     assert num_ops <= 1, "more alu uops than needed"
 
   def test_reduce_upcast(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.supports_float4:
+    if not Device[Device.DEFAULT].renderer.supports_float4:
       self.skipTest("device does not support upcast")
     x, w = Tensor.randn((1,1,3)).realize(), Tensor.randn((1,1,2)).realize()
     r = Tensor.conv2d(x,w,padding=1).relu()
 
     k = Linearizer(*create_schedule([r.lazydata])[-1].ast)
     k.upcast()
     k.upcast()
@@ -153,15 +195,15 @@
     accs = [u for u in k.uops if u.uop is UOps.DEFINE_ACC]
     stores = [u for u in k.uops if u.uop is UOps.STORE]
     assert len(accs) == 1
     assert len(stores) == 1
     assert stores[0].vin[-1].dtype == accs[0].dtype == dtypes.float.vec(4)
 
   def test_upcast_with_locals(self):
-    if not (opts:=Device[Device.DEFAULT].compiler.compiler_opts).has_local or not opts.has_shared or not opts.supports_float4:
+    if not (opts:=Device[Device.DEFAULT].renderer).has_local or not opts.has_shared or not opts.supports_float4:
       self.skipTest("device does not support upcasted reduce with locals")
 
     x, y = Tensor.rand(1,128), Tensor.rand(128, 128)
     r = (x@y).relu()
     k = Linearizer(*create_schedule([r.lazydata])[-1].ast)
     k.hand_coded_optimizations()
     k.linearize()
@@ -210,28 +252,29 @@
       (dtypes.bfloat16, dtypes.bfloat16, dtypes.bfloat16),
       (dtypes.float, dtypes.float16, dtypes.float16),
     )
     for tensor_dtype, acc_dtype, expected_dtype in tests:
       a, b = Tensor.rand(8, 8, dtype=tensor_dtype), Tensor.rand(8, 8, dtype=tensor_dtype)
       helper_arg_acc_dtype(a.sum(acc_dtype=acc_dtype), expected_dtype)
       helper_arg_acc_dtype(a.matmul(b, acc_dtype=acc_dtype), expected_dtype)
+      helper_arg_acc_dtype(Tensor.einsum("ki,ij->kj", a, b, acc_dtype=acc_dtype), expected_dtype)
       d, w = Tensor.rand(4, 8, 8, 8, dtype=tensor_dtype), Tensor.rand(8, 8, 2, 2, dtype=tensor_dtype)
       helper_arg_acc_dtype(d.conv2d(w, acc_dtype=acc_dtype), expected_dtype)
 
   def test_tensor_cores(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_tensor_cores:
+    if not Device[Device.DEFAULT].renderer.has_tensor_cores:
       self.skipTest("device doesn't have tensor cores")
-    for tc in tensor_cores[Device[Device.DEFAULT].compiler.compiler_opts.device]:
+    for tc in tensor_cores[Device[Device.DEFAULT].renderer.device]:
       if getenv("EMULATE_CUDA") and (tc.dtype_in == dtypes.bfloat16 or tc.dtype_out == dtypes.bfloat16): continue
       helper_tc_allclose(tc.dims[0], tc.dims[1], tc.dims[2], tc.dtype_in, tc.dtype_out, axis=0, tc_opt=0)
 
   def test_tensor_cores_padded(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_tensor_cores:
+    if not Device[Device.DEFAULT].renderer.has_tensor_cores:
       self.skipTest("device doesn't have tensor cores")
-    for tc in tensor_cores[Device[Device.DEFAULT].compiler.compiler_opts.device]:
+    for tc in tensor_cores[Device[Device.DEFAULT].renderer.device]:
       if getenv("EMULATE_CUDA") and (tc.dtype_in == dtypes.bfloat16 or tc.dtype_out == dtypes.bfloat16): continue
       pad = 1
 
       # check that TC is triggered for TC_OPT=2
       helper_tc_ensure_uops_and_opts_count(tc.dims[0]+pad, tc.dims[1]+pad, tc.dims[2]+pad,
                                            tc.dtype_in, tc.dtype_out, tc_opt=2, ensure_triggered=True)
 
@@ -245,19 +288,19 @@
       helper_tc_ensure_uops_and_opts_count(tc.dims[0]//4, tc.dims[1], tc.dims[2], tc.dtype_in, tc.dtype_out, tc_opt=2, ensure_triggered=False)
       helper_tc_ensure_uops_and_opts_count(tc.dims[0], tc.dims[1]//4, tc.dims[2], tc.dtype_in, tc.dtype_out, tc_opt=2, ensure_triggered=False)
       helper_tc_ensure_uops_and_opts_count(tc.dims[0], tc.dims[1], tc.dims[2]//4, tc.dtype_in, tc.dtype_out, tc_opt=2, ensure_triggered=False)
 
       # check correctness
       helper_tc_allclose(tc.dims[0]+pad, tc.dims[1]+pad, tc.dims[2]+pad, tc.dtype_in, tc.dtype_out, tc_opt=2)
 
-  @unittest.skipIf(Device.DEFAULT == "RHIP", "RHIP is really slow here")
+  @unittest.skipIf(CI and Device.DEFAULT in {"AMD"}, "AMD CI is really slow here")
   def test_tensor_cores_multi_reduce(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_tensor_cores:
+    if not Device[Device.DEFAULT].renderer.has_tensor_cores:
       self.skipTest("device doesn't have tensor cores")
-    for tc in tensor_cores[Device[Device.DEFAULT].compiler.compiler_opts.device]:
+    for tc in tensor_cores[Device[Device.DEFAULT].renderer.device]:
       if getenv("EMULATE_CUDA") and (tc.dtype_in == dtypes.bfloat16 or tc.dtype_out == dtypes.bfloat16): continue
       # this will be a M=G16, N=G32, M=G16, M=G16, K=R16, K=R16, K=R16 with 9 choices of TC MNK axes
       golden_result = None
       for axis in range(9):
         a = Tensor.rand(16, 16, 29, 29, dtype=tc.dtype_in).realize()
         b = Tensor.rand(32, 16, 16, 16, dtype=tc.dtype_in).realize()
         c = a.conv2d(b, padding=1, acc_dtype=tc.dtype_out)
@@ -265,25 +308,25 @@
 
         k = Linearizer(realized_ast)
         k.apply_tensor_cores(1, axis=axis, tc_opt=2)
         k.linearize()
         assert len([uop for uop in k.uops if uop.uop is UOps.WMMA]) > 0, "tensor core not triggered"
         assert len([x for x in k.applied_opts if x.op is OptOps.TC]) == 1, "tensor core opt not included"
 
-        prg = Device[Device.DEFAULT].to_program(k)
+        prg = CompiledRunner(k.to_program())
         real_bufs[0].copyin(np.zeros((real_bufs[0].size, ), dtype=real_bufs[0].dtype.np).data) # Zero to check that all values are filled
         prg.exec(real_bufs)
         result = np.frombuffer(real_bufs[0].as_buffer(), real_bufs[0].dtype.np)
 
         # ensure the results for each choice of axis matches
         if golden_result is None: golden_result = np.frombuffer(real_bufs[0].as_buffer(), real_bufs[0].dtype.np)
         np.testing.assert_allclose(result, golden_result, atol=0.1, rtol=0.15)
 
       # check that get_linearizer_actions produces all 9 options
-      from tinygrad.features.search import get_linearizer_actions
+      from tinygrad.engine.search import get_linearizer_actions
       tc_actions = [k for i, k in get_linearizer_actions(Linearizer(realized_ast), False).items() if k.applied_opts[0].op == OptOps.TC]
       assert len(tc_actions) == 9, f"get_linearizer_actions should contain 9 possible TC actions, only got {len(tc_actions)}"
 
   def test_limit_dims_to_max_5d_global(self):
     t = Tensor.empty(3, 4, 5, 6, 7).pad(((1, 1), (1, 1), (1, 1), (1, 1), (1, 1))) + 1
     sched = [si for si in create_schedule([t.lazydata]) if si.ast[0].op not in LoadOps]
     assert len(sched) == 1
@@ -324,15 +367,15 @@
       ast = LazyOp(BufferOps.CONST, (),
                    ConstBuffer(42, dtypes.float, ShapeTracker(views=(View(shape=(), strides=(), offset=0, mask=None, contiguous=True),))))
       ast = LazyOp(BufferOps.STORE, (ast,),
                    MemBuffer(0, dtypes.float, ShapeTracker(views=(View(shape=(), strides=(), offset=0, mask=None, contiguous=True),))))
       lin = Linearizer(ast) # this is a dummy ast
 
       lin.uops = UOpGraph()
-      return lin.uops.add(uop, dtype, vin, arg, cachable=False)
+      return lin.uops.add(uop, dtype, vin, arg)
 
     c0 = UOp(UOps.CONST, dtypes.float, vin=(), arg=0.0)
     assert helper_test_simplify(UOps.ALU, dtypes.float, vin=(UOp(UOps.CONST, dtypes.bool, vin=(), arg=True), c0, c0), arg=TernaryOps.WHERE) == c0
 
     c0 = UOp(UOps.CONST, dtypes.float, vin=(), arg=0.0)
     c1 = UOp(UOps.CONST, dtypes.float, vin=(), arg=1.0)
     assert helper_test_simplify(UOps.ALU, dtypes.float, vin=(UOp(UOps.CONST, dtypes.bool, vin=(), arg=True), c0, c1),
@@ -354,15 +397,15 @@
 
     helper(Tensor.arange(5.5, (3.5*300), 3.5))
     helper(Tensor.arange(-1, -100, -5))
     helper(Tensor.arange(-3.2, 6.7, 0.64))
     helper(Tensor.arange(256), max_ops=2)
     helper(Tensor.arange(255), max_ops=0)
 
-@unittest.skipUnless(Device[Device.DEFAULT].compiler.compiler_opts.supports_float4, "need backends that support float4")
+@unittest.skipUnless(Device[Device.DEFAULT].renderer.supports_float4, "need backends that support float4")
 class TestFloat4(unittest.TestCase):
   @staticmethod
   def count_float4(k):
     return (len([uop for uop in k.uops if uop.uop is UOps.LOAD and uop.dtype == dtypes.float.vec(4)]),
             len([uop for uop in k.uops if uop.uop is UOps.STORE and len(uop.vin) == 3 and uop.vin[2].dtype == dtypes.float.vec(4)]))
 
   # TODO: express opts below as auto opts
@@ -563,66 +606,88 @@
     k = Linearizer(*s.ast)
     k.hand_coded_optimizations()
     assert len(k.bufs) == 5  # make sure all ops are done in one kernel
     # check that we don't do too many upcasts
     assert prod(k.full_shape[k.shape_len-k.upcasted:k.shape_len]) <= 49
 
   def test_matvec(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local:
+    if not Device[Device.DEFAULT].renderer.has_local:
       self.skipTest("Only devices with locals")
     N = 128
     a = Tensor.rand(1, N).realize()
     b = Tensor.rand(N, N).realize()
     c = a @ b
 
     s = create_schedule([c.lazydata])[0]
     k = Linearizer(*s.ast)
     k.hand_coded_optimizations()
 
     assert k.group_for_reduces == 1
     assert k.local_dims == 1
     assert k.upcasted == 1
 
-def helper_linearizer_opt(r:Tensor, opts=[], apply_tc=False, atol=1e-4, rtol=1e-4, color_sizes=[]):
-  wanna_output = None
+def helper_linearizer_ast(ast:Tuple[LazyOp, ...], inputs:List[Tensor], *args, **kwargs):
+  inbufs = [x.lazydata.buffer for x in inputs]
+  outbufs = [Buffer(inbufs[-1].device, out.arg.st.size, out.arg.dtype).allocate() for out in ast]
+  return _helper_linearizer_opt_ast(ast, outbufs+inbufs, *args, **kwargs)
+
+def helper_linearizer_opt(r:Tensor, *args, **kwargs):
   realized_ast, real_bufs = helper_realized_ast(r)
+  return _helper_linearizer_opt_ast((realized_ast, ), real_bufs, *args, **kwargs)
+
+def _helper_linearizer_opt_ast(realized_ast:Tuple[LazyOp, ...], real_bufs:List[Buffer], opts=[],
+                               apply_tc=False, atol=1e-4, rtol=1e-4, color_sizes=[], wanna_output=[]) -> List[Linearizer]:
+  lins: List[Linearizer] = []
+  outbufs = [real_bufs[i] for i in range(len(realized_ast))]
 
-  def check_opt(opts, create_k, to_prg, expected_color_size):
+  def get_prg(k:Linearizer): return CompiledRunner(replace(k.to_program(), dname=Device.DEFAULT))
+
+  def check_opt(opts, create_k, expected_color_size):
     k = create_k()
+    lins.append(k)
     if apply_tc:
       assert k.apply_tensor_cores(1, extra_opts=opts), "no tensor core triggered"
     else:
       for opt in opts:
         k.apply_opt(opt)
     if expected_color_size is not None:
       assert (cs:=[(x,y) for x,y in zip(k.colors(), k.full_shape)]) == expected_color_size, f"expected={expected_color_size} got={cs}"
-    prg = to_prg(k)
-    real_bufs[0].copyin(np.zeros((real_bufs[0].size, ), dtype=real_bufs[0].dtype.np).data) # Zero to check that all values are filled
+    prg = get_prg(k)
+    for buf in outbufs: buf.copyin(np.zeros((buf.size, ), dtype=buf.dtype.np).data) # Zero to check that all values are filled
     prg.exec(real_bufs)
-    np.testing.assert_allclose(np.frombuffer(real_bufs[0].as_buffer(), real_bufs[0].dtype.np), wanna_output, atol=atol, rtol=rtol)
 
-  # Get baseline, which is not optimized at all.
-  k = Linearizer(realized_ast)
-  prg = Device[Device.DEFAULT].to_program(k)
+    for i, buf in enumerate(outbufs):
+      np.testing.assert_allclose(np.frombuffer(buf.as_buffer(), buf.dtype.np), wanna_output[i], atol=atol, rtol=rtol)
+
+  # Get baseline if it is not provided, which is not optimized at all.
+  k = Linearizer(*realized_ast)
+  lins.append(k)
+  prg = get_prg(k)
   prg.exec(real_bufs)
-  wanna_output = np.frombuffer(real_bufs[0].as_buffer(), real_bufs[0].dtype.np).copy()
+  if len(wanna_output) == 0: wanna_output = [np.frombuffer(buf.as_buffer(), buf.dtype.np).copy() for buf in outbufs]
+  else:
+    for i, buf in enumerate(outbufs):
+      np.testing.assert_allclose(np.frombuffer(buf.as_buffer(), buf.dtype.np), wanna_output[i], atol=atol, rtol=rtol)
 
   # Check correctness of handcoded optimiztions.
-  k = Linearizer(realized_ast)
+  k = Linearizer(*realized_ast)
+  lins.append(k)
   k.hand_coded_optimizations()
-  prg = Device[Device.DEFAULT].to_program(k)
-  real_bufs[0].copyin(np.zeros((real_bufs[0].size, ), dtype=real_bufs[0].dtype.np).data) # Zero to check that all values are filled
+  prg = get_prg(k)
+  for buf in outbufs: buf.copyin(np.zeros((buf.size, ), dtype=buf.dtype.np).data) # Zero to check that all values are filled
   prg.exec(real_bufs)
-  np.testing.assert_allclose(wanna_output, np.frombuffer(real_bufs[0].as_buffer(), real_bufs[0].dtype.np), atol=atol, rtol=rtol)
+  for i, buf in enumerate(outbufs):
+    np.testing.assert_allclose(np.frombuffer(buf.as_buffer(), buf.dtype.np), wanna_output[i], atol=atol, rtol=rtol)
   for i, x in enumerate(opts): # Check custom transformations if any.
-    check_opt(x, lambda: Linearizer(realized_ast), Device[Device.DEFAULT].to_program, color_sizes[i] if i < len(color_sizes) else None)
+    check_opt(x, lambda: Linearizer(*realized_ast), color_sizes[i] if i < len(color_sizes) else None)
+  return lins
 
 class TestKernelOpts(unittest.TestCase):
   def test_local_and_grouped_reduce(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.has_shared:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.has_shared:
       self.skipTest("Only Compiled uses linearizer with locals and shared")
 
     N = 128
     Tensor.manual_seed(1882)
     a = Tensor.rand(4, 4, N, N)
     b = Tensor.rand(4, 4, N)
     r = (b.sqrt() + ((a+1).sum(axis=3).exp()))
@@ -660,15 +725,15 @@
     b = Tensor.rand(4)
     r = (a+b).sqrt() * ((a+1).exp())
     helper_linearizer_opt(r, [
       [Opt(OptOps.UPCAST, 0, 4)], # Checking how it works with upcasts
     ])
 
   def test_matmul(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.has_shared:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.has_shared:
       self.skipTest("Only Compiled uses linearizer with locals and shared")
 
     N = 128
     Tensor.manual_seed(1552)
     a = Tensor.rand(N, N)
     b = Tensor.rand(N, N)
     r = a@b
@@ -690,15 +755,15 @@
       [Opt(OptOps.LOCAL, 0, 4), Opt(OptOps.LOCAL, 0, 4), Opt(OptOps.GROUPTOP, 0, 8), Opt(OptOps.UNROLL, 0, 4), Opt(OptOps.UPCAST, 0, 4),
        Opt(OptOps.UPCAST, 1, 2)],
       # Full global upcast + local
       [Opt(OptOps.LOCAL, 0, 4), Opt(OptOps.LOCAL, 0, 4), Opt(OptOps.GROUPTOP, 0, 8), Opt(OptOps.UNROLL, 0, 4), Opt(OptOps.UPCAST, 0, 8)],
     ])
 
   def test_double_reduce(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.has_shared:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.has_shared:
       self.skipTest("Only Compiled uses linearizer with locals and shared")
 
     N = 128
     Tensor.manual_seed(1552)
     a = Tensor.rand(8, N, 8, N)
     r = a.sum(axis=(1,3))
     helper_linearizer_opt(r, [
@@ -717,15 +782,15 @@
       [Opt(OptOps.LOCAL, 0, 2), Opt(OptOps.LOCAL, 1, 2), Opt(OptOps.GROUPTOP, 0, 8), Opt(OptOps.GROUPTOP, 1, 4), Opt(OptOps.UPCAST, 0, 2),
        Opt(OptOps.UNROLL, 0, 4), Opt(OptOps.UNROLL, 1, 4)], # Checking how it works with 2 grouped_reduces + upcasts + locals.
       [Opt(OptOps.LOCAL, 0, 4), Opt(OptOps.LOCAL, 1, 4), Opt(OptOps.GROUPTOP, 0, 4), Opt(OptOps.GROUPTOP, 1, 4), Opt(OptOps.UPCAST, 0, 2),
        Opt(OptOps.UPCAST, 0, 2)], # No globals
     ])
 
   def test_invalid_tensor_core_extra_opts(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_tensor_cores:
+    if not Device[Device.DEFAULT].renderer.has_tensor_cores:
       self.skipTest("device doesn't have tensor cores")
     if Device.DEFAULT not in tensor_cores:
       self.skipTest("No tensor cores for device")
 
     N = 128
     Tensor.manual_seed(1552)
     a = Tensor.rand(N, N)
@@ -738,33 +803,33 @@
     ]
     for x in invalid_opts:
       k = Linearizer(realized_ast)
       with self.assertRaises(AssertionError):
         assert k.apply_tensor_cores(use_tensor_cores=1, extra_opts=x), "no valid tensor core" # for METAL in runners
 
   def test_buf_index_not_found_tensor_core(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_tensor_cores:
+    if not Device[Device.DEFAULT].renderer.has_tensor_cores:
       self.skipTest("device doesn't have tensor cores")
     if Device.DEFAULT not in tensor_cores:
       self.skipTest("No tensor cores for device")
 
-    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.CMPEQ, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1243, 256), strides=(0, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1243, 256), strides=(1, 0), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=(dtypes.float, False)), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1243, 256), strides=(1, 0), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=(0,)),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 256), strides=(0, 1), offset=0, mask=None, contiguous=True),))))  # noqa: E501
-    k = Linearizer(ast, opts=Device[Device.DEFAULT].compiler.compiler_opts)
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.CMPEQ, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1243, 256), strides=(0, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1243, 256), strides=(1, 0), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=dtypes.float), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1243, 256), strides=(1, 0), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=(0,)),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 256), strides=(0, 1), offset=0, mask=None, contiguous=True),))))  # noqa: E501
+    k = Linearizer(ast, opts=Device[Device.DEFAULT].renderer)
     with self.assertRaises(KernelOptError):
       k.apply_opt(Opt(OptOps.TC, 0, 1))
 
   def test_tensor_core_opts(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_tensor_cores:
+    if not Device[Device.DEFAULT].renderer.has_tensor_cores:
       self.skipTest("device doesn't have tensor cores")
     if Device.DEFAULT not in tensor_cores:
       self.skipTest("No tensor cores for device")
 
     N = 128
     Tensor.manual_seed(1552)
-    for tc in tensor_cores[Device[Device.DEFAULT].compiler.compiler_opts.device]:
+    for tc in tensor_cores[Device[Device.DEFAULT].renderer.device]:
       # bf16 buffer returns float32 numpy outputs so test would fail. testing opt with half suffices.
       if tc.dtype_in == dtypes.bfloat16: continue
       a, b = Tensor.rand(N, N, dtype=tc.dtype_in), Tensor.rand(N, N, dtype=tc.dtype_in)
       r = a.matmul(b, acc_dtype=tc.dtype_out)
       (atol, rtol) = ((0.25, 0.01) if tc.dtype_out == dtypes.half else (3e-2, 1e-3)) if tc.dtype_in == dtypes.half else (1e-4, 1e-4)
       helper_linearizer_opt(r, [
         [],
@@ -783,29 +848,48 @@
         [Opt(OptOps.UPCAST, 0, 4), Opt(OptOps.UNROLL, 0, 2), Opt(OptOps.UPCAST, 1, 4)],
         [Opt(OptOps.UNROLL, 0, 2), Opt(OptOps.UPCAST, 1, 4), Opt(OptOps.UPCAST, 0, 4), Opt(OptOps.UNROLL, 0, 4)],
         [Opt(OptOps.LOCAL, 0, 2), Opt(OptOps.UPCAST, 1, 4), Opt(OptOps.UNROLL, 0, 2), Opt(OptOps.UPCAST, 0, 4)],
         # [Opt(OptOps.GROUP, 0, 2)] # doesn't work because group_for_reduce dims become early locals (conflicting with TC)
       ], apply_tc=True, atol=atol, rtol=rtol)
 
   def test_padto_matmul(self):
-    if Device.DEFAULT in ["CUDA", "RHIP"]: self.skipTest("super slow on CUDA and RHIP because of the big grid dims")
+    if CI and Device.DEFAULT in ["CUDA", "AMD", "NV"]: self.skipTest("super slow on CUDA and AMD because of the big grid dims")
     N = 17 * 17
     Tensor.manual_seed(289)
     a = Tensor.rand(N, N)
     b = Tensor.rand(N, N)
     helper_linearizer_opt(a@b, [
       [Opt(OptOps.PADTO, 0, 32)],
       [Opt(OptOps.PADTO, 1, 32)],
       [Opt(OptOps.PADTO, 2, 32)],
       [Opt(OptOps.PADTO, 0, 32), Opt(OptOps.PADTO, 1, 32)],
       [Opt(OptOps.PADTO, 0, 32), Opt(OptOps.PADTO, 1, 32), Opt(OptOps.PADTO, 2, 32)],
       # can optimize further post PADTO
       [Opt(OptOps.PADTO, 0, 32), Opt(OptOps.PADTO, 1, 32), Opt(OptOps.UPCAST, 0, 2), Opt(OptOps.UPCAST, 1, 2),],
     ])
 
+  def test_padto_upcasted_not_ok(self):
+    N = 4
+    a = Tensor.rand(N, N)
+    b = Tensor.rand(N, N)
+    helper_linearizer_opt(a@b, [
+      [Opt(OptOps.UPCAST, 0, 0)],
+      [Opt(OptOps.UPCAST, 1, 0)],
+      [Opt(OptOps.UNROLL, 0, 0)],
+      [Opt(OptOps.PADTO, 0, 8)],
+      [Opt(OptOps.PADTO, 1, 8)],
+      [Opt(OptOps.PADTO, 2, 8)],
+    ])
+    with self.assertRaises(KernelOptError):
+      helper_linearizer_opt(a@b, [[Opt(OptOps.UPCAST, 0, 0), Opt(OptOps.PADTO, 2, 8)]])
+    with self.assertRaises(KernelOptError):
+      helper_linearizer_opt(a@b, [[Opt(OptOps.UPCAST, 1, 0), Opt(OptOps.PADTO, 2, 8)]])
+    with self.assertRaises(KernelOptError):
+      helper_linearizer_opt(a@b, [[Opt(OptOps.UNROLL, 0, 0), Opt(OptOps.PADTO, 2, 8)]])
+
   def test_padto_sum_ok(self):
     N = 18 * 18
     # NOTE: this setup prevents 17 * 17 contiguous merged into one dimension
     a = Tensor.rand(N, N).shrink(((0, 17), (0, 17))) * 100
 
     helper_linearizer_opt(a.sum(0), [
       [Opt(OptOps.PADTO, 0, 32)],
@@ -866,15 +950,15 @@
     a = (Tensor.empty(N, N).max(axis=0, keepdim=True) > 1).where(1, 0)
     helper_linearizer_opt(a.max(0), [
       [Opt(OptOps.PADTO, 0, 32)],
       [Opt(OptOps.PADTO, 0, 32), Opt(OptOps.UPCAST, 0, 8),],
     ])
 
   def test_color_shapes_with_local(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.has_shared:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.has_shared:
       self.skipTest("Only Compiled uses linearizer with locals and shared")
 
     N = 32
     Tensor.manual_seed(1552)
     a = Tensor.rand(N, N)
     b = Tensor.rand(N, N)
     r = a@b
@@ -936,43 +1020,43 @@
   def test_expand_idxs(self):
     uidx0 = Variable("_uidx0", 0, 6)
     uidx1 = Variable("_uidx1", 0, 1)
     idxs = (uidx0 // 5, uidx0 * 5, uidx1)
     assert expand_idxs(idxs) == (uidx0, NumNode(0), uidx1)
 
 class TestLinearizerUOptimize(unittest.TestCase):
-  @unittest.skipUnless(Device[Device.DEFAULT].compiler.compiler_opts.supports_float4, "device doesn't support float4")
+  @unittest.skipUnless(Device[Device.DEFAULT].renderer.supports_float4, "device doesn't support float4")
   def test_grouped_store_phis(self):
     x, y = Tensor.randn(64,64), Tensor.randn(64,64)
     out = x.matmul(y)
 
     k = Linearizer(*create_schedule([out.lazydata])[-1].ast)
     k.hand_coded_optimizations()
     k.linearize()
 
     # check that the float4 cast collapses
     store_vals = [u.vin[-1] for u in k.uops if u.uop is UOps.STORE]
     for val in store_vals:
       assert val.dtype == dtypes.float.vec(4) and val.uop is not UOps.CAST
 
-  @unittest.skipUnless(Device[Device.DEFAULT].compiler.compiler_opts.supports_float4, "device doesn't support float4")
+  @unittest.skipUnless(Device[Device.DEFAULT].renderer.supports_float4, "device doesn't support float4")
   def test_grouped_store_values(self):
     x = Tensor.randn((4,3,6,6)).realize()
     out = x.flip((0,1)).contiguous()
 
     k = Linearizer(*create_schedule([out.lazydata])[-1].ast)
     k.hand_coded_optimizations()
     k.linearize()
 
     store_val = [u.vin[-1] for u in k.uops if u.uop is UOps.STORE][0]
     assert store_val.dtype == dtypes.float.vec(4) and store_val.uop is not UOps.CAST
 
   def test_grouped_store_locals_and_globals(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.has_shared or \
-       not Device[Device.DEFAULT].compiler.compiler_opts.supports_float4:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.has_shared or \
+       not Device[Device.DEFAULT].renderer.supports_float4:
       self.skipTest("Only Compiled uses linearizer with locals, shared, and float4")
 
     x, y = Tensor.rand(128, 128), Tensor.rand(128, 128)
     out = x@y
 
     opts = [Opt(OptOps.LOCAL, 0, 4), Opt(OptOps.GROUPTOP, 0, 8),
             Opt(OptOps.UNROLL, 0, 4), Opt(OptOps.UPCAST, 0, 4), Opt(OptOps.UPCAST, 1, 2)] # upcast accs in both reduces
@@ -988,16 +1072,16 @@
     for store in local_stores+global_stores:
       assert store.vin[-1].dtype == dtypes.float.vec(2) and store.vin[-1].uop is not UOps.CAST
     # check the children's vins
     assert barrier.vin == tuple(local_stores)
     assert len([u for u in k.uops if u.uop is UOps.IF and u.vin[-1] == barrier]) == 1
 
   def test_grouped_store_local_only(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.has_shared or \
-       not Device[Device.DEFAULT].compiler.compiler_opts.supports_float4:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.has_shared or \
+       not Device[Device.DEFAULT].renderer.supports_float4:
       self.skipTest("Only Compiled uses linearizer with locals, shared, and float4")
 
     x, y = Tensor.rand(1,128), Tensor.rand(128, 128)
     r = (x@y).relu()
     k = Linearizer(*create_schedule([r.lazydata])[-1].ast)
     k.hand_coded_optimizations()
     k.linearize()
@@ -1008,15 +1092,15 @@
     assert stores[0].vin[-1].dtype == dtypes.float.vec(4)
     assert stores[0].vin[-1].uop is not UOps.CAST
 
     # the global store doesn't change
     assert stores[1].vin[-1].dtype == dtypes.float
 
   def test_skip_unmatching_upcasts(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.supports_float4:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.supports_float4:
       self.skipTest("Needs locals and float4")
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(240, 40, 1, 1), strides=(1, 240, 0, 0), offset=0, mask=None, contiguous=False),)))),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(240, 40, 1, 1), strides=(40, 1, 0, 0), offset=0, mask=None, contiguous=True),)))) # noqa: E501
     opts = [
         Opt(op=OptOps.UPCAST, axis=1, amt=4), Opt(op=OptOps.LOCAL, axis=0, amt=16),
         Opt(op=OptOps.LOCAL, axis=1, amt=2), Opt(op=OptOps.UPCAST, axis=3, amt=2)
     ]
 
@@ -1024,19 +1108,19 @@
     for opt in opts: k.apply_opt(opt)
     k.linearize()
 
     out = [u for u in k.uops if u.uop is UOps.STORE][0]
     assert out.vin[-1].uop is UOps.CAST and out.vin[-1].dtype == dtypes.float.vec(4)
 
   def test_skip_unmatching_upcasts_with_gep(self):
-    if not Device[Device.DEFAULT].compiler.compiler_opts.has_local or not Device[Device.DEFAULT].compiler.compiler_opts.supports_float4:
+    if not Device[Device.DEFAULT].renderer.has_local or not Device[Device.DEFAULT].renderer.supports_float4:
       self.skipTest("Needs locals and float4")
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(8, 32, 1, 1), strides=(1, 8, 0, 0), offset=0, mask=None, contiguous=False),)))),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(8, 32, 1, 1), strides=(32, 1, 0, 0), offset=0, mask=None, contiguous=True),)))) # noqa: E501
     opts = [Opt(op=OptOps.LOCAL, axis=1, amt=4), Opt(op=OptOps.UPCAST, axis=2, amt=2), Opt(op=OptOps.LOCAL, axis=1, amt=8),
-            Opt(op=OptOps.UPCAST, axis=2, amt=0), Opt(op=OptOps.UPCAST, axis=1, amt=4), Opt(op=OptOps.LOCAL, axis=0, amt=8),
+            Opt(op=OptOps.UPCAST, axis=1, amt=0), Opt(op=OptOps.UPCAST, axis=1, amt=4), Opt(op=OptOps.LOCAL, axis=0, amt=8),
             Opt(op=OptOps.UPCAST, axis=1, amt=0), Opt(op=OptOps.UPCAST, axis=0, amt=2)]
 
     k = Linearizer(ast)
     for opt in opts: k.apply_opt(opt)
     k.linearize()
 
     out = [u for u in k.uops if u.uop is UOps.STORE][0]
```

### Comparing `tinygrad_tools-0.8.1/test/test_linearizer_failures.py` & `tinygrad_tools-0.8.2/test/test_linearizer_failures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ruff: noqa: E501
 import unittest, random
 import numpy as np
 from tinygrad.codegen.kernel import KernelOptError
 from tinygrad.codegen.linearizer import Linearizer
-from tinygrad.features.search import Opt, OptOps
+from tinygrad.engine.search import Opt, OptOps
 from tinygrad import Device, dtypes, Tensor
 from tinygrad.helpers import CI
 from test.external.fuzz_linearizer import compare_linearizer
 from test.helpers import is_dtype_supported
 
 from tinygrad.ops import LazyOp, BinaryOps, UnaryOps, ReduceOps, TernaryOps, BufferOps, MemBuffer, ConstBuffer
 from tinygrad.shape.shapetracker import ShapeTracker
@@ -18,25 +18,25 @@
   if any(b.dtype == dtypes.bfloat16 for b in lin.membufs) and not is_dtype_supported(dtypes.bfloat16): return
 
   for opt in opts:
     try:
       lin.apply_opt(opt)
     except KernelOptError:
       # it's considered fixed if we invalidated the opts
-      assert Device.DEFAULT not in failed_platforms
+      assert Device.DEFAULT not in failed_platforms, f"unexpected success on {Device.DEFAULT}"
       return
 
   compare_result = compare_linearizer(lin, rtol=rtol, atol=atol)
   if compare_result[0] in ["PASS", "KernelOptError"]:
     # it's considered fixed if we invalidated the opts
     assert Device.DEFAULT not in failed_platforms, f"unexpected success on {Device.DEFAULT}"
   else:
     assert Device.DEFAULT in failed_platforms, f"failed on {Device.DEFAULT} with {compare_result[0]}"
 
-@unittest.skipIf(CI and Device.DEFAULT=="CUDA", "failed on CUDA CI")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "failed on CUDA CI")
 class TestLinearizerFailures(unittest.TestCase):
   def setUp(self):
     random.seed(42)
     np.random.seed(42)
     Tensor.manual_seed(42)
 
   def test_failure_1(self):
@@ -86,16 +86,16 @@
 
   def test_failure_10(self):
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(1, 1, 1024, 50257), strides=(0, 0, 0, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(1, 1, 1024, 50257), strides=(0, 0, 1, 1024), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=(3,)), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(1, 1, 1024, 1), strides=(0, 0, 1, 0), offset=0, mask=None, contiguous=True),))))), arg=None),), arg=MemBuffer(idx=0, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(1, 1, 1024, 1), strides=(0, 0, 1, 0), offset=0, mask=None, contiguous=True),))))
     helper_test_lin(Linearizer(ast), [], failed_platforms=[])
 
   def test_failure_11(self):
     src = LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=ReduceOps.SUM,
-                                               src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BinaryOps.MAX, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(0, 0, 0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.CMPLT, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BinaryOps.MAX, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=UnaryOps.SQRT, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(0,), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=4, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(1,), offset=0, mask=None, contiguous=True), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=5.425347222222222e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(0,), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(0,), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None)), arg=None),), arg=(dtypes.float, False)),), arg=None)), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=5, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(576, 9, 3, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None),),arg=(dtypes.float,False))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=6, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(576, 9, 3, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=7, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(576, 9, 3, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None)), arg=None),),
-                                               arg=(0, 2, 3)), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.SQRT, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=4, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=5.425347222222222e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None),), arg=(dtypes.float, False)),), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=2.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None)
+                                               src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BinaryOps.MAX, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(0, 0, 0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.CMPLT, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BinaryOps.MAX, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=UnaryOps.SQRT, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(0,), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=4, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(1,), offset=0, mask=None, contiguous=True), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=5.425347222222222e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(0,), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(64,), strides=(0,), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None)), arg=None),), arg=dtypes.float),), arg=None)), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 6, 6), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 3, 2, 2), strides=(2304, 36, 12, 2, 6, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=5, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(576, 9, 3, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None),),arg=dtypes.float)), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=6, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(576, 9, 3, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=7, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(512, 64, 3, 3, 2, 2), strides=(576, 9, 3, 1, 0, 0), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 3, 2, 3, 2), strides=(2304, 36, 12, 2, 4, 1), offset=0, mask=None, contiguous=False), View(shape=(512, 64, 6, 6), strides=(2304, 36, 6, 1), offset=0, mask=None, contiguous=True)))))), arg=None)), arg=None),),
+                                               arg=(0, 2, 3)), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.SQRT, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=4, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=5.425347222222222e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None),), arg=dtypes.float),), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=2.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None)
     ast = LazyOp(op=BufferOps.STORE, src=(src,), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 64, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),))))
     helper_test_lin(Linearizer(ast), [], failed_platforms=[])
 
   def test_failure_12(self):
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 1, 4, 1, 3, 4, 2, 6, 1, 3), strides=(0, 0, 0, 0, 0, 18, 0, 3, 0, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 1, 4, 1, 3, 4, 2, 6, 1, 3), strides=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 1, 4, 1, 3, 4, 2, 6, 1, 3), strides=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 1, 4, 1, 3, 4, 2, 6, 1, 3), strides=(0, 0, 0, 0, 0, 18, 0, 3, 0, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 1, 4, 1, 3, 4, 2, 6, 1, 3), strides=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 1, 4, 1, 3, 4, 2, 6, 1, 3), strides=(0, 0, 0, 0, 0, 0, 0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None),), arg=(0, 2, 4, 8)),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 1, 1, 1, 1, 4, 1, 6, 1, 3), strides=(0, 0, 0, 0, 0, 18, 0, 3, 0, 1), offset=0, mask=None, contiguous=True),))))
     opts = [Opt(op=OptOps.PADTO, axis=0, amt=32), Opt(op=OptOps.GROUP, axis=0, amt=4)]
     helper_test_lin(Linearizer(ast), opts, failed_platforms=[])
@@ -150,18 +150,19 @@
     helper_test_lin(Linearizer(ast), opts, failed_platforms=[])
 
   def test_failure_21(self):
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(45, 65), strides=(0, 0), offset=0, mask=None, contiguous=False),)))),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(45, 65), strides=(65, 1), offset=0, mask=None, contiguous=True),))))
     opts = [Opt(op=OptOps.PADTO, axis=0, amt=32)]
     helper_test_lin(Linearizer(ast), opts, failed_platforms=[])
 
+  @unittest.skipIf(CI and Device.DEFAULT=="METAL", "works fine on CI METAL")
   def test_failure_22(self):
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.000244140625, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.NEG, src=(LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=3, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=4, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=5, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=6, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=7, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(32, 96, 8, 16), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=8, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=9, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=10, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=11, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=12, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=13, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=14, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=15, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 8640, 180, 18, 1), offset=19, mask=((1, 2), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True))))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=16, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(2, 32, 48, 8, 16), strides=(0, 17280, 180, 18, 1), offset=19, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(2, 32, 48, 8, 16), strides=(0, 12288, 128, 16, 1), offset=0, mask=((0, 1), (0, 32), (0, 48), (0, 8), (0, 16)), contiguous=False), View(shape=(1536, 2, 128), strides=(128, 196608, 1), offset=0, mask=None, contiguous=False), View(shape=(32, 96, 8, 16), strides=(12288, 128, 16, 1), offset=0, mask=None, contiguous=True)))))), arg=None)), arg=None)), arg=None)), arg=None)), arg=None)), arg=None)), arg=None)), arg=None)), arg=None),), arg=(0, 2, 3)), LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=17, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=2.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None),), arg=None), LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=18, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.000244140625, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None)), arg=None), LazyOp(op=BinaryOps.DIV, src=(LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=18, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.000244140625, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1e-05, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None)), arg=None)), arg=None)), arg=None),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 96, 1, 1), strides=(0, 1, 0, 0), offset=0, mask=None, contiguous=True),))))
     opts = []
-    helper_test_lin(Linearizer(ast), opts, failed_platforms=[])
+    helper_test_lin(Linearizer(ast), opts, failed_platforms=["METAL", "HSA", "CUDA"])
 
   def test_failure_23(self):
     ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(240, 40, 1, 1), strides=(1, 240, 0, 0), offset=0, mask=None, contiguous=False),)))),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(240, 40, 1, 1), strides=(40, 1, 0, 0), offset=0, mask=None, contiguous=True),))))
     opts = [Opt(op=OptOps.UPCAST, axis=1, amt=4), Opt(op=OptOps.LOCAL, axis=0, amt=16), Opt(op=OptOps.LOCAL, axis=1, amt=2), Opt(op=OptOps.UPCAST, axis=3, amt=2)]
     helper_test_lin(Linearizer(ast), opts, failed_platforms=[])
 
   def test_failure_24(self):
@@ -212,22 +213,28 @@
     all_failing_opts = [
       [Opt(op=OptOps.PADTO, axis=0, amt=32), Opt(op=OptOps.UPCAST, axis=0, amt=4), Opt(op=OptOps.UPCAST, axis=0, amt=7), Opt(op=OptOps.UPCAST, axis=0, amt=0)],
     ]
     for opts in all_failing_opts:
       helper_test_lin(Linearizer(ast), opts, failed_platforms=["METAL", "HSA", "CUDA", "CLANG"]) # "GPU" is a compiler failure
 
   def test_failure_28(self):
-    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=TernaryOps.WHERE, src=(LazyOp(op=BinaryOps.CMPLT, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),)))),), arg=(dtypes.bfloat16, False)), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=230.0, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),)))),), arg=(dtypes.bfloat16, False)), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.004347826086956522, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.199374800625, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.99375e-07, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),)))),), arg=(dtypes.bfloat16, False)), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=230.0, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0012987012987012987, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=-0.19439062499999998, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.199375, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None)), arg=None),), arg=MemBuffer(idx=0, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=TernaryOps.WHERE, src=(LazyOp(op=BinaryOps.CMPLT, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),)))),), arg=dtypes.bfloat16), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=230.0, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),)))),), arg=dtypes.bfloat16), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.004347826086956522, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.199374800625, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.99375e-07, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BinaryOps.ADD, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.int, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),)))),), arg=dtypes.bfloat16), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=230.0, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.0012987012987012987, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=-0.19439062499999998, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=0.199375, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))), arg=None)), arg=None),), arg=MemBuffer(idx=0, dtype=dtypes.bfloat16, st=ShapeTracker(views=(View(shape=(1,), strides=(0,), offset=0, mask=None, contiguous=True),))))
     helper_test_lin(Linearizer(ast), opts=[], failed_platforms=[])
 
   def test_failure_29(self):
-    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(1, 128, 1, 64, 4, 58, 4, 58), strides=(0, 200704, 0, 3136, 0, 56, 0, 1), offset=-57, mask=((0, 1), (0, 128), (0, 1), (0, 64), (0, 4), (1, 57), (0, 4), (1, 57)), contiguous=False), View(shape=(128, 1, 64, 56, 56, 64, 3, 3), strides=(3444736, 0, 0, 232, 1, 53824, 13688, 59), offset=0, mask=None, contiguous=False))))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(128, 1, 64, 56, 56, 64, 3, 3), strides=(0, 0, 576, 0, 0, 9, 3, 1), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=(dtypes.float, False)),), arg=(7, 6, 5)),), arg=(dtypes.half, False)),), arg=MemBuffer(idx=0, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(128, 1, 64, 56, 56, 1, 1, 1), strides=(200704, 0, 3136, 56, 1, 0, 0, 0), offset=0, mask=None, contiguous=True),))))
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(1, 128, 1, 64, 4, 58, 4, 58), strides=(0, 200704, 0, 3136, 0, 56, 0, 1), offset=-57, mask=((0, 1), (0, 128), (0, 1), (0, 64), (0, 4), (1, 57), (0, 4), (1, 57)), contiguous=False), View(shape=(128, 1, 64, 56, 56, 64, 3, 3), strides=(3444736, 0, 0, 232, 1, 53824, 13688, 59), offset=0, mask=None, contiguous=False))))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(128, 1, 64, 56, 56, 64, 3, 3), strides=(0, 0, 576, 0, 0, 9, 3, 1), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=dtypes.float),), arg=(7, 6, 5)),), arg=dtypes.half),), arg=MemBuffer(idx=0, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(128, 1, 64, 56, 56, 1, 1, 1), strides=(200704, 0, 3136, 56, 1, 0, 0, 0), offset=0, mask=None, contiguous=True),))))
     opts = [Opt(op=OptOps.TC, axis=0, amt=1), Opt(op=OptOps.PADTO, axis=2, amt=32)]
     helper_test_lin(Linearizer(ast), opts, failed_platforms=[], atol=1.0)
 
   def test_failure_30(self):
-    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(256, 1, 12, 31, 31, 3, 2, 2), strides=(3072, 0, 0, 32, 1, 1024, 32, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(256, 1, 12, 31, 31, 3, 2, 2), strides=(0, 0, 12, 0, 0, 4, 2, 1), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=(dtypes.float, False)),), arg=(7, 6, 5)),), arg=(dtypes.half, False)),), arg=MemBuffer(idx=0, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(256, 1, 12, 31, 31, 1, 1, 1), strides=(11532, 0, 961, 31, 1, 0, 0, 0), offset=0, mask=None, contiguous=True),))))
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=UnaryOps.CAST, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(256, 1, 12, 31, 31, 3, 2, 2), strides=(3072, 0, 0, 32, 1, 1024, 32, 1), offset=0, mask=None, contiguous=False),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(256, 1, 12, 31, 31, 3, 2, 2), strides=(0, 0, 12, 0, 0, 4, 2, 1), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=dtypes.float),), arg=(7, 6, 5)),), arg=dtypes.half),), arg=MemBuffer(idx=0, dtype=dtypes.half, st=ShapeTracker(views=(View(shape=(256, 1, 12, 31, 31, 1, 1, 1), strides=(11532, 0, 961, 31, 1, 0, 0, 0), offset=0, mask=None, contiguous=True),))))
     opts = [Opt(op=OptOps.PADTO, axis=3, amt=32), Opt(op=OptOps.LOCAL, axis=3, amt=32), Opt(op=OptOps.UPCAST, axis=3, amt=4), Opt(op=OptOps.UPCAST, axis=3, amt=0)]
     helper_test_lin(Linearizer(ast), opts=opts, failed_platforms=[])
 
+  # from METAL=1 fuzz_linearizer command in test.yml
+  def test_failure_31(self):
+    ast = LazyOp(op=BufferOps.STORE, src=(LazyOp(op=ReduceOps.SUM, src=(LazyOp(op=UnaryOps.EXP2, src=(LazyOp(op=BinaryOps.MUL, src=(LazyOp(op=BinaryOps.SUB, src=(LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=1, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 16, 13, 13), strides=(0, 169, 13, 1), offset=0, mask=None, contiguous=True),)))), LazyOp(op=BufferOps.LOAD, src=(), arg=MemBuffer(idx=2, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 16, 13, 13), strides=(0, 13, 1, 0), offset=0, mask=None, contiguous=False),))))), arg=None), LazyOp(op=BufferOps.CONST, src=(), arg=ConstBuffer(val=1.4426950408889634, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 16, 13, 13), strides=(0, 0, 0, 0), offset=0, mask=None, contiguous=False),))))), arg=None),), arg=None),), arg=((3,), dtypes.float)),), arg=MemBuffer(idx=0, dtype=dtypes.float, st=ShapeTracker(views=(View(shape=(1, 16, 13, 1), strides=(0, 13, 1, 0), offset=0, mask=None, contiguous=True),))))
+    opts = [Opt(op=OptOps.UNROLL, axis=0, amt=0), Opt(op=OptOps.PADTO, axis=1, amt=32)]
+    helper_test_lin(Linearizer(ast), opts=opts, failed_platforms=[])
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_linearizer_overflows.py` & `tinygrad_tools-0.8.2/test/test_linearizer_overflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: E501
 import unittest
 from tinygrad import dtypes, Device
 from tinygrad.helpers import CI
 from tinygrad.codegen.linearizer import Linearizer
-from tinygrad.features.search import Opt, OptOps
-from tinygrad.features.search import time_linearizer, bufs_from_lin
+from tinygrad.engine.search import Opt, OptOps
+from tinygrad.engine.search import time_linearizer, bufs_from_lin
 
 # stuff needed to unpack a kernel
 from tinygrad.ops import LazyOp, BinaryOps, UnaryOps, ReduceOps, BufferOps, MemBuffer, ConstBuffer
 from tinygrad.shape.shapetracker import ShapeTracker
 from tinygrad.shape.view import View
 
 def _test_overflow(ast, opts):
```

### Comparing `tinygrad_tools-0.8.1/test/test_masked_st.py` & `tinygrad_tools-0.8.2/test/test_masked_st.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_method_cache.py` & `tinygrad_tools-0.8.2/test/test_method_cache.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_multitensor.py` & `tinygrad_tools-0.8.2/test/test_multitensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import unittest, functools, random
 from typing import List
 from tinygrad import Tensor, Device, nn, GlobalCounters, TinyJit, dtypes
-from tinygrad.device import BufferCopy, CompiledRunner
 from tinygrad.ops import LoadOps, ReduceOps
 from tinygrad.helpers import CI, prod, Context
 from tinygrad.nn.state import get_parameters, get_state_dict
 from tinygrad.engine.schedule import create_schedule
-from tinygrad.engine.realize import lower_schedule
-from tinygrad.features.multi import all_reduce, MultiLazyBuffer
+from tinygrad.engine.realize import lower_schedule, BufferCopy, CompiledRunner
+from tinygrad.multi import all_reduce, MultiLazyBuffer
 from random import randint
 import numpy as np
 from hypothesis import given, strategies as strat, settings
 from test.helpers import is_dtype_supported
 
 settings.register_profile("my_profile", max_examples=200, deadline=None)
 settings.load_profile("my_profile")
@@ -52,15 +51,15 @@
   def test_shard_no_recompile(self):
     X = Tensor.ones(256).contiguous().realize()
     X.shard_((d0, d1), 0)
     out = (X + X)
     sched = create_schedule(out.lazydata.lbs)
     names = []
     for si, ei in zip(sched[:], lower_schedule(sched)):
-      if isinstance(ei.prg, CompiledRunner): names.append(ei.prg.name)
+      if isinstance(ei.prg, CompiledRunner): names.append(ei.prg.p.name)
       ei.run()
     assert names[-2] == names[-1], "function was relinearized"
 
   def test_sharded_memory(self):
     # Buffer may be stuck in track_cross_buffer
     for x in (d_zero, d0, d1, d2, d3): Device[x].synchronize()
     mem_base = GlobalCounters.mem_used
@@ -145,14 +144,15 @@
       np.testing.assert_almost_equal(a.numpy(), b.numpy(), decimal=5)
 
   def test_allreduce_ring(self):
     with Context(RING=2):
       a,b = _test_allreduce(Tensor.rand(256, 256))
       np.testing.assert_almost_equal(a.numpy(), b.numpy(), decimal=5)
 
+  @unittest.skipIf(Device.DEFAULT in {"NV", "AMD"}, "not supported in HCQ")
   def test_copy_jit(self):
     @TinyJit
     def copy_tensor(x:Tensor): return (x.to(f"{x.device.split(':')[0]}:1") + 1)
     for _ in range(5):
       t = Tensor.rand(256).realize()
       x = copy_tensor(t)
       np.testing.assert_equal((t+1).numpy(), x.numpy())
@@ -232,24 +232,25 @@
     conv = nn.Conv2d(3, 16, 3)
     for p in get_parameters(conv): p.shard_((d0, d1))
     fake_image = Tensor.rand((2, 3, 32, 32)).shard((d0, d1), axis=0)
     out = conv(fake_image)
     out.numpy()
 
   def test_backprop_conv(self):
-    conv = nn.Conv2d(3, 16, 3)
-    for p in get_parameters(conv): p.shard_((d0, d1))
-    optim = nn.optim.Adam(get_parameters(conv))
-    fake_image = Tensor.rand((2, 3, 32, 32)).shard((d0, d1), axis=0)
-    out = conv(fake_image)
-    optim.zero_grad()
-    out.mean().backward()
-    #for p in get_parameters(conv): p.grad.realize()
-    optim.step()
-    out.numpy()
+    with Tensor.train():
+      conv = nn.Conv2d(3, 16, 3)
+      for p in get_parameters(conv): p.shard_((d0, d1))
+      optim = nn.optim.Adam(get_parameters(conv))
+      fake_image = Tensor.rand((2, 3, 32, 32)).shard((d0, d1), axis=0)
+      out = conv(fake_image)
+      optim.zero_grad()
+      out.mean().backward()
+      #for p in get_parameters(conv): p.grad.realize()
+      optim.step()
+      out.numpy()
 
   def test_lr_scheduler_OneCycleLR(self):
     from extra.lr_scheduler import OneCycleLR
     conv = nn.Conv2d(3, 16, 3)
     for p in get_parameters(conv): p.shard_((d0, d1))
     optim = nn.optim.SGD(get_parameters(conv))
     lr_sched = OneCycleLR(optim, max_lr=0.1, pct_start=0.1, div_factor=100, final_div_factor=0.1, total_steps=10)
@@ -288,14 +289,15 @@
 
     # if x is being duplicated, then the operations remain inside each GPU
     # which is the common case
     x_sharded = x.shard((d0, d1), axis=None).realize()
     y_shard = layer_norm_sharded(x_sharded).realize()
     np.testing.assert_allclose(y.numpy(), y_shard.numpy(), atol=1e-6, rtol=1e-6)
 
+  @unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
   def test_data_parallel_resnet(self):
     import sys, pathlib
     sys.path.append((pathlib.Path(__file__).parent.parent / "extra" / "models").as_posix())
     from resnet import ResNet18
 
     fake_image = Tensor.rand((2, 3, 224, 224))
     fake_image_sharded = fake_image.shard((d0, d1), axis=0)
@@ -306,14 +308,15 @@
     GlobalCounters.reset()
     shard_output = m(fake_image_sharded).log_softmax().realize()
     assert shard_output.lazydata.lbs[0].shape == (1, 1000)
     assert shard_output.lazydata.lbs[1].shape == (1, 1000)
     shard_output_np = shard_output.numpy()
     np.testing.assert_allclose(real_output, shard_output_np, atol=1e-6, rtol=1e-6)
 
+  @unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
   def test_data_parallel_resnet_train_step(self):
     import sys, pathlib
     sys.path.append((pathlib.Path(__file__).parent.parent / "extra" / "models").as_posix())
     from resnet import ResNet18
     from tinygrad.nn.optim import LARS
 
     fake_image = Tensor.rand((2, 3, 224, 224))
@@ -624,37 +627,38 @@
       added.append(x[bound[0]:bound[1]] + a)
 
     output = added[0].cat(*added[1:])
     expected = np.arange(64).reshape((8,8)) + np.array([[0,0,1,1,2,2,3,3] for _ in range(8)]).T
     np.testing.assert_allclose(output.numpy(), expected)
 
   def test_unsynced_backprop_conv_bn(self):
-    from extra.lr_scheduler import OneCycleLR
+    with Tensor.train():
+      from extra.lr_scheduler import OneCycleLR
 
-    convs = [nn.Conv2d(3, 16, 3), nn.Conv2d(3, 16, 3)]
-    bns = [nn.BatchNorm2d(16), nn.BatchNorm2d(16)]
+      convs = [nn.Conv2d(3, 16, 3), nn.Conv2d(3, 16, 3)]
+      bns = [nn.BatchNorm2d(16), nn.BatchNorm2d(16)]
 
-    for p in get_parameters(convs + bns):
-      p.shard_((d1, d2))
-    optim = nn.optim.Adam(get_parameters(convs + bns))
-    lr_sched = OneCycleLR(optim, max_lr=0.1, pct_start=0.1, div_factor=100, final_div_factor=0.1, total_steps=10)
-    lr_sched.step()
-
-    fake_image = Tensor.rand((8, 3, 32, 32)).shard((d1, d2), axis=0)
-
-    f1 = fake_image.shrink(((0, 4), None, None, None))
-    f2 = fake_image.shrink(((4, 8), None, None, None))
-
-    out1 = bns[0](convs[0](f1))
-    out2 = bns[1](convs[1](f2))
-    out = out1.cat(out2)
-    optim.zero_grad()
-    out.mean().backward()
-    optim.step()
-    out.numpy()
+      for p in get_parameters(convs + bns):
+        p.shard_((d1, d2))
+      optim = nn.optim.Adam(get_parameters(convs + bns))
+      lr_sched = OneCycleLR(optim, max_lr=0.1, pct_start=0.1, div_factor=100, final_div_factor=0.1, total_steps=10)
+      lr_sched.step()
+
+      fake_image = Tensor.rand((8, 3, 32, 32)).shard((d1, d2), axis=0)
+
+      f1 = fake_image.shrink(((0, 4), None, None, None))
+      f2 = fake_image.shrink(((4, 8), None, None, None))
+
+      out1 = bns[0](convs[0](f1))
+      out2 = bns[1](convs[1](f2))
+      out = out1.cat(out2)
+      optim.zero_grad()
+      out.mean().backward()
+      optim.step()
+      out.numpy()
 
   def test_unsynced_backprop_standalone_bn(self):
     from extra.lr_scheduler import OneCycleLR
     GPUS = (d1, d2)
 
     class BatchNorm:
       def __init__(self, num_features):
```

### Comparing `tinygrad_tools-0.8.1/test/test_net_speed.py` & `tinygrad_tools-0.8.2/test/test_net_speed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import time
 import unittest
 import torch
 from tinygrad import Tensor, Device
 from tinygrad.helpers import Profiling, CI
 
-@unittest.skipIf(CI and Device.DEFAULT == "CUDA", "slow")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
 class TestConvSpeed(unittest.TestCase):
 
   def test_mnist(self):
     # https://keras.io/examples/vision/mnist_convnet/
     conv = 3
     inter_chan, out_chan = 32, 64
```

### Comparing `tinygrad_tools-0.8.1/test/test_nn.py` & `tinygrad_tools-0.8.2/test/test_nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import unittest
 import numpy as np
 import torch
 from tinygrad import Tensor, Device, TinyJit
 from tinygrad.helpers import CI, Context
 from tinygrad.ops import BufferOps
 from tinygrad.nn import BatchNorm2d, Conv1d,ConvTranspose1d, Conv2d,ConvTranspose2d, Linear, GroupNorm, LayerNorm,LayerNorm2d, Embedding, InstanceNorm
+from tinygrad.nn.state import load_state_dict
 from tinygrad.engine.schedule import create_schedule
 from tinygrad.engine.realize import run_schedule
 
-@unittest.skipIf(CI and Device.DEFAULT == "CUDA", "slow")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
 class TestNN(unittest.TestCase):
   @unittest.skipIf(Device.DEFAULT == "WEBGPU", "no int64 on WebGPU")
   def test_sparse_cat_cross_entropy(self):
     # create in tinygrad
     input = Tensor.randn(5, 5)
     target = Tensor([0, 0, 0, 1, 2])  # torch doesn't support target=-1
     torch_input = torch.tensor(input.numpy())
@@ -177,15 +178,14 @@
     gx = x.grad.realize()
 
     torch_z.mean().backward()
     np.testing.assert_allclose(gw.numpy(), torch_layer.weight.grad.numpy(), atol=5e-4, rtol=1e-5)
     np.testing.assert_allclose(gb.numpy(), torch_layer.bias.grad.numpy(), atol=5e-4, rtol=1e-5)
     np.testing.assert_allclose(gx.numpy(), torch_x.grad.numpy(), atol=5e-4, rtol=1e-5)
 
-
   @unittest.skipIf(CI and Device.DEFAULT == "WEBGPU", "runs out of memory in CI")
   def test_conv_transpose1d(self):
     BS, C1, W = 4, 16, 224//4
     C2, K, S, P = 64, 7, 2, 1
 
     # create in tinygrad
     layer = ConvTranspose1d(C1, C2, kernel_size=K, stride=S, padding=P)
@@ -368,10 +368,39 @@
                 [4, 5, 6],
                 [7, 8, 9]])
     result = layer(b)
     schedule = create_schedule([result.lazydata])
     self.assertEqual(1, len([item for item in schedule if item.ast[0].op is BufferOps.STORE]), "second run realizes embedding only")
     run_schedule(schedule)
 
+  def test_load_state_dict(self):
+    layer = Conv2d(3, 5, kernel_size=3)
+
+    state_dict = {
+      'weight': Tensor.randn(5, 3, 3, 3),
+      'bias': Tensor.randn(5),
+    }
+    load_state_dict(layer, state_dict)
+
+    np.testing.assert_allclose(layer.weight.numpy(), state_dict['weight'].numpy())
+    np.testing.assert_allclose(layer.bias.numpy(), state_dict['bias'].numpy())
+
+  @unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL"}, "no GPU CI")
+  def test_load_state_dict_sharded(self):
+    devices = (f"{Device.DEFAULT}:1", f"{Device.DEFAULT}:2")
+
+    layer = Conv2d(3, 5, kernel_size=3)
+    layer.weight.shard_(devices, -1)
+    layer.bias.shard_(devices, None)
+    state_dict = {
+      'weight': Tensor.randn(5, 3, 3, 3).shard(devices, -1),
+      'bias': Tensor.randn(5).shard(devices, None),
+    }
+    load_state_dict(layer, state_dict)
+
+    self.assertEqual(layer.weight.device, devices)
+    self.assertEqual(layer.bias.device, devices)
+    np.testing.assert_allclose(layer.weight.numpy(), state_dict['weight'].numpy())
+    np.testing.assert_allclose(layer.bias.numpy(), state_dict['bias'].numpy())
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_ops.py` & `tinygrad_tools-0.8.2/test/test_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     ts = [torch.tensor(data, requires_grad=(not forward_only)) for data in np_data]
   tst = [Tensor(x.detach().numpy(), requires_grad=(not forward_only and not FORWARD_ONLY)) for x in ts]
   return ts, tst
 
 class TestOps(unittest.TestCase):
 
   def helper_test_exception(self, shps, torch_fxn, tinygrad_fxn, expected, exact=False, vals=None, low=-1.5, high=1.5):
-    if getenv("CUDACPU"): self.skipTest('helper_test_exception fails in CUDACPU')
+    if getenv("CUDACPU") or (getenv("MOCKGPU") and Device.DEFAULT == "NV"): self.skipTest('helper_test_exception fails in CUDACPU')
     ts, tst = prepare_test_op(low, high, shps, vals)
     with self.assertRaises(expected) as torch_cm:
       torch_fxn(*ts)
     with self.assertRaises(expected) as tinygrad_cm:
       tinygrad_fxn(*tst)
     if exact: self.assertEqual(str(torch_cm.exception), str(tinygrad_cm.exception))
     if not CI: print("\ntesting %40r   torch/tinygrad exception: %s / %s" % (shps, torch_cm.exception, tinygrad_cm.exception), end="")
@@ -433,14 +433,36 @@
   def test_xor(self):
     tor = torch.tensor([[1,-8,1],[32,1,6]], dtype=torch.int)
     ten = Tensor([[1,-8,1],[32,1,6]], dtype=dtypes.int32)
     helper_test_op([], lambda: tor^tor, lambda: ten^ten, forward_only=True)
     helper_test_op([], lambda: tor^0x1337, lambda: ten^0x1337, forward_only=True)
     helper_test_op([], lambda: 0x1337^tor, lambda: 0x1337^ten, forward_only=True)
 
+  def test_lshift(self):
+    data = [[0,1,2],[1<<8,1<<16,1<<31-1]]
+    tor = torch.tensor(data, dtype=torch.int)
+    ten = Tensor(data, dtype=dtypes.uint32)
+    # cast to int32 because torch does not support uint32
+    helper_test_op([], lambda: tor << 0, lambda: (ten << 0).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor << 2, lambda: (ten << 2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor << 31, lambda: (ten << 31).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.__lshift__(2), lambda: ten.__lshift__(2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.bitwise_left_shift(2), lambda: ten.lshift(2).cast(dtypes.int32), forward_only=True)
+
+  def test_rshift(self):
+    data = [[0,1,2],[1<<8,1<<16,1<<31-1]]
+    tor = torch.tensor(data, dtype=torch.int)
+    ten = Tensor(data, dtype=dtypes.uint32)
+    # cast to int32 because torch does not support uint32
+    helper_test_op([], lambda: tor >> 0, lambda: (ten >> 0).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor >> 2, lambda: (ten >> 2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor >> 31, lambda: (ten >> 31).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.__rshift__(2), lambda: ten.__rshift__(2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.bitwise_right_shift(2), lambda: ten.rshift(2).cast(dtypes.int32), forward_only=True)
+
   def test_sin(self):
     helper_test_op([(45,65)], lambda x: x.sin())
     helper_test_op([()], lambda x: x.sin())
   def test_cos(self):
     helper_test_op([(45,65)], lambda x: x.cos())
     helper_test_op([()], lambda x: x.cos())
   def test_tan(self):
@@ -461,14 +483,16 @@
     for val in range(1, 5):
       helper_test_op([(45,65)], lambda x: torch.nn.functional.celu(x,val), lambda x: x.celu(val))
       helper_test_op([()], lambda x: torch.nn.functional.celu(x,val), lambda x: x.celu(val))
 
   def test_abs(self):
     helper_test_op([(45,65)], torch.abs, Tensor.abs)
     helper_test_op([()], torch.abs, Tensor.abs)
+  def test_abs_exact(self):
+    helper_test_op(None, torch.abs, Tensor.abs, vals=[[-1.,0,1]])
 
   def test_log(self):
     helper_test_op([(45,65)], torch.log, Tensor.log)
     helper_test_op([()], torch.log, Tensor.log)
   def test_log2(self):
     helper_test_op([(45,65)], torch.log2, Tensor.log2)
     helper_test_op([()], torch.log2, Tensor.log2)
@@ -479,17 +503,22 @@
   def test_exp2(self):
     helper_test_op([(45,65)], torch.exp2, Tensor.exp2)
     helper_test_op([()], torch.exp2, Tensor.exp2)
 
   def test_sign(self):
     helper_test_op([(45,65)], torch.sign, Tensor.sign)
     helper_test_op([()], torch.sign, Tensor.sign)
+  def test_sign_exact(self):
+    helper_test_op(None, torch.sign, Tensor.sign, vals=[[-1.,0,1]])
+
   def test_softsign(self):
     helper_test_op([(45,65)], torch.nn.functional.softsign, Tensor.softsign)
     helper_test_op([()], torch.nn.functional.softsign, Tensor.softsign)
+  def test_softsign_exact(self):
+    helper_test_op(None, torch.nn.functional.softsign, Tensor.softsign, vals=[[-1.,0,1]])
 
   def test_sigmoid(self):
     helper_test_op([(45,65)], torch.sigmoid, Tensor.sigmoid)
     helper_test_op([(45,65)], torch.sigmoid, Tensor.sigmoid, low=300, high=303)
     helper_test_op([(45,65)], torch.sigmoid, Tensor.sigmoid, low=-300, high=-297)
     helper_test_op([()], torch.sigmoid, Tensor.sigmoid)
   def test_softplus(self):
@@ -707,14 +736,16 @@
 
   def test_sum_simple(self):
     helper_test_op(None, lambda x: x.sum(), vals=[[1.,1.]])
   def test_sum_full(self):
     helper_test_op([(16384)], lambda x: x.sum())
   def test_sum_relu(self):
     helper_test_op([(3,4,5)], lambda x: x.relu().sum().relu())
+  def test_sum_tiny(self):
+    helper_test_op([(4,2,2)], lambda x: x.sum(axis=(0,2)))
   def test_sum(self):
     helper_test_op([(45,3)], lambda x: x.sum())
     helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=3))
     helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(1,3)))
     helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(0,2)))
     helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(1,2)))
     helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=1))
@@ -806,14 +837,22 @@
     helper_test_op([()], torch.nn.LogSoftmax(dim=0), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
     helper_test_op([()], torch.nn.LogSoftmax(dim=-1), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
   def test_log_softmax_other_axis(self):
     helper_test_op([(10,10,10)], lambda x: x.log_softmax(0), atol=1e-7, grad_atol=1e-7)
     helper_test_op([(10,10,10)], lambda x: x.log_softmax(1), atol=1e-7, grad_atol=1e-7)
     helper_test_op([(10,10,10)], lambda x: x.log_softmax(2), atol=1e-7, grad_atol=1e-7)
 
+  def test_logsumexp(self):
+    helper_test_op([(45,65)], lambda x: torch.logsumexp(x, dim=0), lambda x: x.logsumexp(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45,65)], lambda x: torch.logsumexp(x, dim=0, keepdim=True), lambda x: x.logsumexp(0, True), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45,65)], lambda x: torch.logsumexp(x, dim=1), lambda x: x.logsumexp(1), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45)], lambda x: torch.logsumexp(x, dim=0), lambda x: x.logsumexp(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([()], lambda x: torch.logsumexp(x, dim=0), lambda x: x.logsumexp(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([()], lambda x: torch.logsumexp(x, dim=-1), lambda x: x.logsumexp(-1), atol=1e-7, grad_atol=1e-7)
+
   def test_sinh(self):
     helper_test_op([(45,65)], lambda x: x.sinh(), grad_atol=1e-6)
     # TODO: backward nan instead of inf
     helper_test_op([(45,65)], lambda x: x.sinh(), grad_atol=1e-6, low=-300, high=-297, forward_only=True)
     helper_test_op([(45,65)], lambda x: x.sinh(), grad_atol=1e-6, low=300, high=303, forward_only=True)
   def test_cosh(self):
     helper_test_op([(45,65)], lambda x: x.cosh(), grad_atol=1e-6)
@@ -1457,15 +1496,15 @@
   def test_maxpool2d_bigger_stride_dilation(self):
     for stride, dilation in zip([(2,3), (3,2), 2, 3, 4], [(3,2), (2,3), 2, 3, 6]):
       with self.subTest(stride=stride):
         helper_test_op([(32,2,110,28)],
           lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(2,2), stride=stride, dilation=dilation),
           lambda x: Tensor.max_pool2d(x, kernel_size=(2,2), stride=stride, dilation=dilation))
 
-  @unittest.skipIf(Device.DEFAULT == "CUDA", "CUDA fails on this")
+  @unittest.skipIf( Device.DEFAULT in {"CUDA", "NV"}, "CUDA fails on this")
   def test_maxpool2d_unit_stride(self):
     helper_test_op([(8, 2, 17, 14)],
       lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(5,5), stride=1),
       lambda x: Tensor.max_pool2d(x, kernel_size=(5,5), stride=1))
 
   def test_maxpool2d_smaller_stride(self):
     for stride in [(2,3), (3,2), 2, 3]:
```

### Comparing `tinygrad_tools-0.8.1/test/test_optim.py` & `tinygrad_tools-0.8.2/test/test_optim.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,16 +37,20 @@
   for _ in range(steps):
     out = net.forward()
     optim.zero_grad()
     out.backward()
     optim.step()
   return net.x.detach().numpy(), net.W.detach().numpy()
 
-@unittest.skipIf(CI and Device.DEFAULT == "CUDA", "slow")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
 class TestOptim(unittest.TestCase):
+  def setUp(self):
+    self.old_training = Tensor.training
+    Tensor.training = True
+  def tearDown(self): Tensor.training = self.old_training
 
   def _test_optim(self, tinygrad_optim, torch_optim, steps, opts, atol, rtol):
     for x,y in zip(step(Tensor, tinygrad_optim, steps, **opts),
                    step(torch.tensor, torch_optim, steps, **opts)):
       np.testing.assert_allclose(x, y, atol=atol, rtol=rtol)
 
   def _test_sgd(self, steps, opts, atol, rtol): self._test_optim(SGD, torch.optim.SGD, steps, opts, atol, rtol)
@@ -111,9 +115,21 @@
     old_default_float, dtypes.default_float = dtypes.default_float, dtypes.half
     # weight update would overflow without upcasting
     self._test_sgd(10, {'lr': 1e10}, 1e-6, 3e-4)
     self._test_adam(1, {'lr': 1e10}, 1e-4, 1e-4)
     self._test_adamw(1, {'lr': 1e10}, 1e-4, 1e-4)
     dtypes.default_float = old_default_float
 
+  def test_assert_tensor_train(self):
+    t = Tensor.ones((1,1), requires_grad=True)
+    optimizer = Adam([t])
+    optimizer.zero_grad()
+    old_state = Tensor.training
+    t.sum().backward()
+    Tensor.training = False
+    self.assertRaises(AssertionError, optimizer.step)
+    Tensor.training = True
+    optimizer.step()
+    Tensor.training = old_state
+
 if __name__ == '__main__':
-  unittest.main()
+  unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_pattern_matcher.py` & `tinygrad_tools-0.8.2/test/test_pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_pickle.py` & `tinygrad_tools-0.8.2/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_randomness.py` & `tinygrad_tools-0.8.2/test/test_randomness.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     equal_distribution(lambda *x: Tensor.rand(*x, dtype=dtypes.bfloat16).float(), torch.rand, lambda x: np.random.rand(*x), shape=(2, N, N))
 
   def test_randn(self):
     self.assertTrue(normal_test(Tensor.randn))
     self.assertTrue(equal_distribution(Tensor.randn, torch.randn, lambda x: np.random.randn(*x)))
 
   @given(strat.sampled_from([dtypes.float, dtypes.float16, dtypes.bfloat16]))
-  @unittest.skipIf(Device.DEFAULT in ["HSA", "RHIP"], "bfloat16 local buffer broken in HSA")
+  @unittest.skipIf(Device.DEFAULT in ["HSA", "AMD"], "bfloat16 local buffer broken in HSA")
   def test_randn_finite(self, default_float):
     if not is_dtype_supported(default_float): return
     old_default_float = dtypes.default_float
     # low precision can result in inf from randn
     dtypes.default_float = default_float
     t = Tensor.randn(1024, 1024)
     mx = t.max().numpy().item()
```

### Comparing `tinygrad_tools-0.8.1/test/test_sample.py` & `tinygrad_tools-0.8.2/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_schedule.py` & `tinygrad_tools-0.8.2/test/test_schedule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 # this will be the new test_ops for the next level
 # schedule confirms the right things are capable of fusing
 # NOTE: this has overlap with external_test_opt.py
 
 import unittest
+import numpy as np
 from typing import List, Optional, Union
+from tinygrad.engine.realize import run_schedule
 from tinygrad.tensor import Tensor
 from tinygrad.ops import BinaryOps, LoadOps, ReduceOps
-from tinygrad.helpers import DEBUG, GRAPH, flatten
+from tinygrad.helpers import DEBUG, flatten
 from tinygrad.codegen.linearizer import Linearizer
-from tinygrad.features.graph import print_tree, realized_lazybuffer
+from tinygrad.engine.graph import print_tree
 from tinygrad.engine.schedule import create_schedule
 from tinygrad import nn, dtypes
 from test.helpers import is_dtype_supported
 
 def check_schedule(t:Union[Tensor, List[Tensor]], allowed:int, to_prerealize:Optional[List[Tensor]]=None, filter_loadops=True):
   if isinstance(t, Tensor): t = [t]
   seen = set()
   if to_prerealize:
     for pre in to_prerealize:
       for s in pre.schedule(seen=seen.copy()):
         for i,out in enumerate(s.outputs):
-          if GRAPH: realized_lazybuffer(out, 0)
           seen.add(out)
   sched = create_schedule(flatten([r.lazydata.lbs for r in t]), seen)
-  if GRAPH:
-    for i,s in enumerate(sched):
-      for out in s.outputs: realized_lazybuffer(out, i+1)
   if filter_loadops: sched = [s for s in sched if s.ast[0].op not in LoadOps]
   if len(sched) != allowed: print(f"SCHEDULE ISSUE, expecting {allowed} got {len(sched)}")
   if len(sched) != allowed or DEBUG >= 3:
     for i, s in enumerate(sched):
       print("kernel", i+1)
       for op in s.ast: print_tree(op)
   assert len(sched) == allowed, f"{len(sched)} != {allowed}"
@@ -186,33 +184,64 @@
   def test_fold_batchnorm(self):
     with Tensor.train():
       img = Tensor.empty(1,32,4,4)
       bn = nn.BatchNorm2d(32, track_running_stats=False)
       out = bn(img)
       check_schedule(out, 3)
 
+  def test_fold_conv_batchnorm_notrain(self):
+    with Tensor.train(False):
+      img = Tensor.empty(1,3,8,8)
+      c1 = nn.Conv2d(3,32,3)
+      bn = nn.BatchNorm2d(32, track_running_stats=False)
+      out = bn(c1(img)).relu()
+      check_schedule(out, 1, [c1.weight, c1.bias])
+
   def test_fold_conv_batchnorm(self):
     with Tensor.train():
       img = Tensor.empty(1,3,8,8)
       c1 = nn.Conv2d(3,32,3)
       bn = nn.BatchNorm2d(32, track_running_stats=False)
       out = bn(c1(img)).relu()
       check_schedule(out, 4, [c1.weight, c1.bias])
 
-  def test_fold_conv_batchnorm_sgd(self):
+  def test_fold_conv_batchnorm_optim(self):
+    # this is too high
+    for optim, cnt in [(nn.optim.Adam, 19), (nn.optim.SGD, 17)]:
+      with self.subTest(optim=optim.__name__):
+        with Tensor.train():
+          img = Tensor.ones(1,3,4,4)
+          c1 = nn.Conv2d(3,32,3)
+          bn = nn.BatchNorm2d(32, track_running_stats=False)
+          opt = optim(nn.state.get_parameters([c1, bn]))
+          img_bn = bn(c1(img)).elu().sum()
+          opt.zero_grad()
+          img_bn.backward()
+          check_schedule(opt.schedule_step(), cnt)
+
+  def test_fold_conv_relu_backward(self):
+    c1 = nn.Conv2d(3,16,3, bias=False)
+    c1.weight.requires_grad = True
+
+    # run
+    img = Tensor.rand(2,3,64,64, requires_grad=True)
+    c1(img).relu().mean().backward()
+    # TODO: this should be 4, not 5
+    # img.grad is requiring two reduces
+    check_schedule([img.grad, c1.weight.grad], 5)
+
+  def test_fold_batchnorm_backward(self):
     with Tensor.train():
-      img = Tensor.ones(1,3,4,4)
-      c1 = nn.Conv2d(3,32,3)
-      bn = nn.BatchNorm2d(32, track_running_stats=False)
-      opt = nn.optim.SGD(nn.state.get_parameters([c1, bn]))
-      img_bn = bn(c1(img)).elu().sum()
-      opt.zero_grad()
-      img_bn.backward()
-      # this is too high
-      check_schedule(opt.schedule_step(), 17)
+      x = Tensor.empty((2, 16, 8, 8)).contiguous()
+      bn = nn.BatchNorm2d(16)
+      bn.weight.requires_grad = bn.bias.requires_grad = x.requires_grad = True
+      fw = bn(x).contiguous_backward().relu().contiguous()
+      fw.sum().backward()
+      # TODO: this is too many
+      check_schedule([x.grad, bn.weight.grad, bn.bias.grad, fw], 10)
 
   def test_fold_conv_relu(self):
     c1 = nn.Conv2d(3,16,3)
 
     # run
     img = Tensor.ones(2,3,64,64)
     out = c1(img).relu()
@@ -573,38 +602,39 @@
 
   def test_scaled_dot_product_attention_causal_fusion(self):
     x, y, z, m = (Tensor.empty(32, 8, 16, 16) for _ in range(4))
     out = Tensor.scaled_dot_product_attention(x, y, z, attn_mask=m, is_causal=True)
     check_schedule(out, 7)
 
   def test_adam_step_fusion(self):
-    x = Tensor.empty(4, 64, 768)
-    layer = nn.Linear(768, 768*4)
-    opt = nn.optim.Adam(nn.state.get_parameters(layer), lr=1e-4)
-    layer(x).relu().sum().backward()
-    check_schedule(opt.schedule_step(), 12)
+    with Tensor.train():
+      x = Tensor.empty(4, 64, 768)
+      layer = nn.Linear(768, 768*4)
+      opt = nn.optim.Adam(nn.state.get_parameters(layer), lr=1e-4)
+      layer(x).relu().sum().backward()
+      check_schedule(opt.schedule_step(), 11)
 
   def test_adam_conv_fuse(self):
     with Tensor.train():
       img = Tensor.empty(2,3,4,4)
       c1 = nn.Conv2d(3,32,3)
       opt = nn.optim.Adam(nn.state.get_parameters(c1), lr=1e-4)
       opt.zero_grad()
       c1(img).relu().sum().backward()
-      check_schedule(opt.schedule_step(), 12)
+      check_schedule(opt.schedule_step(), 11)
 
   def test_adam_2convs_fuse(self):
     with Tensor.train():
       img = Tensor.empty(2,3,4,4)
       c1 = nn.Conv2d(3,16,3,bias=False)
       c2 = nn.Conv2d(16,32,3,bias=False)
       opt = nn.optim.Adam(nn.state.get_parameters([c1, c2]), lr=1e-4)
       opt.zero_grad()
       c2(c1(img).relu()).relu().sum().backward()
-      check_schedule(opt.schedule_step(), 14)
+      check_schedule(opt.schedule_step(), 13)
 
   def test_sgd_conv_fuse(self):
     with Tensor.train():
       img = Tensor.empty(2,3,4,4)
       c1 = nn.Conv2d(3,32,3)
       opt = nn.optim.SGD(nn.state.get_parameters(c1))
       opt.zero_grad()
@@ -743,9 +773,74 @@
     b = Tensor.empty(16, 16)
     c = a.sum() + 2
     d = a.sum() * 2
     e = c * d
     f = (b - d).sum() - e
     check_schedule([c, d, e, f], 3)
 
+  def test_pad_reduce_safe(self):
+    Tensor.manual_seed(0)
+    a = Tensor.rand(3, 4, 5).realize()
+    b = Tensor.rand(3, 4, 5).realize()
+    out = (a + b).pad(((0, 1), (0, 1), (0, 1)), 1.0).sum().contiguous()
+    run_schedule(check_schedule(out, 1))
+    np.testing.assert_allclose(out.numpy(), np.pad(a.numpy()+b.numpy(), ((0, 1), (0, 1), (0, 1)), constant_values=1.0).sum())
+
+  def test_pad_reduce_usafe(self):
+    Tensor.manual_seed(0)
+    a = Tensor.rand(3, 4, 5).realize()
+    out = a.log2().pad(((0, 1), (0, 1), (0, 1)), 1.0).sum().contiguous()
+    run_schedule(check_schedule(out, 2))
+    np.testing.assert_allclose(out.numpy(), np.pad(np.log2(a.numpy()), ((0, 1), (0, 1), (0, 1)), constant_values=1.0).sum(), rtol=1e-6)
+
+  def test_shrink_pad_safe(self):
+    a = Tensor.ones((3, )).contiguous().realize()
+    b = Tensor.ones((3, )).contiguous().realize()
+    out = (a + b).shrink(((0, 1),)).pad(((0, 1),)).contiguous()
+    run_schedule(check_schedule(out, 1))
+    np.testing.assert_equal(out.numpy(), [2, 0])
+
+  # TODO: should not shuffle unsafe pad ops through any pads, even if buffer is shrunk overall (#3437)
+  def test_shrink_pad_unsafe(self):
+    a = Tensor.ones((3, )).contiguous().realize()
+    out = a.exp2().shrink(((0, 1),)).pad(((0, 1),)).contiguous()
+    run_schedule(check_schedule(out, 1))
+    with self.assertRaises(AssertionError):
+      np.testing.assert_equal(out.numpy(), [2, 0])
+
+  def test_base_change_shrink_pad(self):
+    a = Tensor.ones(3, 3).contiguous().realize()
+    b = a.exp2()
+    c = b[:-1, :-1]
+    d = c.pad(((0, 1), (0, 1))) * 2
+    run_schedule(check_schedule(d, 1))
+    with self.assertRaises(AssertionError): # TODO unsafe pads
+      np.testing.assert_equal(d.numpy(), np.pad(np.exp2(a.numpy())[:-1, :-1], ((0, 1), (0, 1)))*2)
+
+  def test_base_change_expand_pad(self):
+    a = Tensor.ones(3, 3).contiguous().realize()
+    b = a.exp2()
+    c = b[:, None, :]
+    d = c.pad(((0, 0), (1, 1), (0, 0))) * 2
+    run_schedule(check_schedule(d, 2))
+    np.testing.assert_equal(d.numpy(), np.pad(np.exp2(a.numpy())[:, None, :], ((0, 0), (1, 1), (0, 0)))*2)
+
+  # TODO like openpilot with imagef
+  @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
+  def test_base_change_expand_expand(self):
+    a = Tensor.ones(4, 4).contiguous().realize()
+    b = a.cast(dtypes.half).expand(2, 4, 4)
+    c = b.cast(dtypes.int).expand(2, 2, 4, 4)
+    run_schedule(check_schedule(c, 2))
+    np.testing.assert_equal(c.numpy(), np.ones(((2, 2, 4, 4)), dtype=np.int32))
+
+  def test_base_change_pad_expand(self):
+    a = Tensor.full((4, 4), 1.).contiguous().realize()
+    b = Tensor.full((4, 4), 2.).contiguous().realize()
+    c = (a + b).pad(((1, 1), (1, 1)))
+    d = c.cast(dtypes.int).expand((2, 6, 6)) * 4
+    run_schedule(check_schedule(d, 2))
+    c_np = np.pad((np.full((4, 4), 2., dtype=np.float32) + np.full((4, 4), 1., dtype=np.float32)), ((1, 1), (1, 1)), constant_values=0.0)
+    np.testing.assert_equal(d.numpy(), np.broadcast_to(c_np.astype(np.half), (2, *c_np.shape)) * 4)
+
 if __name__ == '__main__':
   unittest.main(verbosity=2)
```

### Comparing `tinygrad_tools-0.8.1/test/test_search.py` & `tinygrad_tools-0.8.2/test/test_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import unittest
 
 from tinygrad.codegen.kernel import Opt, OptOps
 from tinygrad.codegen.linearizer import Linearizer
 from tinygrad.engine.schedule import create_schedule
-from tinygrad.features.search import time_linearizer, bufs_from_lin, actions
+from tinygrad.engine.search import time_linearizer, bufs_from_lin, actions
 from tinygrad.device import Device, Buffer
 from tinygrad.ops import LoadOps, BufferOps
 from tinygrad.tensor import Tensor
 from tinygrad.helpers import Context
 from tinygrad.engine.realize import capturing
 
 class TestTimeLinearizer(unittest.TestCase):
+  @unittest.skipIf(Device.DEFAULT in {"AMD", "NV"}, "Tries to open HSA/CUDA. #4607")
   def test_reasonable_time(self):
     si = [i for i in create_schedule([Tensor([1,2,3,4]).add(1).lazydata]) if i.ast[0].op not in LoadOps][0]
     out = Buffer(Device.DEFAULT, si.outputs[0].size, si.outputs[0].dtype).allocate()
     memops = {x.arg.idx:x.arg.st.real_size() for x in si.ast[0].lazyops if x.op is BufferOps.LOAD}
     rawbufs = [out] + [Buffer(Device.DEFAULT, memops[i], x.dtype).allocate() for i,x in enumerate(si.inputs, start=len(si.outputs))]
     tm = time_linearizer(Linearizer(*si.ast), rawbufs, allow_test_size=False, cnt=10)
     assert tm > 0 and tm != float('inf')
 
+  @unittest.skipIf(Device.DEFAULT in {"AMD", "NV"}, "Tries to open HSA/CUDA. #4607")
   def test_bufs_from_lin(self):
     si = [i for i in create_schedule([Tensor([1,2,3,4]).add(1).lazydata]) if i.ast[0].op not in LoadOps][0]
     rawbufs = bufs_from_lin(lin:=Linearizer(*si.ast))
     assert len(rawbufs) == len(lin.membufs)
     assert all(r is not None for r in rawbufs)
     assert all(isinstance(r, Buffer) for r in rawbufs)
     assert all(r.size > 0 for r in rawbufs)
 
 class TestBEAM(unittest.TestCase):
+  @unittest.skipIf(Device.DEFAULT in {"AMD", "NV"}, "Tries to open HSA/CUDA. #4607")
   def test_dynamic_beam(self):
     # TODO: make this infra globally usable
     class Capture:
       def __init__(self): self.captured = []
       def add(self, x): self.captured.append(x)
     capturing.append(Capture())
     with Context(BEAM=1): Tensor.zeros(16).contiguous().realize()
     k_beam_1 = capturing[0].captured
     capturing.clear()
     capturing.append(Capture())
     with Context(BEAM=0): Tensor.zeros(16).contiguous().realize()
     k_beam_0 = capturing[0].captured
     capturing.clear()
-    assert k_beam_0[-1].prg.prg != k_beam_1[-1].prg.prg
+    assert k_beam_0[-1].prg.p.src != k_beam_1[-1].prg.p.src
 
   def test_get_linearizer_actions(self):
     from test.test_linearizer import helper_realized_ast
     a = Tensor.rand(4, 3)
     b = Tensor.rand(3)
     realized_ast, _ = helper_realized_ast(a @ b)
-    from tinygrad.features.search import get_linearizer_actions
+    from tinygrad.engine.search import get_linearizer_actions
     lins = get_linearizer_actions(Linearizer(realized_ast), False).values()
 
     # ensure amt=0 are not duplicated
     if Opt(OptOps.UPCAST, 0, 0) in actions:
       assert len([x for x in lins if x.applied_opts[0] == Opt(OptOps.UPCAST, axis=0, amt=4)]) == 0, "did not de-dup UPCAST"
     if Opt(OptOps.LOCAL, 0, 0) in actions:
       assert len([x for x in lins if x.applied_opts[0] == Opt(OptOps.LOCAL, axis=0, amt=4)]) == 0, "did not de-dup LOCAL"
```

### Comparing `tinygrad_tools-0.8.1/test/test_specific_conv.py` & `tinygrad_tools-0.8.2/test/test_specific_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from tinygrad.helpers import CI
 from tinygrad import Tensor, Device, dtypes
 from test.helpers import is_dtype_supported
 # similar to test/external/external_test_gpu_ast.py, but universal
 
-@unittest.skipIf(Device.DEFAULT == "CUDA" and CI, "slow on CUDA CI")
+@unittest.skipIf(Device.DEFAULT in {"CUDA", "NV"} and CI, "slow on CUDA CI")
 class TestSpecific(unittest.TestCase):
   # from openpilot
 
   # 1x1 6 <- 24
   def test_1x1_6_24(self):
     x = Tensor.randn(1,   24*4, 32, 64)
     w = Tensor.randn(6*4, 24*4, 1,  1)
```

### Comparing `tinygrad_tools-0.8.1/test/test_speed_v_torch.py` & `tinygrad_tools-0.8.2/test/test_speed_v_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
   tiny_conv.weight = Tensor(torch_conv.weight.detach().cpu().numpy())
 
   def f1(torch_dat): return torch_conv(torch_dat)
   def f2(tiny_dat): return tiny_conv(tiny_dat).realize()
   helper_test_generic(f"conv bs:{bs:3d} chans:{in_chans:3d} -> {out_chans:3d} k:{kernel_size}", f1, (torch_dat,), TinyJit(f2), (tiny_dat,))
 
 @unittest.skipIf(getenv("BIG") == 0, "no big tests")
-@unittest.skipIf(getenv("CUDACPU"), "no CUDACPU")
+@unittest.skipIf(getenv("CUDACPU") or getenv("MOCKGPU"), "no CUDACPU or MOCKGPUs")
 class TestBigSpeed(unittest.TestCase):
   def test_add(self):
     def f(a, b): return a+b
     helper_test_generic_square('add', 8192, f, f)
   def test_exp(self):
     def f(a, b): return a.exp()
     helper_test_generic_square('exp', 8192, f, f, onearg=True)
@@ -134,15 +134,15 @@
   def test_large_conv_1x1(self): helper_test_conv(bs=32, in_chans=128, out_chans=128, kernel_size=1, img_size_y=128, img_size_x=128)
   def test_large_conv_3x3(self): helper_test_conv(bs=4, in_chans=128, out_chans=128, kernel_size=3, img_size_y=130, img_size_x=130)
   def test_large_conv_5x5(self): helper_test_conv(bs=4, in_chans=128, out_chans=128, kernel_size=5, img_size_y=132, img_size_x=132)
   def test_matvec_4096_16384(self): helper_test_matvec('matvec_4096_16384', 4096, 16384)
   def test_matvec_16384_4096(self): helper_test_matvec('matvec_16384_4096', 16384, 4096)
 
 @unittest.skipIf(getenv("BIG") == 1, "only big tests")
-@unittest.skipIf(getenv("CUDACPU"), "no CUDACPU")
+@unittest.skipIf(getenv("CUDACPU") or getenv("MOCKGPU"), "no CUDACPU or MOCKGPUs")
 class TestSpeed(unittest.TestCase):
   def test_sub(self):
     def f(a, b): return a-b
     helper_test_generic_square('sub', 4096, f, f)
 
   @unittest.skipIf(CI and Device.DEFAULT == "WEBGPU", "breaking on webgpu CI")
   def test_pow(self):
```

### Comparing `tinygrad_tools-0.8.1/test/test_subbuffer.py` & `tinygrad_tools-0.8.2/test/test_subbuffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from tinygrad import Device, dtypes, Tensor
 from tinygrad.helpers import CI
-from tinygrad.buffer import Buffer
+from tinygrad.device import Buffer
 from tinygrad.lazy import view_supported_devices
 
 @unittest.skipIf(Device.DEFAULT not in view_supported_devices, "subbuffer not supported")
 class TestSubBuffer(unittest.TestCase):
   def setUp(self):
     self.buf = Buffer(Device.DEFAULT, 10, dtypes.uint8).ensure_allocated()
     self.buf.copyin(memoryview(bytearray(range(10))))
```

### Comparing `tinygrad_tools-0.8.1/test/test_symbolic_jit.py` & `tinygrad_tools-0.8.2/test/test_symbolic_jit.py`

 * *Files 16% similar despite different names*

```diff
@@ -173,9 +173,62 @@
       a = Tensor.rand(7, 11)
       symbolic = a.shrink(((3,5),(vi,vi+2)))
       symbolic = jf(symbolic).numpy()
       expected = f(a.shrink(((3,5),(i,i+2)))).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
     assert_jit_cache_len(jf, 1)
 
+  def test_mean(self):
+    def f(a): return a.mean().realize()
+    def f0(a): return a.mean(0).realize()
+    def f1(a): return a.mean(1).realize()
+    jf = TinyJit(f)
+    jf0 = TinyJit(f0)
+    jf1 = TinyJit(f1)
+    for i in range(1, 5):
+      vi = Variable("i", 1, 10).bind(i)
+      # aixs = None
+      a = Tensor.rand(i, 3)
+      symbolic = jf(a.reshape(vi, 3)).numpy()
+      expected = a.mean().numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+      # aixs = 0
+      a = Tensor.rand(i, 3)
+      symbolic = jf0(a.reshape(vi, 3)).numpy()
+      expected = a.mean(0).numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+      # aixs = 1
+      a = Tensor.rand(i, 3)
+      symbolic = jf1(a.reshape(vi, 3)).reshape(i).numpy()
+      expected = a.mean(1).numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+
+  @unittest.skip("failed for some")
+  def test_mean_2d(self):
+    def f(a): return a.mean().realize()
+    def f0(a): return a.mean(0).realize()
+    def f1(a): return a.mean(1).realize()
+    jf = TinyJit(f)
+    jf0 = TinyJit(f0)
+    jf1 = TinyJit(f1)
+    for i in range(1, 5):
+      for j in range(1, 5):
+        vi = Variable("i", 1, 10).bind(i)
+        vj = Variable("j", 1, 10).bind(j)
+        # aixs = None
+        a = Tensor.rand(i, j)
+        symbolic = jf(a.reshape(vi, vj)).numpy()
+        expected = a.mean().numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+        # aixs = 0
+        a = Tensor.rand(i, j)
+        symbolic = jf0(a.reshape(vi, vj)).reshape(j).numpy()
+        expected = a.mean(0).numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+        # aixs = 1
+        a = Tensor.rand(i, j)
+        symbolic = jf1(a.reshape(vi, vj)).reshape(i).numpy()
+        expected = a.mean(1).numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_symbolic_ops.py` & `tinygrad_tools-0.8.2/test/test_symbolic_ops.py`

 * *Files 19% similar despite different names*

```diff
@@ -137,9 +137,49 @@
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(7, 11)
       symbolic = a.shrink(((3,5),(vi,vi+2)))
       symbolic = symbolic.numpy()
       expected = a.shrink(((3,5),(i,i+2))).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
 
+  def test_mean(self):
+    for i in range(1, 5):
+      vi = Variable("i", 1, 10).bind(i)
+      # aixs = None
+      a = Tensor.rand(i, 3)
+      symbolic = a.reshape(vi, 3).mean().numpy()
+      expected = a.mean().numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+      # aixs = 0
+      a = Tensor.rand(i, 3)
+      symbolic = a.reshape(vi, 3).mean(0).numpy()
+      expected = a.mean(0).numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+      # aixs = 1
+      a = Tensor.rand(i, 3)
+      symbolic = a.reshape(vi, 3).mean(1).reshape(i).numpy()
+      expected = a.mean(1).numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+
+  def test_mean_2d(self):
+    for i in range(1, 5):
+      for j in range(1, 5):
+        vi = Variable("i", 1, 10).bind(i)
+        vj = Variable("j", 1, 10).bind(j)
+        # aixs = None
+        a = Tensor.rand(i, j)
+        symbolic = a.reshape(vi, vj).mean().numpy()
+        expected = a.mean().numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+        # aixs = 0
+        a = Tensor.rand(i, j)
+        symbolic = a.reshape(vi, vj).mean(0).reshape(j).numpy()
+        expected = a.mean(0).numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+        # aixs = 1
+        a = Tensor.rand(i, j)
+        symbolic = a.reshape(vi, vj).mean(1).reshape(i).numpy()
+        expected = a.mean(1).numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad_tools-0.8.1/test/test_symbolic_shapetracker.py` & `tinygrad_tools-0.8.2/test/test_symbolic_shapetracker.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_tensor.py` & `tinygrad_tools-0.8.2/test/test_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
 
   def test_repr_with_grad(self):
     a = Tensor([1])
     b = Tensor([1])
     c = (a + b).mean().backward()
     print(c)
 
-@unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL"}, "no GPU CI")
+@unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL", "NV", "AMD"}, "no GPU CI")
 class TestMoveTensor(unittest.TestCase):
   d0, d1 = f"{Device.DEFAULT}:0", f"{Device.DEFAULT}:1"
   @given(strat.sampled_from([d0, d1]), strat.sampled_from([d0, d1]),
          strat.sampled_from([dtypes.float16, dtypes.float32]), strat.sampled_from([True, False, None]))
   def test_to_preserves(self, src, dest, dtype, requires_grad):
     s = Tensor([1, 2, 3], device=src, dtype=dtype, requires_grad=requires_grad)
     if requires_grad: s.sum().backward()
```

### Comparing `tinygrad_tools-0.8.1/test/test_tensor_data.py` & `tinygrad_tools-0.8.2/test/test_tensor_data.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_tensor_variable.py` & `tinygrad_tools-0.8.2/test/test_tensor_variable.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_uop_graph.py` & `tinygrad_tools-0.8.2/test/test_uop_graph.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_uops.py` & `tinygrad_tools-0.8.2/test/test_uops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Optional, Tuple, Any, List
 import unittest, math
 import numpy as np
 from tinygrad.tensor import Tensor
 from tinygrad.helpers import getenv
 from tinygrad.dtype import dtypes, DType, PtrDType
-from tinygrad.device import Buffer, Device, CompiledRunner
-from tinygrad.ops import UnaryOps, BinaryOps, TernaryOps
+from tinygrad.device import Buffer, Device
+from tinygrad.ops import UnaryOps, BinaryOps, TernaryOps, exec_alu
+from tinygrad.renderer import Program
 from tinygrad.engine.schedule import create_schedule
+from tinygrad.engine.realize import CompiledRunner, lower_schedule_item
 from tinygrad.codegen.linearizer import UOps, UOp
-from tinygrad.codegen.uops import exec_alu, UOpGraph
+from tinygrad.codegen.uops import UOpGraph
 from test.helpers import is_dtype_supported
 
 def _uops_to_prg(uops):
-  src = Device[Device.DEFAULT].compiler.render("test", uops)
-  has_local = Device[Device.DEFAULT].compiler.compiler_opts.has_local
-  return CompiledRunner("test", src, Device.DEFAULT, [1] if has_local else None, [1] if has_local else None, uops=uops)
+  src = Device[Device.DEFAULT].renderer.render("test", uops)
+  has_local = Device[Device.DEFAULT].renderer.has_local
+  return CompiledRunner(Program("test", src, Device.DEFAULT, [1,1,1] if has_local else None, [1,1,1] if has_local else None, uops=uops))
 
 def uop(uops:List[UOp], uop:UOps, dtype:Optional[DType], vin:Tuple[UOp, ...], arg:Any=None) -> UOp:
   uops.append(UOp(uop, dtype, tuple(vin), arg))
   return uops[-1]
 
 def _test_single_value(vals, op, dts):
   uops = []
@@ -206,17 +208,16 @@
     si = create_schedule([t.lazydata])
     assert len(si) == 0
 
   def test_bitcast_const(self):
     t = Tensor(1, dtype=dtypes.float).bitcast(dtypes.int)
     si = create_schedule([t.lazydata])
     assert len(si) == 1
-    si = si[0]
-    lin = Device[Device.DEFAULT].get_linearizer(si.ast[0]).linearize()
-    assert any(uop.uop is UOps.BITCAST for uop in lin.uops.uops), f"{[uop.uop for uop in lin.uops.uops]} does not contain bitcast"
+    ji = lower_schedule_item(si[-1])
+    assert any(uop.uop is UOps.BITCAST for uop in ji.prg.p.uops), f"{[uop.uop for uop in ji.prg.p.uops]} does not contain bitcast"
 
 class TestLocalAccess(unittest.TestCase):
   @unittest.skipIf(Device.DEFAULT in {"LLVM"}, "device doesn't support local memory")
   def test_local_basic(self):
     uops = []
     smem = uop(uops, UOps.DEFINE_LOCAL, PtrDType(dtypes.float32), (), ('smem', 16))
     uop(uops, UOps.STORE, None, (smem, uop(uops, UOps.CONST, dtypes.int32, (), 0), uop(uops, UOps.CONST, dtypes.float32, (), 42.0)))
@@ -252,9 +253,29 @@
     ptr_ar(u10, uops)
     self.assertEqual(u9.vin[0], u10.vin[0])
     self.assertEqual(u9.vin[1].uop, UOps.CONST)
     self.assertEqual(u9.vin[1].arg, u5.arg*dtypes.float.itemsize)
     self.assertEqual(u10.vin[1].uop, UOps.CONST)
     self.assertEqual(u10.vin[1].arg, u6.arg*dtypes.float.itemsize)
 
+  def test_gated_load(self):
+    from tinygrad.renderer.assembly import optimize_gated_loads
+    uops = UOpGraph()
+    u1 = uops.add(UOps.DEFINE_GLOBAL, PtrDType(dtypes.int), tuple(), (0, 'data0', True))
+    u2 = uops.add(UOps.SPECIAL, dtypes.int, tuple(), (0, 'gidx0', 9))
+    u3 = uops.add(UOps.CONST, dtypes.int, tuple(), arg=42)
+    u4 = uops.add(UOps.ALU, dtypes.int, (u2, u3), BinaryOps.MUL)
+    u5 = uops.add(UOps.CONST, dtypes.int, tuple(), arg=0)
+    u6 = uops.add(UOps.CONST, dtypes.int, tuple(), arg=1)
+    u7 = uops.add(UOps.CONST, dtypes.bool, tuple(), arg=1)
+    u8 = uops.add(UOps.ALU, dtypes.int, (u4, u5), BinaryOps.ADD)
+    u9 = uops.add(UOps.LOAD, dtypes.int, (u1, u8, u7, u6))
+    optimize_gated_loads(uops)
+    if_op = next(filter(lambda x: x.uop is UOps.IF, uops.uops), None)
+    self.assertNotEqual(if_op, None)
+    self.assertNotEqual(next(filter(lambda x: x.uop is UOps.ENDIF, uops.uops), None), None)
+    for uu in [u2, u3, u4, u5, u6, u8, u9]:
+      self.assertLess(uops.uops.index(if_op), uops.uops.index(uu))
+
+
 if __name__ == '__main__':
   unittest.main(verbosity=2)
```

### Comparing `tinygrad_tools-0.8.1/test/test_uops_stats.py` & `tinygrad_tools-0.8.2/test/test_uops_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import unittest
-from tinygrad import Tensor, Device
+from tinygrad import Tensor
 from tinygrad.engine.schedule import create_schedule
+from tinygrad.engine.realize import lower_schedule_item
 
 # TODO: can copy this in here when we remove it
 #from tinygrad.ops import get_lazyop_info
 #info = get_lazyop_info(ast)
 #print(ops, mem, expected_mem)
 #print(info.flops, info.mem_estimate)
 
 # **************** new FlopCounter ****************
 
 def get_stats(x:Tensor):
   si = create_schedule([x.lazydata])[-1]
-  runner = Device[Device.DEFAULT].get_runner(*si.ast)
-  return runner.op_estimate, runner.mem_estimate
+  ei = lower_schedule_item(si)
+  return ei.prg.op_estimate, ei.prg.mem_estimate
 
 class TestUOpsStats(unittest.TestCase):
   def test_simple_add(self):
     a = Tensor.empty(100,100)
     b = Tensor.empty(100,100)
     c = a+b
     ops, mem = get_stats(c)
```

### Comparing `tinygrad_tools-0.8.1/test/test_winograd.py` & `tinygrad_tools-0.8.2/test/test_winograd.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/test/test_zero_copy.py` & `tinygrad_tools-0.8.2/test/test_zero_copy.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/codegen/kernel.py` & `tinygrad_tools-0.8.2/tinygrad/codegen/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import math, itertools
 from typing import NamedTuple, Optional, List, Tuple, cast, Dict, Union
 from tinygrad.ops import LazyOp, UnaryOps, BinaryOps, ReduceOps, MemBuffer, ConstBuffer, BufferOps, UNSAFE_PAD_OPS
-from tinygrad.device import Device, CompilerOptions
+from tinygrad.device import Device
+from tinygrad.renderer import Renderer
 from tinygrad.dtype import dtypes, ImageDType, DType
 from tinygrad.helpers import colored, ansilen, dedup, flatten, getenv, prod, DEBUG, round_up, all_int, get_contraction
 from tinygrad.shape.shapetracker import ShapeTracker
 from tinygrad.shape.symbolic import sint
 from tinygrad.shape.view import View, strides_for_shape
 from dataclasses import dataclass
 from enum import Enum, auto
@@ -50,48 +51,48 @@
   axes_exist: List[bool] # true if the original N and M axes are still in the shape
   def fix_axes(self, removed_axis:int): # adjust the TC axes if necesssary when an dimension is removed
     for tc_dim in [i for i in range(2) if self.axes_exist[i]]:
       if removed_axis < self.axes[tc_dim]: self.axes[tc_dim] -= 1
       elif removed_axis == self.axes[tc_dim]: self.axes_exist[tc_dim] = False
 
 tensor_cores: Dict[str, List[TensorCore]] = {
-  "METAL": [TensorCore(dims=(8,8,8), threads=[(0,2),(1,4),(0,2),(1,2)], thread_local_sizes=[[2],[2],[2]], thread_local_aliases=[ [[4],[0],[2],[0],[-1, 1, 3],[0]], [[0],[3],[0],[1],[2, 4],[-1]], [[4],[3],[2],[1],[0],[-1]] ], dtype_in=di, dtype_out=do) for (di, do) in [(dtypes.float, dtypes.float), (dtypes.half, dtypes.float), (dtypes.half, dtypes.half)]],  # noqa: E501
-  "HSA": [TensorCore(dims=(16,16,16), threads=[(0,8),(0,2),(1,2)], thread_local_sizes=[[16],[16],[4,2]], thread_local_aliases=[ [[2],[0],[0],[-1],[1]], [[0],[2],[1],[-1],[0]], [[-2],[2],[1],[0],[3,-1]] ], dtype_in=di, dtype_out=do) for (di, do) in [(dtypes.half, dtypes.float), (dtypes.half, dtypes.half)]],  # noqa: E501
-  "CUDA": [TensorCore(dims=(8,16,16), threads=[(0,2),(0,2),(1,2),(1,2),(0,2)], thread_local_sizes=[[2,2,2],[2,2],[2,2]], thread_local_aliases=[ [[0],[-2],[5],[0],[0],[-1,1,2,-3],[3,4]], [[5],[0],[0],[4],[3],[-1,1,2,-2],[0]], [[2],[-2],[5],[1],[-1],[0],[3,4]] ], dtype_in=di, dtype_out=do) for (di, do) in ([(dtypes.half, dtypes.float)] if getenv("PTX") else [(dtypes.half, dtypes.float), (dtypes.bfloat16, dtypes.float)])],  # noqa: E501
+  "METAL": [TensorCore(dims=(8,8,8), threads=[(0,2),(1,4),(0,2),(1,2)], thread_local_sizes=[[2],[2],[2]], thread_local_aliases=[ [[0],[2],[0],[4],[-1, 1, 3],[0]], [[1],[0],[3],[0],[2, 4],[-1]], [[1],[2],[3],[4],[0],[-1]] ], dtype_in=di, dtype_out=do) for (di, do) in [(dtypes.float, dtypes.float), (dtypes.half, dtypes.float), (dtypes.half, dtypes.half)]],  # noqa: E501
+  "HSA": [TensorCore(dims=(16,16,16), threads=[(0,8),(0,2),(1,2)], thread_local_sizes=[[16],[16],[4,2]], thread_local_aliases=[ [[0],[0],[2],[-1],[1]], [[1],[2],[0],[-1],[0]], [[1],[2],[-2],[0],[3,-1]] ], dtype_in=di, dtype_out=do) for (di, do) in [(dtypes.half, dtypes.float), (dtypes.half, dtypes.half)]],  # noqa: E501
+  "CUDA": [TensorCore(dims=(8,16,16), threads=[(0,2),(0,2),(1,2),(1,2),(0,2)], thread_local_sizes=[[2,2,2],[2,2],[2,2]], thread_local_aliases=[ [[0],[0],[5],[-2],[0],[-1,1,2,-3],[3,4]], [[3],[4],[0],[0],[5],[-1,1,2,-2],[0]], [[-1],[1],[5],[-2],[2],[0],[3,4]] ], dtype_in=di, dtype_out=do) for (di, do) in ([(dtypes.half, dtypes.float)] if getenv("PTX") else [(dtypes.half, dtypes.float), (dtypes.bfloat16, dtypes.float)])],  # noqa: E501
 }
-tensor_cores["AMD"] = tensor_cores["HSA"]
-tensor_cores["NV"] = tensor_cores["CUDA"]
 
 class LocalBuffer(NamedTuple):
   name: str
   size: int
   dtype: DType = dtypes.float32
   realized: None = None
   def __str__(self): return f"localbuffer<{self.name}[{self.size}]>"
 
 class Kernel:
-  def __init__(self, *ast:LazyOp, opts:Optional[CompilerOptions]=None):
-    self.opts = opts if opts is not None else (device.compiler.compiler_opts if (device:=Device[Device.DEFAULT]).compiler is not None else
-                                               CompilerOptions(Device.DEFAULT))
+  def __init__(self, *ast:LazyOp, opts:Optional[Renderer]=None):
+    self.opts = opts if opts is not None else Device[Device.DEFAULT].renderer
     assert all(op.op is BufferOps.STORE for op in ast), f"kernels must have stores as the output, got {ast}"
     assert len(set(op.arg.st.size for op in ast)) == 1, f"all outbufs should have the same size, got {[op.arg.st for op in ast]}"
     self.ast = ast
     self.lazyops = flatten([op.lazyops for op in self.ast])
 
     # there's only allowed to be one reduceop
-    reduceops = [x for x in self.lazyops if x.op in ReduceOps]
-    assert len(dedup(reduceops)) <= 1, "max one reduce op in an ast"
-    self.reduceop = reduceops[0] if reduceops else None
+    cached_ordered_lazyops: Dict[LazyOp, List[LazyOp]] = {}
+    def ordered_lazyops(op):
+      if op not in cached_ordered_lazyops: cached_ordered_lazyops[op] = dedup([item for x in op.src for item in ordered_lazyops(x)] + [op])
+      return cached_ordered_lazyops[op]
+    self.reduceops = dedup([x for out in self.ast for x in ordered_lazyops(out) if x.op in ReduceOps])
+    assert len(self.reduceops) < 2, "Only one reduceop allowed"
 
     self.outbufs, self.vars = [x.arg for x in self.ast], flatten([x.vars() for x in self.ast])
     loadops = [BufferOps.LOAD, BufferOps.CONST]
     self.bufs: List[Union[MemBuffer, ConstBuffer, LocalBuffer]] = self.outbufs + dedup([x.arg for x in self.lazyops if x.op in loadops])
 
     # get earlybufs, before the one reduce op
-    self.earlybufs = [x.arg for x in self.reduceop.lazyops if x.op in BufferOps] if self.reduceop else []
+    self.earlybufs = [x.arg for reduceop in self.reduceops for x in reduceop.lazyops if x.op in BufferOps]
     self.full_buf_index: int = self.bufs.index(self.earlybufs[0]) if self.earlybufs else 0
 
     # create new shapetrackers inside this kernel, we will permute them
     self.sts: List[ShapeTracker] = [x.st for x in cast(List[Union[MemBuffer, ConstBuffer]], self.bufs)]
 
     # move all reduce axes to the end
     reduce = list(enumerate(zip(self.full_shape, self.output_shape)))
@@ -118,16 +119,16 @@
   def copy(self):
     ret = type(self).__new__(type(self))
 
     # base linearizer params
     ret.opts, ret.ast, ret.lazyops = self.opts, self.ast, self.lazyops
 
     # things downstream of the AST
-    ret.reduceop, ret.outbufs, ret.vars, ret.bufs, ret.earlybufs, ret.full_buf_index = \
-      self.reduceop, self.outbufs, self.vars, [x for x in self.bufs if not isinstance(x, LocalBuffer)], self.earlybufs, self.full_buf_index
+    ret.reduceops, ret.outbufs, ret.vars, ret.bufs, ret.earlybufs, ret.full_buf_index = \
+      self.reduceops, self.outbufs, self.vars, [x for x in self.bufs if not isinstance(x, LocalBuffer)], self.earlybufs, self.full_buf_index
     ret.sts = self.sts[:len(ret.bufs)] # NOTE: must redo the local buffers with TC in beam
 
     # parameters for optimizations
     ret.applied_opts, ret.group_for_reduces, ret.upcasted, ret.local_dims, ret.dont_use_locals = \
       self.applied_opts[:], self.group_for_reduces, self.upcasted, self.local_dims, self.dont_use_locals
     ret.tensor_core, ret.tensor_core_opts, ret.local_alias = self.tensor_core, self.tensor_core_opts, {}
 
@@ -161,14 +162,17 @@
     return [x for x in self.sts[i].unit_stride_axes() if x >= self.shape_len-self.upcasted and self.sts[i].shape[x] > 1] if should_upcast else []
 
   @property
   def first_reduce(self) -> int:
     return [x!=y for x,y in zip(self.sts[0].shape[:self.shape_len-self.upcasted]+(0,), self.full_shape[:self.shape_len-self.upcasted]+(1,))].index(True)  # noqa: E501
 
   @property
+  def reduceop(self) -> LazyOp: return self.reduceops[0] if len(self.reduceops) > 0 else None
+
+  @property
   def output_shape(self) -> Tuple[sint, ...]: return self.sts[0].shape
 
   @property
   def full_shape(self) -> Tuple[sint, ...]: return self.sts[self.full_buf_index].shape
 
   @property
   def full_unupcasted_shape(self) -> Tuple[sint, ...]: return self.full_shape[:self.shape_len-self.upcasted]
@@ -335,24 +339,24 @@
 
   # ******************** high level optimizers ********************
 
   def _apply_tc_opt(self, use_tensor_cores:int, axis:int, opt_level:int) -> bool:
     if use_tensor_cores and self.opts.has_local and self.reduceop and self.reduceop.op is ReduceOps.SUM and self.opts.device in tensor_cores:
       for tc in tensor_cores[self.opts.device]:
         has_cast = tc.dtype_in != tc.dtype_out
-        if has_cast and not(self.reduceop.src[0].op is UnaryOps.CAST and self.reduceop.src[0].arg[0] == tc.dtype_out): continue
+        if has_cast and not(self.reduceop.src[0].op is UnaryOps.CAST and self.reduceop.src[0].arg == tc.dtype_out): continue
 
         mul_op = self.reduceop.src[0].src[0] if has_cast else self.reduceop.src[0]
         if mul_op.op is not BinaryOps.MUL: continue
 
         def buf_index(src: LazyOp) -> Optional[int]:
           # TODO: apply tc even if the sources are not from LOAD
           if src.op is BufferOps.LOAD and src.arg.dtype == tc.dtype_in: return self.bufs.index(cast(MemBuffer, src.arg))
           try:
-            if opt_level >= 1 and src.op is UnaryOps.CAST and src.arg[0] == tc.dtype_in: return self.bufs.index(cast(MemBuffer, src.src[0].arg))
+            if opt_level >= 1 and src.op is UnaryOps.CAST and src.arg == tc.dtype_in: return self.bufs.index(cast(MemBuffer, src.src[0].arg))
           except ValueError: return None
           return None
         if (buf0:=buf_index(mul_op.src[0])) is None or (buf1:=buf_index(mul_op.src[1])) is None: continue
 
         buf0_strides, buf1_strides = self.sts[buf0].real_strides(), self.sts[buf1].real_strides()
         axis_buf0 = [(i,self.full_shape[i],buf1_strides[i]) for i,s in enumerate(buf0_strides[:self.first_reduce]) if s == 0]
         axis_buf1 = [(i,self.full_shape[i],buf0_strides[i]) for i,s in enumerate(buf1_strides[:self.first_reduce]) if s == 0]
@@ -380,15 +384,14 @@
 
         # assert tensor core
         if DEBUG >= 3: print("TENSOR CORES", axis_buf0, axis_buf1, tc)
         if use_tensor_cores == 1: self.tensor_core = tc # TC=2 will do the shape ops without the WMMA
         return True
     return False
 
-
   def apply_tensor_cores(self, use_tensor_cores=1, extra_opts:Optional[List[Opt]]=None, axis:int=0, tc_opt:int=getenv("TC_OPT")) -> bool:
     """ Attempts to apply a tensor core optimization to the kernel.  If one exists and applies properly, return true, otherwise return false.
     Tensor cores are optimized instructions that matrix multiply-accumulate across a wave of threads: D(M, N) = A(M, K) * B(K, N) + C(M, N).
 
     Keyword arguments:
     use_tensor_cores -- controls how tensor cores are applied (default 1)
       0: will disable any tensor core matching
@@ -446,20 +449,21 @@
       if opt.op is not OptOps.PADTO: check(self.full_shape[axis] % amt == 0, "no longer valid shift")
     else: amt = -1
 
     if self.reduceop and (opt.op in {OptOps.GROUP, OptOps.GROUPTOP} or (self.group_for_reduces and opt.op not in {OptOps.NOLOCALS, OptOps.PADTO})):
       acc_sz, upcast_idx = dt.base.itemsize if isinstance((dt:=self.reduceop.dtype), ImageDType) else dt.itemsize, self.shape_len-self.upcasted
       upcast_sz = prod([a for a,b in zip(self.full_shape[upcast_idx:], self.sts[0].shape[upcast_idx:]) if a == b])
       local_sz = prod(self.full_shape[self.first_reduce-self.local_dims:self.first_reduce+self.group_for_reduces])
-      check(amt*acc_sz*upcast_sz*local_sz <= self.opts.shared_max, "exceeds maximum shared memory size")
+      smem_sz = amt*acc_sz*upcast_sz*local_sz
+      check(smem_sz <= self.opts.shared_max, f"exceeds maximum shared memory size: needs {smem_sz}, max {self.opts.shared_max}")
 
     if opt.op is OptOps.LOCAL:    # cyan
       check(self.opts.has_local, "target does not support local")
       check(axis < self.global_dims, "local is for globals")
-      self.shift_to(axis, amt, insert_before=self.first_reduce-self.local_dims)
+      self.shift_to(axis, amt, insert_before=self.first_reduce)
       self.local_dims += 1
     elif opt.op in {OptOps.GROUP, OptOps.GROUPTOP}:   # green
       check(self.opts.has_local and self.opts.has_shared, "target does not support local or shared mem")
       check(axis >= self.first_reduce + self.group_for_reduces and axis < self.shape_len-self.upcasted, "must be reduce axis to group")
       check(not self.tensor_core, "can't group with tensor cores")
       self.shift_to(axis, amt, top=(opt.op is OptOps.GROUPTOP), insert_before=self.first_reduce + self.group_for_reduces)
       self.group_for_reduces += 1
@@ -471,15 +475,15 @@
       #self.shift_to(axis, amt, insert_before=None if upcast_count == 0 else self.shape_len-upcast_count)
       if self.full_shape[axis] == amt and axis == self.first_reduce: self.local_dims += 1 # first_reduce will ++, so offset loss in simplify_ones
       if self.full_shape[axis] == amt and axis < self.first_reduce+self.group_for_reduces: self.group_for_reduces -= 1 # fully unrolling a GROUP
       self.shift_to(axis, amt, insert_before=None)
       self.upcast()
     elif opt.op is OptOps.UPCAST:                     # yellow
       check(axis < self.first_reduce, "upcast is for non-reduce")
-      check(not(self.tensor_core and axis >= self.first_reduce-len(self.tensor_core.threads)), "can't upcast TC locals")
+      check(not(self.tensor_core and self.global_dims <= axis < self.global_dims+len(self.tensor_core.threads)), "can't upcast TC locals")
       check(amt <= 8, "don't upcast more than 8")
       self.shift_to(axis, amt, insert_before=None)
       self.upcast()
     elif opt.op is OptOps.UPCASTMID:                  # white
       check(self.bufs[0].dtype.name.startswith('image') and not self.float4_axis(0) and self.group_for_reduces != 0 and self.first_reduce <= 2 and prod(self.sts[0].shape) > 1, "invalid upcast mid reduce")  # noqa: E501
       axes = self.sts[0].unit_stride_axes()
       check(len(axes) == 1, f"wrong number of stride 1 axis : {axes}")
@@ -489,16 +493,17 @@
       self.group_for_reduces += 1
     elif opt.op is OptOps.NOLOCALS:
       check(self.opts.has_local and not self.dont_use_locals, "NOLOCALS is meaningless if target does not support local or already not using locals")
       check(self.local_dims == 0 and self.group_for_reduces == 0, "can't have no locals with locals")
       self.dont_use_locals = True
     elif opt.op is OptOps.PADTO:
       check(not self.vars, "does not work with symbolic shape")
+      check(axis < self.shape_len - self.upcasted, "cannot pad upcasted")
       # ok to pad SUM if all parent ops have f(0) = 0
-      if self.first_reduce <= axis < self.shape_len - self.upcasted:
+      if self.first_reduce <= axis:
         check(self.reduceop.op is ReduceOps.SUM and all(op.op not in UNSAFE_PAD_OPS for ops in self.reduceop.src for op in ops.lazyops), "cannot pad")
       padded = False
       for i,st in enumerate(self.sts):
         if self.sts[i].shape[axis] == 1: continue  # reduced
         check(self.sts[i].shape[axis] > amt//4, f"pad adds more than quadruple the work {self.sts[i].shape[axis]=} > {amt//4=}")
         if (ru := round_up(cast(int, self.sts[i].shape[axis]), cast(int, amt)) - self.sts[i].shape[axis]):
           # pad right seems to be faster
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/codegen/linearizer.py` & `tinygrad_tools-0.8.2/tinygrad/codegen/linearizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 from __future__ import annotations
 from typing import List, Tuple, Any, Optional, cast, DefaultDict, Dict, Union, Final, Iterator, Sequence
 import itertools, math, functools
 from collections import defaultdict
 
 from tinygrad.dtype import ImageDType, dtypes, DType, PtrDType, ConstType
 from tinygrad.helpers import colored, DEBUG, prod, getenv, to_function_name
-from tinygrad.ops import LazyOp, UnaryOps, BinaryOps, TernaryOps, ReduceOps, ConstBuffer, MemBuffer, BufferOps
+from tinygrad.ops import LazyOp, UnaryOps, BinaryOps, TernaryOps, ReduceOps, ConstBuffer, MemBuffer, BufferOps, get_lazyop_info
 from tinygrad.shape.shapetracker import ShapeTracker
 from tinygrad.shape.symbolic import Variable, NumNode, Node, SumNode, MulNode, DivNode, ModNode, LtNode, AndNode, create_lt_node
 from tinygrad.codegen.kernel import LocalBuffer, Kernel
-from tinygrad.features.image import to_image_idx
+from tinygrad.renderer import Program
 
 from tinygrad.codegen.uops import UOps, UOp, UOpGraph
 
 def get_grouped_dims(prefix, start_dim, local_dims, maxdim:int=0):
-  local_idxs = loop_local_idxs = [Variable(f"{prefix}{start_dim+i}", 0, s-1) for i,s in enumerate(local_dims[0:maxdim-1] + (prod(local_dims[maxdim-1:]),) if len(local_dims) > maxdim else local_dims)]  # noqa: E501
+  local_idxs = loop_local_idxs = [Variable(f"{prefix}{start_dim+i}", 0, s-1) for i,s in enumerate((prod(local_dims[:-(maxdim-1)]),) + local_dims[-(maxdim-1):] if len(local_dims) > maxdim else local_dims)]  # noqa: E501
   if maxdim != 0 and len(local_dims) > maxdim:
-    dd = local_idxs[maxdim-1]
+    dd = local_idxs[0]
     nli = []
-    for s in local_dims[maxdim-1:][::-1]:
+    for s in local_dims[:-(maxdim-1)]:
       nli.append(dd % s)
       dd //= s
-    local_idxs = local_idxs[0:maxdim-1] + nli[::-1]
+    local_idxs = nli + local_idxs[-(maxdim-1):]
   return local_idxs, [x for x in loop_local_idxs if not isinstance(x, NumNode)]
 
 def expand_idx(node:Node) -> Union[Variable, NumNode]: return next((v for v in node.vars() if v.expr.startswith("_uidx")), NumNode(0))
 def expand_idxs(nodes:Sequence[Node]) -> Tuple[Union[Variable, NumNode], ...]:
   eidxs = [expand_idx(node) for node in nodes]
   return tuple([v if v not in eidxs[:j] else NumNode(0) for j, v in enumerate(eidxs)])  # take only first occurrence of expand variable
 def iter_idxs(idxs:Tuple[Union[Variable, NumNode], ...]) -> Iterator[Tuple[int,...]]:
   yield from (x[::-1] for x in itertools.product(*[[x for x in range(v.min, v.max + 1)] for v in idxs[::-1]]))
 
+def to_image_idx(base_shape:Tuple[int, ...], idxy:Node, valid:Node) -> Tuple[Tuple[Node, Node], Node]:
+  idx, idy = (idxy // 4) % base_shape[1], (idxy // (4 * base_shape[1]))
+  # TODO: bring back the valid removal logic (correct!)
+  if DEBUG>=5: print("to_image_idx", base_shape, idx.min, idx.max, idy.min, idy.max, idx, idy, valid)
+  return (idx, idy), valid
+
 # expand a Node into List[Node] that enumerates the underlying Variables from min to max
 # expand increments earlier variables faster than later variables (as specified in the argument)
 @functools.lru_cache(maxsize=None)
 def expand_node(node:Node, idxs:Optional[Tuple[Union[Variable, NumNode], ...]]=None) -> List[Node]:
   if idxs is None: idxs = (expand_idx(node),)
   return [node.substitute({k:v for k,v in zip(idxs, (NumNode(x) for x in rep)) if isinstance(k, Variable)}) for rep in iter_idxs(idxs)]
 
@@ -89,21 +95,23 @@
     # todo: multioutput test with different output valids to add if acc is None: g_valid = NumNode(1)
 
     if amt > 1: localtype = localtype.vec(amt)
     e_idxs, e_valids = expand_node(g_idx, expand_vars), expand_node(g_valid, expand_vars)
 
     ret = []
     invalid_value = 0
+    acc_count = 0
     for idx, valid, rep_idx in zip(e_idxs, e_valids, iter_idxs(expand_vars)):
       this_const, idx, valid = (invalid_value, NumNode(0), NumNode(1)) if valid.max == 0 else (const, idx, valid)
       # todo: when multiple reduceops are supported, clearly disambiguate and test acc load keys are unique for each reduceop
       key = f"{acc is not None}{localtype}{'CONST'+str(this_const) if this_const is not None and acc is None else (buf.idx if isinstance(buf, MemBuffer) else cast(LocalBuffer, buf).name)}{idx.render()}{valid.render()}"  # noqa: E501
       if key not in self.load_cache:
         if acc is not None:
-          self.load_cache[key] = self.uops.add(UOps.DEFINE_ACC, localtype, (), self.get_reduce_acc(acc), cachable=False)
+          self.load_cache[key] = self.uops.add(UOps.DEFINE_ACC, localtype, (), (self.get_reduce_acc(acc), i, acc_count))
+          acc_count += 1
         elif this_const is not None:
           self.load_cache[key] = self.const(this_const, localtype)
           if valid.min == 0 and valid.max == 1:
             valid_rendered = valid.render(self.render_ops, self)
             self.load_cache[key] = self.uops.add(UOps.ALU, localtype, (valid_rendered, self.load_cache[key], self.const(invalid_value, localtype)), TernaryOps.WHERE)  # noqa: E501
         elif isinstance(buf.dtype, ImageDType):
           buf_uop = self.buf_uops[i]
@@ -164,18 +172,18 @@
       else:
         rendered_idx = idx.render(self.render_ops, self)
       if valid.min == 1: stores.append(self.uops.add(UOps.STORE, None, (buf_uop, rendered_idx, var)))
       else: stores.append(self.uops.add(UOps.STORE, None, (buf_uop, rendered_idx, var, valid.render(self.render_ops, self))))
     return stores
 
   # render loop
-  def render_loop(self, xx:List[Variable]) -> Tuple[UOp, ...]:
+  def render_loop(self, xx:List[Variable], nm:str) -> Tuple[UOp, ...]:
     new_loops = {x.expr:self.uops.add(UOps.LOOP, dtypes.int32, (
       self.const(x.min) if isinstance(x.min, int) else cast(Node, x.min).render(self.render_ops, self),
-      self.const(x.max+1) if isinstance(x.max, int) else cast(Node, x.max+1).render(self.render_ops, self)), cachable=False) for x in xx if not isinstance(x, NumNode) and x.expr is not None}  # noqa: E501
+      self.const(x.max+1) if isinstance(x.max, int) else cast(Node, x.max+1).render(self.render_ops, self)), arg=(nm,i)) for i,x in enumerate(xx) if not isinstance(x, NumNode) and x.expr is not None}  # noqa: E501
     self.loop_uops.update(new_loops)
     return tuple(new_loops.values())
 
   def render_reduceop(self, reduceop: LazyOp, loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]], \
                       global_idxs, local_idxs, upcast_idxs):
     # define indicies
     full_upcast_idxs = [Variable(f"_uidx{i}", 0, s-1) for i, s in enumerate(self.full_shape[self.shape_len-self.upcasted:])]
@@ -187,48 +195,48 @@
       for s in local_sizes:
         thread_idxs.append(thread_idx % s)
         thread_idx //= s
       for alias in aliases:
         full_var, full_var_sz = NumNode(0), 1
         if alias[0] != 0:
           for i in alias:
-            next_var = local_idxs[-i] if i > 0 else thread_idxs[-i-1]
+            next_var = local_idxs[i-1] if i > 0 else thread_idxs[-i-1]
             full_var += next_var * full_var_sz
             full_var_sz *= next_var.max+1
         replace_idxs.append(full_var)
       return replace_idxs
 
     # compute local aliases - modify idxs if necessary for TC
     alias_buf_idxs = []
     for i in self.local_alias:
       localbuf_idx = self.bufs.index(self.local_alias[i])
       buf_idxs = [idx*0 if s == 0 else idx for idx,s in zip(global_idxs+local_idxs+reduce_idxs+full_upcast_idxs,self.sts[i].real_strides())]
       if (tc:=self.tensor_core):
         min_alias_idx = min(self.local_alias.keys())
         replace_input_idxs = calc_tc_idxs(tc.thread_local_sizes[i-min_alias_idx], tc.thread_local_aliases[i-min_alias_idx])
         for n in range(len(tc.threads)):
-          buf_idxs[self.first_reduce-len(tc.threads)+n] = replace_input_idxs[n] # replace locals
+          buf_idxs[self.global_dims+n] = replace_input_idxs[n] # replace locals
         for n in range(tc.num_upcasts()):
           buf_idxs[self.shape_len-self.upcasted+n] = replace_input_idxs[len(tc.threads)+n] # replace upcasts
       if DEBUG >= 3: print(f"{localbuf_idx} alias {i}: sts={self.sts[i]} idxs={buf_idxs}")
       alias_buf_idxs.append((i, localbuf_idx, buf_idxs,))
 
     # define accumulator - modify idxs if necessary for TC
     out_buf = -1 if self.group_for_reduces else 0
     if (tc:=self.tensor_core):
       replace_acc_idxs = calc_tc_idxs(tc.thread_local_sizes[2], tc.thread_local_aliases[2])
       for n in range(len(tc.threads)):
-        local_idxs[self.local_dims-len(tc.threads)+n] = replace_acc_idxs[n] # replace locals
+        local_idxs[n] = replace_acc_idxs[n] # replace locals
       for n in range(len(replace_acc_idxs)-len(tc.threads)):
         upcast_idxs[n] = replace_acc_idxs[len(tc.threads)+n] # replace upcasts
       if DEBUG >= 3: print(f"store alias: sts={self.sts[0]} idxs={global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs}")
     acc = self.global_load(out_buf, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, acc=reduceop)
 
     # reduce loop
-    loop_ctx = self.render_loop(reduce_idxs)
+    loop_ctx = self.render_loop(reduce_idxs, "2_reduce")
 
     # store local aliases
     locals_to_store = [(localbuf_idx, buf_idxs, self.global_load(i, buf_idxs)) for i, localbuf_idx, buf_idxs in alias_buf_idxs]
 
     if (tc:=self.tensor_core):
       # run tensor cores AST
       wmma_sz = [prod(l) for l in tc.thread_local_sizes]
@@ -260,20 +268,20 @@
     # end the reduce loop
     self.load_cache.clear()
 
     # end the local loop, do the local reduce
     if self.group_for_reduces:
       fake_global_idxs = [x*0 for x in global_idxs]
       stores = self.global_store(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, acc)  # store accumulators
-      barrier = self.uops.add(UOps.BARRIER, None, tuple(stores), cachable=False)
+      barrier = self.uops.add(UOps.BARRIER, None, tuple(stores))
       if self.opts.has_local:
         fake_idxs = [NumNode(0)]*len(self.sts[-1].shape)
         fake_idxs[self.global_dims+self.local_dims:self.global_dims+len(local_idxs)] = local_idxs[self.local_dims:]
         if_cond: UOp = create_lt_node(self.sts[-1].expr_idxs(fake_idxs)[0], 1).render(self.render_ops, self)
-        barrier = self.uops.add(UOps.IF, None, (if_cond, barrier), cachable=False)
+        barrier = self.uops.add(UOps.IF, None, (if_cond, barrier))
 
       # create new late reduce local loops and replace local_idxs that have been used
       end_local_idxs = [Variable(f"tidx{i}", 0, self.full_shape[i]-1 if i >= self.first_reduce and i not in self.upcast_in_mid_reduce_axes else 0) for i in range(0, self.first_reduce+self.group_for_reduces)]  # noqa: E501
       local_idxs = local_idxs[:self.local_dims] + end_local_idxs[self.global_dims + self.local_dims:]
 
       # if any group_for_reduce items aren't reduces, upcast them here
       for j in self.upcast_in_mid_reduce_axes:
@@ -287,15 +295,15 @@
 
       # NOTE: this structure is the same as the reduce op above
 
       # define late accumulator
       acc = self.global_load(0, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, acc=reduceop)
 
       # late reduce loop
-      loop_ctx = self.render_loop(end_local_idxs)
+      loop_ctx = self.render_loop(end_local_idxs, "3_late_reduce")
 
       # load localbufs
       loaded_buffers[self.bufs[-1]] = self.global_load(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, barrier=barrier)
 
       # there's no AST here (and there's no shape for the reduce LazyOp)
       self.ast_parse(LazyOp(reduceop.op, (LazyOp(BufferOps.LOAD, (), self.bufs[-1]),)), acc, self.acc_offsets(-1), loaded_buffers, do_reduce=True, loop_ctx=loop_ctx)  # noqa: E501
 
@@ -309,15 +317,15 @@
   kernel_cnt: Final[DefaultDict[str, int]] = defaultdict(int)
   def linearize(self):
     # no new opts and we already ran? skip relinearizing
     if self.applied_opts == self.applied_opts_cache: return self
 
     # late alias the tensor core buffers
     if (tc:=self.tensor_core) and (tc_opts:=self.tensor_core_opts):
-      alias_pattern = [0]*(self.global_dims+(self.local_dims-len(tc.threads))) + [2]*(len(tc.threads)) + [0]*(self.shape_len-self.upcasted-self.first_reduce) + [1]*tc.num_upcasts() + [3]*(self.upcasted-tc.num_upcasts())  # noqa: E501
+      alias_pattern = [0]*(self.global_dims) + [2]*(len(tc.threads)) + [0]*(self.local_dims-len(tc.threads)) + [0]*(self.shape_len-self.upcasted-self.first_reduce) + [1,1] + [3]*(self.upcasted-2)  # noqa: E501
       for tc_buf in tc_opts.bufs:
         self.alias_buffer(tc_buf, alias_pattern)
 
     # save backups
     sts_backup, gfr_backup, upc_backup = self.sts[:], self.group_for_reduces, self.upcasted
 
     # global uop cache
@@ -371,19 +379,21 @@
     # set global/local size
     self.global_size: Optional[List[int]] = None
     self.local_size: Optional[List[int]] = None
     if self.dont_use_locals:
       self.global_size = [x.max+1 for x in loop_global_idxs][::-1]
       self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (len(loop_global_idxs)-1-i, x.expr.replace("gidx", "idx"), x.max+1)) for i,x in enumerate(loop_global_idxs)})  # noqa: E501
     elif self.opts.has_local:
-      self.global_size, self.local_size = [x.max+1 for x in loop_global_idxs][::-1], [x.max+1 for x in loop_local_idxs][::-1]
+      self.global_size, self.local_size = [x.max+1 for x in loop_global_idxs][::-1], [x.max+1 for x in loop_local_idxs]
       self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (len(loop_global_idxs)-1-i, x.expr, x.max+1)) for i,x in enumerate(loop_global_idxs)})  # noqa: E501
-      self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (len(loop_local_idxs)-1-i, x.expr, x.max+1)) for i,x in enumerate(loop_local_idxs)})  # noqa: E501
+      self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (i, x.expr, x.max+1)) for i,x in enumerate(loop_local_idxs)})
     else:
-      self.render_loop(loop_global_idxs+loop_local_idxs)
+      self.render_loop(loop_global_idxs+loop_local_idxs, "1_global_local")
+    if self.global_size is not None: self.global_size += [1]*(3-len(self.global_size))
+    if self.local_size is not None: self.local_size += [1]*(3-len(self.local_size))
 
     # parse AST
     loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]] = {}
     acc: List[UOp] = []
     self.load_cache: Dict[str, UOp] = {}
 
     # reduce op
@@ -414,16 +424,16 @@
     self.applied_opts_cache = self.applied_opts[:]
     return self
 
   def ast_parse(self, x:LazyOp, acc: List[UOp], offs:Optional[List[int]], loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]], do_reduce=False, loop_ctx=tuple(), cache=None) -> List[UOp]: # noqa: E501
     if cache is None: cache = {}
     if x in cache: return cache[x]
     if x.op in BufferOps: return loaded_buffers[x.arg]
-    if x.op is UnaryOps.CAST: return [self.uops.add(UOps.BITCAST if x.arg[1] else UOps.CAST, self.get_base_dtype(x.arg[0]), (u,), x.arg[0]) \
-                                      for u in self.ast_parse(x.src[0], acc, offs, loaded_buffers)]
+    if x.op in [UnaryOps.CAST, UnaryOps.BITCAST]: return [self.uops.add(UOps.BITCAST if x.op is UnaryOps.BITCAST else UOps.CAST, \
+                                      self.get_base_dtype(x.arg), (u,), x.arg) for u in self.ast_parse(x.src[0], acc, offs, loaded_buffers)]
     if x.op in ReduceOps and not do_reduce:
       assert offs is None, "not available if we aren't doing reduce"
       return acc
 
     values = [self.ast_parse(v, acc, offs, loaded_buffers, loop_ctx=loop_ctx, cache=cache) for v in x.src]
     ops = {ReduceOps.SUM:BinaryOps.ADD, ReduceOps.MAX:BinaryOps.MAX}
     if x.op in ops:
@@ -435,7 +445,16 @@
       for off in range(len(acc)):
         if input_acc[off] != acc[off]:
           acc[off] = self.uops.add(UOps.PHI, input_acc[off].dtype, (input_acc[off], acc[off]) + tuple(loop_ctx))
     else:
       ret = [self.uops.add(UOps.ALU, dtypes.bool if x.op in {BinaryOps.CMPLT, BinaryOps.CMPEQ} else val[-1].dtype, val, x.op) for val in zip(*values)]
     cache[x] = ret
     return ret
+
+  def to_program(self) -> Program:
+    self.linearize()
+    info = get_lazyop_info(self.ast[0])
+    ops, mem = self.uops.flops_mem()
+    run_count = prod((self.global_size if self.global_size else []) + (self.local_size if self.local_size else []))
+    # NOTE: we use min here to ignore the indexing FLOPS
+    return Program(self.name, self.opts.render(to_function_name(self.name), self.uops), self.opts.device,
+                   self.global_size, self.local_size, self.uops, min(info.flops, ops * run_count), min(info.mem_estimate, mem * run_count))
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/codegen/uops.py` & `tinygrad_tools-0.8.2/tinygrad/codegen/uops.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,19 @@
           u.vin = tuple(n if x == o else x for x in u.vin)
       if rew := self.rewrite(u): replace[u] = rew
 
     for o,n in replace.items():
       queue = [n]
       while queue:
         if all([qq in uops.uops for qq in queue[-1].vin]):
-          q = queue.pop()
-          new = uops.add(q.uop, q.dtype, q.vin, q.arg, insert_before=max([0]+[uops.uops.index(vv) for vv in q.vin])+1)
-          for vv in uops.uops + queue: vv.vin = tuple(new if x is q else x for x in vv.vin)
+          new = uops.add_op(q:=queue.pop(), insert_before=max([0]+[uops.uops.index(vv) for vv in q.vin])+1)
+          if new != q:
+            for vv in uops.uops + queue: vv.vin = tuple(new if x is q else x for x in vv.vin)
         else: queue.extend([qq for qq in queue[-1].vin if qq not in uops.uops])
-      if not any([o in u.vin for u in uops]): uops.uops.remove(o)
+      if not any([o in u.vin for u in uops.uops[uops.uops.index(o):]]): uops.uops.remove(o)
 
 constant_folder = PatternMatcher([
   # const rules
   ({"__name__": "root", "uop": UOps.GEP, "vin": ({"__name__": "c", "uop": UOps.CONST},)}, lambda root, c: UOp.const(root.dtype, c.arg)),
   ({"__name__": "root", "uop": UOps.CAST, "vin": {"__name__": "c", "uop": UOps.CONST}}, lambda root, c: UOp.const(root.dtype, c.arg)),
   # a phi without loops (len(vin)==2) is a noop
   ({"uop": UOps.PHI, "vin": ({}, {"__name__": "x"})}, lambda x: x),
@@ -137,34 +137,35 @@
 
   def __iter__(self): return iter(self.uops)
 
   def vars(self) -> List[Variable]: return [x.arg for x in self.uops if x.uop is UOps.DEFINE_VAR]
   def globals(self) -> List[Tuple[int, bool]]: return [x.arg for x in self.uops if x.uop is UOps.DEFINE_GLOBAL]
 
   def graph(self):
-    from tinygrad.features.graph import graph_uops
+    from tinygrad.engine.graph import graph_uops
     graph_uops(self.uops)
 
   def print(self):
     for u in self.uops:
       print(f"{self.uops.index(u):4d} {str(u.uop):20s}: {str(u.dtype) if u.dtype is not None else '':25s} "
             f"{str([self.uops.index(x) for x in u.vin]):32s} {u.arg}")
 
-  def add(self, uop:UOps, dtype:Optional[DType]=None, vin:Tuple[UOp, ...]=tuple(), arg:Any=None, cachable=True, insert_before=None,
-          simplify=True) -> UOp:
-    ret = UOp(uop, dtype, vin, arg) if uop is not UOps.CONST else UOp.const(dtype, arg)
+  def add(self, uop:UOps, dtype:Optional[DType]=None, vin:Tuple[UOp, ...]=tuple(), arg:Any=None, insert_before=None, simplify=True) -> UOp:
+    return self.add_op(UOp(uop, dtype, vin, arg) if uop is not UOps.CONST else UOp.const(dtype, arg), insert_before, simplify)
+
+  def add_op(self, ret:UOp, insert_before=None, simplify=True) -> UOp:
     if simplify and (rewritten:=constant_folder.rewrite(ret)) is not None:
-      if rewritten in self.uops: return rewritten  # ignore cachable
+      if rewritten in self.uops: return rewritten
       ret = rewritten
     key = (ret.uop, ret.dtype, ret.vin, ret.arg)
     if insert_before is None: insert_before = len(self.uops)
     # check if the cached expr is valid with the given insert place.
-    if cachable and (expr:=self.saved_exprs.get(key, None)) is not None and self.uops.index(expr) <= insert_before: return expr
+    if (expr:=self.saved_exprs.get(key, None)) is not None and self.uops.index(expr) <= insert_before: return expr
     self.uops.insert(insert_before, ret)
-    if cachable: self.saved_exprs[key] = ret
+    self.saved_exprs[key] = ret
     return ret
 
   def remove_childless(self, keep:Set[UOp]):
     while 1:
       has_child: Set[UOp] = set()
       for ru in self.uops:
         for vu in ru.vin:
@@ -176,14 +177,15 @@
     self.saved_exprs = {k:v for k,v in self.saved_exprs.items() if v in nu}
 
   # optional
   def type_verify(self):
     for u in self.uops:
       uop, arg, vin, dtype = u.uop, u.arg, u.vin, u.dtype
       if uop in {UOps.CONST, UOps.DEFINE_ACC}:
+        if uop is UOps.DEFINE_ACC: arg = arg[0]
         assert dtype is not None and type(arg) is type(dtypes.as_const(arg, dtype)), f"type of {arg=} does not match {dtype}"
       if uop is UOps.ALU:
         if arg in UnaryOps:
           assert dtype == vin[0].dtype, f"{arg} dtype mismatch {dtype=} != {vin[0].dtype=}"
         elif arg in (BinaryOps.CMPLT, BinaryOps.CMPEQ):
           assert dtype == dtypes.bool, f"{arg} output dtype mismatch {dtype=} != {dtypes.bool}"
           assert vin[0].dtype == vin[1].dtype, f"{arg} dtype mismatch {dtype=} != {vin[0].dtype=} != {vin[1].dtype=}"
@@ -204,18 +206,18 @@
     return deps
 
   def add_ends(self):
     for u in self.uops:
       if u.uop is UOps.LOOP:
         # add END of loops after the last thing that (recursively) depends on them
         insert_before = self.uops.index(sorted(list(self.get_recursive_children(u)), key=self.uops.index)[-1])+1
-        self.add(UOps.ENDLOOP, None, (u,), cachable=False, insert_before=insert_before)
+        self.add(UOps.ENDLOOP, None, (u,), insert_before=insert_before)
       elif u.uop is UOps.IF:
         # END any if statements at the end of the uops
-        self.add(UOps.ENDIF, None, (u,), cachable=False)
+        self.add(UOps.ENDIF, None, (u,))
 
   def fix_loop_scope(self, get_recursive_parents:Callable[..., Set[UOp]]):
     loop_stack: List[List[UOp]] = [[]]
     # push uops upward out of loop if it does not depend on the loop
     for u in self.uops:
       if not loop_stack[-1]: loop_stack[-1].append(u)
       elif u.uop is UOps.LOOP: loop_stack.append([u])
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/device.py` & `tinygrad_tools-0.8.2/tinygrad/lazy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,249 +1,220 @@
 from __future__ import annotations
-import multiprocessing
-from collections import defaultdict
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, List, Optional, Dict, Tuple, ClassVar, cast
-import importlib, inspect, functools, pathlib, time, ctypes, os
-from tinygrad.helpers import prod, getenv, colored, all_int, to_function_name, from_mv, flat_mv, diskcache_get, diskcache_put, DEBUG, BEAM, NOOPT
-from tinygrad.shape.symbolic import Variable, sym_infer, sint
-from tinygrad.ops import LazyOp, get_lazyop_info
-from tinygrad.buffer import Buffer, BufferOptions
-from tinygrad.codegen.uops import UOpGraph
-
-if TYPE_CHECKING:
-  from tinygrad.codegen.linearizer import Linearizer
-
-# **************** Device ****************
-
-class _Device:
-  def __init__(self) -> None: self._devices: List[str] = [x.stem[len("ops_"):].upper() for x in (pathlib.Path(__file__).parent/"runtime").iterdir() if x.stem.startswith("ops_")]  # noqa: E501
-  @functools.lru_cache(maxsize=None)  # this class is a singleton, pylint: disable=method-cache-max-size-none
-  def _canonicalize(self, device:str) -> str: return (device.split(":", 1)[0].upper() + ((":"+device.split(":", 1)[1]) if ':' in device else '')).replace(":0", "")   # noqa: E501
-  # NOTE: you can't cache canonicalize in case Device.DEFAULT changes
-  def canonicalize(self, device:Optional[str]) -> str: return self._canonicalize(device) if device is not None else Device.DEFAULT
-  def __getitem__(self, ix:str) -> Compiled: return self.__get_canonicalized_item(self.canonicalize(ix))
-  @functools.lru_cache(maxsize=None)  # this class is a singleton, pylint: disable=method-cache-max-size-none
-  def __get_canonicalized_item(self, ix:str) -> Compiled:
-    if DEBUG >= 1: print(f"opening device {ix} from pid:{os.getpid()}")
-    assert multiprocessing.current_process().name == "MainProcess" or ix.split(":")[0] == "DISK", f"can only open device {ix} from parent"
-    x = ix.split(":")[0].upper()
-    return [cls for cname, cls in inspect.getmembers(importlib.import_module(f'tinygrad.runtime.ops_{x.lower()}')) if (cname.lower() == x.lower() + "device") and x in self._devices][0](ix)  # noqa: E501
-  @functools.cached_property
-  def DEFAULT(self) -> str:
-    device_from_env: Optional[str] = functools.reduce(lambda val, ele: ele if getenv(ele) == 1 else val, self._devices, None)   # type: ignore
-    if device_from_env: return device_from_env
-    for device in ["METAL", "HSA", "CUDA", "GPU", "CLANG", "LLVM"]:
-      try:
-        if self[device]:
-          os.environ[device] = "1"   # we set this in environment for spawned children
-          return device
-      except Exception: pass
-    raise RuntimeError("no usable devices")
-Device = _Device()
-
-# **************** base Runner + helpers ****************
-
-class Runner:
-  def __init__(self, display_name:str, dname:str, op_estimate:sint=0, mem_estimate:sint=0):
-    self.first_run, self.display_name, self.dname, self.op_estimate, self.mem_estimate = True, display_name, dname, op_estimate, mem_estimate
-  @property
-  def device(self): return Device[self.dname]
-  def exec(self, rawbufs:List[Buffer], var_vals:Optional[Dict[Variable, int]]=None) -> Optional[float]:
-    return self(rawbufs, {} if var_vals is None else var_vals)
-  def __call__(self, rawbufs:List[Buffer], var_vals:Dict[Variable, int], wait=False) -> Optional[float]:
-    raise NotImplementedError("override this")
-
-# **************** Buffer / Allocator ****************
-
-class BufferCopy(Runner):
-  def __init__(self, total_sz, dest_device, src_device):
-    if total_sz >= 1e6: name = f"{type(self).__name__[6:].lower()} {total_sz/1e6:7.2f}M, {dest_device[:7]:>7s} <- {src_device[:7]:7s}"
-    else: name = f"{type(self).__name__[6:].lower()} {total_sz:8d}, {dest_device[:7]:>7s} <- {src_device[:7]:7s}"
-    super().__init__(colored(name, "yellow"), dest_device, 0, total_sz)
-  def copy(self, dest, src):
-    if src.device.startswith("DISK") and hasattr(dest.allocator, 'copy_from_fd') and src.nbytes >= 4096 and hasattr(src.allocator.device, 'fd'):
-      dest.allocator.copy_from_fd(dest._buf, src.allocator.device.fd, src._buf.offset, src.nbytes)
-    elif src.device.startswith("DISK") and hasattr(dest.allocator, 'as_buffer'):
-      # fast(ish) path, uses readinto in diskbuffers
-      src.allocator.copyout(dest.allocator.as_buffer(dest._buf), src._buf)
-    else:
-      dest.copyin(src.as_buffer(allow_zero_copy=True))  # may allocate a CPU buffer depending on allow_zero_copy
-  def __call__(self, rawbufs:List[Buffer], var_vals:Dict[Variable, int], wait=False):
-    dest, src = rawbufs[0:2]
-    assert dest.size == src.size and dest.dtype == src.dtype, f"buffer copy mismatch, {dest.size} != {src.size}, {dest.dtype} != {src.dtype}"
-    st = time.perf_counter()
-    self.copy(dest, src)
-    if wait:
-      Device[dest.device].synchronize()
-      return time.perf_counter() - st
-
-class BufferXfer(BufferCopy):
-  def copy(self, dest, src):
-    if hasattr(dest.allocator.device, "track_cross_buffer") and hasattr(src.allocator, "track_cross_device"):
-      dest.allocator.device.track_cross_buffer.append(src)
-      src.allocator.track_cross_device.add(dest.allocator.device)
-    dest.allocator.transfer(dest._buf, src._buf, dest.nbytes, src_dev=src.allocator.device, dest_dev=dest.allocator.device)
-
-# TODO: size, dest, src are the same type. can we enforce this?
-class Allocator:
-  def alloc(self, size:int, options:Optional[BufferOptions]=None):
-    assert not isinstance(size, int) or size > 0, f"alloc size must be positve, getting {size}"
-    return self._alloc(size, options if options is not None else BufferOptions())
-  def _alloc(self, size:int, options:BufferOptions): raise NotImplementedError("need alloc")
-  def free(self, opaque, size:int, options:Optional[BufferOptions]=None):
-    self._free(opaque, options if options is not None else BufferOptions())
-  def _free(self, opaque, options:BufferOptions): pass  # if opaque is a Python object, you don't need a free
-  def copyin(self, dest, src:memoryview): raise NotImplementedError("need copyin")
-  def copyout(self, dest:memoryview, src): raise NotImplementedError("need copyout")
-
-class LRUAllocator(Allocator):  # pylint: disable=abstract-method
-  def __init__(self): self.cache: Dict[Tuple[int, Optional[BufferOptions]], Any] = defaultdict(list)
-  def alloc(self, size:int, options:Optional[BufferOptions]=None):
-    if len(c := self.cache[(size, options)]): return c.pop()
-    try: return super().alloc(size, options)
-    except (RuntimeError, MemoryError):
-      self.free_cache()
-      return super().alloc(size, options)
-  def free_cache(self):
-    for (sz,options),opaques in self.cache.items():
-      for opaque in opaques: super().free(opaque, sz, options)
-      opaques.clear()
-  def free(self, opaque:Any, size:int, options:Optional[BufferOptions]=None):
-    if getenv("LRU", 1) and (options is None or not options.nolru): self.cache[(size, options)].append(opaque)
-    else: super().free(opaque, size, options)
-
-class _MallocAllocator(LRUAllocator):
-  def _alloc(self, size:int, options:BufferOptions): return (ctypes.c_uint8 * size)()
-  def as_buffer(self, src) -> memoryview: return flat_mv(memoryview(src))
-  def copyin(self, dest, src:memoryview): ctypes.memmove(dest, from_mv(src), len(src))
-  def copyout(self, dest:memoryview, src): ctypes.memmove(from_mv(dest), src, len(dest))
-  def offset(self, buf, size:int, offset:int): return from_mv(self.as_buffer(buf)[offset:offset+size])
-
-MallocAllocator = _MallocAllocator()
-
-# **************** for Compiled Devices ****************
-
-@dataclass(frozen=True)
-class CompilerOptions:
-  device: str = ""
-  suffix: str = ""
-  # TODO: make this generic with a list of supported types
-  supports_float4: bool = True
-  has_local: bool = True
-  has_shared: bool = True
-  has_tensor_cores: bool = False
-  # NOTE: these two should be in z,y,x(reversed) order for cstyle backends, they are flipped when kernel is rendered
-  global_max: Optional[List[int]] = None
-  local_max: Optional[List[int]] = None
-  shared_max: int = 32768
-
-class Compiler:
-  compiler_opts: ClassVar[CompilerOptions]
-  def __init__(self, cachekey:Optional[str]=None): self.cachekey = None if getenv("DISABLE_COMPILER_CACHE") else cachekey
-  def render(self, name:str, uops:UOpGraph) -> str: raise NotImplementedError("need a render function")
-  def compile(self, src:str) -> bytes: raise NotImplementedError("need a compile function")
-  def compile_cached(self, src:str) -> bytes:
-    if self.cachekey is None or (lib := diskcache_get(self.cachekey, src)) is None:
-      lib = self.compile(src)
-      if self.cachekey is not None: diskcache_put(self.cachekey, src, lib)
-    return lib
-
-class CompiledRunner(Runner):
-  def __init__(self, name:str, prg:str, dname:str, global_size:Optional[List[int]]=None, local_size:Optional[List[int]]=None,
-               uops:Optional[UOpGraph]=None, op_estimate:sint=0, mem_estimate:sint=0, precompiled:Optional[bytes]=None):
-    if DEBUG >= 4: print(prg)
-    if global_size is not None: global_size = global_size + [1]*(3-len(global_size))
-    if local_size is not None: local_size = local_size + [1]*(3-len(local_size))
-    self.name, self.prg, self.global_size, self.local_size, self.first_run = \
-      to_function_name(name), prg, global_size, local_size, True
-    lib:bytes = precompiled if precompiled is not None else cast(Compiler, Device[dname].compiler).compile_cached(prg)
-    self.uops = uops
-    self.vars: List[Variable] = [] if uops is None else uops.vars()
-    self.globals: List[Tuple[int, bool]] = [] if uops is None else uops.globals()
-    self.lib, self.clprg, self.outcount = lib, Device[dname].runtime(self.name, lib), sum(x[1] for x in self.globals)
-    super().__init__(name, dname, op_estimate, mem_estimate)
-
-  def to_other_device(self, dname:str):
-    return CompiledRunner(self.display_name, self.prg, dname, self.global_size, self.local_size,
-                          self.uops, self.op_estimate, self.mem_estimate, self.lib)
-
-  def __reduce__(self):
-    return self.__class__, (self.display_name, self.prg, self.dname, self.global_size, self.local_size,
-                            self.uops, self.op_estimate, self.mem_estimate, self.lib)
-
-  def launch_dims(self, var_vals):
-    global_size = [sym_infer(sz, var_vals) for sz in self.global_size] if self.global_size is not None else self.global_size
-    local_size = [sym_infer(sz, var_vals) for sz in self.local_size] if self.local_size is not None else self.local_size
-    return global_size, local_size
-
-  def __call__(self, rawbufs:List[Buffer], var_vals:Dict[Variable, int], wait=False) -> Optional[float]:
-    global_size, local_size = self.launch_dims(var_vals)
-    if global_size is not None and local_size is None and all_int(self.global_size): # type: ignore[arg-type]
-      # TODO: this is copied from get_program
-      from tinygrad.features.search import optimize_local_size
-      local_size = self.local_size = optimize_local_size(self.clprg, global_size, rawbufs)
-      global_size = self.global_size = [g//l if g%l == 0 else g/l for g,l in zip(global_size, local_size)]
-    lra = {}
-    if global_size: lra['global_size'] = global_size
-    if local_size: lra['local_size'] = local_size
-    return self.clprg(*[x._buf for x in rawbufs], **lra, vals=tuple(var_vals[k] for k in self.vars), wait=wait)
-
-method_cache: Dict[Tuple[str, Tuple[LazyOp, ...], int, bool], CompiledRunner] = {}
-logkerns, logkerns_level = open(getenv("LOGKERNS", ""), "a") if getenv("LOGKERNS", "") else None, getenv("LOGKERNS_LEVEL", 1)
-class Compiled:
-  def __init__(self, device:str, allocator:Allocator, compiler:Optional[Compiler], runtime, graph=None):
-    self.dname, self.allocator, self.compiler, self.runtime, self.graph = device, allocator, compiler, runtime, graph
-  def synchronize(self): pass  # override this in your device
-
-  def to_program(self, k:Linearizer) -> CompiledRunner:
-    assert self.compiler is not None, "compiler is required to run AST"
-    k.linearize()
-    info = get_lazyop_info(k.ast[0])
-    ops, mem = k.uops.flops_mem()
-    run_count = prod((k.global_size if k.global_size else []) + (k.local_size if k.local_size else []))
-    # NOTE: we use min here to ignore the indexing FLOPS
-    ret = CompiledRunner(k.name, self.compiler.render(to_function_name(k.name), k.uops), self.dname, k.global_size, k.local_size,
-                         k.uops, min(info.flops, ops * run_count), min(info.mem_estimate, mem * run_count))
-    return ret
-
-  def get_linearizer(self, *ast:LazyOp) -> Linearizer:
-    assert self.compiler is not None, "compiler is required to build AST"
-    if DEBUG >= 3:
-      from tinygrad.features.graph import print_tree
-      for op in ast: print_tree(op)
-    from tinygrad.codegen.linearizer import Linearizer
-    k = Linearizer(*ast, opts=self.compiler.compiler_opts)
-    k.required_optimizations()
-    if not NOOPT:
-      if not (used_tensor_cores:=k.apply_tensor_cores(getenv("TC", 1))): k.hand_coded_optimizations()
-      if BEAM >= 1:
-        from tinygrad.features.search import beam_search, time_linearizer, bufs_from_lin
-        kb, k_opt = Linearizer(*ast, opts=self.compiler.compiler_opts), k
-        kb.required_optimizations()
-        rawbufs = bufs_from_lin(kb, allocate=False)
-        k = beam_search(kb, rawbufs, BEAM.value, bool(getenv("BEAM_ESTIMATE", 1)))
-        if getenv("BEAM_COMPARE", 1):
-          # TODO: move the HC/TC/BEAM compare to beam_search so it can be optionally cached which choice is better
-          lins: List[Tuple[str, Linearizer]] = [(f"beam{BEAM.value}", k), (("tc" if used_tensor_cores else "hc"), k_opt)]
-          if used_tensor_cores:
-            lins.append(("hc", Linearizer(*ast, opts=self.compiler.compiler_opts)))
-            lins[-1][1].hand_coded_optimizations()
-          timed = sorted([(nm, tk, time_linearizer(tk, rawbufs, allow_test_size=False, clear_l2=True)) for nm, tk in lins], key=lambda x: x[2])
-          if DEBUG >= 1: print("  <  ".join(f"{nm:6s} : {lin.colored_shape(30, dense=True)} : {tm*1e6:8.2f} us" for nm, lin, tm in timed))
-          k = timed[0][1]
-          if logkerns is not None and logkerns_level > 1: logkerns.writelines([f"{(lin.ast, lin.applied_opts)}\n" for (_,lin,_) in timed[1:]])
-    # TODO: check the correctness inline once compare_linearizer is in core
-    if logkerns is not None: logkerns.writelines([f"{(k.ast, k.applied_opts)}\n"])
-    if DEBUG >= 4: print((k.ast, k.applied_opts)) # print here to show final applied_opts for all kernels instead of just in beam_search
-    return k
-
-  def get_runner(self, *ast:LazyOp) -> CompiledRunner:
-    ckey = (self.dname, ast, BEAM.value, False)
-    if cret:=method_cache.get(ckey): return cret
-    bkey = (self.dname.split(":")[0], ast, BEAM.value, True)
-    if bret:=method_cache.get(bkey):
-      method_cache[ckey] = ret = bret.to_other_device(self.dname)
+import math
+from typing import Union, Optional, Any, Tuple, List
+from tinygrad.dtype import dtypes, DType, ConstType
+from tinygrad.helpers import prod, getenv, all_int, all_same, DEBUG
+from tinygrad.ops import LoadOps, UnaryOps, BinaryOps, TernaryOps, ReduceOps, Op, exec_alu, python_alu
+from tinygrad.shape.symbolic import sint, Variable
+from tinygrad.shape.shapetracker import ShapeTracker
+from tinygrad.device import Buffer
+from weakref import ref, ReferenceType, WeakValueDictionary
+
+lazycache: WeakValueDictionary[Any, LazyBuffer] = WeakValueDictionary()
+def create_lazybuffer(device:str, st:ShapeTracker, dtype:DType, op:Optional[Op]=None, arg:Any=None, srcs:Tuple[LazyBuffer, ...]=(),
+                      base:Optional[LazyBuffer]=None, enable_cache=bool(getenv("LAZYCACHE", 1))):
+  if st.size == 0: op, arg, srcs, base = LoadOps.CONST, 0, (), None
+  if op is LoadOps.CONST: arg, enable_cache = dtypes.as_const(arg, dtype) if not isinstance(arg, Variable) else arg, True
+
+  cache_key = (device, st, dtype, op, arg, tuple(ref(x) for x in srcs)) if base is None else (st, ref(base))
+  if enable_cache and (rret := lazycache.get(cache_key, None)): return rret
+
+  ret = LazyBuffer(device, st, dtype, op, arg, srcs, base=base)
+  if enable_cache: lazycache[cache_key] = ret
+  return ret
+
+view_supported_devices = {"LLVM", "CLANG", "CUDA", "DISK"}
+class LazyBuffer:
+  def __init__(self, device:str, st:ShapeTracker, dtype:DType,
+               op:Optional[Op]=None, arg:Any=None, srcs:Tuple[LazyBuffer, ...]=(),
+               base:Optional[LazyBuffer]=None):
+    self.device, self.st, self.dtype, self.shape, self.size = device, st, dtype, st.shape, st.size
+    self._base: Optional[LazyBuffer] = None
+    if base is None:
+      # properties on base
+      self.op, self.arg, self.srcs = op, arg, srcs  # this is a LazyOp, except the src is LazyBuffers and not LazyOps
+      assert self.op is not LoadOps.ASSIGN or srcs[1].base.realized is not None, "assign target must be realized"
+
+      if (self.op is LoadOps.CONTIGUOUS or self.op is UnaryOps.BITCAST) and srcs[0].st.consecutive and \
+          not srcs[0].is_unrealized_const() and device.split(":")[0] in view_supported_devices:
+        # some LazyBuffers can be processed with only a view, no AST required
+        self.buffer: Buffer = srcs[0].base.buffer.view(st.size, dtype, srcs[0].st.views[0].offset * srcs[0].dtype.itemsize)
+        self.op = LoadOps.VIEW
+      else:
+        self.buffer = srcs[1].base.buffer if self.op is LoadOps.ASSIGN else Buffer(device, self.size, dtype)
+      self.buffer.ref(1)
+      self.contiguous_child: Optional[Tuple[ReferenceType[LazyBuffer], ShapeTracker]] = None
+      self.forced_realize = False
     else:
-      method_cache[ckey] = method_cache[bkey] = ret = self.to_program(self.get_linearizer(*ast))
-    return ret
+      # properties on view
+      assert base.base == base, "base must be a base itself"
+      self._base = base
+
+  def __del__(self):
+    if hasattr(self, 'buffer'): self.buffer.ref(-1)
+
+  def __repr__(self) -> str:
+    return f"<LB {self.device} {self.shape} {str(self.dtype)[7:]} {self.st if self.base != self else (self.op, self.realized)}>"
+
+  @property
+  def realized(self) -> Optional[Buffer]:
+    # NOTE: we check for a lack of srcs instead of an allocated buffer to make unrealized assigns return None here
+    return self.buffer if self._base is None and not hasattr(self, 'srcs') else None
+
+  # NOTE: this has to be a function to prevent self reference
+  @property
+  def base(self) -> LazyBuffer: return self._base if self._base is not None else self
+
+  # same API as multi
+  @property
+  def lbs(self) -> List[LazyBuffer]: return [self]
 
+  @staticmethod
+  def loadop(op, shape:Tuple[sint,...], dtype:DType, device:str, arg=None, src:Tuple[LazyBuffer, ...]=(), enable_cache=False) -> LazyBuffer:
+    assert isinstance(src, tuple)
+    return create_lazybuffer(device, ShapeTracker.from_shape(shape), dtype, op, arg, src, enable_cache=enable_cache)
+
+  def const(self, val:ConstType, shape:Optional[Tuple[sint,...]]=None) -> LazyBuffer:
+    shape = self.shape if shape is None else shape
+    return LazyBuffer.loadop(LoadOps.CONST, tuple(), self.dtype, self.device, arg=val).reshape((1,)*len(shape)).expand(shape)
+
+  def is_realized(self) -> bool: return self.base.realized is not None
+
+  def assign(self, x:LazyBuffer) -> LazyBuffer:
+    assert x.size == self.size, f"assign target must have same size {self.size=} != {x.size=}"
+    return LazyBuffer.loadop(LoadOps.ASSIGN, self.shape, self.dtype, self.device, arg=() if self.st.contiguous else (self.st,), src=(x, self.base))
+
+  def contiguous(self):
+    if not self.st.contiguous or self.size != self.base.size or self.is_unrealized_const():
+      ret = self.e(LoadOps.CONTIGUOUS)
+      if (sti := self.st.invert(self.base.shape)) is not None: self.base.contiguous_child = ref(ret), sti
+      return ret
+    self.base.forced_realize = True
+    return self
+
+  def cast(self, dtype:DType, bitcast:bool=False):
+    if self.dtype == dtype: return self
+    if self.device.startswith("DISK") and not bitcast: raise RuntimeError("attempted to cast disk buffer (bitcast only)")
+    if self.is_unrealized_unmasked_const() and not bitcast:
+      return create_lazybuffer(self.device, self.st, dtype, LoadOps.CONST, dtypes.as_const(self.base.arg, dtype))
+    # TODO: applying this makes gpt2 slower
+    if getenv("CAST_BEFORE_VIEW", 1) and dtype.itemsize <= self.dtype.itemsize and self != self.base:
+      return self.base.cast(dtype, bitcast)._view(self.st)
+    new_shape = self.shape
+    if bitcast and self.dtype.itemsize != dtype.itemsize:
+      if not self.device.startswith("DISK"): raise RuntimeError("shape changing bitcast only supported on DISK right now")
+      if not all_int(new_shape): raise RuntimeError("shape changing bitcast with symbolic shape isn't supported yet")
+      # https://pytorch.org/docs/stable/generated/torch.Tensor.view.html
+      if not (new_shape[-1]*self.dtype.itemsize) % dtype.itemsize == 0: raise RuntimeError("unsupported size in bitcast")
+      new_shape = new_shape[:-1] + ((new_shape[-1]*self.dtype.itemsize) // dtype.itemsize,)
+    cast_op = UnaryOps.BITCAST if bitcast else UnaryOps.CAST
+    return create_lazybuffer(self.device, ShapeTracker.from_shape(new_shape), dtype, cast_op, dtype, (self,))
+
+  def is_unrealized_const(self): return self.base.realized is None and self.base.op is LoadOps.CONST and not isinstance(self.base.arg, Variable)
+  def is_unrealized_unmasked_const(self): return self.is_unrealized_const() and all(v.mask is None for v in self.st.views)
+
+  def _copy(self, device:str) -> LazyBuffer:
+    return create_lazybuffer(device, ShapeTracker.from_shape(self.shape), self.dtype, LoadOps.COPY, self.buffer.nbytes, (self,), enable_cache=False)
+
+  def copy_to_device(self, device:str, force: bool = False) -> LazyBuffer:
+    # no COPY
+    if self.device == device: return self
+
+    # double COPY = one COPY
+    if not force and self.st.contiguous and self.size == self.base.size and not self.base.realized and self.base.op is LoadOps.COPY:
+      return self.base.srcs[0].copy_to_device(device).reshape(self.st.shape)
+
+    # const doesn't have to be copied (issues with disk tensor)
+    if self.is_unrealized_const():
+      return LazyBuffer.loadop(LoadOps.CONST, tuple(), self.dtype, device, arg=self.base.arg)._view(self.st)
+
+    # if it's a shrink, do the shrink before the copy with CONTIGUOUS
+    if prod(self.st.shape) < prod(self.base.st.shape): return self.contiguous()._copy(device)
+
+    # copy the base and apply the shapetracker on the new device
+    return self.base._copy(device)._view(self.st)
+
+  def e(self, op:Union[LoadOps, UnaryOps, BinaryOps, TernaryOps], *in_srcs:LazyBuffer, arg:Optional[Any]=None) -> LazyBuffer:
+    srcs: List[LazyBuffer] = []
+    for s in (self,)+in_srcs:
+      if s == s.base and s.base.contiguous_child and (root:=s.base.contiguous_child[0]()) is not None:
+        srcs.append(root._view(s.base.contiguous_child[1]))
+      else:
+        srcs.append(s)
+    assert all_same(dts:=[x.dtype.scalar() for x in (srcs[1:] if op is TernaryOps.WHERE else srcs)]), f"all dtypes must match {dts} on {op}"
+    assert all_same([x.shape for x in srcs]), f"all shapes must be the same {[x.shape for x in srcs]}"
+    if op is TernaryOps.WHERE: assert srcs[0].dtype == dtypes.bool, "TernaryOps.WHERE must have the first arg be bool"
+    if op is UnaryOps.NEG: assert srcs[0].dtype != dtypes.bool, "UnaryOps.NEG does not accept dtype bool"
+
+    out_dtype = dtypes.bool if op in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else srcs[-1].dtype
+
+    # const folding
+    if op in python_alu and all(s.is_unrealized_unmasked_const() for s in srcs):
+      return self.cast(out_dtype).const(exec_alu(op, out_dtype, [s.base.arg for s in srcs]))
+    if op is UnaryOps.NEG and self.base.op is UnaryOps.NEG: return self.base.srcs[0]
+    if op in BinaryOps: x, y = self, in_srcs[0]
+    if op is BinaryOps.ADD:
+      if y.is_unrealized_unmasked_const() and y.base.arg == 0: return x # pylint: disable=possibly-used-before-assignment
+      if x.is_unrealized_unmasked_const() and x.base.arg == 0: return y # pylint: disable=possibly-used-before-assignment
+    if op is BinaryOps.SUB and y.is_unrealized_unmasked_const() and y.base.arg == 0: return x
+    if op is BinaryOps.MUL:
+      if x.is_unrealized_unmasked_const() and (val := x.base.arg) in (1, 0, -1):
+        return y if val == 1 else y.const(0) if val == 0 else y.e(UnaryOps.NEG)
+      if y.is_unrealized_unmasked_const() and (val := float(y.base.arg)) in (1, 0, -1):
+        return x if val == 1 else x.const(0) if val == 0 else x.e(UnaryOps.NEG)
+    if op is BinaryOps.DIV and dtypes.is_float(x.dtype) and y.is_unrealized_unmasked_const() and y.base.arg != 0:
+      return x.e(BinaryOps.MUL, x.const(1 / y.base.arg))
+
+    return create_lazybuffer(self.device, ShapeTracker.from_shape(self.shape), out_dtype, op, arg, tuple(srcs))
+
+  # *** reduce ops ***
+
+  def _reduce_op(self, op:ReduceOps, axis:Tuple[int, ...]) -> LazyBuffer:
+    assert all(0 <= x < len(self.shape) for x in axis), f"axis args {axis} out of range for shape {self.shape}"
+    axis = tuple(x for x in axis if self.shape[x] != 1)
+    if len(axis) == 0: return self
+    new_shape = tuple(1 if i in axis else s for i,s in enumerate(self.shape))
+    return create_lazybuffer(self.device, ShapeTracker.from_shape(new_shape), self.dtype, op, axis, (self,))
+
+  def r(self, op:ReduceOps, axis:Tuple[int, ...]) -> LazyBuffer:
+    new_shape = tuple(1 if i in axis else s for i,s in enumerate(self.shape))
+    # TODO: this logic should move to the scheduler
+    if self.size == 0 and 0 not in new_shape: return self.const({ReduceOps.SUM: 0.0, ReduceOps.MAX: -math.inf}[op], new_shape)
+
+    # const folding
+    if self.is_unrealized_unmasked_const():
+      return self.const(self.base.arg * {ReduceOps.SUM: prod(self.shape[i] for i in axis), ReduceOps.MAX: 1}[op], new_shape)
+
+    # TODO: can we split symbolic shape if the reduce axis is not symbolic?
+    if not getenv("SPLIT_REDUCEOP", 1) or not all_int(self.shape) or (0 in self.shape) or \
+      prod(self.shape) // prod(new_shape) < getenv("REDUCEOP_SPLIT_THRESHOLD", 32768):
+      return self._reduce_op(op, axis)
+
+    # if there are few globals, make some reduces into globals by splitting into two kernels
+    # cap output buffer to 2**22: heuristic number of global outputs to achieve max occupancy with enough locals+upcasts for gemm
+    #   ~2**10 should be enough if GROUP is used
+    # 256 split maximum should be "negligible reduce" for low prod(new_shape), 8 split minimum.
+    # split is moved to the end to provide maximum locality for the second phase reduce.
+    self_real_strides = self.st.real_strides(ignore_valid=True)
+    split_candidates = [(i, x) for i in axis for x in range(min(256,2**getenv("REDUCEOP_SPLIT_SIZE",22)//prod(new_shape)),8-1,-1)
+                        if self.shape[i] % x == 0 and self_real_strides[i] != 0]
+    if not split_candidates: return self._reduce_op(op, axis)
+    dim_to_split, divisor = split_candidates[0]
+    splitted_shape = self.shape[:dim_to_split] + (divisor,) + (self.shape[dim_to_split]//divisor,) + self.shape[dim_to_split+1:]
+    splitted = self.reshape(splitted_shape).permute(tuple([x for x in range(len(splitted_shape)) if x != dim_to_split]+[dim_to_split]))
+    if DEBUG >= 3: print(f"split {divisor}: {self.shape} -> {splitted.shape} -> {new_shape}")
+    return splitted._reduce_op(op, axis)._reduce_op(op, (len(new_shape),)).reshape(new_shape)  # reduce original axes, then split
+
+  # *** movement ops ***
+
+  def _view(self, new_st:ShapeTracker) -> LazyBuffer:
+    if self.st.size == 0 or (new_st.views[-1].mask is not None and any((x[1]-x[0]) == 0 for x in new_st.views[-1].mask)):
+      return self.const(0, new_st.shape)
+    if new_st.contiguous and self.base.shape == new_st.shape: return self.base
+    return create_lazybuffer(self.device, new_st, self.dtype, base=self.base)
+
+  def reshape(self, arg:Tuple[sint, ...]): return self._view(self.st.reshape(arg))
+  def pad(self, arg:Tuple[Tuple[sint, sint], ...]): return self._view(self.st.pad(arg))
+  def expand(self, arg:Tuple[sint, ...]): return self._view(self.st.expand(arg))
+  def permute(self, arg:Tuple[int, ...]): return self._view(self.st.permute(arg))
+  def shrink(self, arg:Tuple[Tuple[sint, sint], ...]): return self._view(self.st.shrink(arg))
+  def stride(self, arg:Tuple[int, ...]): return self._view(self.st.stride(arg))
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/dtype.py` & `tinygrad_tools-0.8.2/tinygrad/dtype.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,7 +101,13 @@
 def least_upper_dtype(*ds:DType) -> DType:
   return min(set.intersection(*[_get_recursive_parents(d) for d in ds])) if not (images:=[d for d in ds if isinstance(d, ImageDType)]) else images[0]
 def least_upper_float(dt:DType) -> DType: return dt if dtypes.is_float(dt) else least_upper_dtype(dt, dtypes.float32)
 
 # HACK: staticmethods are not callable in 3.8 so we have to compare the class
 DTYPES_DICT = {k: v for k, v in dtypes.__dict__.items() if not (k.startswith(('__', 'default')) or v.__class__ is staticmethod)}
 INVERSE_DTYPES_DICT = {v.name:k for k,v in DTYPES_DICT.items()}
+
+def sum_acc_dtype(dt:DType):
+  # default acc dtype for sum
+  if dtypes.is_unsigned(dt): return least_upper_dtype(dt, dtypes.uint)
+  if dtypes.is_int(dt) or dt == dtypes.bool: return least_upper_dtype(dt, dtypes.int)
+  return least_upper_dtype(dt, dtypes.float)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/engine/jit.py` & `tinygrad_tools-0.8.2/tinygrad/engine/jit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 from typing import TypeVar, Generic, Callable, List, Tuple, Union, Dict, cast, Optional, Any
 import functools, itertools, collections
 from tinygrad.tensor import Tensor
 from tinygrad.lazy import LazyBuffer
 from tinygrad.helpers import flatten, merge_dicts, DEBUG, Context, GRAPH, BEAM, getenv, all_int, GraphException, colored, JIT
-from tinygrad.device import Buffer, CompiledRunner, BufferXfer, Compiled, Device, Runner
+from tinygrad.device import Buffer, Compiled, Device
 from tinygrad.dtype import DType
 from tinygrad.shape.shapetracker import ShapeTracker
 from tinygrad.shape.symbolic import Variable, sint
-from tinygrad.engine.realize import ExecItem, capturing, _internal_memory_planner, EmptyOp, ViewOp
+from tinygrad.engine.realize import ExecItem, capturing, EmptyOp, ViewOp, BufferXfer, CompiledRunner, Runner
+from tinygrad.engine.schedule import _internal_memory_planner
 from tinygrad.nn.state import get_parameters
 from weakref import WeakKeyDictionary
 
 def apply_graph_to_jit(jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]) -> List[ExecItem]:
   # Split JIT cache into batches for faster graph execution.
   # This allows the accelerator to run some batches while subsequent graphs are still being updated.
   max_batch_size = getenv("JIT_BATCH_SIZE", 32)
@@ -36,20 +37,22 @@
     current_batch = []
     current_device = None
 
   for ji in jit_cache:
     if ji.prg.__class__ in {EmptyOp, ViewOp}: continue
     ji_graph_dev: Optional[Compiled] = None # device on which the ji will be graphed. Not graphed if None.
     if isinstance(ji.prg, CompiledRunner): ji_graph_dev = ji.prg.device
-    elif isinstance(ji.prg, BufferXfer) and ji.bufs[0] and ji.bufs[0].device.split(":", 1)[0] in {"HSA", "CUDA"}:
+    elif isinstance(ji.prg, BufferXfer) and ji.bufs[0] and ji.bufs[0].device.split(":", 1)[0] in {"HSA", "CUDA", "NV", "AMD"}:
       ji_graph_dev = Device[ji.bufs[0].device]
 
+    graph_class = (ji_graph_dev.graph.func if isinstance(ji_graph_dev.graph, functools.partial) else ji_graph_dev.graph) if ji_graph_dev else None #type: ignore
     can_be_graphed = ji_graph_dev and ji_graph_dev.graph
-    can_extend_graph_batch = can_be_graphed and len(current_batch) < max_batch_size and (ji_graph_dev == current_device or
-      (isinstance(ji_graph_dev.graph, type) and issubclass(ji_graph_dev.graph, MultiGraphRunner) and type(ji_graph_dev) == type(current_device))) #type:ignore
+    can_share_graph = (ji_graph_dev == current_device or (isinstance(graph_class, type) and issubclass(graph_class, MultiGraphRunner)) and
+                       type(ji_graph_dev) == type(current_device))
+    can_extend_graph_batch = can_be_graphed and len(current_batch) < max_batch_size and can_share_graph
     if not can_extend_graph_batch and len(current_batch) > 0: flush_batch()
 
     if can_be_graphed: current_batch.append(ji)
     else: graphed_jit_cache.append(ji)
 
     current_device = ji_graph_dev
 
@@ -72,16 +75,16 @@
     self.jc_idx_with_updatable_var_vals = []
     op_estimate: sint = 0
     mem_estimate: sint = 0
     for j,ji in enumerate(jit_cache):
       op_estimate += ji.prg.op_estimate
       mem_estimate += ji.prg.mem_estimate
       if isinstance(ji.prg, CompiledRunner):
-        if ji.prg.vars: self.jc_idx_with_updatable_var_vals.append(j)
-        if (ji.prg.global_size and not all_int(ji.prg.global_size)) or (ji.prg.local_size and not all_int(ji.prg.local_size)):
+        if ji.prg.p.vars: self.jc_idx_with_updatable_var_vals.append(j)
+        if (ji.prg.p.global_size and not all_int(ji.prg.p.global_size)) or (ji.prg.p.local_size and not all_int(ji.prg.p.local_size)):
           self.jc_idx_with_updatable_launch_dims.append(j)
     self.vars = list(var_vals.keys())
     super().__init__(colored(f"<batched {len(self.jit_cache)}>", "cyan"), jit_cache[0].prg.dname.split(":")[0], op_estimate, mem_estimate)
 
 class MultiGraphRunner(GraphRunner):  # pylint: disable=abstract-method
   def __init__(self, jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
     self.w_dependency_map: Dict[Any, Any] = {}
@@ -173,15 +176,16 @@
       # Condense the items into a graph executor.
       if JIT < 2: self.jit_cache = apply_graph_to_jit(self.jit_cache, input_rawbuffers, var_vals)
 
       self.input_replace = get_input_replace(self.jit_cache, input_rawbuffers)
       if DEBUG >= 1 and len(set(self.input_replace.values())) != len(input_rawbuffers): print("WARNING: some input tensors not found")
     elif self.cnt >= 2:
       # jit exec
-      assert self.expected_names == expected_names and self.expected_lbs == expected_lbs, "args mismatch in JIT"
+      assert self.expected_names == expected_names, f"args mismatch in JIT: {self.expected_names=} != {expected_names}"
+      assert self.expected_lbs == expected_lbs, f"args mismatch in JIT: {self.expected_lbs=} != {expected_lbs=}"
       for idx, offset, device, size, dtype in self.extra_view_inputs:
         input_rawbuffers.append(Buffer(device, size, dtype, base=input_rawbuffers[idx], offset=offset).ensure_allocated())
       for (j,i),input_idx in self.input_replace.items(): self.jit_cache[j].bufs[i] = input_rawbuffers[input_idx]
       if DEBUG >= 1 and len(self.jit_cache) >= 10: print(f"jit execs {len(self.jit_cache)} kernels")
       for ei in self.jit_cache: ei.run(var_vals, jit=True)
 
     # clear jit inputs
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/engine/schedule.py` & `tinygrad_tools-0.8.2/tinygrad/engine/schedule.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 import sys, pickle, atexit
 from collections import defaultdict, deque
 from dataclasses import dataclass
-from typing import Tuple, List, Dict, Optional, Set, DefaultDict
-from tinygrad.ops import LoadOps, ScheduleItem, BufferOps, LazyOp, ReduceOps, ConstBuffer, MemBuffer, UNSAFE_PAD_OPS, UnaryOps
-from tinygrad.features.graph import log_lazybuffer, realized_lazybuffer
+from typing import Tuple, List, Dict, Optional, Set, DefaultDict, Union
+from tinygrad.ops import LoadOps, BufferOps, LazyOp, ReduceOps, ConstBuffer, MemBuffer, UNSAFE_PAD_OPS, UnaryOps
+from tinygrad.engine.graph import log_lazybuffer, realized_lazybuffer
 from tinygrad.helpers import GRAPH, DEBUG, MULTIOUTPUT, SAVE_SCHEDULE, GlobalCounters, prod, dedup, all_int, merge_dicts, getenv
 from tinygrad.shape.symbolic import Variable
-from tinygrad.dtype import ImageDType, dtypes
+from tinygrad.dtype import ImageDType, dtypes, DType
 from tinygrad.lazy import LazyBuffer
 from tinygrad.shape.shapetracker import ShapeTracker
+from tinygrad.device import Buffer
 
 # creation can recurse a lot
 sys.setrecursionlimit(10000)
 
 # optionally log the ops to disk
 logops = open(getenv("LOGOPS", ""), "a") if getenv("LOGOPS", "") else None
 
+# *** ScheduleItem return type ***
+
+@dataclass(frozen=True)
+class ScheduleItem:
+  ast: Tuple[LazyOp, ...]
+  bufs: Tuple[Buffer, ...]
+  @property
+  def outputs(self) -> Tuple[Buffer, ...]:
+    """Read/write or write only buffers in the schedule."""
+    return self.bufs[:len(self.ast)]
+  @property
+  def inputs(self) -> Tuple[Buffer, ...]:
+    """Read only buffers in the schedule."""
+    return self.bufs[len(self.ast):]
+
+# *** DAG transformation: List[LazyBuffer] -> ScheduleItem ***
+
 # TODO: it's unfortunate this needs to exist, but because of ASSIGN, we have to retain the LazyBuffer structure until post toposort
 @dataclass(frozen=True)
 class _LBScheduleItem:
   ast: Tuple[LazyOp, ...]
   outputs: Tuple[LazyBuffer, ...]
   inputs: Tuple[LazyBuffer, ...]
   var_vals: Dict[Variable, int]
 
-# recursively create a lazyop
-def _recursive_lazyop(buf:LazyBuffer, inputs:List[LazyBuffer], outbufs:Tuple[LazyBuffer, ...], var_vals:Dict[Variable, int], st:ShapeTracker,
-                      realizes:Dict[LazyBuffer, None], cache, assign_to:Optional[LazyBuffer]=None, assign_idx:Optional[int]=None) -> LazyOp:
+def _recursive_lazyop(buf:LazyBuffer, inputs:List[LazyBuffer], outputs:Tuple[LazyBuffer, ...], var_vals:Dict[Variable, int], st:ShapeTracker,
+                      realizes:Dict[LazyBuffer, None], assign_targets:Dict[LazyBuffer, LazyBuffer], cache) -> LazyOp:
+  """recursively create a lazyop"""
   if (buf, st) in cache: return cache[(buf, st)]
   if buf != buf.base:
     st = buf.st + st
     buf = buf.base
   # all buffers here are base now
   assert buf.op is not None
 
@@ -38,204 +56,217 @@
   if buf.op is LoadOps.CONST:
     unbound_st, st_var_vals = st.simplify().unbind()
     var_vals.update(st_var_vals)
     if isinstance(buf.arg, Variable): var_vals.__setitem__(*buf.arg.unbind())
     return LazyOp(BufferOps.CONST, (), ConstBuffer(buf.arg, buf.dtype, unbound_st))
 
   # if we aren't fusing it, it's a load and we add it to the inputs
-  if buf.realized or (buf in realizes and buf not in outbufs):
+  if buf.realized is not None or (buf in realizes and buf not in outputs):
     unbound_st, st_var_vals = st.simplify().unbind()
     var_vals.update(st_var_vals)
-    if assign_to is not None and buf is assign_to:
-      assert assign_idx is not None
+    if buf in assign_targets:
+      # can only assign to contiguous read+write buffer
       if not unbound_st.contiguous:
         # we also allow masked views. if it has a single view and it's equal when you shrink a contig, it's fine
         if not (len(unbound_st.views) == 1 and unbound_st.views[0].mask is not None and
             ShapeTracker.from_shape(unbound_st.shape).shrink(unbound_st.views[0].mask) == unbound_st.shrink(unbound_st.views[0].mask)):
           raise RuntimeError(f"must be contiguous for assign {unbound_st}")
-      return LazyOp(BufferOps.LOAD, (), MemBuffer(assign_idx, buf.dtype, unbound_st))
+      return LazyOp(BufferOps.LOAD, (), MemBuffer(outputs.index(assign_targets[buf]), buf.dtype, unbound_st))
     if buf not in inputs: inputs.append(buf)
-    return LazyOp(BufferOps.LOAD, (), MemBuffer(len(outbufs)+inputs.index(buf), buf.dtype, unbound_st))
+    return LazyOp(BufferOps.LOAD, (), MemBuffer(len(outputs)+inputs.index(buf), buf.dtype, unbound_st))
 
   # if a CONTIGUOUS or ASSIGN made it all the way here, just skip it
   if buf.op is LoadOps.CONTIGUOUS:
-    assert buf in outbufs
-    return _recursive_lazyop(buf.srcs[0], inputs, outbufs, var_vals, st, realizes, cache)
+    assert buf in outputs
+    return _recursive_lazyop(buf.srcs[0], inputs, outputs, var_vals, st, realizes, assign_targets, cache)
   if buf.op is LoadOps.ASSIGN:
-    assert buf in outbufs
+    assert buf in outputs
     assert buf.srcs[1].base is buf.srcs[1], "assign must be to base"
     assert buf.srcs[1].realized is not None, f"assign must be already realized to schedule {buf.srcs[1]}"
-    return _recursive_lazyop(buf.srcs[0], inputs, outbufs, var_vals, st, realizes, cache, assign_to=buf.srcs[1], assign_idx=outbufs.index(buf))
+    return _recursive_lazyop(buf.srcs[0], inputs, outputs, var_vals, st, realizes, assign_targets, cache)
 
   # if it's a reduce, we have to change the shapetracker
   if buf.op in ReduceOps:
     assert st.contiguous, "ReduceOps late fusion must be contiguous"
     st = ShapeTracker.from_shape(buf.srcs[0].shape)
 
   # otherwise we fuse it like normal
   cache[(buf, st)] = ret = \
-    LazyOp(buf.op, tuple(_recursive_lazyop(x, inputs, outbufs, var_vals, st, realizes, cache, assign_to, assign_idx) for x in buf.srcs), buf.arg)
+    LazyOp(buf.op, tuple(_recursive_lazyop(x, inputs, outputs, var_vals, st, realizes, assign_targets, cache) for x in buf.srcs), buf.arg)
   return ret
 
 def _schedule_group(outs:Tuple[LazyBuffer, ...], realizes:Dict[LazyBuffer, None], reduce_for_op: Dict[LazyBuffer, LazyBuffer]) -> _LBScheduleItem:
+  """create a schedule item from a list of outputs"""
   inputs: List[LazyBuffer] = []
   ast: List[LazyOp] = []
   var_vals: Dict[Variable, int] = merge_dicts([out.st.var_vals.copy() for out in outs])
-  if outs[0].op in {LoadOps.CUSTOM, LoadOps.COPY, LoadOps.EMPTY, LoadOps.VIEW}:
-    ast, inputs = [LazyOp(outs[0].op, (), outs[0].arg)], [x.base for x in outs[0].srcs]
+  # single output AST
+  if (op:=(out:=outs[0]).op) in {LoadOps.CUSTOM, LoadOps.COPY, LoadOps.EMPTY, LoadOps.VIEW}:
+    assert len(outs) == 1, f"can't schedule a group of {op}"
+    inputs = [x.base for x in out.srcs]
+    if getenv("USE_COPY_KERNEL") and op is LoadOps.COPY and out.device.split(":")[0] == out.srcs[0].device.split(":")[0]:
+      rd = LazyOp(BufferOps.LOAD, (), MemBuffer(1, dtypes.uint8, st:=ShapeTracker.from_shape((out.arg,))))
+      ast = [LazyOp(BufferOps.STORE, (rd,), MemBuffer(0, dtypes.uint8, st))]
+    else: ast = [LazyOp(op, (), out.arg)]
+  # multi output AST
   else:
+    assign_targets = {x.srcs[1]:x for x in outs if x.op is LoadOps.ASSIGN}
     for i, out in enumerate(outs):
       output_st = ShapeTracker.from_shape(reduce_for_op[out].shape if out in reduce_for_op else out.shape)
       output_view = out.arg[0] if out.op is LoadOps.ASSIGN and out.arg else output_st
-      op = _recursive_lazyop(out, inputs, outs, var_vals, output_st, realizes, cache={})
+      lop = _recursive_lazyop(out, inputs, outs, var_vals, output_st, realizes, assign_targets, cache={})
       output_view, vv = output_view.simplify().unbind()
       if vv: var_vals.update(vv)
-      ast.append(LazyOp(BufferOps.STORE, (op, ), MemBuffer(i, out.dtype, output_view)))
+      ast.append(LazyOp(BufferOps.STORE, (lop, ), MemBuffer(i, out.dtype, output_view)))
   return _LBScheduleItem(tuple(ast), outs, tuple(inputs), var_vals)
 
-# recursively search the entire graph for all LazyBuffers, insert realizes after expands
+# *** DAG creation: decide which LazyBuffers should realize ***
+
 def _recurse_lb(buf:LazyBuffer, realizes:Dict[LazyBuffer, None], allbufs:Dict[LazyBuffer, None],
                 simple_pads:Set[LazyBuffer], children:DefaultDict[LazyBuffer, Dict[LazyBuffer, None]], scheduled=False):
-  if buf in allbufs or buf.base.realized: return
+  """recursively search the entire graph for all LazyBuffers, insert realizes after expands"""
+  if buf in allbufs or buf.base.realized is not None: return
   if GRAPH: log_lazybuffer(buf, scheduled)
-  if isinstance(buf.dtype, ImageDType) and (prod(buf.shape) != prod(buf.dtype.shape) or
-                                            not any(buf.shape[x]%4 == 0 for x in buf.st.unit_stride_axes())):
-    if DEBUG >= 3: print(f"forcing image {buf.dtype} with shape {buf.shape} to float32")
-    buf.dtype = dtypes.float32  # NOTE: this is what makes the dtype above not match
-    # hack the underlying buffer too
-    if buf.base is buf:
-      assert not hasattr(buf.buffer, '_buf'), "can't fixup allocated buffer"
-      buf.buffer.dtype = dtypes.float32
-      buf.buffer.options = None
+  # view
   if buf.base != buf:
     # realize all places where the buffer is expanded
     if prod(buf.base.st.shape) < prod(buf.st.shape):
-      if len(buf.st.views) == 1 and buf.st.views[-1].mask and all_int(buf.base.st.shape) and \
+      if len(buf.st.views) == 1 and buf.st.views[-1].mask is not None and all_int(buf.base.st.shape) and \
           prod(buf.base.st.shape) >= prod([y-x for x,y in buf.st.views[-1].mask]):
         simple_pads.add(buf.base)
+      elif buf.base.op is UnaryOps.CAST and isinstance(buf.base.srcs[0].dtype, ImageDType) and isinstance(buf.base.arg, ImageDType):
+        pass # don't realize image to image casts. this is part of a larger problem
       else:
         realizes[buf.base] = None
     return _recurse_lb(buf.base, realizes, allbufs, simple_pads, children)
-  if buf.forced_realize: realizes[buf] = None
+  # base
   allbufs[buf] = None
+  if buf.forced_realize: realizes[buf] = None
   if buf.op in LoadOps: realizes[buf.base] = None
   if buf.op is LoadOps.COPY:
     assert buf.srcs[0].st.contiguous and buf.srcs[0].size == buf.srcs[0].base.size, "can only copy contig"
     realizes[buf.srcs[0].base] = None
   if buf.op is LoadOps.VIEW: realizes[buf.srcs[0].base] = None
   for x in buf.srcs:
     children[x.base][buf] = None
     _recurse_lb(x, realizes, allbufs, simple_pads, children)
 
 def _is_padding_okay(buf:LazyBuffer, realizes:Dict[LazyBuffer, None]) -> bool:
-  if buf in realizes or buf.realized: return True
+  if buf in realizes or buf.realized is not None: return True
   # NOTE: this broke to_image_idx and coder with JIT
   if buf.op in UNSAFE_PAD_OPS: return False
   return all(_is_padding_okay(x.base, realizes) for x in buf.srcs)
 
+def _recursive_group(tr:LazyBuffer, st:ShapeTracker, r:LazyBuffer, children:DefaultDict[LazyBuffer, Dict[LazyBuffer, None]],
+                     realizes:Dict[LazyBuffer, None], reduce_for_op:Dict[LazyBuffer, LazyBuffer], group:Set[LazyBuffer]):
+  """recursively search the LazyBuffer for groupable children, realize the LazyBuffer if a child can't group"""
+  if tr in realizes:
+    # can only fuse contiguous
+    # max one reduceop per kernel
+    if not st.contiguous or st.size != r.st.size or tr in reduce_for_op: group.add(r)
+    return group.add(tr)
+  for tr_next in children[tr]:
+    if tr_next.realized is None:
+      # max one reduceop per kernel
+      if tr_next.op in ReduceOps: return group.add(r)
+      # can only fuse contiguous
+      if len(st_childs:=dedup(s for s in tr_next.srcs if s.base == tr)) > 1: return group.add(r)
+      _recursive_group(tr_next, st+st_childs[0].st, r, children, realizes, reduce_for_op, group)
+
 def _graph_schedule(outs:List[LazyBuffer], seen:Set[LazyBuffer]) -> Tuple[DefaultDict[LazyBuffer, List[LazyBuffer]], DefaultDict[LazyBuffer, int],
                                                                     Dict[LazyBuffer, _LBScheduleItem]]:
+  """create a graph for realizing the outputs"""
   # start by just realizing the buffers passed in
-  realizes: Dict[LazyBuffer, None] = {x.base: None for x in outs if not x.base.realized}
+  realizes: Dict[LazyBuffer, None] = {x.base:None for x in outs if x.base.realized is None}
   allbufs: Dict[LazyBuffer, None] = {}
   simple_pads: Set[LazyBuffer] = set()
   children: DefaultDict[LazyBuffer, Dict[LazyBuffer, None]] = defaultdict(dict)
   for out in outs: _recurse_lb(out.base, realizes, allbufs, simple_pads, children, scheduled=True)
   assign_targets = {x.srcs[1]:x for x in realizes if x.op is LoadOps.ASSIGN and x not in seen and x.realized is None}
 
   # check if we have to realize pads
   for p in simple_pads:
     if not _is_padding_okay(p, realizes):
       realizes[p] = None
 
   # find all reduces, and pair them to a elementwise op. if they can't be cleanly paired, force realize the reduce (or a contig child)
   reduce_for_op: Dict[LazyBuffer, LazyBuffer] = {}
-  for r in allbufs.keys():
-    if r != r.base or r.op not in ReduceOps or r in realizes: continue
+  for r in allbufs:
+    if r.op not in ReduceOps or r in realizes: continue
 
-    # follow the reduce down
-    child_set: Dict[LazyBuffer, ShapeTracker] = {r: r.st}
-    realized_children: Dict[LazyBuffer, ShapeTracker] = {}
-    forced_realize = False
-    can_chase = True
-    while not forced_realize and len(child_set):
-      next_child_set = {}
-      for tr,st in child_set.items():
-        if tr in realizes:
-          realized_children[tr] = st
-          # can only reduce contiguous
-          # max one reduceop per kernel
-          if not st.contiguous or st.size != r.st.size or tr in reduce_for_op:
-            can_chase = tr not in reduce_for_op
-            forced_realize = True
-            break
-          if len(realized_children) > 1:
-            rc_parents, rc_children = deque(realized_children), deque(realized_children)
-            while rc_parents and not forced_realize:
-              # max one reduceop per kernel
-              if (p:=rc_parents.pop()).op in ReduceOps: forced_realize = True
-              else: rc_parents.extend(x.base for x in p.srcs if x.base.realized is None and x.base is not r)
-            realized_descendants: Set[LazyBuffer] = set()
-            while rc_children and not forced_realize:
-              if (c:=rc_children.pop()).op in ReduceOps or not c.st.contiguous or c.st.size != r.st.size or c in reduce_for_op:
-                realized_descendants.clear()
-                break
-              if c in realizes and c not in (*realized_children, tr): realized_descendants.add(c)
-              rc_children.extend(x for x in children[c] if x.realized is None and x.device == r.device)
-            realized_children.update((rd, st) for rd in realized_descendants)
-          continue
-        for tr_next in children[tr].keys():
-          if not tr_next.realized:
-            # max one reduceop per kernel
-            if tr_next.op in ReduceOps:
-              forced_realize = True
-              break
-            st_childs = dedup([s for s in tr_next.srcs if s.base == tr])
-            if len(st_childs) > 1:
-              forced_realize = True
-              break
-            next_child_set[tr_next] = st + st_childs[0].st
-      child_set = next_child_set
-    if not forced_realize and any(x.op is LoadOps.ASSIGN for x in realized_children):
-      parents = deque((r, *realized_children))
+    group: Set[LazyBuffer] = set()
+    _recursive_group(r, r.st, r, children, realizes, reduce_for_op, group)
+    # max one reduceop per kernel
+    can_chase = all(tr not in reduce_for_op for tr in group)
+    # TODO: forced_realize exists because the scheduler is incapable of checking for self-contained DAGs
+    forced_realize = r in group
+    if not forced_realize and len(group) > 1:
+      # create a multi output kernel if the LazyBufferss can cleanly group
+      rc_parents, rc_children = deque(group), deque(group)
+      while rc_parents and not forced_realize:
+        # max one reduceop per kernel
+        if (p:=rc_parents.pop()).op in ReduceOps: forced_realize = True
+        else: rc_parents.extend(x.base for x in p.srcs if x.base.realized is None and x.base is not r)
+      # search descendants of the reduceop that can cleanly group
+      realized_descendants: Set[LazyBuffer] = set()
+      while rc_children and not forced_realize:
+        if (c:=rc_children.pop()).op in ReduceOps or not c.st.contiguous or c.st.size != r.st.size or c in reduce_for_op:
+          realized_descendants.clear()
+          break
+        if c in realizes and c not in group: realized_descendants.add(c)
+        rc_children.extend(x for x in children[c] if x.realized is None and x.device == r.device)
+      group.update(realized_descendants)
+    # can only fuse assign if no other assign_target is used in the kernel
+    if not forced_realize and any(x.op is LoadOps.ASSIGN for x in group):
+      parents = deque((r, *group))
       while parents and not forced_realize:
         if (p:=parents.pop().base).realized or p in realizes:
-          if p in assign_targets and assign_targets[p] not in realized_children: forced_realize, can_chase = True, False
+          if p in assign_targets and assign_targets[p] not in group: forced_realize, can_chase = True, False
           continue
         parents.extend(p.srcs)
     if forced_realize:
       tr = r
       if can_chase:
         # can chase this down to contiguous children
         st = tr.st
         while len(children[tr]) == 1:
-          tr_next = next(iter(children[tr].keys()))
-          st_childs = dedup([s for s in tr_next.srcs if s.base == tr])
+          tr_next = next(iter(children[tr]))
+          st_childs = dedup(s for s in tr_next.srcs if s.base is tr)
           if len(st_childs) > 1: break
           if st.size != st_childs[0].st.size: break
           st = st + st_childs[0].st
           if not st.contiguous or tr_next.op in ReduceOps: break
           tr = tr_next
         # don't cast to higher size before store (tr cannot be realized if forced_realize)
-        if tr.op is UnaryOps.CAST and tr.arg[0].itemsize > tr.srcs[0].dtype.itemsize:
+        if tr.op is UnaryOps.CAST and tr.arg.itemsize > tr.srcs[0].dtype.itemsize:
           tr = tr.srcs[0].base
         reduce_for_op[tr] = r
       realizes[tr] = None
-    else: reduce_for_op.update((tr, r) for tr in realized_children)
+    else: reduce_for_op.update((tr, r) for tr in group)
 
-  output_groups: DefaultDict[Tuple, List[LazyBuffer]] = defaultdict(list)
-  for r in realizes:
-    if r.realized is not None or r.op is LoadOps.CONST or r in seen: continue
-    output_groups[(reduce_for_op[r], ) if r in reduce_for_op and MULTIOUTPUT else (r, )].append(r)
+  output_groups: DefaultDict[LazyBuffer, List[LazyBuffer]] = defaultdict(list)
+  for buf in realizes:
+    if buf.realized is not None or buf.op is LoadOps.CONST or buf in seen: continue
+    output_groups[reduce_for_op[buf] if buf in reduce_for_op and MULTIOUTPUT else buf].append(buf)
+
+    # make things that can't be images not images
+    if isinstance(buf.dtype, ImageDType) and (prod(buf.shape) != prod(buf.dtype.shape) or
+                                              not any(buf.shape[x]%4 == 0 for x in buf.st.unit_stride_axes())):
+      if DEBUG >= 2: print(f"forcing image {buf.dtype} with shape {buf.shape} to float32")
+      buf.dtype = dtypes.float32
+      # hack the underlying buffer too
+      if buf.base is buf:
+        assert not hasattr(buf.buffer, '_buf'), "can't fixup allocated buffer"
+        buf.buffer.dtype = dtypes.float32
+        buf.buffer.options = None
 
   # preschedule all buffers in realizes
   prescheduled = {group[0]:_schedule_group(tuple(group), realizes, reduce_for_op) for group in output_groups.values()}
   schedule_targets = {out:ps for ps in prescheduled.values() for out in ps.outputs}
 
-  # breadth first ordering
   graph: DefaultDict[LazyBuffer, List[LazyBuffer]] = defaultdict(list)
   in_degree: DefaultDict[LazyBuffer, int] = defaultdict(int)
   for key, lsi in prescheduled.items():
     if key not in in_degree: in_degree[key] = 0
     # realize outputs after all parents are realized
     scheduled_parents = set(schedule_targets[x].outputs[0] for x in lsi.inputs if x in schedule_targets)
     for x in scheduled_parents:
@@ -245,14 +276,16 @@
     parents_assigns = set(schedule_targets[assign_targets[x]].outputs[0] for x in lsi.inputs if x in assign_targets)
     for assign in parents_assigns:
       graph[key].append(assign)
       in_degree[assign] += 1
 
   return graph, in_degree, prescheduled
 
+# *** DAG ordering: breadth first search ***
+
 SCHEDULES: List = []
 def create_schedule_with_vars(outs:List[LazyBuffer], seen:Optional[Set[LazyBuffer]]=None) -> Tuple[List[ScheduleItem], Dict[Variable, int]]:
   if seen is None: seen = set()
   graph, in_degree, prescheduled = _graph_schedule(outs, seen)
   queue = deque(si for key, si in prescheduled.items() if in_degree[key] == 0)
   schedule: List[ScheduleItem] = []
   var_vals: Dict[Variable, int] = {}
@@ -283,7 +316,46 @@
   if DEBUG >= 1 and len(schedule) >= 10: print(f"scheduled {len(schedule)} kernels")
   return schedule, var_vals
 
 def create_schedule(outs:List[LazyBuffer], seen:Optional[Set[LazyBuffer]]=None) -> List[ScheduleItem]:
   schedule, var_vals = create_schedule_with_vars(outs, seen)
   assert len(var_vals) == 0
   return schedule
+
+# *** memory planning ***
+
+def _internal_memory_planner(buffers:List[Union[List[Buffer], Tuple[Buffer, ...]]], debug_prefix="") -> Dict[Buffer, Buffer]:
+  if getenv("NO_MEMORY_PLANNER"): return {}
+  last_appearance = {}
+  for i,u in enumerate(buffers):
+    for buf in u: last_appearance[buf] = i
+
+  # LRU algorithm
+  assigned: Dict[Buffer, Buffer] = {}
+  local_cache: DefaultDict[Tuple[str, int, DType], List[Buffer]] = defaultdict(list)
+
+  def handle_buffer(buf):
+    key = (buf.device, buf.size, buf.dtype)
+    if buf not in assigned:
+      if len(ll:=local_cache[key]): assigned[buf] = ll.pop()
+      else: assigned[buf] = Buffer(*key)
+    if i == last_appearance[buf]:
+      if assigned[buf] not in local_cache[key]: local_cache[key].append(assigned[buf])
+
+  for i,u in enumerate(buffers):
+    for buf in u:
+      # all unallocated unparented buffers are fair game to replace
+      if buf.is_allocated() or buf.lb_refcount > 0: continue
+      # handle view buffers
+      if buf._base is not None:
+        assigned[buf] = Buffer(buf.device, buf.size, buf.dtype, base=assigned.get(buf._base, buf._base), offset=buf.offset)
+      else:
+        handle_buffer(buf)
+
+  if DEBUG >= 1 and len(ak:=dedup(assigned.keys())) != len(av:=dedup(assigned.values())):
+    print(debug_prefix+f"memory reduced from {sum([x.nbytes for x in ak])/1e6:.2f} MB -> {sum([x.nbytes for x in av])/1e6:.2f} MB,",
+          f"{len(ak)} -> {len(av)} bufs")
+  return assigned
+
+def memory_planner(schedule:List[ScheduleItem]) -> List[ScheduleItem]:
+  assigned = _internal_memory_planner([si.bufs for si in schedule])
+  return [ScheduleItem(si.ast, tuple(assigned.get(x, x) for x in si.bufs)) for si in schedule]
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/features/graph.py` & `tinygrad_tools-0.8.2/tinygrad/engine/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os, atexit, functools
 from collections import defaultdict
-from typing import List, Any, DefaultDict, TYPE_CHECKING
+from typing import List, Any, DefaultDict
 from tinygrad.ops import UnaryOps, BinaryOps, ReduceOps, LoadOps, BufferOps, TernaryOps, LazyOp
 from tinygrad.device import Device
 from tinygrad.helpers import GRAPHPATH, DEBUG, GlobalCounters, getenv
 from tinygrad.codegen.linearizer import UOps, UOp
 from tinygrad.shape.symbolic import NumNode
-if TYPE_CHECKING: from tinygrad.lazy import LazyBuffer
+from tinygrad.lazy import LazyBuffer
 
 try: import networkx as nx
 except ImportError: pass
 
 # **** debugging and graphing ****
 
 if DEBUG >= 2:
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/features/multi.py` & `tinygrad_tools-0.8.2/tinygrad/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     llbs = []
     for i,lb in enumerate([lb.copy_to_device(device) for lb in self.real_lbs]):
       pad_arg = tuple((0,0) if a != self.axis else (sz*i, max(0, self.shape[self.axis]-sz*(i+1))) for a in range(len(lb.shape)))
       llbs.append(lb.pad(pad_arg))
     return functools.reduce(lambda x,y: x.e(BinaryOps.ADD, y), llbs)
 
   # passthroughs
-  def is_realized(self) -> bool: return all([lb.base.realized is not None for lb, r in zip(self.lbs, self.real) if r is True])
+  def is_realized(self) -> bool: return all(lb.base.realized is not None for lb, r in zip(self.lbs, self.real) if r is True)
   def cast(self, dtype:DType, bitcast:bool=False): return MultiLazyBuffer([x.cast(dtype, bitcast) for x in self.lbs], self.axis, self.real)
   def const(self, val:ConstType) -> MultiLazyBuffer: return MultiLazyBuffer([x.const(val) for x in self.lbs], self.axis, self.real)
   def assign(self, x:MultiLazyBuffer): return MultiLazyBuffer([s.assign(d) for s,d in zip(self.lbs, x.lbs)], self.axis, self.real)
   def contiguous(self): return MultiLazyBuffer([x.contiguous() for x in self.lbs], self.axis, self.real)
 
   # elementwise is simple
   def e(self, op:Union[LoadOps, UnaryOps, BinaryOps, TernaryOps], *in_srcs:MultiLazyBuffer, arg:Optional[Any]=None) -> MultiLazyBuffer:
@@ -109,22 +109,22 @@
       else: srcs.append(to_sharded([mlb.copy_to_device(lb.device) for lb in mlb.lbs], axis))
     # NOTE: lsrcs[-1].const(0) is correct for where
     return MultiLazyBuffer([lsrcs[0].e(op, *lsrcs[1:], arg=arg) if r else lsrcs[-1].const(0) for lsrcs,r in zip(zip(*srcs),new_real)], axis, new_real)
 
   def _shape_to_single_shard(self, shape:Tuple[sint, ...], lb:LazyBuffer) -> Tuple[sint, ...]:
     return tuple(lb.shape[self.axis] if a == self.axis else s for a,s in enumerate(shape))
 
-  def r(self, op:ReduceOps, axis:Tuple[int, ...], acc_dt:Optional[DType]=None) -> MultiLazyBuffer:
+  def r(self, op:ReduceOps, axis:Tuple[int, ...]) -> MultiLazyBuffer:
     if self.axis is not None and self.axis in axis:
       # all-reduce on sharded axes
-      reduced_parts = [(x if r else x.const(0)).r(op, axis, acc_dt) for x,r in zip(self.lbs, self.real)]
+      reduced_parts = [(x if r else x.const(0)).r(op, axis) for x,r in zip(self.lbs, self.real)]
       if all(self.real): return MultiLazyBuffer(all_reduce(op, reduced_parts), None)
       return MultiLazyBuffer(reduced_parts, None, self.real)
     # reduce on non sharded axes, piecewise is fine. if axis is None this is also correct
-    return MultiLazyBuffer([x.r(op, axis, acc_dt) for x in self.lbs], self.axis, self.real)
+    return MultiLazyBuffer([x.r(op, axis) for x in self.lbs], self.axis, self.real)
 
   # *** movement ops ***
 
   def reshape(self, arg:Tuple[sint, ...]):
     if self.axis is None: return MultiLazyBuffer([x.reshape(arg) for x in self.lbs], None, self.real)
     arg_acc:List[sint] = list(itertools.accumulate(arg, operator.mul, initial=1))
     # new_axis is the last one that preserves prod(prior to new_axis) and must not move items between shards
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/features/search.py` & `tinygrad_tools-0.8.2/tinygrad/engine/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from typing import Dict, List, cast, DefaultDict, Optional, Tuple, Callable
 import itertools, functools, random, math, time, multiprocessing, traceback, signal
 from collections import defaultdict
-from tinygrad.device import Device, Compiled, Buffer, CompiledRunner, Compiler
+from dataclasses import replace
+from tinygrad.device import Device, Buffer, Compiler
 from tinygrad.ops import MemBuffer
 from tinygrad.helpers import prod, flatten, DEBUG, CACHELEVEL, diskcache_get, diskcache_put, getenv, Context, colored, to_function_name
 from tinygrad.dtype import ImageDType
 from tinygrad.codegen.linearizer import Linearizer
 from tinygrad.codegen.kernel import Opt, OptOps, KernelOptError
 from tinygrad.codegen.uops import UOpGraph
 from tinygrad.tensor import Tensor
 from tinygrad.shape.symbolic import sym_infer
+from tinygrad.engine.realize import CompiledRunner
+from tinygrad.renderer import Program
 
 actions = [Opt(op=OptOps.UPCAST, axis=axis, amt=amt) for amt in [0,2,3,4,5,7] for axis in range(6)]
-actions += [Opt(op=OptOps.UNROLL, axis=axis, amt=amt) for amt in [0,4,7] for axis in range(4)]
+actions += [Opt(op=OptOps.UNROLL, axis=axis, amt=amt) for amt in [0,4,7] for axis in range(5)]
 actions += [Opt(op=OptOps.LOCAL, axis=axis, amt=amt) for amt in [2,3,4,8,13,16,29] for axis in range(5)]
 actions += [Opt(op=OptOps.GROUPTOP, axis=axis, amt=amt) for amt in [13,16,28,29,32,49,64,256] for axis in range(3)]
 actions += [Opt(op=OptOps.GROUP, axis=axis, amt=amt) for amt in [0,4,8,16] for axis in range(3)]
 if getenv("BEAM_PADTO", 1): actions += [Opt(op=OptOps.PADTO, axis=axis, amt=amt) for amt in [32] for axis in range(7)]
 actions += [Opt(op=OptOps.LOCAL, axis=0, amt=32), Opt(op=OptOps.UPCASTMID, axis=1, amt=4), Opt(op=OptOps.TC, axis=0, amt=0)]
 actions += [Opt(op=OptOps.TC, axis=axis, amt=getenv("TC_OPT", 2)) for axis in range(9)] # covers resnet kernels (3 global * 3 reduce)
 if getenv("NOLOCALS"): actions += [Opt(op=OptOps.NOLOCALS)]
@@ -27,42 +30,38 @@
     for j in range(len(global_size)-1,-1,-1):
       if test_global_size[j] > 16:
         test_global_size[j] //= 2
         factor *= 2
         break
   return test_global_size, factor
 
-def _time_program(uops, rdev:Compiled, lib:bytes, global_size, local_size, var_vals, rawbufs,
-                  early_stop=None, max_global_size=65536, clear_l2=False, cnt=3, name="test"):
+def _time_program(p:Program, lib:bytes, var_vals, rawbufs, early_stop=None, max_global_size=65536, clear_l2=False, cnt=3, name="test"):
   factor = 1
-  if global_size is not None and max_global_size is not None:
-    global_size, factor = _get_test_global_size(global_size, max_global_size, var_vals)
-  try: car = CompiledRunner(name, "", rdev.dname, global_size, local_size, uops, precompiled=lib)
+  if p.global_size is not None and max_global_size is not None:
+    global_size, factor = _get_test_global_size(p.global_size, max_global_size, var_vals)
+    p = replace(p, global_size=global_size)
+  try: car = CompiledRunner(p, precompiled=lib)
   except AssertionError: return [math.inf] * cnt
   tms = []
   for _ in range(cnt):
     if clear_l2:
       with Context(DEBUG=0, BEAM=0, CACHECOLLECTING=0): Tensor.ones(1024,1024).contiguous().realize()
     tms.append(cast(float, car(rawbufs, var_vals, wait=True))*factor)
     if early_stop is not None and early_stop < tms[-1]: break
   return tms
 
-def _compile_linearizer(compiler:Compiler, lin:Linearizer, name:Optional[str]=None, enforce_max:bool=False) \
-  -> Tuple[bytes, Optional[List[int]], Optional[List[int]], UOpGraph, float]:
-  lin.linearize()
-  if enforce_max and len(lin.uops.uops) >= getenv("BEAM_UOPS_MAX", 3000) > 0: raise RuntimeError("too many uops")
-  src = compiler.render(name if name is not None else to_function_name(lin.name), lin.uops)   # NOTE: these all have the same name for deduping
-  if DEBUG >= 5: print(src)
-  st = time.perf_counter()
-  prog = compiler.compile(src)
-  et = time.perf_counter() - st
-  return prog, lin.global_size, lin.local_size, lin.uops, et
-
-def _try_compile_linearized_w_idx(x:Tuple[int,Linearizer], compiler:Compiler):
-  try: return x[0], _compile_linearizer(compiler, x[1], "test", enforce_max=True)
+def _try_compile_linearized_w_idx(x:Tuple[int,Linearizer], compiler:Compiler) -> Tuple[int, Optional[Tuple[Program, bytes, float]]]:
+  try:
+    x[1].linearize()
+    if len(x[1].uops.uops) >= getenv("BEAM_UOPS_MAX", 3000) > 0: raise RuntimeError("too many uops")
+    p = x[1].to_program()
+    st = time.perf_counter()
+    prog = compiler.compile(p.src)
+    et = time.perf_counter() - st
+    return x[0], (p, prog, et)
   except Exception:
     if DEBUG >= 4: traceback.print_exc()
     return x[0], None
 
 # workers should ignore ctrl c
 def _init_worker(): signal.signal(signal.SIGINT, signal.SIG_IGN)
 
@@ -127,22 +126,22 @@
     dev = Device[lin.opts.device]
     while not exiting:
       acted_lins: List[Linearizer] = flatten([get_linearizer_actions(lin, include_0=False).values() for lin,_ in beam])
       timed_lins: List[Tuple[Linearizer, float]] = []
       _compile_fn = functools.partial(_try_compile_linearized_w_idx, compiler=dev.compiler)
       for i,proc in (map(_compile_fn, enumerate(acted_lins)) if beam_pool is None else beam_pool.imap_unordered(_compile_fn, enumerate(acted_lins))):
         if proc is None: continue
-        lib, global_size, local_size, uops, compile_et = proc
+        p, lib, compile_et = proc
         if lib in seen_libs: continue
         #print(acted_lins[i].colored_shape(), acted_lins[i].applied_opts)  # for debugging BEAMs that segfault
         seen_libs.add(lib)
-        try: tms = _time_program(uops, dev, lib, global_size, local_size, var_vals, rawbufs, early_stop=beam[0][1]*3 if len(beam) else 1.0)
+        try: tms = _time_program(p, lib, var_vals, rawbufs, early_stop=beam[0][1]*3 if len(beam) else 1.0)
         except RuntimeError: continue # for runtime issues
         timed_lins.append((acted_lins[i], min(tms)))
-        if BEAM_DEBUG > 1: print(f"{time.perf_counter() - st:7.2f}s: {i:5d} {len(uops.uops):5d} uops {compile_et*1e6:12.2f} us compile/{timed_lins[-1][1]*1e6:12.2f} us run       {len(timed_lins):4d}/{len(acted_lins):4d}         {timed_lins[-1][0].colored_shape()}")  # noqa: E501
+        if BEAM_DEBUG > 1: print(f"{time.perf_counter() - st:7.2f}s: {i:5d} {len(cast(UOpGraph, p.uops).uops):5d} uops {compile_et*1e6:12.2f} us compile/{timed_lins[-1][1]*1e6:12.2f} us run       {len(timed_lins):4d}/{len(acted_lins):4d}         {timed_lins[-1][0].colored_shape()}")  # noqa: E501
         elif DEBUG >= 2: print(f"\r{time.perf_counter() - st:7.2f}s: {timed_lins[-1][1]*1e6:12.2f} us       {len(timed_lins):4d}/{len(acted_lins):4d}         {timed_lins[-1][0].colored_shape()}\033[K", end="")  # noqa: E501
 
       # done
       opts = sorted(timed_lins, key=lambda x: x[1])
       exiting = len(opts) == 0 or (opts[0][1] < min_progress) or (len(beam) > 0 and ((beam[0][1]-opts[0][1]) < min_progress))
       if not exiting: beam = opts[:amt]
       elif len(opts) > 0 and opts[0][1] < beam[0][1]: beam = opts[:1]
@@ -164,20 +163,22 @@
     try: return clprg(*[x._buf for x in test_rawbuffers], global_size=[g//l if g%l == 0 else g/l for g,l in zip(global_size, local_size)], local_size=local_size, wait=True)  # noqa: E501
     except Exception: return float('inf')
   ret = min([(try_exec(local_size), local_size) for local_size in random.sample(local_sizes, len(local_sizes))])
   assert not math.isinf(ret[0]), "all optimize_local_size exec failed"
   return ret[1]
 
 def time_linearizer(lin:Linearizer, rawbufs:List[Buffer], allow_test_size=True, max_global_size=65536, cnt=3, disable_cache=False, clear_l2=False) -> float:  # noqa: E501
-  key = {"ast": lin.ast[0].key, "opts": str(lin.applied_opts), "allow_test_size": allow_test_size, "max_global_size": max_global_size, "clear_l2": clear_l2, "device": lin.opts.device, "suffix": lin.opts.suffix}  # noqa: E501
+  key = {"ast": lin.ast[0].key, "opts": str(lin.applied_opts), "allow_test_size": allow_test_size,
+         "max_global_size": max_global_size, "clear_l2": clear_l2, "device": lin.opts.device, "suffix": lin.opts.suffix}
   if not disable_cache and CACHELEVEL >= 2 and (val:=diskcache_get("time_linearizer", key)) is not None: return min(val)
 
   dev = Device[lin.opts.device]
   assert dev.compiler is not None
 
   rawbufs = _ensure_buffer_alloc(rawbufs)
   var_vals = {k:(k.max+k.min)//2 for k in lin.ast[0].vars()}
-  lib, global_size, local_size, uops, _ = _compile_linearizer(dev.compiler, lin)
-  tms = _time_program(uops, dev, lib, global_size, local_size, var_vals, rawbufs, max_global_size=max_global_size if allow_test_size else None, clear_l2=clear_l2, cnt=cnt, name=to_function_name(lin.name))  # noqa: E501
+  p = lin.to_program()
+  tms = _time_program(p, dev.compiler.compile(p.src), var_vals, rawbufs,
+                      max_global_size=max_global_size if allow_test_size else None, clear_l2=clear_l2, cnt=cnt, name=to_function_name(lin.name))
 
   if CACHELEVEL >= 2: diskcache_put("time_linearizer", key, tms)
   return min(tms)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/function.py` & `tinygrad_tools-0.8.2/tinygrad/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This is where the forwards and backwards passes live."""
 import math
 from typing import Tuple, Optional
 from tinygrad.helpers import argsort
-from tinygrad.dtype import DType
+from tinygrad.dtype import dtypes, DType, sum_acc_dtype
 from tinygrad.ops import UnaryOps, BinaryOps, TernaryOps, ReduceOps
 from tinygrad.tensor import Function
 from tinygrad.lazy import LazyBuffer
 from tinygrad.shape.symbolic import sint
 
 class Contiguous(Function):
   def forward(self, x:LazyBuffer) -> LazyBuffer: return x.contiguous()
@@ -82,14 +82,21 @@
   def forward(self, x:LazyBuffer) -> LazyBuffer:
     self.ret = x.const(1).e(BinaryOps.DIV, x.const(1).e(BinaryOps.ADD, x.e(BinaryOps.MUL, x.const(-1/math.log(2))).e(UnaryOps.EXP2)))
     return self.ret
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
     return self.ret.e(BinaryOps.MUL, self.ret.const(1).e(BinaryOps.SUB, self.ret)).e(BinaryOps.MUL, grad_output)
 
+class Sign(Function):
+  def forward(self, x:LazyBuffer) -> LazyBuffer:
+    return x.e(BinaryOps.CMPEQ, x.const(0)).e(TernaryOps.WHERE, x.const(0),
+                                              x.e(BinaryOps.CMPLT, x.const(0)).e(TernaryOps.WHERE, x.const(-1), x.const(1)))
+  # backward always return 0 to match torch
+  def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.const(0)
+
 # ************* binary ops *************
 
 class Less(Function):
   def forward(self, x:LazyBuffer, y:LazyBuffer) -> LazyBuffer: return x.e(BinaryOps.CMPLT, y)
   def backward(self, grad_output:LazyBuffer) -> Tuple[Optional[LazyBuffer], Optional[LazyBuffer]]: return None, None
 
 class Eq(Function):
@@ -142,40 +149,41 @@
     return None, \
       self.x.e(TernaryOps.WHERE, grad_output, grad_output.const(0)) if self.needs_input_grad[1] else None, \
       self.x.e(TernaryOps.WHERE, grad_output.const(0), grad_output) if self.needs_input_grad[2] else None
 
 # ************* reduce ops *************
 
 class Sum(Function):
-  def forward(self, x:LazyBuffer, axis:Tuple[int, ...], acc_dtype:Optional[DType]=None) -> LazyBuffer:
+  def forward(self, x:LazyBuffer, axis:Tuple[int, ...]) -> LazyBuffer:
     self.input_shape = x.shape
-    return x.r(ReduceOps.SUM, axis, acc_dtype)
+    return x.r(ReduceOps.SUM, axis)
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.expand(self.input_shape)
 
 class Max(Function):
-  def forward(self, x:LazyBuffer, axis:Tuple[int, ...], acc_dtype:Optional[DType]=None) -> LazyBuffer:
+  def forward(self, x:LazyBuffer, axis:Tuple[int, ...]) -> LazyBuffer:
     self.x, self.ret, self.axis = x, x.r(ReduceOps.MAX, axis), axis
     return self.ret
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
     # 1s in locations where the max was chosen (can be two locations)
-    max_is_1s = self.x.e(BinaryOps.CMPEQ, self.ret.expand(self.x.shape)).cast(self.x.dtype)
+    max_is_1s = self.x.e(BinaryOps.CMPEQ, self.ret.expand(self.x.shape)).cast(dtypes.float)
     div = max_is_1s.r(ReduceOps.SUM, self.axis).expand(self.x.shape)
-    return max_is_1s.e(BinaryOps.DIV, div).e(BinaryOps.MUL, grad_output.expand(self.x.shape))
+    return max_is_1s.e(BinaryOps.DIV, div).cast(grad_output.dtype).e(BinaryOps.MUL, grad_output.expand(self.x.shape))
 
 # ************* movement ops *************
 
 # NOTE: this is sum in reverse
 class Expand(Function):
   def forward(self, x:LazyBuffer, shape:Tuple[int, ...]) -> LazyBuffer:
     self.expanded_axis = tuple(i for i, (si, so) in enumerate(zip(x.shape, shape)) if si != so)
     return x.expand(shape)
 
-  def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.r(ReduceOps.SUM, self.expanded_axis)
+  def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
+    return grad_output.cast(sum_acc_dtype(grad_output.dtype)).r(ReduceOps.SUM, self.expanded_axis).cast(grad_output.dtype)
 
 class Reshape(Function):
   def forward(self, x:LazyBuffer, shape:Tuple[int, ...]) -> LazyBuffer:
     self.input_shape = x.shape
     return x.reshape(shape)
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.reshape(self.input_shape)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/helpers.py` & `tinygrad_tools-0.8.2/tinygrad/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import os, functools, platform, time, re, contextlib, operator, hashlib, pickle, sqlite3, cProfile, pstats, tempfile, pathlib, string, ctypes
-import itertools, urllib.request
+import itertools, urllib.request, subprocess
 from tqdm import tqdm
 from typing import Dict, Tuple, Union, List, ClassVar, Optional, Iterable, Any, TypeVar, TYPE_CHECKING, Callable, Sequence
 if TYPE_CHECKING:  # TODO: remove this and import TypeGuard from typing once minimum python supported version is 3.10
   from typing_extensions import TypeGuard
   from tinygrad.shape.shapetracker import sint
 
 T = TypeVar("T")
@@ -141,24 +141,29 @@
 
 # *** universal database cache ***
 
 _cache_dir: str = getenv("XDG_CACHE_HOME", os.path.expanduser("~/Library/Caches" if OSX else "~/.cache"))
 CACHEDB: str = getenv("CACHEDB", os.path.abspath(os.path.join(_cache_dir, "tinygrad", "cache.db")))
 CACHELEVEL = getenv("CACHELEVEL", 2)
 
-VERSION = 15
+VERSION = 16
 _db_connection = None
 def db_connection():
   global _db_connection
   if _db_connection is None:
     os.makedirs(CACHEDB.rsplit(os.sep, 1)[0], exist_ok=True)
     _db_connection = sqlite3.connect(CACHEDB)
     if DEBUG >= 7: _db_connection.set_trace_callback(print)
   return _db_connection
 
+def diskcache_clear():
+  cur = db_connection().cursor()
+  drop_tables = cur.execute("SELECT 'DROP TABLE IF EXISTS ' || quote(name) || ';' FROM sqlite_master WHERE type = 'table';").fetchall()
+  cur.executescript("\n".join([s[0] for s in drop_tables]))
+
 def diskcache_get(table:str, key:Union[Dict, str, int]) -> Any:
   if CACHELEVEL == 0: return None
   if isinstance(key, (str,int)): key = {"key": key}
   conn = db_connection()
   cur = conn.cursor()
   try:
     res = cur.execute(f"SELECT val FROM '{table}_{VERSION}' WHERE {' AND '.join([f'{x}=?' for x in key.keys()])}", tuple(key.values()))
@@ -211,14 +216,19 @@
 # *** Exec helpers
 
 def cpu_time_execution(cb, enable):
   if enable: st = time.perf_counter()
   cb()
   if enable: return time.perf_counter()-st
 
+def cpu_objdump(lib):
+  with tempfile.NamedTemporaryFile(delete=True) as f:
+    pathlib.Path(f.name).write_bytes(lib)
+    print(subprocess.check_output(['objdump', '-d', f.name]).decode('utf-8'))
+
 # *** ctypes helpers
 
 # TODO: make this work with read only memoryviews (if possible)
 def from_mv(mv:memoryview, to_type=ctypes.c_char):
   return ctypes.cast(ctypes.addressof(to_type.from_buffer(mv)), ctypes.POINTER(to_type * len(mv))).contents
 def to_mv(ptr, sz) -> memoryview: return memoryview(ctypes.cast(ptr, ctypes.POINTER(ctypes.c_uint8 * sz)).contents).cast("B")
 def to_char_p_p(options: List[bytes], to_type=ctypes.c_char): return (ctypes.POINTER(to_type) * len(options))(*[ctypes.cast(ctypes.create_string_buffer(o), ctypes.POINTER(to_type)) for o in options])  # noqa: E501
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/nn/__init__.py` & `tinygrad_tools-0.8.2/tinygrad/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/nn/optim.py` & `tinygrad_tools-0.8.2/tinygrad/nn/optim.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,19 @@
     self.lr = Tensor(lr if getenv("CONST_LR") else [lr], requires_grad=False, device=self.device,
                      dtype=least_upper_dtype(dtypes.default_float, dtypes.float32))
 
   def zero_grad(self):
     for param in self.params: param.grad = None
 
   def step(self): Tensor.realize(*self.schedule_step())
-  def schedule_step(self) -> List[Tensor]: return self._step()+self.params+self.buffers
+  def schedule_step(self) -> List[Tensor]:
+    assert Tensor.training, (
+            f"""Tensor.training={Tensor.training}, Tensor.training must be enabled to use the optimizer.
+                - help: Consider setting Tensor.training=True before calling Optimizer.step().""")
+    return self._step()+self.params+self.buffers
   def _step(self) -> List[Tensor]: raise NotImplementedError
 
 class OptimizerGroup(Optimizer):
   def __init__(self, *optimizers: Optimizer): # pylint: disable=super-init-not-called
     self.optimizers = optimizers
     self.params, self.buffers = flatten([o.params for o in self.optimizers]), flatten([o.buffers for o in self.optimizers])
   def __getitem__(self, i): return self.optimizers[i]
@@ -68,29 +72,30 @@
 # LAMB is essentially just the trust ratio part of LARS applied to Adam/W so if we just set the trust ratio to 1.0 its just Adam/W.
 def AdamW(params: List[Tensor], lr=0.001, b1=0.9, b2=0.999, eps=1e-8, wd=0.01): return LAMB(params, lr, b1, b2, eps, wd, adam=True)
 def Adam(params: List[Tensor], lr=0.001, b1=0.9, b2=0.999, eps=1e-8): return LAMB(params, lr, b1, b2, eps, 0.0, adam=True)
 
 class LAMB(Optimizer):
   def __init__(self, params: List[Tensor], lr=0.001, b1=0.9, b2=0.999, eps=1e-6, wd=0.0, adam=False):
     super().__init__(params, lr)
-    self.eps, self.wd, self.adam = eps, wd, adam
-    self.b1, self.b2, self.t = (Tensor([x], device=self.device, requires_grad=False).realize() for x in [b1, b2, 0])
-    self.m = [Tensor.zeros(*t.shape, dtype=t.dtype, device=t.device, requires_grad=False).contiguous() for t in self.params]
-    self.v = [Tensor.zeros(*t.shape, dtype=t.dtype, device=t.device, requires_grad=False).contiguous() for t in self.params]
+    self.b1, self.b2, self.eps, self.wd, self.adam = b1, b2, eps, wd, adam
+    self.b1_t, self.b2_t = (Tensor([1], dtype=dtypes.float32, device=self.device, requires_grad=False).realize() for _ in [b1, b2])
+    self.m = [Tensor.zeros(*t.shape, dtype=dtypes.float32, device=t.device, requires_grad=False).contiguous() for t in self.params]
+    self.v = [Tensor.zeros(*t.shape, dtype=dtypes.float32, device=t.device, requires_grad=False).contiguous() for t in self.params]
 
   def _step(self) -> List[Tensor]:
-    self.t.assign(self.t + 1)
+    self.b1_t *= self.b1
+    self.b2_t *= self.b2
     for i, t in enumerate(self.params):
       assert t.grad is not None
       self.m[i].assign(self.b1 * self.m[i] + (1.0 - self.b1) * t.grad)
       self.v[i].assign(self.b2 * self.v[i] + (1.0 - self.b2) * (t.grad * t.grad))
-      m_hat = self.m[i] / (1.0 - self.b1 ** self.t)
-      v_hat = self.v[i] / (1.0 - self.b2 ** self.t)
+      m_hat = self.m[i] / (1.0 - self.b1_t)
+      v_hat = self.v[i] / (1.0 - self.b2_t)
       up = (m_hat / (v_hat.sqrt() + self.eps)) + self.wd * t.detach()
       if not self.adam:
         r1 = t.detach().square().sum().sqrt()
         r2 = up.square().sum().sqrt()
         r = Tensor.where(r1 > 0, Tensor.where(r2 > 0, r1 / r2, 1.0), 1.0)
       else:
         r = 1.0
       t.assign((t.detach() - self.lr * r * up).cast(t.dtype))
-    return [self.t] + self.m + self.v
+    return [self.b1_t, self.b2_t] + self.m + self.v
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/nn/state.py` & `tinygrad_tools-0.8.2/tinygrad/nn/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, json, pathlib, zipfile, pickle, tarfile, struct
 from tqdm import tqdm
 from typing import Dict, Union, List, Optional, Any, Tuple
 from tinygrad.tensor import Tensor
 from tinygrad.dtype import dtypes
 from tinygrad.helpers import prod, argsort, DEBUG, Timing, CI, unwrap, GlobalCounters
 from tinygrad.shape.view import strides_for_shape
-from tinygrad.features.multi import MultiLazyBuffer
+from tinygrad.multi import MultiLazyBuffer
 
 safe_dtypes = {"BOOL":dtypes.bool, "I8":dtypes.int8, "U8":dtypes.uint8, "I16":dtypes.int16, "U16":dtypes.uint16, "I32":dtypes.int, "U32":dtypes.uint,
                "I64":dtypes.int64, "U64":dtypes.uint64, "F16":dtypes.float16, "BF16":dtypes.bfloat16, "F32":dtypes.float32, "F64":dtypes.float64}
 inverse_safe_dtypes = {v:k for k,v in safe_dtypes.items()}
 
 def safe_load_metadata(fn:Union[Tensor,str]) -> Tuple[Tensor, int, Any]:
   t = fn if isinstance(fn, Tensor) else Tensor.empty(os.stat(fn).st_size, dtype=dtypes.uint8, device=f"disk:{fn}")
@@ -63,15 +63,18 @@
     if DEBUG >= 1 and len(state_dict) > len(model_state_dict):
       print("WARNING: unused weights in state_dict", sorted(list(state_dict.keys() - model_state_dict.keys())))
     for k,v in (t := tqdm(model_state_dict.items(), disable=CI or not verbose)):
       t.set_description(f"ram used: {GlobalCounters.mem_used/1e9:5.2f} GB, {k:50s}")
       if k not in state_dict and not strict:
         if DEBUG >= 1: print(f"WARNING: not loading {k}")
         continue
-      v.replace(state_dict[k].shard(mlb.device, mlb.axis) if isinstance((mlb:=v.lazydata), MultiLazyBuffer) else state_dict[k].to(v.device)).realize()
+      if isinstance((mlb:=v.lazydata), MultiLazyBuffer):
+        if isinstance(state_dict[k].lazydata, MultiLazyBuffer): v.replace(state_dict[k]).realize()
+        else: v.replace(state_dict[k].shard(mlb.device, mlb.axis)).realize()
+      else: v.replace(state_dict[k].to(v.device)).realize()
       if consume: del state_dict[k]
 
 # torch support!
 
 def torch_load(fn:str) -> Dict[str, Tensor]:
   t = Tensor.empty(os.stat(fn).st_size, dtype=dtypes.uint8, device=f"disk:{fn}")
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/ops.py` & `tinygrad_tools-0.8.2/tinygrad/ops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from __future__ import annotations
-from typing import Union, Type, Tuple, Any, List, Dict, Callable
+from typing import Union, Tuple, Any, List, Dict, Callable
 import functools, hashlib, math, operator, ctypes
 from enum import Enum, auto
 from dataclasses import dataclass
 from tinygrad.helpers import prod, dedup
 from tinygrad.dtype import dtypes, DType, ConstType
 from tinygrad.shape.symbolic import Variable, sint
 from tinygrad.shape.shapetracker import ShapeTracker
-from tinygrad.buffer import Buffer
 
 # these are the llops your accelerator must implement, along with toCpu
 # the Enum class doesn't work with mypy, this is static. sorry it's ugly
 # NOTE: MOD, CMPLT don't have to be implemented on vectors, just scalars
 # NOTE: many GPUs don't have DIV, but UnaryOps.RECIP doesn't work for integer division
 class UnaryOps(Enum):
   """A -> A (elementwise)"""
-  EXP2 = auto(); LOG2 = auto(); CAST = auto(); SIN = auto(); SQRT = auto(); NEG = auto() # noqa: E702
+  EXP2 = auto(); LOG2 = auto(); CAST = auto(); BITCAST = auto(); SIN = auto(); SQRT = auto(); NEG = auto() # noqa: E702
 class BinaryOps(Enum):
   """A + A -> A (elementwise)"""
   ADD = auto(); SUB = auto(); MUL = auto(); DIV = auto(); MAX = auto(); MOD = auto(); CMPLT = auto(); CMPEQ = auto(); XOR = auto() # noqa: E702
 class TernaryOps(Enum):
   """A + A + A -> A (elementwise)"""
   WHERE = auto(); MULACC = auto() # noqa: E702
 class ReduceOps(Enum):
   """A -> B (reduce)"""
   SUM = auto(); MAX = auto() # noqa: E702
 class BufferOps(Enum): LOAD = auto(); CONST = auto(); STORE = auto() # noqa: E702
 class LoadOps(Enum): EMPTY = auto(); CONST = auto(); COPY = auto(); CONTIGUOUS = auto(); CUSTOM = auto(); ASSIGN = auto(); VIEW = auto() # noqa: E702
 
 Op = Union[UnaryOps, BinaryOps, ReduceOps, LoadOps, TernaryOps, BufferOps]
-OpType = Union[Type[UnaryOps], Type[BinaryOps], Type[ReduceOps], Type[LoadOps], Type[TernaryOps], Type[BufferOps]]
 
 # do not preserve f(0) = 0
 UNSAFE_PAD_OPS = {BinaryOps.DIV, BinaryOps.CMPLT, BinaryOps.CMPEQ, UnaryOps.LOG2, UnaryOps.EXP2}
 
 @dataclass(frozen=True)
 class MemBuffer:
   idx: int
@@ -42,27 +40,14 @@
 
 @dataclass(frozen=True)
 class ConstBuffer:
   val: ConstType
   dtype: DType
   st: ShapeTracker
 
-@dataclass(frozen=True)
-class ScheduleItem:
-  ast: Tuple[LazyOp, ...]
-  bufs: Tuple[Buffer, ...]
-  @property
-  def outputs(self) -> Tuple[Buffer, ...]:
-    """Read/write or write only buffers in the schedule."""
-    return self.bufs[:len(self.ast)]
-  @property
-  def inputs(self) -> Tuple[Buffer, ...]:
-    """Read only buffers in the schedule."""
-    return self.bufs[len(self.ast):]
-
 @dataclass(frozen=True, eq=False)
 class LazyOp:
   op: Op
   src: Tuple[LazyOp, ...] = ()
   arg: Any = None
   def cached_compare(self, x, context):
     if id(self) == id(x): return True
@@ -71,15 +56,15 @@
     ret = context[key] = all(a.cached_compare(b, context) for a,b in zip(self.src, x.src))
     return ret
   def __eq__(self, x): return self.cached_compare(x, context={})
   def __repr__(self): return f"LazyOp(op={self.op}, src={self.src}, arg={self.arg})"
   @functools.cached_property
   def dtype(self) -> DType:
     if self.op in BufferOps: return self.arg.dtype
-    if self.op is UnaryOps.CAST: return self.arg[0]
+    if self.op in [UnaryOps.CAST, UnaryOps.BITCAST]: return self.arg
     return dtypes.bool if self.op in {BinaryOps.CMPLT, BinaryOps.CMPEQ} else self.src[-1].dtype
 
   @functools.cached_property
   def key(self) -> bytes:
     return hashlib.sha256(functools.reduce(lambda x,y: x+y, [s.key for s in self.src], str((self.op, self.arg)).encode())).digest()
   @functools.cached_property
   def hash(self): return hash((self.op, self.src, self.arg))
@@ -87,18 +72,14 @@
   @functools.cached_property
   def lazyops(self) -> List[LazyOp]: return dedup([self] + [item for x in self.src for item in x.lazyops])
   def vars(self) -> List[Variable]:
     extract_vars = [x.arg.st.vars() for x in self.lazyops if x.op in BufferOps]
     const_vars = [x.arg.val.unbind()[0] for x in self.lazyops if x.op is BufferOps.CONST and isinstance(x.arg.val, Variable)]
     return sorted(set.union(*extract_vars, set(const_vars)), key=lambda x: str(x.expr))
 
-def copy_ast(sz) -> LazyOp:
-  rd = LazyOp(BufferOps.LOAD, (), MemBuffer(1, dtypes.uint8, st:=ShapeTracker.from_shape((sz,))))
-  return LazyOp(BufferOps.STORE, (rd,), MemBuffer(0, dtypes.uint8, st))
-
 # **************** independent FlopCounter ****************
 
 @dataclass
 class FlopCounter:
   shape: Tuple[int, ...]
   flops: sint
   mem: Dict[int, int]
@@ -109,15 +90,16 @@
     return ret
 
 InterpretedFlopCounter: Dict[Op, Callable] = {
   BufferOps.LOAD: lambda arg: FlopCounter(arg.st.shape, 0, {arg.idx: arg.dtype.itemsize * arg.st.real_size()}),
   BufferOps.CONST: lambda arg: FlopCounter(arg.st.shape, 0, {}),
   BufferOps.STORE: lambda self,arg: FlopCounter(arg.st.shape, self.consume_flops(), {**self.mem, arg.idx: arg.dtype.itemsize * arg.st.real_size()}),
   UnaryOps.CAST: lambda self,arg: FlopCounter(self.shape, self.consume_flops(), self.mem),   # cast uses no flops
-  **{op:lambda self: FlopCounter(self.shape, self.consume_flops() + prod(self.shape), self.mem) for op in UnaryOps if op is not UnaryOps.CAST},
+  UnaryOps.BITCAST: lambda self,arg: FlopCounter(self.shape, self.consume_flops(), self.mem),   # bitcast uses no flops
+  **{op:lambda self: FlopCounter(self.shape, self.consume_flops() + prod(self.shape), self.mem) for op in UnaryOps if op not in {UnaryOps.CAST, UnaryOps.BITCAST}},  # noqa: E501
   **{op:lambda self,y: FlopCounter(self.shape, self.consume_flops() + y.consume_flops() + prod(self.shape), {**self.mem, **y.mem}) for op in BinaryOps},  # noqa: E501
   **{op:lambda self,axis: FlopCounter(tuple(1 if i in axis else s for i,s in enumerate(self.shape)), self.consume_flops() + prod(self.shape), self.mem) for op in ReduceOps},  # noqa: E501
   TernaryOps.WHERE: lambda self,y,z: FlopCounter(self.shape, self.consume_flops() + y.consume_flops() + z.consume_flops() + prod(self.shape), {**self.mem, **y.mem, **z.mem})}  # noqa: E501
 
 @functools.lru_cache(None)
 def get_lazyop_info(ast:LazyOp) -> FlopCounter:
   @functools.lru_cache(None) # NOTE: this cache needs to be recreated for new ASTs
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/renderer/assembly.py` & `tinygrad_tools-0.8.2/tinygrad/renderer/assembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Callable, DefaultDict, Dict, List, Union, NamedTuple, Optional, cast
-import functools, struct, copy
+from typing import DefaultDict, Dict, List, Union, Optional, cast, Callable
+import struct, copy
 from collections import defaultdict
 from tinygrad.codegen.linearizer import UOps, UOp
 from tinygrad.ops import BinaryOps, UnaryOps, TernaryOps, Op
-from tinygrad.dtype import dtypes, DType, PtrDType, ConstType, INVERSE_DTYPES_DICT
+from tinygrad.dtype import dtypes, DType, PtrDType, ConstType
 from tinygrad.codegen.uops import UOpGraph, PatternMatcher
+from tinygrad.renderer import Renderer
 
 def render_val(x, dtype):
   if dtypes.is_float(dtype):
     if dtype == dtypes.double: return "0d%02X%02X%02X%02X%02X%02X%02X%02X" % tuple(struct.pack("d",x)[::-1])
-    elif dtype == dtypes.half: return "0x%02X%02X" % tuple(struct.pack("e",x)[::-1])
+    if dtype == dtypes.half: return "0x%02X%02X" % tuple(struct.pack("e",x)[::-1])
     return "0f%02X%02X%02X%02X" % tuple(struct.pack("f",x)[::-1])
   return str(int(x)) + ("U" if dtypes.is_unsigned(dtype) else "")
 
 def ptr_ar(root, uops):
   assert root.arg in {'.shared', '.global', None}
   if root.arg is None: root.arg = '.shared' if root.vin[0].uop is UOps.DEFINE_LOCAL else '.global'  # move this to the argL
   val = uops.add(UOps.CONST, dtypes.int, tuple(), arg=root.vin[0].dtype.itemsize, insert_before=uops.uops.index(root))
@@ -24,216 +25,52 @@
     ptr = uops.add(UOps.ALU, dtypes.int, (root.vin[1].vin[1], val), arg=BinaryOps.MUL, insert_before=uops.uops.index(root))
     if root.vin[1].arg == BinaryOps.SUB: ptr = uops.add(UOps.ALU, dtypes.int, (ptr,), arg=UnaryOps.NEG, insert_before=uops.uops.index(root))
     root.vin = (cache, ptr) + root.vin[2:]
   else:
     ptr = uops.add(UOps.ALU, dtypes.int, (root.vin[1], val), arg=BinaryOps.MUL, insert_before=uops.uops.index(root))
     if ptr.uop is UOps.CONST: root.vin = (root.vin[0], ptr) + root.vin[2:]
     else:
-      zero = uops.add(UOps.CONST, dtypes.int, tuple(), arg=0, cachable=False, insert_before=uops.uops.index(root))
+      zero = uops.add(UOps.CONST, dtypes.int, tuple(), arg=0, insert_before=uops.uops.index(root))
       bptr = uops.add(UOps.CAST, dtypes.uint64, (ptr,), insert_before=uops.uops.index(root))
       fptr = uops.add(UOps.ALU, dtypes.uint64, (root.vin[0], bptr), arg=BinaryOps.ADD, insert_before=uops.uops.index(root))
       root.vin = (fptr, zero) + root.vin[2:]
 
-class AssemblyLanguage(NamedTuple):
-  kernel_prefix: str = ""
-  barrier: str = ""
-  load_global: bool = False
-  label_prefix: str = ""
-  gid: List[str] = []
-  gdim: List[str] = []
-  lid: List[str] = []
-  const_requires_mov: List[DType] = [] # list of dtypes for which creating a const requires a move
-  asm_for_op: Dict[Op, Callable[...,str]] = {}
-  types: Dict[DType, str] = INVERSE_DTYPES_DICT
-  supports_half: List[Op] = []
-
-  def render_const(self, x:ConstType, dtype:DType, mov=None) -> Union[List[str], str]: raise NotImplementedError()
-  def render_local(self, dest, name, size, dtype) -> List[str]: raise NotImplementedError()
-
-  def render_loop(self, idx, start, label, acc=None) -> List[str]: raise NotImplementedError()
-  def render_bra(self, b1, pred=None, b2=None) -> List[str]: raise NotImplementedError()
-  def render_gep(self, loc, base, offset, dtype, gate=None) -> List[str]: raise NotImplementedError()
-  def render_load(self, loc, dest, dtype, gate=None, alt=None, ss="", offset=0) -> List[str]: raise NotImplementedError()
-  def render_store(self, loc, val, dtype, gate=None, ss="", offset=0) -> List[str]: raise NotImplementedError()
-  def render_cast(self, d:str, a:str, dtype:DType, atype:DType, bitcast=False, pred=False) -> List[str]: raise NotImplementedError()
-
-  def render_kernel(self, kernel, function_name, bufs, regs) -> str: raise NotImplementedError()
-  def mem_type(self, dtype) -> str: raise NotImplementedError()
-
-def uops_to_asm(lang:AssemblyLanguage, function_name:str, _uops:UOpGraph) -> str:
-  # editing the uops breaks beam search
-  uops = copy.deepcopy(_uops)
-  kernel:List[str] = []
-  bufs = []
-
-  matcher = PatternMatcher([
-    ({"__name__": "root", "uop": UOps.ALU, "arg": BinaryOps.CMPEQ, "vin": ({"dtype": dtypes.bool},{})},
-     lambda root: UOp(UOps.ALU, dtypes.bool, (UOp(root.uop, root.dtype, root.vin, BinaryOps.XOR),), UnaryOps.NEG)),
-    ({"__name__": "root", "uop": UOps.ALU, "arg": BinaryOps.CMPLT, "vin": ({"__name__": "x", "dtype": dtypes.bool},{"__name__": "y"})},
-     lambda root,x,y: UOp(root.uop, root.dtype, (UOp(UOps.ALU, dtypes.bool, (x,), UnaryOps.NEG), y), BinaryOps.MUL)),
-    ({"__name__": "root", "uop": UOps.ALU, "arg": BinaryOps.ADD, "dtype": set([dtypes.float16, dtypes.bfloat16, dtypes.float32, dtypes.float64]),
-      "vin": [{"__name__": "non_muls"}, {"__name__": "muls", "uop": UOps.ALU, "arg": BinaryOps.MUL}]},
-      lambda root, muls, non_muls: UOp(UOps.ALU, root.dtype, muls.vin + (non_muls,), TernaryOps.MULACC)),
-    *[({"__name__": "x", "uop": UOps.ALU, "dtype": dtypes.half, "arg": op},
-       lambda x: UOp(UOps.CAST, dtypes.half, (UOp(x.uop, dtypes.float32, tuple([UOp(UOps.CAST, dtypes.float32, (vv,)) for vv in x.vin]), x.arg),)))
-      for op in lang.asm_for_op.keys() if op not in lang.supports_half],
-    ({"__name__": "root", "uop": UOps.LOAD, "dtype": dtypes.bool,
-      "vin": ({"__name__": "x"},{"__name__": "y"},{"__name__": "z"},{"__name__": "k"})},
-     lambda root,x,y,z,k: UOp(UOps.CAST, dtypes.bool, (UOp(root.uop, dtypes.int8, (x,y,z,UOp(UOps.CAST, dtypes.uint8, (k,)))),), root.arg)),
-    ({"__name__": "root", "uop": UOps.LOAD,"dtype": dtypes.bool, "vin": ({},{})},
-     lambda root: UOp(UOps.CAST, dtypes.bool, (UOp(root.uop, dtypes.uint8, root.vin, root.arg),))),
-    ({"__name__": "root", "uop": UOps.STORE, "vin": ({},{},{"__name__": "z","dtype": dtypes.bool}, {})},
-     lambda root,z: UOp(root.uop, root.dtype, root.vin[:2] + (UOp(UOps.CAST, dtypes.uint8, (z,), None),), root.arg)),
-    ({"__name__": "root", "uop": UOps.STORE, "vin": ({},{},{"__name__": "z","dtype": dtypes.bool})},
-     lambda root,z: UOp(root.uop, root.dtype, root.vin[:2] + (UOp(UOps.CAST, dtypes.uint8, (z,), None),), root.arg)),
-    ({"__name__": "root", "uop": UOps.STORE, "vin": ({},{},{},{"__name__": "g"})},
-     lambda root,g: UOp(root.uop, root.dtype, root.vin[:3] + (UOp(UOps.CAST, dtypes.bool, (g,), root.arg),))),
-  ])
-
-  # here we do a pretransform on UOps to fix some shortcomings of PTX
-  # all uops must be a register
-  matcher.rewrite_graph(uops)
-
-  for pointer_op in list(filter(lambda uop: uop.uop in [UOps.LOAD, UOps.STORE], uops.uops)): ptr_ar(pointer_op, uops)
-  uops.remove_childless(set(x for x in uops if x.uop in {UOps.PHI, UOps.ENDIF, UOps.ENDLOOP, UOps.STORE}))
-  uops.optimize_loops()
-
-  def kk(*s: str): kernel.append("\n".join(s))
-
-  c: DefaultDict[str, int] = defaultdict(int)
-  r: Dict[UOp, Union[List[str], str]] = {}
-  def ssa(prefix:str, u:Optional[UOp]=None, dtype:Optional[str]=None) -> str:
-    nonlocal c, r
-    prefix += f"_{dtype if dtype is not None else lang.types[cast(DType, cast(UOp, u).dtype)]}_"
-    c[prefix] += 1
-    if u is not None: r[u] = f"%{prefix}{c[prefix]-1}"
-    return f"%{prefix}{c[prefix]-1}"
-
-  c_label: DefaultDict[str, int] = defaultdict(int)
-  r_label: Dict[UOp, str] = {}
-  def ssa_label(prefix:str, u:UOp):
-    nonlocal c_label, r_label
-    c_label[prefix] += 1
-    r_label[u] = f"{lang.label_prefix}{prefix}_{c_label[prefix]-1}"
-    return r_label[u]
-
-  def const(x:ConstType, dtype:DType, mov=False):
-    if mov or dtype in lang.const_requires_mov:
-      kk(*lang.render_const(x, dtype, mov=(out:=ssa('const', dtype=lang.types[dtype]))))
-      return out
-    return lang.render_const(x, dtype)
-
-  def _cast(a, dtype:DType, atype:DType, bitcast=False, u=None, pred=False):
-    if atype == dtype:
-      if u: r[u] = a
-      return a
-    kk(*lang.render_cast((ret:=ssa('cast', u, lang.types[dtype])), a, dtype, atype, bitcast))
-    return ret
-
-  for u in uops:
-    uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
-    if uop is UOps.IF:
-      assert vin[0].dtype is not None
-      kk(*lang.render_bra(lb:=ssa_label('if', u), _cast(r[vin[0]], dtypes.bool, vin[0].dtype, u=u, pred=True), f"{lb}_true"), f"{lb}_true:")
-    elif uop is UOps.BARRIER and lang.barrier: kk(lang.barrier)
-    elif uop is UOps.ENDLOOP:
-      kk(lang.asm_for_op[BinaryOps.ADD](r[vin[0]], r[vin[0]], "1", dtypes.int, lang.types[dtypes.int]),
-          lang.asm_for_op[BinaryOps.CMPLT](pred:=ssa("pred", dtype="pred"), r[vin[0]], r[vin[0].vin[1]], dtypes.int, lang.types[dtypes.int]))
-      kk(*lang.render_bra(r_label[vin[0]], pred, f"{r_label[vin[0]]}_exit"), f"{r_label[vin[0]]}_exit:")
-    elif uop is UOps.ENDIF:
-      kk(f"{r_label[vin[0]]}:")
-    elif uop is UOps.STORE:
-      assert vin[0].dtype is not None and vin[1].dtype is not None and vin[2].dtype is not None
-      if vin[2].dtype.count > 1:
-        kk((f"@{r[vin[3]]} " if len(vin)>3 else "") + \
-            f"st{u.arg}.v{vin[2].dtype.count}.{lang.mem_type(vin[2].dtype.scalar())} [{r[vin[0]]}+{vin[1].arg}], {{{', '.join(r[vin[2]])}}};")
-      else:
-        kk(*lang.render_store(r[vin[0]], r[vin[2]], vin[2].dtype, gate=r[vin[3]] if len(vin)>3 else None, ss=u.arg, offset=vin[1].arg))
-    else:
-      assert dtype is not None, f"None dtype for uop {uop}"
-      if uop is UOps.LOOP: kk(*lang.render_loop(ssa('ridx', u), r[vin[0]], ssa_label('loop', u)))
-      elif uop is UOps.ALU:
-        assert vin[0].dtype is not None
-        if args is BinaryOps.CMPLT or args is BinaryOps.CMPEQ:
-          # pass in the other dtype here
-          kk(lang.asm_for_op[args](ssa("alu", u), *[r[x] for x in vin], vin[0].dtype, lang.types[vin[0].dtype]))
-        else:
-          kk(lang.asm_for_op[args](ssa("alu", u), *[r[x] for x in vin], dtype, lang.types[dtype]))
-      elif uop is UOps.DEFINE_ACC:
-        if dtype.count > 1:
-          r[u] = [ssa('acc', dtype=lang.types[dtype.scalar()]) for _ in range(dtype.count)]
-          for uu in r[u]: kk(f"mov.b{lang.types[dtype.scalar()][1:]} {uu}, {const(args, dtype.scalar())};")
-        else: kk(f"mov.b{lang.types[dtype][1:]} {ssa('acc', u)}, {const(args, dtype)};")
-      elif uop is UOps.SPECIAL:
-        assert args[1][0] != "i", "idx not supported"
-        kk(f"mov.u32 %{args[1]}, {(lang.gid if args[1][0] == 'g' else lang.lid)[args[0]]};")
-        r[u] = "%" + args[1]
-        kernel = [f".reg .u32 %{args[1]};"] + kernel
-      elif uop is UOps.CONST:
-        if dtype.count > 1: r[u] = [const(args, dtype.scalar(), mov=True) for _ in range(dtype.count)]
-        else: r[u] = const(args, dtype, mov=True)
-      elif uop is UOps.GEP: r[u] = r[vin[0]][u.arg]
-      elif uop is UOps.LOAD:
-        assert vin[1].dtype is not None
-        if dtype.count > 1:
-          r[u] = [ssa('val', dtype=lang.types[dtype.scalar()]) for _ in range(dtype.count)]
-          if(len(vin)>3):
-            for v in r[u]: kk(f"mov.{lang.mem_type(dtype.scalar())} {v}, {render_val(0, dtype.scalar())};")
-          kk((f"@{r[vin[2]]}"if len(vin) > 3 else "")
-            + f" ld{u.arg}.v{dtype.count}.{lang.mem_type(dtype.scalar())} {{{', '.join(r[u])}}}, [{r[vin[0]]}+{vin[1].arg}];")
-        else:
-          kk(*lang.render_load(r[vin[0]], ssa('val', u), dtype, gate=r[vin[2]] if len(vin) > 3 else None,
-                              alt=r[vin[3]] if len(vin) > 3 else None, ss=u.arg, offset=vin[1].arg))
-      elif uop is UOps.PHI:
-        kk(f"mov.b{lang.types[dtype][1:]} {r[vin[0]]}, {r[vin[1]]};")
-        r[u] = r[vin[0]]
-      elif uop in {UOps.CAST, UOps.BITCAST}:
-        assert vin[0].dtype is not None
-        if dtype.count>1: r[u] = [r[x] for x in vin] # type: ignore
-        else: _cast(r[vin[0]], dtype, vin[0].dtype, bitcast=uop is UOps.BITCAST, u=u)
-      elif uop is UOps.DEFINE_LOCAL:
-        # TODO: we should sum these, and fetch 0xC000 from somewhere
-        assert args[1]*dtype.itemsize <= 0xC000, "too large local"
-        kk(*lang.render_local(ssa('local', u, lang.types[dtypes.ulong]), args[0], args[1], dtype))
-      elif uop is UOps.DEFINE_VAR:
-        bufs.append((args.expr, dtype))
-        r[u] = f"%{args.expr}"
-        if lang.load_global: kk(*lang.render_load(args.expr, ssa('dat', u, lang.types[dtype]), dtype, ss=".param"))
-      elif uop is UOps.DEFINE_GLOBAL:
-        bufs.append((nm:=f"data{args[0]}", dtype))
-        r[u] = f"%{nm}"
-        if lang.load_global:
-          dt = dtypes.ulong if dtype.__class__ == PtrDType else dtype
-          kk(*lang.render_load(nm, ssa('dat', u, lang.types[dt]), dt, ss=".param"))
-      elif uop is UOps.WMMA:
-        wmma = []
-        for vv in vin[:2]:
-          for i in range(0, len(r[vv]), 2):
-            wmma.append(ssa("wmma", dtype="b32"))
-            kk(f'mov.b32 {wmma[-1]}, {{{", ".join(r[vv][i:i+2])}}};')
-        r[u] = r[vin[2]]
-        kk(f'mma.sync.aligned.m16n8k16.row.col.f32.f16.f16.f32\
-           {{{", ".join(r[u])}}}, {{{", ".join(wmma[:4])}}}, {{{", ".join(wmma[4:])}}}, {{{", ".join(r[u])}}};')
-      else: raise NotImplementedError(f"no code for {uop}")
+def optimize_gated_loads(uops: UOpGraph):
+  def successors(uop): return list(filter(lambda u: uop in u.vin, uops.uops))
+  for gl in list(filter(lambda u:u.uop is UOps.LOAD and len(u.vin)>3, uops.uops)):
+    uops.uops.insert(uops.uops.index(gl), gate:=UOp(UOps.IF, None, (gl.vin[2],)))
+    uops.uops.insert(uops.uops.index(gl)+1, end:=UOp(UOps.ENDIF, None, (gate,) + (gl, gl.vin[3])))
+    for u in reversed(uops.uops.copy()[:uops.uops.index(gate)]):
+      if (u.uop not in [UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR, UOps.DEFINE_LOCAL, UOps.PHI, UOps.STORE, UOps.ENDIF, UOps.ENDLOOP] and
+          all(uops.uops.index(s)>uops.uops.index(gate) and uops.uops.index(s)<=uops.uops.index(end) for s in successors(u))):
+        uops.uops.insert(uops.uops.index(gate), uops.uops.pop(uops.uops.index(u)))
+    gl.vin = gl.vin[:2]
+
+class PTXRenderer(Renderer):
+  device = "CUDA"
+  suffix = "PTX"
+  global_max=[65535, 65535, 2147483647]
+  local_max=[64, 1024, 1024]
+  shared_max=49152
+  has_tensor_cores = False
+  def __init__(self, arch:str): self.has_tensor_cores=int(arch[3:]) >= 80
 
-  return lang.render_kernel(kernel, function_name, bufs, c.items())
-
-class PTXLanguage(AssemblyLanguage):
+  # language options
   kernel_prefix = """.version VERSION
 .target TARGET
 .address_size 64
 .visible .entry"""
   barrier = "bar.sync\t0;"
   has_pred = True
   load_global = True
   label_prefix = "$"
   gid = [f'%ctaid.{chr(120+i)}' for i in range(3)]
   gdim = [f'%nctaid.{chr(120+i)}' for i in range(3)]
   lid = [f'%tid.{chr(120+i)}' for i in range(3)]
-  asm_for_op = {
+  asm_for_op: Dict[Op, Callable] = {
     UnaryOps.NEG: lambda d,a,dt,name: f"not.pred {d}, {a};" if name == "pred" else f"neg.{name} {d}, {a};",
     UnaryOps.EXP2: lambda d,a,dt,name: f"ex2.approx.{name} {d}, {a};", UnaryOps.LOG2: lambda d,a,dt,name: f"lg2.approx.{name} {d}, {a};",
     UnaryOps.SIN: lambda d,a,dt,name: f"sin.approx.{name} {d}, {a};", UnaryOps.SQRT: lambda d,a,dt,name: f"sqrt.approx.{name} {d}, {a};",
     BinaryOps.ADD: lambda d,a,b,dt,name: f"{'or' if name == 'pred' else 'add'}.{name} {d}, {a}, {b};",
     BinaryOps.SUB: lambda d,a,b,dt,name: f"sub.{name} {d}, {a}, {b};",
     BinaryOps.MUL: lambda d,a,b,dt,name: ('and' if dt == dtypes.bool else 'mul') + f"{'.lo' if dtypes.is_int(dt) else ''}.{name} {d}, {a}, {b};",
     BinaryOps.XOR: lambda d,a,b,dt,name: f"xor.pred {d}, {a}, {b};" if name == "pred" else f"xor.b{name[1:]} {d}, {a}, {b};",
@@ -241,40 +78,40 @@
     BinaryOps.MAX: lambda d,a,b,dt,name: f"max.{name} {d}, {a}, {b};", BinaryOps.MOD: lambda d,a,b,dt,name: f"rem.{name} {d}, {a}, {b};",
     BinaryOps.CMPLT: lambda d,a,b,dt,name: f"setp.lt.{name} {d}, {a}, {b};",
     BinaryOps.CMPEQ: lambda d,a,b,dt,name: f"setp.eq.{name} {d}, {a}, {b};",
     TernaryOps.MULACC: lambda d,a,b,c,dt,name: f"fma.rn.{name} {d}, {a}, {b}, {c};",
     TernaryOps.WHERE: lambda d,a,b,c,dt,name:
       f"@{a} mov.{name} {d}, {b};\n@!{a} mov.{name} {d}, {c};" if name == "pred" else f"selp.{'b16' if name == 'f16' else name} {d}, {b}, {c}, {a};"
   }
-  supports_half = [UnaryOps.NEG, UnaryOps.EXP2, BinaryOps.ADD, BinaryOps.SUB, BinaryOps.MUL, BinaryOps.MAX, BinaryOps.CMPLT, TernaryOps.WHERE]
+  supports_half: List[Op] = [UnaryOps.NEG, UnaryOps.EXP2, BinaryOps.ADD, BinaryOps.SUB, BinaryOps.MUL, BinaryOps.MAX, BinaryOps.CMPLT,
+                             TernaryOps.WHERE]
   # HACK: Use s16 and u16 for int8 and uint8 buffers. This can be wrong in cast.
-  types = { dtypes.int8: "s16", dtypes.int16: "s16", dtypes.int32: "s32", dtypes.int64: "s64",
-            dtypes.uint8: "u16", dtypes.uint16: "u16", dtypes.uint32: "u32", dtypes.uint64: "u64",
-            dtypes.float16: "f16", dtypes.float32: "f32", dtypes.float64: "f64", dtypes.bool: "pred" }
+  types: Dict[DType, str] = { dtypes.int8: "s16", dtypes.int16: "s16", dtypes.int32: "s32", dtypes.int64: "s64",
+                              dtypes.uint8: "u16", dtypes.uint16: "u16", dtypes.uint32: "u32", dtypes.uint64: "u64",
+                              dtypes.float16: "f16", dtypes.float32: "f32", dtypes.float64: "f64", dtypes.bool: "pred" }
 
-  const_requires_mov = [dtypes.half, dtypes.bool]
+  const_requires_mov: List[DType] = [dtypes.half, dtypes.bool]
 
   def render_const(self, x:ConstType, dtype:DType, mov=None) -> Union[List[str], str]:
     val = render_val(x, dtype)
     if dtype == dtypes.bool: return [f"setp.ne.s16 {mov}, {val}, 0;"]
     return [f"mov.b{self.types[dtype][1:]} {mov}, {val};"] if mov else val
 
   def render_local(self, dest, name, size, dtype) -> List[str]:
     return [f".shared .align 4 .b8 {name}[{size*dtype.itemsize}];", f"mov.u64 {dest}, {name}[0];"]
 
   def render_loop(self, idx, start, label, acc=None) -> List[str]: return [f"mov.u32 {idx}, {start};", f"{label}:"]
 
-  def render_bra(self, b1, pred=None, b2=None) -> List[str]: return [f"@{pred} bra {b1};", f"@!{pred} bra {b2};"] if pred else [f"bra {b1};"]
+  def render_bra(self, b1, pred=None, neg=False) -> List[str]: return [f"@{'!' if neg else ''}{pred} bra {b1};"] if pred else [f"bra {b1};"]
 
   def mem_type(self, dtype): return 's8' if dtype.itemsize == 1 else 'b16' if dtype == dtypes.float16 else self.types[dtype]
 
-  def render_load(self, loc, dest, dtype, gate=None, alt=None, ss="", offset=0) -> List[str]:
+  def render_load(self, loc, dest, dtype, ss="", offset=0) -> List[str]:
     assert dtype is not dtypes.bool
-    if gate: return [f"@{gate} ld{ss}.{self.mem_type(dtype)} {dest}, [{loc}+{offset}];", f"@!{gate} mov.b{self.types[dtype][1:]} {dest}, {alt};"]
-    else: return [f"ld{ss}.{self.mem_type(dtype)} {dest}, [{loc}+{offset}];"]
+    return [f"ld{ss}.{self.mem_type(dtype)} {dest}, [{loc}+{offset}];"]
 
   def render_store(self, loc, val, dtype, gate=None, ss="", offset=0) -> List[str]:
     return [(f"@{gate} " if gate else "") + f"st{ss}.{self.mem_type(dtype)} [{loc}+{offset}], {val};"]
 
   def render_cast(self, d:str, a:str, dtype:DType, atype:DType, bitcast=False, pred=False) -> List[str]:
     if bitcast: return [f"mov.b{self.types[dtype][1:]} {d}, {a};"]
     if atype == dtypes.bool: return[f"selp.b{self.types[dtype][1:]} {d}, {render_val(1, dtype)}, {render_val(0, dtype)}, {a};"]
@@ -287,8 +124,167 @@
     kernel = [f".reg .{reg.split('_')[-2]} %{reg}<{cnt}>;" for reg,cnt in regs] + kernel + ["ret;"]
     def fmt(line): return line if line[0]=="$" else "\t" + line.replace(" ", "\t" if len(line.split(" ")[0]) > 7 else "\t\t", 1)
     return (f"{self.kernel_prefix} {function_name}(\n\t" +
             ',\n\t'.join([f".param .{'u64' if dtype.__class__ == PtrDType else self.types[dtype]} {name}" for name,dtype in bufs]) + "\n)\n{\n" +
             '\n'.join([fmt(line) for op in kernel for line in op.splitlines()]) +
             "\n}")
 
-PTXRenderer = functools.partial(uops_to_asm, PTXLanguage())
+  def render(self, name:str, _uops:UOpGraph) -> str:
+    # editing the uops breaks beam search
+    uops = copy.deepcopy(_uops)
+    kernel:List[str] = []
+    bufs = []
+
+    matcher = PatternMatcher([
+      ({"__name__": "root", "uop": UOps.ALU, "arg": BinaryOps.CMPEQ, "vin": ({"dtype": dtypes.bool},{})},
+      lambda root: UOp(UOps.ALU, dtypes.bool, (UOp(root.uop, root.dtype, root.vin, BinaryOps.XOR),), UnaryOps.NEG)),
+      ({"__name__": "root", "uop": UOps.ALU, "arg": BinaryOps.CMPLT, "vin": ({"__name__": "x", "dtype": dtypes.bool},{"__name__": "y"})},
+      lambda root,x,y: UOp(root.uop, root.dtype, (UOp(UOps.ALU, dtypes.bool, (x,), UnaryOps.NEG), y), BinaryOps.MUL)),
+      ({"__name__": "root", "uop": UOps.ALU, "arg": BinaryOps.ADD, "dtype": set([dtypes.float16, dtypes.bfloat16, dtypes.float32, dtypes.float64]),
+        "vin": [{"__name__": "non_muls"}, {"__name__": "muls", "uop": UOps.ALU, "arg": BinaryOps.MUL}]},
+        lambda root, muls, non_muls: UOp(UOps.ALU, root.dtype, muls.vin + (non_muls,), TernaryOps.MULACC)),
+      *[({"__name__": "x", "uop": UOps.ALU, "dtype": dtypes.half, "arg": op},
+        lambda x: UOp(UOps.CAST, dtypes.half, (UOp(x.uop, dtypes.float32, tuple([UOp(UOps.CAST, dtypes.float32, (vv,)) for vv in x.vin]), x.arg),)))
+        for op in self.asm_for_op.keys() if op not in self.supports_half],
+      ({"__name__": "root", "uop": UOps.LOAD, "dtype": dtypes.bool,
+        "vin": ({"__name__": "x"},{"__name__": "y"},{"__name__": "z"},{"__name__": "k"})},
+      lambda root,x,y,z,k: UOp(UOps.CAST, dtypes.bool, (UOp(root.uop, dtypes.int8, (x,y,z,UOp(UOps.CAST, dtypes.uint8, (k,)))),), root.arg)),
+      ({"__name__": "root", "uop": UOps.LOAD,"dtype": dtypes.bool, "vin": ({},{})},
+      lambda root: UOp(UOps.CAST, dtypes.bool, (UOp(root.uop, dtypes.uint8, root.vin, root.arg),))),
+      ({"__name__": "root", "uop": UOps.STORE, "vin": ({},{},{"__name__": "z","dtype": dtypes.bool}, {})},
+      lambda root,z: UOp(root.uop, root.dtype, root.vin[:2] + (UOp(UOps.CAST, dtypes.uint8, (z,), None),), root.arg)),
+      ({"__name__": "root", "uop": UOps.STORE, "vin": ({},{},{"__name__": "z","dtype": dtypes.bool})},
+      lambda root,z: UOp(root.uop, root.dtype, root.vin[:2] + (UOp(UOps.CAST, dtypes.uint8, (z,), None),), root.arg)),
+      ({"__name__": "root", "uop": UOps.STORE, "vin": ({},{},{},{"__name__": "g"})},
+      lambda root,g: UOp(root.uop, root.dtype, root.vin[:3] + (UOp(UOps.CAST, dtypes.bool, (g,), root.arg),))),
+    ])
+
+    # here we do a pretransform on UOps to fix some shortcomings of PTX
+    # all uops must be a register
+    matcher.rewrite_graph(uops)
+
+    for pointer_op in list(filter(lambda uop: uop.uop in [UOps.LOAD, UOps.STORE], uops.uops)): ptr_ar(pointer_op, uops)
+    uops.remove_childless(set(x for x in uops if x.uop in {UOps.PHI, UOps.ENDIF, UOps.ENDLOOP, UOps.STORE}))
+    uops.optimize_loops()
+    optimize_gated_loads(uops)
+
+    def kk(*s: str): kernel.append("\n".join(s))
+
+    c: DefaultDict[str, int] = defaultdict(int)
+    r: Dict[UOp, Union[List[str], str]] = {}
+    def ssa(prefix:str, u:Optional[UOp]=None, dtype:Optional[str]=None) -> str:
+      nonlocal c, r
+      prefix += f"_{dtype if dtype is not None else self.types[cast(DType, cast(UOp, u).dtype)]}_"
+      c[prefix] += 1
+      if u is not None: r[u] = f"%{prefix}{c[prefix]-1}"
+      return f"%{prefix}{c[prefix]-1}"
+
+    c_label: DefaultDict[str, int] = defaultdict(int)
+    r_label: Dict[UOp, str] = {}
+    def ssa_label(prefix:str, u:UOp):
+      nonlocal c_label, r_label
+      c_label[prefix] += 1
+      r_label[u] = f"{self.label_prefix}{prefix}_{c_label[prefix]-1}"
+      return r_label[u]
+
+    def const(x:ConstType, dtype:DType, mov=False):
+      if mov or dtype in self.const_requires_mov:
+        kk(*self.render_const(x, dtype, mov=(out:=ssa('const', dtype=self.types[dtype]))))
+        return out
+      return self.render_const(x, dtype)
+
+    def _cast(a, dtype:DType, atype:DType, bitcast=False, u=None, pred=False):
+      if atype == dtype:
+        if u: r[u] = a
+        return a
+      kk(*self.render_cast((ret:=ssa('cast', u, self.types[dtype])), a, dtype, atype, bitcast))
+      return ret
+
+    for u in uops:
+      uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
+      if uop is UOps.IF:
+        assert vin[0].dtype is not None
+        kk(*self.render_bra(ssa_label('if', u), _cast(r[vin[0]], dtypes.bool, vin[0].dtype, u=u, pred=True), neg=True))
+      elif uop is UOps.BARRIER and self.barrier: kk(self.barrier)
+      elif uop is UOps.ENDLOOP:
+        kk(self.asm_for_op[BinaryOps.ADD](r[vin[0]], r[vin[0]], "1", dtypes.int, self.types[dtypes.int]),
+            self.asm_for_op[BinaryOps.CMPLT](pred:=ssa("pred", dtype="pred"), r[vin[0]], r[vin[0].vin[1]], dtypes.int, self.types[dtypes.int]))
+        kk(*self.render_bra(r_label[vin[0]], pred))
+      elif uop is UOps.ENDIF:
+        kk(f"@{_cast(r[vin[0].vin[0]], dtypes.bool, vin[0].vin[0].dtype, u=u, pred=True)} bra {r_label[vin[0]]}_true;")
+        kk(f"{r_label[vin[0]]}:")
+        if len(vin) > 1 and vin[1].dtype.count > 1:
+          kk(*[f"mov.b{self.types[vin[1].dtype.scalar()][1:]} {dd}, {r[vin[2]][i]};" for i, dd in enumerate(r[vin[1]])])
+        elif len(vin) > 1:
+          kk(*[f"mov.b{self.types[vin[1].dtype][1:]} {r[vin[1]]}, {r[vin[2]]};" ])
+        kk(f"{r_label[vin[0]]}_true:")
+      elif uop is UOps.STORE:
+        assert vin[0].dtype is not None and vin[1].dtype is not None and vin[2].dtype is not None
+        if vin[2].dtype.count > 1:
+          kk((f"@{r[vin[3]]} " if len(vin)>3 else "") + \
+              f"st{u.arg}.v{vin[2].dtype.count}.{self.mem_type(vin[2].dtype.scalar())} [{r[vin[0]]}+{vin[1].arg}], {{{', '.join(r[vin[2]])}}};")
+        else:
+          kk(*self.render_store(r[vin[0]], r[vin[2]], vin[2].dtype, gate=r[vin[3]] if len(vin)>3 else None, ss=u.arg, offset=vin[1].arg))
+      else:
+        assert dtype is not None, f"None dtype for uop {uop}"
+        if uop is UOps.LOOP: kk(*self.render_loop(ssa('ridx', u), r[vin[0]], ssa_label('loop', u)))
+        elif uop is UOps.ALU:
+          assert vin[0].dtype is not None
+          if args is BinaryOps.CMPLT or args is BinaryOps.CMPEQ:
+            # pass in the other dtype here
+            kk(self.asm_for_op[args](ssa("alu", u), *[r[x] for x in vin], vin[0].dtype, self.types[vin[0].dtype]))
+          else:
+            kk(self.asm_for_op[args](ssa("alu", u), *[r[x] for x in vin], dtype, self.types[dtype]))
+        elif uop is UOps.DEFINE_ACC:
+          if dtype.count > 1:
+            r[u] = [ssa('acc', dtype=self.types[dtype.scalar()]) for _ in range(dtype.count)]
+            for uu in r[u]: kk(f"mov.b{self.types[dtype.scalar()][1:]} {uu}, {const(args[0], dtype.scalar())};")
+          else: kk(f"mov.b{self.types[dtype][1:]} {ssa('acc', u)}, {const(args[0], dtype)};")
+        elif uop is UOps.SPECIAL:
+          assert args[1][0] != "i", "idx not supported"
+          kk(f"mov.u32 %{args[1]}, {(self.gid if args[1][0] == 'g' else self.lid)[args[0]]};")
+          r[u] = "%" + args[1]
+          kernel = [f".reg .u32 %{args[1]};"] + kernel
+        elif uop is UOps.CONST:
+          if dtype.count > 1: r[u] = [const(args, dtype.scalar(), mov=True) for _ in range(dtype.count)]
+          else: r[u] = const(args, dtype, mov=True)
+        elif uop is UOps.GEP: r[u] = r[vin[0]][u.arg]
+        elif uop is UOps.LOAD:
+          assert vin[1].dtype is not None
+          if dtype.count > 1:
+            r[u] = [ssa('val', dtype=self.types[dtype.scalar()]) for _ in range(dtype.count)]
+            kk(f"ld{u.arg}.v{dtype.count}.{self.mem_type(dtype.scalar())} {{{', '.join(r[u])}}}, [{r[vin[0]]}+{vin[1].arg}];")
+          else:
+            kk(*self.render_load(r[vin[0]], ssa('val', u), dtype, ss=u.arg, offset=vin[1].arg))
+        elif uop is UOps.PHI:
+          kk(f"mov.b{self.types[dtype][1:]} {r[vin[0]]}, {r[vin[1]]};")
+          r[u] = r[vin[0]]
+        elif uop in {UOps.CAST, UOps.BITCAST}:
+          assert vin[0].dtype is not None
+          if dtype.count>1: r[u] = [r[x] for x in vin] # type: ignore
+          else: _cast(r[vin[0]], dtype, vin[0].dtype, bitcast=uop is UOps.BITCAST, u=u)
+        elif uop is UOps.DEFINE_LOCAL:
+          # TODO: we should sum these, and fetch 0xC000 from somewhere
+          assert args[1]*dtype.itemsize <= 0xC000, "too large local"
+          kk(*self.render_local(ssa('local', u, self.types[dtypes.ulong]), args[0], args[1], dtype))
+        elif uop is UOps.DEFINE_VAR:
+          bufs.append((args.expr, dtype))
+          r[u] = f"%{args.expr}"
+          if self.load_global: kk(*self.render_load(args.expr, ssa('dat', u, self.types[dtype]), dtype, ss=".param"))
+        elif uop is UOps.DEFINE_GLOBAL:
+          bufs.append((nm:=f"data{args[0]}", dtype))
+          r[u] = f"%{nm}"
+          if self.load_global:
+            dt = dtypes.ulong if dtype.__class__ == PtrDType else dtype
+            kk(*self.render_load(nm, ssa('dat', u, self.types[dt]), dt, ss=".param"))
+        elif uop is UOps.WMMA:
+          wmma = []
+          for vv in vin[:2]:
+            for i in range(0, len(r[vv]), 2):
+              wmma.append(ssa("wmma", dtype="b32"))
+              kk(f'mov.b32 {wmma[-1]}, {{{", ".join(r[vv][i:i+2])}}};')
+          r[u] = r[vin[2]]
+          kk(f'mma.sync.aligned.m16n8k16.row.col.f32.f16.f16.f32\
+            {{{", ".join(r[u])}}}, {{{", ".join(wmma[:4])}}}, {{{", ".join(wmma[4:])}}}, {{{", ".join(r[u])}}};')
+        else: raise NotImplementedError(f"no code for {uop}")
+
+    return self.render_kernel(kernel, name, bufs, c.items())
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/renderer/cstyle.py` & `tinygrad_tools-0.8.2/tinygrad/renderer/cstyle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from typing import Dict, List, Optional, NamedTuple, Tuple, Union, DefaultDict, cast, Literal, Callable
-import math, functools
+from typing import Dict, List, Optional, Tuple, Union, DefaultDict, cast, Literal, Callable
+import os, math
 from collections import defaultdict, Counter
 from tinygrad.codegen.linearizer import UOps, UOp
 from tinygrad.ops import UnaryOps, BinaryOps, TernaryOps
 from tinygrad.helpers import strip_parens, getenv, prod
 from tinygrad.dtype import ImageDType, dtypes, DType, PtrDType, ConstType
 from tinygrad.codegen.uops import UOpGraph
+from tinygrad.renderer import Renderer
 
-class CStyleLanguage(NamedTuple):
+class CStyleLanguage(Renderer):
   kernel_prefix: str = ""
   buffer_prefix: str = ""
   buffer_suffix: str = ""
   smem_align: str = ""
   smem_prefix: str = ""
   smem_prefix_for_cast: bool = True
   arg_int_prefix: str = "const int"
   barrier: str = ""
   code_for_workitem: Dict[Union[Literal["g"], Literal["l"], Literal["i"]], Callable] = {}
-  global_max: List[int] = []
-  local_max: List[int] = []
   extra_args: List[str] = []
   float4: Optional[str] = None
   uses_vload: bool = False
   uses_ptr_arithmetic: bool = False
   type_map: Dict[DType, str] = {}
   code_for_op: Dict = {
     UnaryOps.NEG: lambda x,dtype: f"(!{x})" if dtype is dtypes.bool else f"(-{x})", UnaryOps.SQRT: lambda x,dtype: f"sqrt({x})",
@@ -84,108 +83,115 @@
       prefix = self.smem_prefix if local and self.smem_prefix_for_cast else self.buffer_prefix
       return f"*(({prefix}{self.render_dtype(buf_dtype)}{var_dtype.count}*)({buf_name}+{idx})) = {var_name};"
     return f"*({buf_name}+{idx}) = {var_name};" if self.uses_ptr_arithmetic else f"{buf_name}[{idx}] = {var_name};"
 
   def render_local(self, name:str, dtype:DType, size:int): return self.smem_align + self.smem_prefix + f"{self.render_dtype(dtype)} {name}[{size}];"
   def render_dtype(self, var_dtype:DType) -> str: return self.type_map.get(var_dtype, var_dtype.name)
 
-def uops_to_cstyle(lang:CStyleLanguage, function_name:str, uops:UOpGraph) -> str:
-  kernel = []
-  bufs: List[Tuple[str, Tuple[DType, bool]]] = []
-  depth = 1
-  def kk(s): kernel.append("  "*depth+s)
-
-  c: DefaultDict[str, int] = defaultdict(int)
-  r: Dict[UOp, str] = {}
-
-  def ssa(prefix:str, u:Optional[UOp]=None):
-    nonlocal c, r
-    ret = f"{prefix}{c[prefix]}"
-    if u is not None: r[u] = ret
-    c[prefix] += 1
-    return ret
-
-  child_count = Counter(v for ru in uops for v in ru.vin)
-
-  for u in uops:
-    uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
-    # these four uops don't have output dtypes
-    if uop is UOps.IF:
-      kk(f"if ({r[vin[0]]}) {{")
-      depth += 1
-    elif uop is UOps.BARRIER: kk(lang.barrier)
-    elif uop in {UOps.ENDLOOP, UOps.ENDIF}:
-      depth -= 1
-      kk("}")
-    elif uop is UOps.STORE:
-      assert vin[0].dtype is not None and vin[2].dtype is not None
-      rendered_store = lang.render_store(r[vin[0]], vin[0].dtype, r[vin[2]], vin[2].dtype, strip_parens(r[vin[1]]), vin[0].uop is UOps.DEFINE_LOCAL)
-      kk(f"if ({r[vin[3]]}) {{ {rendered_store} }}" if len(vin) > 3 else rendered_store)
-    else:
-      assert dtype is not None, f"None dtype for uop {uop}"
-      if uop is UOps.LOOP:
-        kk(f"for (int {(expr := ssa('ridx',u))} = {r[vin[0]]}; {expr} < {r[vin[1]]}; {expr}++) {{")
+  def render(self, name:str, uops:UOpGraph) -> str:
+    kernel = []
+    bufs: List[Tuple[str, Tuple[DType, bool]]] = []
+    depth = 1
+    def kk(s): kernel.append("  "*depth+s)
+
+    c: DefaultDict[str, int] = defaultdict(int)
+    r: Dict[UOp, str] = {}
+
+    def ssa(prefix:str, u:Optional[UOp]=None):
+      nonlocal c, r
+      ret = f"{prefix}{c[prefix]}"
+      if u is not None: r[u] = ret
+      c[prefix] += 1
+      return ret
+
+    child_count = Counter(v for ru in uops for v in ru.vin)
+
+    for u in uops:
+      uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
+      # these four uops don't have output dtypes
+      if uop is UOps.IF:
+        kk(f"if ({r[vin[0]]}) {{")
         depth += 1
-      elif uop is UOps.ALU:
-        # remove parens if ALU types are the same. TODO: can do more here
-        if args in {BinaryOps.ADD,BinaryOps.MUL,BinaryOps.XOR}: operands = [strip_parens(r[v]) if v.arg == args else r[v]for v in vin]
-        else: operands = [r[v] for v in vin]
-        val = lang.code_for_op[args](*operands, dtype)
-        assert child_count[u] != 0, f"childless ALU op found {u}"
-        # TODO: fix index rendering issue. fix clang nested max macro issue
-        if child_count[u] <= 1 and args is not BinaryOps.MAX and not getenv("EXPAND_SSA"): r[u] = val
-        else: kk(f"{lang.render_dtype(dtype)} {ssa('alu',u)} = {val};")
-      elif uop is UOps.SPECIAL:
-        kk(f"int {args[1]} = {lang.code_for_workitem[args[1][0]](args[0])}; /* {args[2]} */")
-        r[u] = args[1]
-      elif uop is UOps.LOAD:
-        val = lang.render_load(dtype, r[vin[0]], vin[0].dtype, strip_parens(r[vin[1]]), vin[0].uop is UOps.DEFINE_LOCAL)
-        # NOTE: this relies on the load not happening if it's in the unselected branch
-        if len(vin) > 3: val = lang.code_for_op[TernaryOps.WHERE](r[vin[2]], val, r[vin[3]], dtype)
-        kk(f"{lang.render_dtype(dtype)} {ssa('val',u)} = {val};")
-      elif uop is UOps.PHI:
-        kk(f"{r[vin[0]]} = {r[vin[1]]};")
-        r[u] = r[vin[0]]
-      elif uop in {UOps.CAST, UOps.BITCAST}:
-        if uop is UOps.BITCAST:
-          assert len(vin) == 1
-          precast = ssa('precast')
-          kk(f"{lang.render_dtype(cast(DType, vin[0].dtype))} {precast} = {r[vin[0]]};")
-          val = lang.render_cast([precast], dtype, bitcast=True)
-        else:
-          val = lang.render_cast([r[x] for x in vin], dtype, bitcast=False)
-        if child_count[u] <= 1: r[u] = val
-        else: kk(f"{lang.render_dtype(dtype)} {ssa('cast',u)} = {val};")
-      elif uop is UOps.DEFINE_LOCAL:
-        kk(lang.render_local(args[0], dtype, args[1]))
-        r[u] = args[0]
-      elif uop is UOps.DEFINE_VAR:
-        bufs.append((args.expr, (dtype,False)))
-        r[u] = args.expr
-      elif uop is UOps.DEFINE_GLOBAL:
-        bufs.append((nm:=f"data{args[0]}", (dtype,args[1])))
-        r[u] = nm
-      elif uop is UOps.WMMA: kk(f"{lang.render_dtype(dtype)} {ssa('wmma',u)} = __{args[0]}({r[vin[0]]}, {r[vin[1]]}, {r[vin[2]]});")
-      elif uop is UOps.DEFINE_ACC: kk(f"{lang.render_dtype(dtype)} {ssa('acc',u)} = {lang.render_const(args, dtype)};")
-      elif uop is UOps.CONST: r[u] = lang.render_const(args, dtype) if args >= 0 else f"({lang.render_const(args, dtype)})"
-      elif uop is UOps.GEP:
-        assert vin[0].dtype is not None
-        from_ssa = vin[0].uop in {UOps.LOAD, UOps.WMMA, UOps.DEFINE_ACC}
-        r[u] = (r[vin[0]] if from_ssa else f"{(r[vin[0]])}") + (f"[{args}]" if vin[0].dtype.count > 4 else f".{'xyzw'[args]}")
-      else: raise RuntimeError(f"failed to render {uop}")
-
-  return lang.render_kernel(function_name, kernel, bufs, uops)
+      elif uop is UOps.BARRIER: kk(self.barrier)
+      elif uop in {UOps.ENDLOOP, UOps.ENDIF}:
+        depth -= 1
+        kk("}")
+      elif uop is UOps.STORE:
+        assert vin[0].dtype is not None and vin[2].dtype is not None
+        rendered_store = self.render_store(r[vin[0]], vin[0].dtype, r[vin[2]], vin[2].dtype, strip_parens(r[vin[1]]), vin[0].uop is UOps.DEFINE_LOCAL)
+        kk(f"if ({r[vin[3]]}) {{ {rendered_store} }}" if len(vin) > 3 else rendered_store)
+      else:
+        assert dtype is not None, f"None dtype for uop {uop}"
+        if uop is UOps.LOOP:
+          kk(f"for (int {(expr := ssa('ridx',u))} = {r[vin[0]]}; {expr} < {r[vin[1]]}; {expr}++) {{")
+          depth += 1
+        elif uop is UOps.ALU:
+          # remove parens if ALU types are the same. TODO: can do more here
+          if args in {BinaryOps.ADD,BinaryOps.MUL,BinaryOps.XOR}: operands = [strip_parens(r[v]) if v.arg == args else r[v]for v in vin]
+          else: operands = [r[v] for v in vin]
+          val = self.code_for_op[args](*operands, dtype)
+          assert child_count[u] != 0, f"childless ALU op found {u}"
+          # TODO: fix index rendering issue. fix clang nested max macro issue
+          if child_count[u] <= 1 and args is not BinaryOps.MAX and not getenv("EXPAND_SSA"): r[u] = val
+          else: kk(f"{self.render_dtype(dtype)} {ssa('alu',u)} = {val};")
+        elif uop is UOps.SPECIAL:
+          kk(f"int {args[1]} = {self.code_for_workitem[args[1][0]](args[0])}; /* {args[2]} */")
+          r[u] = args[1]
+        elif uop is UOps.LOAD:
+          val = self.render_load(dtype, r[vin[0]], vin[0].dtype, strip_parens(r[vin[1]]), vin[0].uop is UOps.DEFINE_LOCAL)
+          # NOTE: this relies on the load not happening if it's in the unselected branch
+          if len(vin) > 3: val = self.code_for_op[TernaryOps.WHERE](r[vin[2]], val, r[vin[3]], dtype)
+          kk(f"{self.render_dtype(dtype)} {ssa('val',u)} = {val};")
+        elif uop is UOps.PHI:
+          kk(f"{r[vin[0]]} = {r[vin[1]]};")
+          r[u] = r[vin[0]]
+        elif uop in {UOps.CAST, UOps.BITCAST}:
+          if uop is UOps.BITCAST:
+            assert len(vin) == 1
+            precast = ssa('precast')
+            kk(f"{self.render_dtype(cast(DType, vin[0].dtype))} {precast} = {r[vin[0]]};")
+            val = self.render_cast([precast], dtype, bitcast=True)
+          else:
+            val = self.render_cast([r[x] for x in vin], dtype, bitcast=False)
+          if child_count[u] <= 1: r[u] = val
+          else: kk(f"{self.render_dtype(dtype)} {ssa('cast',u)} = {val};")
+        elif uop is UOps.DEFINE_LOCAL:
+          kk(self.render_local(args[0], dtype, args[1]))
+          r[u] = args[0]
+        elif uop is UOps.DEFINE_VAR:
+          bufs.append((args.expr, (dtype,False)))
+          r[u] = args.expr
+        elif uop is UOps.DEFINE_GLOBAL:
+          bufs.append((nm:=f"data{args[0]}", (dtype,args[1])))
+          r[u] = nm
+        elif uop is UOps.WMMA: kk(f"{self.render_dtype(dtype)} {ssa('wmma',u)} = __{args[0]}({r[vin[0]]}, {r[vin[1]]}, {r[vin[2]]});")
+        elif uop is UOps.DEFINE_ACC: kk(f"{self.render_dtype(dtype)} {ssa('acc',u)} = {self.render_const(args[0], dtype)};")
+        elif uop is UOps.CONST: r[u] = self.render_const(args, dtype) if args >= 0 else f"({self.render_const(args, dtype)})"
+        elif uop is UOps.GEP:
+          assert vin[0].dtype is not None
+          from_ssa = vin[0].uop in {UOps.LOAD, UOps.WMMA, UOps.DEFINE_ACC}
+          r[u] = (r[vin[0]] if from_ssa else f"{(r[vin[0]])}") + (f"[{args}]" if vin[0].dtype.count > 4 else f".{'xyzw'[args]}")
+        else: raise RuntimeError(f"failed to render {uop}")
+
+    return self.render_kernel(name, kernel, bufs, uops)
+
+class ClangRenderer(CStyleLanguage):
+  device = "CLANG"
+  supports_float4 = False
+  has_local = False
 
-class ClangLanguage(CStyleLanguage):
+  # language options
   buffer_suffix = " restrict"
   type_map = {dtypes.bool:"_Bool", dtypes.half:"__fp16"}
   code_for_op = {**CStyleLanguage().code_for_op, BinaryOps.MAX: lambda a,b,dtype: f"(({a}>{b})?{a}:{b})"}
-ClangRenderer = functools.partial(uops_to_cstyle, ClangLanguage())
 
-class OpenCLLanguage(CStyleLanguage):
+class OpenCLRenderer(CStyleLanguage):
+  device = "GPU"
+
+  # language options
   kernel_prefix = "__kernel "
   buffer_prefix = "__global "
   smem_align = "__attribute__ ((aligned (16))) "
   smem_prefix = "__local "
   barrier = "barrier(CLK_LOCAL_MEM_FENCE);"
   float4 = "(float4)"
   code_for_workitem = {"g": lambda x: f"get_group_id({x})", "l": lambda x: f"get_local_id({x})", "i": lambda x: f"get_global_id({x})"}
@@ -193,17 +199,21 @@
   type_map = { dtypes.uint8: "uchar", dtypes.uint32: "uint", dtypes.uint16: "ushort", dtypes.uint64: "ulong" }
   def render_cast(self, x, var_dtype, bitcast=False) -> str:
     return f"as_{self.render_dtype(var_dtype)}({x[0]})" if bitcast else super().render_cast(x, var_dtype)
 
   def render_kernel(self, function_name, kernel, bufs, uops, prefix=None) -> str:
     if any(uop.dtype == dtypes.half for uop in uops): prefix = ["#pragma OPENCL EXTENSION cl_khr_fp16 : enable"]
     return super().render_kernel(function_name, kernel, bufs, uops, prefix)
-OpenCLRenderer = functools.partial(uops_to_cstyle, OpenCLLanguage())
 
-class MetalLanguage(CStyleLanguage):
+class MetalRenderer(CStyleLanguage):
+  device = "METAL"
+  has_tensor_cores=os.uname().machine == "arm64"
+  shared_max=32768
+
+  # language options
   kernel_prefix = "kernel "
   buffer_prefix = "device "
   smem_prefix = "threadgroup "
   arg_int_prefix = "constant int&"
   barrier = "threadgroup_barrier(mem_flags::mem_threadgroup);"
   float4 = "float4"
   uses_ptr_arithmetic = True
@@ -223,28 +233,35 @@
   def render_kernel(self, function_name, kernel, bufs, uops, prefix=None):
     prefix, wmma_args = ["#include <metal_stdlib>","using namespace metal;"], set([uop.arg for uop in uops if uop.uop is UOps.WMMA])
     for arg in wmma_args: prefix.append(f"""{arg[3].name}2 __{arg[0]}({arg[2].name}2 m, {arg[2].name}2 n, {arg[3].name}2 o) {{
   simdgroup_{arg[3].name}8x8 a,b,c; a.thread_elements()[0] = m.x; a.thread_elements()[1] = m.y; b.thread_elements()[0] = n.x;
   b.thread_elements()[1] = n.y; c.thread_elements()[0] = o.x; c.thread_elements()[1] = o.y; simdgroup_multiply_accumulate(c, a, b, c);
   return {arg[3].name}2(c.thread_elements()[0], c.thread_elements()[1]);\n}}""")
     return super().render_kernel(function_name, kernel, bufs, uops, prefix)
-MetalRenderer = functools.partial(uops_to_cstyle, MetalLanguage())
 
 code_for_op_half = {BinaryOps.MAX: lambda a,b,dtype: f"__hmax({a},{b})" if dtype in (dtypes.half, dtypes.bfloat16) else f"max({a},{b})",
                     UnaryOps.SQRT: lambda x,dtype: f"hsqrt({x})" if dtype in (dtypes.half, dtypes.bfloat16) else f"sqrt({x})",
                     UnaryOps.SIN: lambda x,dtype: f"hsin({x})" if dtype in (dtypes.half, dtypes.bfloat16) else f"sin({x})",
                     UnaryOps.LOG2: lambda x,dtype: f"hlog2({x})" if dtype in (dtypes.half, dtypes.bfloat16) else f"log2({x})",
                     UnaryOps.EXP2: lambda x,dtype: f"hexp2({x})" if dtype in (dtypes.half, dtypes.bfloat16) else f"exp2({x})",}
 
 _nms = "xyzwabcdefghijkl"
 def _make_cuda_dtype(base_type, name, cnt):
   vec, elems, header = f"{name}{cnt}", ', '.join(_nms[:cnt]), ', '.join([f"{base_type} {x}" for x in _nms[:cnt]])
   return f"struct {vec} {{ {base_type} {elems}; }}; __device__ {vec} make_{vec}({header}) {{ {vec} r={{{elems}}}; return r; }}"
 
-class CUDALanguage(CStyleLanguage):
+class CUDARenderer(CStyleLanguage):
+  device = "CUDA"
+  global_max=[65535, 65535, 2147483647]
+  local_max=[64, 1024, 1024]
+  shared_max=49152
+  has_tensor_cores = False
+  def __init__(self, arch:str): self.has_tensor_cores=int(arch[3:]) >= 80
+
+  # language options
   kernel_prefix = "extern \"C\" __global__ "
   smem_prefix = "__shared__ "
   smem_prefix_for_cast = False
   barrier = "__syncthreads();"
   float4 = "make_float4"
   code_for_workitem = {"g": lambda x: f"blockIdx.{chr(120+x)}", "l": lambda x: f"threadIdx.{chr(120+x)}",
                        "i": lambda x: f"(blockIdx.{chr(120+x)}*blockDim.{chr(120+x)}+threadIdx.{chr(120+x)})"}
@@ -267,15 +284,14 @@
       fn, ti, to, ci, co = arg[0], dt_map[arg[2]][0], dt_map[arg[3]][0], dt_map[arg[2]][1], dt_map[arg[3]][1]
       prefix.append(f"""__device__ {to}4 __{fn}({ti}8 a, {ti}4 b, {to}4 c) {{ int *a_pk = (int *) (&a), *b_pk = (int *) (&b);
 asm( "mma.sync.aligned.m16n8k16.row.col.{co}.{ci}.{ci}.{co} {{ %0, %1, %2, %3 }}, {{ %4, %5, %6, %7 }}, {{ %8, %9 }}, {{ %0, %1, %2, %3 }};"
   : "+f"(c.x), "+f"(c.y), "+f"(c.z), "+f"(c.w) : "r"(a_pk[0]), "r"(a_pk[1]), "r"(a_pk[2]),  "r"(a_pk[3]), "r"(b_pk[0]), "r"(b_pk[1]) );
 return c;}}""")
 
     return super().render_kernel(function_name, kernel, bufs, uops, prefix=prefix)
-CUDARenderer = functools.partial(uops_to_cstyle, CUDALanguage())
 
 code_for_op_hip = { UnaryOps.SQRT: lambda x,dtype: f"__ocml_sqrt_f{ {dtypes.half:16, dtypes.double:64}.get(dtype, 32)}({x})",
                     UnaryOps.SIN: lambda x,dtype: f"__ocml_sin_f{ {dtypes.half:16, dtypes.double:64}.get(dtype, 32)}({x})",
                     UnaryOps.LOG2: lambda x,dtype: f"__ocml_log2_f{ {dtypes.half:16, dtypes.double:64}.get(dtype, 32)}({x})",
                     UnaryOps.EXP2: lambda x,dtype: f"__ocml_exp2_f{ {dtypes.half:16, dtypes.double:64}.get(dtype, 32)}({x})",
                     # TODO: MAX with int uses fmax_f32?
                     BinaryOps.MAX: lambda a,b,dtype: f"__ocml_fmax_f{ {dtypes.half:16, dtypes.double:64}.get(dtype, 32) }({a},{b})",}
@@ -291,15 +307,20 @@
   return { k:wrapper(k,v) for k,v in {**CStyleLanguage().code_for_op, **code_for_op_hip}.items() }
 
 def _make_hip_dtype(base_type, name, cnt):
   elems, header = ', '.join(_nms[:cnt]), ', '.join([f"{base_type} {x}" for x in _nms[:cnt]])
   return f"typedef {base_type} {name}{cnt} __attribute__((ext_vector_type({cnt})));\n" + \
          f"static inline __attribute__((device)) {name}{cnt} make_{name}{cnt}({header}) {{ return {{{elems}}}; }}"
 
-class HIPLanguage(CStyleLanguage):
+class HIPRenderer(CStyleLanguage):
+  device = "HSA"
+  has_tensor_cores = True
+  shared_max = 65536
+
+  # language options
   kernel_prefix = """extern "C" __attribute__((device)) __attribute__((const)) size_t __ockl_get_local_id(unsigned int);
 extern "C" __attribute__((device)) __attribute__((const)) size_t __ockl_get_group_id(unsigned int);
 extern "C" __attribute__((device)) __attribute__((const)) size_t __ockl_get_local_size(unsigned int);
 extern "C" {\n""" + "".join([
 f"""  __attribute__((device)) __attribute__((const)) {dt} __ocml_fmax_f{n}({dt}, {dt});
   __attribute__((device)) __attribute__((pure)) {dt} __ocml_exp2_f{n}({dt});
   __attribute__((device)) __attribute__((pure)) {dt} __ocml_log2_f{n}({dt});
@@ -353,9 +374,7 @@
     return super().render_kernel(function_name, kernel, bufs, uops, prefix)
 
   def get_kernel_modifier(self, uops:UOpGraph) -> str:
     requiredMaxThreadsPerBlock = prod(u.arg[2] for u in uops if u.uop is UOps.SPECIAL and u.arg[1][0] == "l")
     # https://clang.llvm.org/docs/AttributeReference.html#amdgpu-flat-work-group-size
     # NOTE: this makes hlb_cifar10 twice as fast, there may be more gains in tweaking these parameters
     return f"__attribute__((amdgpu_flat_work_group_size(1, {requiredMaxThreadsPerBlock})))"
-
-HIPRenderer = functools.partial(uops_to_cstyle, HIPLanguage())
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/renderer/llvmir.py` & `tinygrad_tools-0.8.2/tinygrad/renderer/llvmir.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Final, Dict, Callable, Any, List, Optional
 from llvmlite import ir
 from tinygrad.codegen.linearizer import UOps, UOp
 from tinygrad.dtype import DType, PtrDType, dtypes
 from tinygrad.ops import Op, UnaryOps, BinaryOps, TernaryOps
 from tinygrad.codegen.uops import UOpGraph
+from tinygrad.renderer import Renderer
 
 MFLAGS = ('nsz', 'arcp', 'contract', 'afn', 'reassoc') # All from fast math, but nnan and ninf
 
 def is_bool_or_unsigned(dtype: DType): return dtype == dtypes.bool or dtypes.is_unsigned(dtype)
 
 code_for_op: Final[Dict[Op, Callable]] = {
   UnaryOps.NEG: lambda builder, x, dtype: builder.neg(x) if dtypes.is_int(dtype) else \
@@ -61,92 +62,99 @@
     if dtypes.is_int(output_type): return bb[-1].trunc(val, llvm_type) if input_type.itemsize > output_type.itemsize else bb[-1].sext(val, llvm_type)
     if output_type == dtypes.bool: return bb[-1].icmp_signed('!=', val, ir.Constant(val.type, 0))
 
   raise NotImplementedError(f"cast from {input_type} -> {output_type} not implemented")
 
 def const(args, dtype): return ir.Constant(dtype_to_llvm_dtype[dtype], args)
 
-def uops_to_llvm_ir(function_name:str, uops:UOpGraph) -> str:
-  # all llvm stuff goes into a module
-  module = ir.Module(name=__file__)
-
-  # extract global buffers (NOTE: this isn't right if DEFINE_GLOBAL is out of order)
-  buf_to_dtype = {u.arg:u.dtype for u in uops if u.uop in {UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR}}
-  buf_index = {x:i for i,x in enumerate(buf_to_dtype.keys())}
-
-  # create llvm function
-  func_dtypes = [(dtype_to_llvm_dtype[dtype],dtype) for dtype in buf_to_dtype.values() if dtype is not None]
-  func = ir.Function(module, ir.FunctionType(ir.VoidType(), [x.as_pointer() if isinstance(dt, PtrDType) else x for x,dt in func_dtypes]), name=function_name)  # noqa: E501
-  for a in func.args:
-    if a.type.is_pointer: a.add_attribute("noalias")
-
-  # add the function attribute "no-nans-fp-math"="true", which informs llvm that it allowed to use vectorization optimizations
-  func.attributes._known = func.attributes._known.union(frozenset(['"no-nans-fp-math"="true"']))
-  func.attributes.add('"no-nans-fp-math"="true"')
-
-  bb = [ir.IRBuilder(func.append_basic_block("entry"))]
-  loop_blocks: List = []
-  reduce_phis: List = []
-  # TODO: newvar probably shouldn't be optional
-  lvars: Dict[Optional[UOp], Any] = {}  # this Any is an llvm type
-
-  for bufname,dtype in buf_to_dtype.items():
-    if not isinstance(dtype, PtrDType) and dtype == dtypes.int32: lvars[bufname] = bb[-1].sext(func.args[buf_index[bufname]], ir.IntType(32))
-
-  for u in uops:
-    uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
-    if uop is UOps.STORE:
-      element = cast(bb, lvars[vin[2]], vin[2].dtype, vin[0].dtype)
-      def store_op(): bb[-1].store(element, bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
-      if len(vin) > 3:
-        with bb[-1].if_then(lvars[vin[3]]): store_op()
-      else: store_op()
-    elif uop is UOps.ENDLOOP:
-      loop_entry_bb, phis = loop_blocks.pop()
-      idx_p1 = bb[-1].add(lvars[vin[0]], ir.Constant(ir.IntType(32), 1))
-      lvars[vin[0]].add_incoming(idx_p1, bb[-1].block)
-      for n,phi in phis: phi.add_incoming(lvars[n], bb[-1].block)
-      bb.append(ir.IRBuilder(func.append_basic_block(f"loop_exit_{len(loop_blocks)}")))
-      bb[-2].cbranch(bb[-2].icmp_unsigned("<", idx_p1, lvars[vin[0].vin[1]]), loop_entry_bb, bb[-1].block)
-    else:
-      assert dtype is not None, f"None dtype for uop {uop}"
-      if uop is UOps.LOOP:
-        bb.append(ir.IRBuilder(func.append_basic_block(f"loop_body_{len(loop_blocks)}")))
-        bb[-2].branch(bb[-1].block)
-
-        phis = []
-        for rp in reduce_phis:
-          incoming = lvars[rp]
-          lvars[rp] = bb[-1].phi(dtype_to_llvm_dtype[rp.dtype])
-          lvars[rp].add_incoming(incoming, bb[-2].block)
-          phis.append((rp, lvars[rp]))
-
-        lvars[u] = bb[-1].phi(ir.IntType(32), name=f"loop{len(loop_blocks)}")
-        lvars[u].add_incoming(lvars[vin[0]], bb[-2].block)
-        loop_blocks.append((bb[-1].block, phis))
-      elif uop is UOps.DEFINE_ACC:
-        lvars[u] = const(args, dtype)
-        reduce_phis.append(u)
-      elif uop is UOps.LOAD:
-        if len(vin) > 2:
-          aug_idx = bb[-1].select(lvars[vin[2]], lvars[vin[1]], ir.Constant(ir.IntType(32), 0))
-          val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [aug_idx], inbounds=True))
-          val = bb[-1].select(lvars[vin[2]], val, lvars[vin[3]])
+class LLVMRenderer(Renderer):
+  device = "LLVM"
+  supports_float4=False
+  has_local=False
+  has_shared=False
+
+  def render(self, name:str, uops:UOpGraph) -> str:
+    # all llvm stuff goes into a module
+    module = ir.Module(name=__file__)
+
+    # extract global buffers (NOTE: this isn't right if DEFINE_GLOBAL is out of order)
+    buf_to_dtype = {u.arg:u.dtype for u in uops if u.uop in {UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR}}
+    buf_index = {x:i for i,x in enumerate(buf_to_dtype.keys())}
+
+    # create llvm function
+    func_dtypes = [(dtype_to_llvm_dtype[dtype],dtype) for dtype in buf_to_dtype.values() if dtype is not None]
+    func = ir.Function(module, ir.FunctionType(ir.VoidType(), [x.as_pointer() if isinstance(dt, PtrDType) else x for x,dt in func_dtypes]), name=name)
+    for a in func.args:
+      if a.type.is_pointer: a.add_attribute("noalias")
+
+    # add the function attribute "no-nans-fp-math"="true", which informs llvm that it allowed to use vectorization optimizations
+    func.attributes._known = func.attributes._known.union(frozenset(['"no-nans-fp-math"="true"']))
+    func.attributes.add('"no-nans-fp-math"="true"')
+
+    bb = [ir.IRBuilder(func.append_basic_block("entry"))]
+    loop_blocks: List = []
+    reduce_phis: List = []
+    # TODO: newvar probably shouldn't be optional
+    lvars: Dict[Optional[UOp], Any] = {}  # this Any is an llvm type
+
+    for bufname,dtype in buf_to_dtype.items():
+      if not isinstance(dtype, PtrDType) and dtype == dtypes.int32: lvars[bufname] = bb[-1].sext(func.args[buf_index[bufname]], ir.IntType(32))
+
+    for u in uops:
+      uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
+      if uop is UOps.STORE:
+        element = cast(bb, lvars[vin[2]], vin[2].dtype, vin[0].dtype)
+        if len(vin) > 3:
+          with bb[-1].if_then(lvars[vin[3]]):
+            bb[-1].store(element, bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
         else:
-          val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
-        lvars[u] = val
-      elif uop is UOps.PHI:
-        lvars[u] = lvars[vin[1]]
-        # PHI UOps can link to other PHI Uops, backtrace this to DEFINE_ACC
-        backward = vin[0]
-        while backward.uop is UOps.PHI: backward = backward.vin[0]
-        lvars[backward] = lvars[u]
-      elif uop is UOps.ALU:
-        lvars[u] = code_for_op[args](bb[-1], *[lvars[x] for x in vin], dtype if args not in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else vin[0].dtype)
-      elif uop in {UOps.CAST, UOps.BITCAST}: lvars[u] = cast(bb, lvars[vin[0]], vin[0].dtype, dtype, bitcast=uop is UOps.BITCAST)
-      elif uop in {UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR}: lvars[u] = func.args[buf_index[args]]
-      elif uop is UOps.SPECIAL: lvars[u] = lvars[args.expr]
-      elif uop is UOps.CONST: lvars[u] = const(args, dtype)
-      else: raise RuntimeError(f"failed to render {uop}")
+          bb[-1].store(element, bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
+      elif uop is UOps.ENDLOOP:
+        loop_entry_bb, phis = loop_blocks.pop()
+        idx_p1 = bb[-1].add(lvars[vin[0]], ir.Constant(ir.IntType(32), 1))
+        lvars[vin[0]].add_incoming(idx_p1, bb[-1].block)
+        for n,phi in phis: phi.add_incoming(lvars[n], bb[-1].block)
+        bb.append(ir.IRBuilder(func.append_basic_block(f"loop_exit_{len(loop_blocks)}")))
+        bb[-2].cbranch(bb[-2].icmp_unsigned("<", idx_p1, lvars[vin[0].vin[1]]), loop_entry_bb, bb[-1].block)
+      else:
+        assert dtype is not None, f"None dtype for uop {uop}"
+        if uop is UOps.LOOP:
+          bb.append(ir.IRBuilder(func.append_basic_block(f"loop_body_{len(loop_blocks)}")))
+          bb[-2].branch(bb[-1].block)
+
+          phis = []
+          for rp in reduce_phis:
+            incoming = lvars[rp]
+            lvars[rp] = bb[-1].phi(dtype_to_llvm_dtype[rp.dtype])
+            lvars[rp].add_incoming(incoming, bb[-2].block)
+            phis.append((rp, lvars[rp]))
+
+          lvars[u] = bb[-1].phi(ir.IntType(32), name=f"loop{len(loop_blocks)}")
+          lvars[u].add_incoming(lvars[vin[0]], bb[-2].block)
+          loop_blocks.append((bb[-1].block, phis))
+        elif uop is UOps.DEFINE_ACC:
+          lvars[u] = const(args[0], dtype)
+          reduce_phis.append(u)
+        elif uop is UOps.LOAD:
+          if len(vin) > 2:
+            aug_idx = bb[-1].select(lvars[vin[2]], lvars[vin[1]], ir.Constant(ir.IntType(32), 0))
+            val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [aug_idx], inbounds=True))
+            val = bb[-1].select(lvars[vin[2]], val, lvars[vin[3]])
+          else:
+            val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
+          lvars[u] = val
+        elif uop is UOps.PHI:
+          lvars[u] = lvars[vin[1]]
+          # PHI UOps can link to other PHI Uops, backtrace this to DEFINE_ACC
+          backward = vin[0]
+          while backward.uop is UOps.PHI: backward = backward.vin[0]
+          lvars[backward] = lvars[u]
+        elif uop is UOps.ALU:
+          lvars[u] = code_for_op[args](bb[-1], *[lvars[x] for x in vin], dtype if args not in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else vin[0].dtype)
+        elif uop in {UOps.CAST, UOps.BITCAST}: lvars[u] = cast(bb, lvars[vin[0]], vin[0].dtype, dtype, bitcast=uop is UOps.BITCAST)
+        elif uop in {UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR}: lvars[u] = func.args[buf_index[args]]
+        elif uop is UOps.SPECIAL: lvars[u] = lvars[args.expr]
+        elif uop is UOps.CONST: lvars[u] = const(args, dtype)
+        else: raise RuntimeError(f"failed to render {uop}")
 
-  bb[-1].ret_void()
-  return str(module)
+    bb[-1].ret_void()
+    return str(module)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/amd_gpu.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/amd_gpu.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/comgr.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/comgr.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/cuda.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/cuda.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/hip.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/hip.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/hsa.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/hsa.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/kfd.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/kfd.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/nv_gpu.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/nv_gpu.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/autogen/opencl.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/autogen/opencl.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/driver/hip_comgr.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/driver/hip_comgr.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/driver/hsa.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/driver/hsa.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/graph/clang.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/graph/clang.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import List, Dict, cast
 import ctypes
 from tinygrad.helpers import dedup, cpu_time_execution, GraphException, DEBUG
 from tinygrad.engine.jit import GraphRunner
-from tinygrad.device import Buffer, Device, CompiledRunner
-from tinygrad.engine.realize import ExecItem
+from tinygrad.device import Buffer, Device
+from tinygrad.engine.realize import ExecItem, CompiledRunner
 from tinygrad.shape.symbolic import Variable
 from tinygrad.runtime.ops_clang import ClangProgram
-from tinygrad.renderer.cstyle import ClangLanguage
-render_dtype = ClangLanguage().render_dtype
+from tinygrad.renderer.cstyle import ClangRenderer
+render_dtype = ClangRenderer().render_dtype
 
 class ClangGraph(GraphRunner):
   def __init__(self, jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
     super().__init__(jit_cache, input_rawbuffers, var_vals)
     if not all(isinstance(ji.prg, CompiledRunner) for ji in jit_cache): raise GraphException
 
-    prgs = '\n'.join(dedup([cast(CompiledRunner, ji.prg).prg for ji in jit_cache]))
+    prgs = '\n'.join(dedup([cast(CompiledRunner, ji.prg).p.src for ji in jit_cache]))
     args = [f"{render_dtype(x.dtype)}* arg{i}" for i,x in enumerate(input_rawbuffers)]
     args += [f"int {v.expr}" for v in var_vals]
     code = ["void batched("+','.join(args)+") {"]
     for ji in jit_cache:
       args = []
       for buf in ji.bufs:
         assert buf is not None
         if buf in input_rawbuffers:
           args.append(f"arg{input_rawbuffers.index(buf)}")
         else:
           args.append(f"({render_dtype(buf.dtype)}*)0x{ctypes.addressof(buf._buf):X}")
-      args += [x.expr for x in cast(CompiledRunner, ji.prg).vars]
-      code.append(f"  {cast(CompiledRunner, ji.prg).name}({','.join(args)});")
+      args += [x.expr for x in cast(CompiledRunner, ji.prg).p.vars]
+      code.append(f"  {cast(CompiledRunner, ji.prg).p.function_name}({','.join(args)});")
     code.append("}")
     if DEBUG >= 4: print("\n".join(code))
     compiler = Device["CLANG"].compiler
     assert compiler is not None
     self.clprg = ClangProgram("batched", compiler.compile(prgs+"\n"+"\n".join(code))) # no point in caching the pointers
 
   def __call__(self, rawbufs: List[Buffer], var_vals: Dict[Variable, int], wait=False):
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/graph/cuda.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/graph/cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes
 from typing import Any, Optional, Tuple, Dict, List, cast
 import tinygrad.runtime.autogen.cuda as cuda
 from tinygrad.helpers import init_c_var, GraphException
-from tinygrad.device import CompiledRunner, Buffer, BufferXfer, Device
+from tinygrad.device import Buffer, Device
 from tinygrad.runtime.ops_cuda import CUDADevice, check, encode_args, cu_time_execution
 from tinygrad.shape.symbolic import Variable
-from tinygrad.engine.realize import ExecItem
+from tinygrad.engine.realize import ExecItem, BufferXfer, CompiledRunner
 from tinygrad.engine.jit import MultiGraphRunner
 
 class CUDAGraph(MultiGraphRunner):
   def __init__(self, jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
     super().__init__(jit_cache, input_rawbuffers, var_vals)
 
     # Check all jit items are compatible.
@@ -18,22 +18,22 @@
     self.jc_idx_with_updatable_rawbufs = list(set([x[0] for x in self.input_replace.keys()]))
     self.updatable_nodes: Dict[int, Tuple[Any, Any, Any, bool]] = {} # Dict[jc index] = tuple(graph node, node params, input kernel params, is memcpy)
 
     self.graph = init_c_var(cuda.CUgraph(), lambda x: check(cuda.cuGraphCreate(ctypes.byref(x), 0)))
 
     for j,ji in enumerate(self.jit_cache):
       if isinstance(ji.prg, CompiledRunner):
-        global_size, local_size = ji.prg.launch_dims(var_vals)
+        global_size, local_size = ji.prg.p.launch_dims(var_vals)
 
         new_node = cuda.CUgraphNode()
-        deps = self._access_resources([x.base for x in ji.bufs[ji.prg.outcount:] if x is not None],
-                                      [x.base for x in ji.bufs[:ji.prg.outcount] if x is not None], new_dependency=new_node)
+        deps = self._access_resources([x.base for x in ji.bufs[ji.prg.p.outcount:] if x is not None],
+                                      [x.base for x in ji.bufs[:ji.prg.p.outcount] if x is not None], new_dependency=new_node)
         c_deps = (cuda.CUgraphNode*len(deps))(*deps) if deps else None
 
-        c_args, vargs = encode_args([cast(Buffer, x)._buf for x in ji.bufs], [var_vals[x] for x in ji.prg.vars])
+        c_args, vargs = encode_args([cast(Buffer, x)._buf for x in ji.bufs], [var_vals[x] for x in ji.prg.p.vars])
         kern_params = cuda.CUDA_KERNEL_NODE_PARAMS(ji.prg.clprg.prg, *global_size, *local_size, 0, None, vargs)
         check(cuda.cuGraphAddKernelNode(ctypes.byref(new_node), self.graph, c_deps, len(deps), ctypes.byref(kern_params)))
 
         if j in self.jc_idx_with_updatable_launch_dims or j in self.jc_idx_with_updatable_var_vals or j in self.jc_idx_with_updatable_rawbufs:
           self.updatable_nodes[j] = (new_node, kern_params, c_args, False)
       elif isinstance(ji.prg, BufferXfer):
         dest, src = [cast(Buffer, x) for x in ji.bufs[0:2]]
@@ -55,20 +55,20 @@
       if not self.updatable_nodes[j][3]: setattr(self.updatable_nodes[j][2], f'f{i}', input_rawbuffers[input_idx]._buf)
       else:
         if i == 0: self.updatable_nodes[j][1].destDevice = input_rawbuffers[input_idx]._buf
         elif i == 1: self.updatable_nodes[j][1].srcDevice = input_rawbuffers[input_idx]._buf
 
     # Update var_vals in the c_args struct.
     for j in self.jc_idx_with_updatable_var_vals:
-      for i,v in enumerate(cast(CompiledRunner, self.jit_cache[j].prg).vars):
+      for i,v in enumerate(cast(CompiledRunner, self.jit_cache[j].prg).p.vars):
         setattr(self.updatable_nodes[j][2], f'v{i}', var_vals[v])
 
     # Update launch dims in the kern_params struct.
     for j in self.jc_idx_with_updatable_launch_dims:
-      self.set_kernel_node_launch_dims(self.updatable_nodes[j][1], *cast(CompiledRunner, self.jit_cache[j].prg).launch_dims(var_vals))
+      self.set_kernel_node_launch_dims(self.updatable_nodes[j][1], *cast(CompiledRunner, self.jit_cache[j].prg).p.launch_dims(var_vals))
 
     # Update graph nodes with the updated structs.
     for node, c_node_params, c_args, is_copy in self.updatable_nodes.values():
       if not is_copy: check(cuda.cuGraphExecKernelNodeSetParams(self.instance, node, ctypes.byref(c_node_params)))
       else: check(cuda.cuGraphExecMemcpyNodeSetParams(self.instance, node, ctypes.byref(c_node_params), c_args))
 
     return cu_time_execution(lambda: check(cuda.cuGraphLaunch(self.instance, None)), enable=wait)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/graph/hsa.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/graph/hsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes, collections, time, itertools
 from typing import List, Any, Dict, cast, Optional, Tuple
 from tinygrad.helpers import GraphException, init_c_var, round_up
-from tinygrad.buffer import Buffer, BufferOptions
-from tinygrad.device import Compiled, CompiledRunner, BufferXfer, Device
+from tinygrad.device import Buffer, BufferOptions
+from tinygrad.device import Compiled, Device
 from tinygrad.shape.symbolic import Variable
 from tinygrad.runtime.ops_hsa import HSADevice, PROFILE, Profiler
-from tinygrad.engine.realize import ExecItem
+from tinygrad.engine.realize import ExecItem, BufferXfer, CompiledRunner
 from tinygrad.engine.jit import MultiGraphRunner
 import tinygrad.runtime.autogen.hsa as hsa
 from tinygrad.runtime.driver.hsa import check, AQLQueue, AQL_PACKET_SIZE, EMPTY_SIGNAL
 
 def dedup_signals(signals): return [hsa.hsa_signal_t(hndl) for hndl in set([x.handle for x in signals if isinstance(x, hsa.hsa_signal_t)])]
 
 class VirtAQLQueue(AQLQueue):
@@ -49,15 +49,15 @@
     # Fill initial arguments.
     self.ji_kargs_structs: Dict[int, ctypes.Structure] = {}
     for j,ji in enumerate(self.jit_cache):
       if not isinstance(ji.prg, CompiledRunner): continue
       self.ji_kargs_structs[j] = ji.prg.clprg.args_struct_t.from_address(kernargs_ptrs[ji.prg.device])
       kernargs_ptrs[ji.prg.device] += round_up(ctypes.sizeof(ji.prg.clprg.args_struct_t), 16)
       for i in range(len(ji.bufs)): self.ji_kargs_structs[j].__setattr__(f'f{i}', cast(Buffer, ji.bufs[i])._buf)
-      for i in range(len(ji.prg.vars)): self.ji_kargs_structs[j].__setattr__(f'v{i}', var_vals[ji.prg.vars[i]])
+      for i in range(len(ji.prg.p.vars)): self.ji_kargs_structs[j].__setattr__(f'v{i}', var_vals[ji.prg.p.vars[i]])
 
     # Build queues.
     self.virt_aql_queues: Dict[Compiled, VirtAQLQueue] = {dev:VirtAQLQueue(dev, 2*len(self.jit_cache)+16) for dev in self.devices}
     self.packets = {}
     self.transfers = []
     self.ji_to_transfer: Dict[int, int] = {} # faster to store transfers as list and update using this mapping table.
     self.signals_to_reset: List[hsa.hsa_signal_t] = []
@@ -66,21 +66,21 @@
 
     # Special packet to wait for the world.
     self.kickoff_signals: Dict[HSADevice, hsa.hsa_signal_t] = {dev:self.alloc_signal(reset_on_start=True) for dev in self.devices}
     for dev in self.devices: self.virt_aql_queues[dev].submit_barrier([], self.kickoff_signals[dev])
 
     for j,ji in enumerate(self.jit_cache):
       if isinstance(ji.prg, CompiledRunner):
-        wait_signals = self.access_resources(ji.bufs[(outs:=ji.prg.outcount):], ji.bufs[:outs], new_dependency=j, sync_with_aql_packets=False)
+        wait_signals = self.access_resources(ji.bufs[(outs:=ji.prg.p.outcount):], ji.bufs[:outs], new_dependency=j, sync_with_aql_packets=False)
         for i in range(0, len(wait_signals), 5):
           self.virt_aql_queues[ji.prg.device].submit_barrier(wait_signals[i:i+5])
         self.packets[j] = hsa.hsa_kernel_dispatch_packet_t.from_address(self.virt_aql_queues[ji.prg.device].write_addr)
 
         sync_signal = self.alloc_signal(reset_on_start=True) if PROFILE else None
-        self.virt_aql_queues[ji.prg.device].submit_kernel(ji.prg.clprg, *ji.prg.launch_dims(var_vals), #type:ignore
+        self.virt_aql_queues[ji.prg.device].submit_kernel(ji.prg.clprg, *ji.prg.p.launch_dims(var_vals), #type:ignore
                                                           ctypes.addressof(self.ji_kargs_structs[j]), completion_signal=sync_signal)
         if PROFILE: self.profile_info[ji.prg.device].append((sync_signal, ji.prg.clprg.name, False))
       elif isinstance(ji.prg, BufferXfer):
         dest, src = [cast(Buffer, x) for x in ji.bufs[0:2]]
         dest_dev, src_dev = cast(HSADevice, Device[dest.device]), cast(HSADevice, Device[src.device])
         sync_signal = self.alloc_signal(reset_on_start=True, wait_on=[dest_dev, src_dev])
 
@@ -118,20 +118,20 @@
         self.ji_kargs_structs[j].__setattr__(f'f{i}', input_rawbuffers[input_idx]._buf)
       else:
         if i == 0: self.transfers[self.ji_to_transfer[j]][0] = input_rawbuffers[input_idx]._buf # dest
         elif i == 1: self.transfers[self.ji_to_transfer[j]][2] = input_rawbuffers[input_idx]._buf # src
 
     # Update var_vals
     for j in self.jc_idx_with_updatable_var_vals:
-      for i,v in enumerate(cast(CompiledRunner, self.jit_cache[j].prg).vars):
+      for i,v in enumerate(cast(CompiledRunner, self.jit_cache[j].prg).p.vars):
         self.ji_kargs_structs[j].__setattr__(f'v{i}', var_vals[v])
 
     # Update launch dims
     for j in self.jc_idx_with_updatable_launch_dims:
-      gl, lc = cast(CompiledRunner, self.jit_cache[j].prg).launch_dims(var_vals)
+      gl, lc = cast(CompiledRunner, self.jit_cache[j].prg).p.launch_dims(var_vals)
       self.packets[j].workgroup_size_x = lc[0]
       self.packets[j].workgroup_size_y = lc[1]
       self.packets[j].workgroup_size_z = lc[2]
       self.packets[j].grid_size_x = gl[0] * lc[0]
       self.packets[j].grid_size_y = gl[1] * lc[1]
       self.packets[j].grid_size_z = gl[2] * lc[2]
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/graph/metal.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/graph/metal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Any, Dict, cast, Optional
 import Metal
 from tinygrad.dtype import dtypes
 from tinygrad.helpers import dedup, unwrap2, GraphException
-from tinygrad.device import Buffer, CompiledRunner
-from tinygrad.engine.realize import ExecItem
+from tinygrad.device import Buffer
+from tinygrad.engine.realize import ExecItem, CompiledRunner
 from tinygrad.engine.jit import GraphRunner
 from tinygrad.shape.symbolic import Variable
 from tinygrad.runtime.ops_metal import wait_check
 
 class MetalGraph(GraphRunner):
   def __init__(self, jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
     super().__init__(jit_cache, input_rawbuffers, var_vals)
@@ -34,32 +34,32 @@
       icb_command = self.icb.indirectComputeCommandAtIndex_(j)
       icb_command.setComputePipelineState_(unwrap2(
         self.device.device.newComputePipelineStateWithDescriptor_options_reflection_error_(descriptor, Metal.MTLPipelineOption(0), None, None)))
       for i,b in enumerate(ji.bufs):
         if b is not None:
           icb_command.setKernelBuffer_offset_atIndex_(b._buf, 0, i)
           all_resources.append(b._buf)
-      for i,v in enumerate(prg.vars): icb_command.setKernelBuffer_offset_atIndex_(self.int_buf, self.vars.index(v)*4, len(ji.bufs)+i)
+      for i,v in enumerate(prg.p.vars): icb_command.setKernelBuffer_offset_atIndex_(self.int_buf, self.vars.index(v)*4, len(ji.bufs)+i)
       if j not in self.jc_idx_with_updatable_launch_dims:
-        global_size, local_size = prg.launch_dims(var_vals)
+        global_size, local_size = prg.p.launch_dims(var_vals)
         icb_command.concurrentDispatchThreadgroups_threadsPerThreadgroup_(Metal.MTLSize(*global_size), Metal.MTLSize(*local_size))
       icb_command.setBarrier()
 
     self.all_resources = dedup(all_resources)
     self.command_buffer: Any = None
     if len(self.vars): self.int_buf_view = self.int_buf.contents().as_buffer(self.int_buf.length()).cast('i')
 
   def __call__(self, input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int], wait=False) -> Optional[float]:
     if self.command_buffer is not None and self.command_buffer in self.device.mtl_buffers_in_flight: wait_check(self.command_buffer)
     all_resources = dedup(self.all_resources + [x._buf for x in input_rawbuffers])
 
     for (j,i),input_idx in self.input_replace.items():
       self.icb.indirectComputeCommandAtIndex_(j).setKernelBuffer_offset_atIndex_(input_rawbuffers[input_idx]._buf, 0, i)
     for j in self.jc_idx_with_updatable_launch_dims:
-      global_size, local_size = cast(CompiledRunner, self.jit_cache[j].prg).launch_dims(var_vals)
+      global_size, local_size = cast(CompiledRunner, self.jit_cache[j].prg).p.launch_dims(var_vals)
       self.icb.indirectComputeCommandAtIndex_(j).concurrentDispatchThreadgroups_threadsPerThreadgroup_(Metal.MTLSize(*global_size),
                                                                                                        Metal.MTLSize(*local_size))
     for j, var in enumerate(self.vars): self.int_buf_view[j] = var_vals[var]
 
     command_buffer = self.device.mtl_queue.commandBuffer()
     encoder = command_buffer.computeCommandEncoder()
     encoder.useResources_count_usage_(all_resources, len(all_resources), Metal.MTLResourceUsageRead | Metal.MTLResourceUsageWrite)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_amd.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_amd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
-from typing import Tuple, List, Any
-import os, fcntl, ctypes, functools, re, pathlib, mmap, struct, errno, subprocess
-from tinygrad.device import Compiled, LRUAllocator, Compiler, CompilerOptions
-from tinygrad.buffer import BufferOptions
+from typing import Tuple, List, Any, cast
+import os, fcntl, ctypes, ctypes.util, functools, re, pathlib, mmap, struct, errno, subprocess, time
+from tinygrad.device import Compiled, Compiler, BufferOptions, LRUAllocator
 from tinygrad.helpers import getenv, from_mv, init_c_struct_t, to_mv, round_up, DEBUG
 from tinygrad.renderer.cstyle import HIPRenderer
 from tinygrad.runtime.driver.hip_comgr import compile_hip
+from tinygrad.runtime.ops_hsa import HSACompiler
 import tinygrad.runtime.autogen.kfd as kfd
 import tinygrad.runtime.autogen.hsa as hsa
 import tinygrad.runtime.autogen.amd_gpu as amd_gpu
 if getenv("IOCTL"): import extra.hip_gpu_driver.hip_ioctl  # noqa: F401
 
-libc = ctypes.CDLL("libc.so.6")
+libc = ctypes.CDLL(ctypes.util.find_library("c"))
 libc.mmap.argtypes = [ctypes.c_void_p, ctypes.c_size_t, ctypes.c_int, ctypes.c_int, ctypes.c_int, ctypes.c_long]
 libc.mmap.restype = ctypes.c_void_p
 libc.munmap.argtypes = [ctypes.c_void_p, ctypes.c_size_t]
 libc.munmap.restype = ctypes.c_int
 
+if getenv("MOCKGPU"):
+  import extra.mockgpu.mockgpu  # noqa: F401
+  libc.mmap = extra.mockgpu.mockgpu._mmap # type: ignore
+  libc.munmap = extra.mockgpu.mockgpu._munmap # type: ignore
+
 def is_usable_gpu(gpu_id):
   try:
     with gpu_id.open() as f:
       return int(f.read()) != 0
   except OSError:
     return False
 
@@ -65,31 +70,25 @@
     new_name = name[16:-4].lower()
     structs[new_name] = init_c_struct_t(tuple(fields))
     assert ctypes.sizeof(structs[new_name]) == ctypes.sizeof(pkt), f"{ctypes.sizeof(structs[new_name])} != {ctypes.sizeof(pkt)}"
   return type("SDMA_PKTS", (object, ), structs)
 sdma_pkts = create_sdma_packets()
 
 class AMDCompiler(Compiler):
-  compiler_opts = CompilerOptions("AMD", has_tensor_cores=True, shared_max=65536)
   def __init__(self, arch:str):
     self.arch = arch
     super().__init__(f"compile_hip_{self.arch}")
-  def render(self, name:str, uops) -> str: return HIPRenderer(name, uops)
   def compile(self, src:str) -> bytes: return compile_hip(src, self.arch)
 
-SDMA_MAX_COPY_SIZE = 0x400000
 PAGE_SIZE = 0x1000
 SIGNAL_SIZE, SIGNAL_COUNT = ctypes.sizeof(hsa.amd_signal_t), 16384
-SHT_PROGBITS, SHF_ALLOC = 0x1, 0x2
-EMPTY_SIGNAL = hsa.hsa_signal_t()
 SIGNAL_VALUE_OFFSET = getattr(hsa.amd_signal_t, 'value').offset
 
 BASE_ADDR = 0x00001260
-PACKET3_SET_SH_REG_START = 0x2c00
-SUB = PACKET3_SET_SH_REG_START - BASE_ADDR
+SUB = amd_gpu.PACKET3_SET_SH_REG_START - BASE_ADDR
 
 regCOMPUTE_PGM_LO = 0x1bac - SUB
 regCOMPUTE_PGM_RSRC1 = 0x1bb2 - SUB
 regCOMPUTE_USER_DATA_0 = 0x1be0 - SUB
 regCOMPUTE_START_X = 0x1ba4 - SUB
 regCOMPUTE_TMPRING_SIZE = 0x1bb8 - SUB
 regCOMPUTE_RESOURCE_LIMITS = 0x1bb5 - SUB
@@ -101,68 +100,28 @@
 regBIF_BX_PF1_GPU_HDP_FLUSH_REQ = 0x0106
 regBIF_BX_PF1_GPU_HDP_FLUSH_DONE = 0x0107
 
 # VGT_EVENT_TYPE in navi10_enum.h
 CACHE_FLUSH_AND_INV_TS_EVENT = 0x14
 CS_PARTIAL_FLUSH = 0x7
 
+WAIT_REG_MEM_FUNCTION_EQ = 3 # ==
+WAIT_REG_MEM_FUNCTION_GEQ = 5 # >=
+
 COMPUTE_SHADER_EN = 1
 FORCE_START_AT_000 = 1 << 2
 CS_W32_EN = 1 << 15
 
-def format_struct(s):
-  sdats = []
-  for field_name, field_type in s._fields_:
-    dat = getattr(s, field_name)
-    if isinstance(dat, int): sdats.append(f"{field_name}:0x{dat:X}")
-    else: sdats.append(f"{field_name}:{dat}")
-  return sdats
-
-"""
-regCOMPUTE_PGM_RSRC1 0 0x1bb2 12 0 0
-	VGPRS 0 5
-	SGPRS 6 9
-	PRIORITY 10 11
-	FLOAT_MODE 12 19
-	PRIV 20 20
-	DX10_CLAMP 21 21
-	IEEE_MODE 23 23
-	BULKY 24 24
-	FP16_OVFL 26 26
-	WGP_MODE 29 29
-	MEM_ORDERED 30 30
-	FWD_PROGRESS 31 31
-regCOMPUTE_PGM_RSRC2 0 0x1bb3 11 0 0
-	SCRATCH_EN 0 0
-	USER_SGPR 1 5
-	TRAP_PRESENT 6 6
-	TGID_X_EN 7 7
-	TGID_Y_EN 8 8
-	TGID_Z_EN 9 9
-	TG_SIZE_EN 10 10
-	TIDIG_COMP_CNT 11 12
-	EXCP_EN_MSB 13 14
-	LDS_SIZE 15 23
-	EXCP_EN 24 30
-regCOMPUTE_RESOURCE_LIMITS 0 0x1bb5 6 0 0
-	WAVES_PER_SH 0 9
-	TG_PER_CU 12 15
-	LOCK_THRESHOLD 16 21
-	SIMD_DEST_CNTL 22 22
-	FORCE_SIMD_DIST 23 23
-	CU_GROUP_COUNT 24 26
-"""
-
 class HWPM4Queue:
   def __init__(self): self.q = []
 
   def hdp_flush(self):
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_WAIT_REG_MEM, 5),
-      amd_gpu.WAIT_REG_MEM_MEM_SPACE(0) | amd_gpu.WAIT_REG_MEM_OPERATION(1) | amd_gpu.WAIT_REG_MEM_FUNCTION(3) | amd_gpu.WAIT_REG_MEM_ENGINE(0),
-      regBIF_BX_PF1_GPU_HDP_FLUSH_REQ, regBIF_BX_PF1_GPU_HDP_FLUSH_DONE, 0x0, 0x0, 0x20]
+      amd_gpu.WAIT_REG_MEM_MEM_SPACE(0) | amd_gpu.WAIT_REG_MEM_OPERATION(1) | amd_gpu.WAIT_REG_MEM_FUNCTION(WAIT_REG_MEM_FUNCTION_EQ) | \
+      amd_gpu.WAIT_REG_MEM_ENGINE(0), regBIF_BX_PF1_GPU_HDP_FLUSH_REQ, regBIF_BX_PF1_GPU_HDP_FLUSH_DONE, 0x0, 0x0, 0x20]
 
   def invalidate_cache(self):
     # overkill?
     addr=0x0
     sz=(1 << 64)-1
     gli=1
     glv=1
@@ -197,43 +156,36 @@
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 2), regCOMPUTE_PGM_RSRC1, rsrc1, rsrc2 | (lds_size << 15)]
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 1), regCOMPUTE_TMPRING_SIZE, 0x00200200] # (waveSize << 12) | (numWaves)
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 4), regCOMPUTE_RESTART_X, 0,0,0,0]
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 2), regCOMPUTE_STATIC_THREAD_MGMT_SE0, 0xFFFFFFFF,0xFFFFFFFF]
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 2), regCOMPUTE_STATIC_THREAD_MGMT_SE2, 0xFFFFFFFF,0xFFFFFFFF]
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 4), regCOMPUTE_STATIC_THREAD_MGMT_SE4, 0xFFFFFFFF,0xFFFFFFFF,0xFFFFFFFF,0xFFFFFFFF]
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 2), regCOMPUTE_USER_DATA_0, kernargs&0xFFFFFFFF, kernargs>>32]
-    self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 8), regCOMPUTE_START_X, 0,0,0, local_size[0],local_size[1],local_size[2],0,0]
+    self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 8), regCOMPUTE_START_X, 0, 0, 0, *local_size, 0, 0]
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_SET_SH_REG, 1), regCOMPUTE_RESOURCE_LIMITS, 0]
-    self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_DISPATCH_DIRECT, 3),
-               global_size[0],global_size[1],global_size[2], CS_W32_EN | FORCE_START_AT_000 | COMPUTE_SHADER_EN]
-
-    # have to self wait since flush doesn't work
-    self.signal(sig:=AMDDevice._get_signal())
-    self.wait(sig)
+    self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_DISPATCH_DIRECT, 3), *global_size, CS_W32_EN | FORCE_START_AT_000 | COMPUTE_SHADER_EN]
     return self
 
   def wait(self, signal:hsa.amd_signal_t, value=0):
     addr = ctypes.addressof(signal) + SIGNAL_VALUE_OFFSET
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_WAIT_REG_MEM, 5),
-      amd_gpu.WAIT_REG_MEM_MEM_SPACE(1) | amd_gpu.WAIT_REG_MEM_OPERATION(0) | amd_gpu.WAIT_REG_MEM_FUNCTION(3) | amd_gpu.WAIT_REG_MEM_ENGINE(0),
-      addr&0xFFFFFFFF, addr>>32, value, 0xffffffff, 4]
+      amd_gpu.WAIT_REG_MEM_MEM_SPACE(1) | amd_gpu.WAIT_REG_MEM_OPERATION(0) | amd_gpu.WAIT_REG_MEM_FUNCTION(WAIT_REG_MEM_FUNCTION_GEQ) | \
+      amd_gpu.WAIT_REG_MEM_ENGINE(0), addr&0xFFFFFFFF, addr>>32, value, 0xffffffff, 4]
     return self
 
   def timestamp(self, addr):
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_RELEASE_MEM, 6),
       # event_index__mec_release_mem__end_of_pipe = 5
       amd_gpu.PACKET3_RELEASE_MEM_EVENT_TYPE(CACHE_FLUSH_AND_INV_TS_EVENT) | amd_gpu.PACKET3_RELEASE_MEM_EVENT_INDEX(5),
       # * 3 - send 64bit GPU counter value
       amd_gpu.PACKET3_RELEASE_MEM_DATA_SEL(3) | amd_gpu.PACKET3_RELEASE_MEM_INT_SEL(0) | amd_gpu.PACKET3_RELEASE_MEM_DST_SEL(0),
       addr&0xFFFFFFFF, addr>>32, 0, 0, 0]
     return self
 
   def signal(self, signal:hsa.amd_signal_t, value=0):
-    #assert signal.value == 0, f"entering signal without it being set to 0, but {signal.value}"
-    signal.value = 1
     # NOTE: this needs an EOP buffer on the queue or it will NULL pointer
     addr = ctypes.addressof(signal) + SIGNAL_VALUE_OFFSET
     self.q += [amd_gpu.PACKET3(amd_gpu.PACKET3_RELEASE_MEM, 6),
         # event_index__mec_release_mem__end_of_pipe = 5
         # event_index__mec_release_mem__shader_done = 6
         amd_gpu.PACKET3_RELEASE_MEM_EVENT_TYPE(CACHE_FLUSH_AND_INV_TS_EVENT) | amd_gpu.PACKET3_RELEASE_MEM_EVENT_INDEX(5) | \
           amd_gpu.PACKET3_RELEASE_MEM_GCR_GLV_INV | amd_gpu.PACKET3_RELEASE_MEM_GCR_GL1_INV | amd_gpu.PACKET3_RELEASE_MEM_GCR_GL2_INV | \
@@ -268,14 +220,15 @@
 sdma_flush_hdp_pkt = sdma_pkts.hdp_flush(0x8, 0x0, 0x80000000, 0x0, 0x0, 0x0)
 sdma_cache_inv = sdma_pkts.gcr(op=amd_gpu.SDMA_OP_GCR, sub_op=amd_gpu.SDMA_SUBOP_USER_GCR, GCR_CONTROL_GL2_WB=1, GCR_CONTROL_GLK_WB=1,
                               GCR_CONTROL_GL2_INV=1, GCR_CONTROL_GL1_INV=1, GCR_CONTROL_GLV_INV=1, GCR_CONTROL_GLK_INV=1,
                               GCR_CONTROL_GL2_RANGE=0)
 sdma_cache_wb = sdma_pkts.gcr(op=amd_gpu.SDMA_OP_GCR, sub_op=amd_gpu.SDMA_SUBOP_USER_GCR, GCR_CONTROL_GL2_WB=1, GCR_CONTROL_GLK_WB=1,
                               GCR_CONTROL_GL2_RANGE=0)
 
+SDMA_MAX_COPY_SIZE = 0x400000
 class HWCopyQueue:
   def __init__(self): self.q = []
 
   def submit(self, device:AMDDevice):
     read_ptr = device.sdma_read_pointer[0]
     if (device.sdma_doorbell_value-read_ptr) > device.sdma_ring.size: raise RuntimeError("SDMA queue overrun")
     for cmd in self.q:
@@ -302,28 +255,27 @@
       self.q.append(sdma_pkts.copy_linear(op=amd_gpu.SDMA_OP_COPY, sub_op=amd_gpu.SDMA_SUBOP_COPY_LINEAR,
                                           count=step_copy_size-1, src_addr=src+copied, dst_addr=dest+copied))
       copied += step_copy_size
     self.q.append(sdma_cache_wb)
     return self
 
   def signal(self, signal:hsa.amd_signal_t, value=0):
-    #assert signal.value == 0
-    signal.value = 1
     self.q.append(sdma_pkts.fence(op=amd_gpu.SDMA_OP_FENCE, mtype=3, addr=ctypes.addressof(signal) + SIGNAL_VALUE_OFFSET, data=value))
     if signal.event_mailbox_ptr != 0:
       self.q.append(sdma_pkts.fence(op=amd_gpu.SDMA_OP_FENCE, mtype=3, addr=signal.event_mailbox_ptr, data=signal.event_id))
       self.q.append(sdma_pkts.trap(op=amd_gpu.SDMA_OP_TRAP, int_ctx=signal.event_id))
     return self
 
-  def wait(self, signal:hsa.amd_signal_t):
-    self.q.append(sdma_pkts.poll_regmem(op=amd_gpu.SDMA_OP_POLL_REGMEM, mem_poll=1, func=0x3,
+  def wait(self, signal:hsa.amd_signal_t, value=0):
+    self.q.append(sdma_pkts.poll_regmem(op=amd_gpu.SDMA_OP_POLL_REGMEM, mem_poll=1, func=WAIT_REG_MEM_FUNCTION_GEQ,
                                         addr=ctypes.addressof(signal) + SIGNAL_VALUE_OFFSET,
-                                        value=0, mask=0xffffffff, interval=0x04, retry_count=0xfff))
+                                        value=value, mask=0xffffffff, interval=0x04, retry_count=0xfff))
     return self
 
+SHT_PROGBITS, SHF_ALLOC = 0x1, 0x2
 class AMDProgram:
   def __init__(self, device:AMDDevice, name:str, lib:bytes):
     # TODO; this API needs the type signature of the function and global_size/local_size
     self.device, self.name, self.lib = device, name, lib
 
     if DEBUG >= 6:
       asm = subprocess.check_output(["/opt/rocm/llvm/bin/llvm-objdump", '-d', '-'], input=lib)
@@ -335,24 +287,25 @@
     lib_gpu_size = round_up(max(sh[5]+sh[3] for sh in sections if sh[1] == SHT_PROGBITS), 0x1000)
     self.lib_gpu = self.device._gpu_alloc(lib_gpu_size, kfd.KFD_IOC_ALLOC_MEM_FLAGS_VRAM, public=True)
     lib_gpu_view = to_mv(self.lib_gpu.va_addr, lib_gpu_size)
 
     for _, sh_type, sh_flags, sh_addr, sh_offset, sh_size, _, _, _ in sections:
       if sh_type == SHT_PROGBITS and sh_flags & SHF_ALLOC: lib_gpu_view[sh_addr:sh_addr+sh_size] = self.lib[sh_offset:sh_offset+sh_size]
 
-    self.device._submit_cache_inv(gli=2)
-
     entry_point = min(sh[3] for sh in sections if sh[1] == SHT_PROGBITS and sh[2] & SHF_ALLOC)
     self.handle = self.lib_gpu.va_addr + entry_point
     self.group_segment_size = lib_gpu_view.cast("I")[entry_point//4]
     self.private_segment_size = lib_gpu_view.cast("I")[entry_point//4 + 1]
     self.kernargs_segment_size = lib_gpu_view.cast("I")[entry_point//4 + 2]
+    self.kernargs_offset = 0
     assert self.private_segment_size <= self.device.max_private_segment_size, \
       f"{self.private_segment_size=} > {self.device.max_private_segment_size=}"
 
+    HWPM4Queue().invalidate_cache().submit(self.device)
+
   # NOTE: no programs are ever freed
   def __del__(self):
     if hasattr(self, 'lib_gpu'): self.device._gpu_free(self.lib_gpu)
 
   def __call__(self, *args, global_size:Tuple[int,int,int]=(1,1,1), local_size:Tuple[int,int,int]=(1,1,1), vals:Tuple[int, ...]=(), wait=False):
     if self.device.kernargs_ptr + self.kernargs_segment_size > (self.device.kernargs.va_addr + self.device.kernargs.size):
       self.device.kernargs_ptr = self.device.kernargs.va_addr
@@ -363,38 +316,39 @@
       if ctypes.sizeof(self.args_struct_t) != self.kernargs_segment_size:
         raise RuntimeError(f"HSAProgram.__call__: incorrect args struct size {ctypes.sizeof(self.args_struct_t)} != {self.kernargs_segment_size}")
     args_st = self.args_struct_t.from_address(self.device.kernargs_ptr)
     for i in range(len(args)): args_st.__setattr__(f'f{i}', args[i].va_addr)
     for i in range(len(vals)): args_st.__setattr__(f'v{i}', vals[i])
 
     q = HWPM4Queue()
-    if wait: q.timestamp(ctypes.addressof(self.device.completion_signal) + getattr(hsa.amd_signal_t, 'start_ts').offset)
+    q.wait(self.device.timeline_signal, self.device.timeline_value - 1)
+    if wait: q.timestamp(ctypes.addressof(self.device.timeline_signal) + getattr(hsa.amd_signal_t, 'start_ts').offset)
     q.exec(self, self.device.kernargs_ptr, global_size, local_size)
-    if wait:
-      q.timestamp(ctypes.addressof(self.device.completion_signal) + getattr(hsa.amd_signal_t, 'end_ts').offset)
-      q.signal(self.device.completion_signal)
-    q.submit(self.device)
+    if wait: q.timestamp(ctypes.addressof(self.device.timeline_signal) + getattr(hsa.amd_signal_t, 'end_ts').offset)
+    q.signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+    self.device.timeline_value += 1
     self.device.kernargs_ptr += self.kernargs_segment_size
 
     if wait:
-      self.device._wait_signal(self.device.completion_signal)
-      #assert (wp:=self.device.amd_aql_queue.write_dispatch_id) == (rp:=self.device.amd_aql_queue.read_dispatch_id), f"didn't run {wp} != {rp}"
-      return (self.device.completion_signal.end_ts-self.device.completion_signal.start_ts)/1e8
+      self.device._wait_signal(self.device.timeline_signal, self.device.timeline_value - 1)
+      return (self.device.timeline_signal.end_ts - self.device.timeline_signal.start_ts) / 1e8
 
 class AMDAllocator(LRUAllocator):
   def __init__(self, device:AMDDevice):
     self.device = device
     # NOTE: KFD_IOC_ALLOC_MEM_FLAGS_GTT doesn't work here for readinto
-    self.b = [self.device._gpu_alloc(SDMA_MAX_COPY_SIZE*4, kfd.KFD_IOC_ALLOC_MEM_FLAGS_USERPTR, public=True) for _ in range(2)]
+    self.b = [self.device._gpu_alloc(SDMA_MAX_COPY_SIZE, kfd.KFD_IOC_ALLOC_MEM_FLAGS_USERPTR, public=True) for _ in range(16)]
+    self.b_timeline = [0] * len(self.b)
+    self.b_next = 0
     super().__init__()
 
   def _alloc(self, size:int, options:BufferOptions):
     try:
       if options.host: return self.device._gpu_alloc(size, kfd.KFD_IOC_ALLOC_MEM_FLAGS_USERPTR, public=True)
-      else: return self.device._gpu_alloc(size, kfd.KFD_IOC_ALLOC_MEM_FLAGS_VRAM, public=True)
+      else: return self.device._gpu_alloc(size, kfd.KFD_IOC_ALLOC_MEM_FLAGS_VRAM, public=options.cpu_access)
     except OSError as e:
       if e.errno == errno.ENOMEM: raise MemoryError("Cannot allocate memory") from e
       else: raise
 
   def _free(self, gpumem, options:BufferOptions): self.device._gpu_free(gpumem)
   #def as_buffer(self, src:Any) -> memoryview:
   #  self.device.synchronize()
@@ -416,33 +370,42 @@
 
   #    copied_in += copy_size
   #    minor_offset = 0 # only on the first
   #  self.device._wait_signal(self.device.signal_sdma)
 
   def copyin(self, dest, src: memoryview):
     for i in range(0, src.nbytes, self.b[0].size):
-      ctypes.memmove(self.b[1].va_addr, from_mv(src[i:]), lsize:=min(self.b[0].size, src.nbytes-i))
-      if i != 0: self.device._wait_signal(self.device.signal_sdma)
-      self.b = self.b[::-1]
-      self.device._submit_sdma(dest.va_addr+i, self.b[0].va_addr, lsize, completion_signal=self.device.signal_sdma)
-    self.device._wait_signal(self.device.signal_sdma)
+      self.b_next = (self.b_next + 1) % len(self.b)
+      AMDDevice._wait_signal(self.device.timeline_signal, self.b_timeline[self.b_next])
+      ctypes.memmove(self.b[self.b_next].va_addr, from_mv(src[i:]), lsize:=min(self.b[self.b_next].size, src.nbytes-i))
+      HWCopyQueue().wait(self.device.timeline_signal, self.device.timeline_value - 1) \
+                   .copy(dest.va_addr+i, self.b[self.b_next].va_addr, lsize) \
+                   .signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+      self.b_timeline[self.b_next] = self.device.timeline_value
+      self.device.timeline_value += 1
 
   def copyout(self, dest:memoryview, src):
     self.device.synchronize()
     for i in range(0, dest.nbytes, self.b[0].size):
-      self.device._submit_sdma(self.b[0].va_addr, src.va_addr+i, lsize:=min(self.b[0].size, dest.nbytes-i), completion_signal=self.device.signal_sdma)
-      self.device._wait_signal(self.device.signal_sdma)
+      HWCopyQueue().wait(self.device.timeline_signal, self.device.timeline_value - 1) \
+                   .copy(self.b[0].va_addr, src.va_addr+i, lsize:=min(self.b[0].size, dest.nbytes-i)) \
+                   .signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+      AMDDevice._wait_signal(self.device.timeline_signal, self.device.timeline_value)
+      self.device.timeline_value += 1
+
       ctypes.memmove(from_mv(dest[i:]), self.b[0].va_addr, lsize)
 
   def transfer(self, dest, src, sz:int, src_dev:AMDDevice, dest_dev:AMDDevice):
-    dest_dev._gpu_map(src)
-    q = HWPM4Queue().signal(sig := AMDDevice._get_signal())
-    HWCopyQueue().wait(sig).copy(dest.va_addr, src.va_addr, sz).signal(sigc := AMDDevice._get_signal()).submit(dest_dev)
-    HWPM4Queue().wait(sigc).submit(dest_dev)
-    q.wait(sigc).submit(src_dev)
+    src_dev._gpu_map(dest)
+    HWCopyQueue().wait(src_dev.timeline_signal, src_dev.timeline_value - 1) \
+                 .wait(dest_dev.timeline_signal, dest_dev.timeline_value - 1) \
+                 .copy(dest.va_addr, src.va_addr, sz) \
+                 .signal(src_dev.timeline_signal, src_dev.timeline_value).submit(src_dev)
+    HWPM4Queue().wait(src_dev.timeline_signal, src_dev.timeline_value).submit(dest_dev)
+    src_dev.timeline_value += 1
 
 MAP_FIXED, MAP_NORESERVE = 0x10, 0x400
 class AMDDevice(Compiled):
   kfd:int = -1
   event_page:Any = None  # TODO: fix types in kfd, Optional[kfd.struct_kfd_ioctl_alloc_memory_of_gpu_args]
   signals_page:Any = None
   signal_number:int = 16
@@ -476,39 +439,41 @@
       c_gpus = (ctypes.c_int32 * len(gpus))(*gpus)
       stm = kio.unmap_memory_from_gpu(self.kfd, handle=mem.handle, device_ids_array_ptr=ctypes.addressof(c_gpus), n_devices=len(gpus))
       assert stm.n_success == len(gpus)
     libc.munmap(mem.va_addr, mem.size)
     kio.free_memory_of_gpu(self.kfd, handle=mem.handle)
 
   @classmethod
-  def _get_signal(self, num=None, sync_event=None) -> hsa.amd_signal_t:
+  def _set_signal(self, sig, value): sig.value = value
+
+  @classmethod
+  def _get_signal(self, num=None, sync_event=None, value=0) -> hsa.amd_signal_t:
     if num is None:
       num = AMDDevice.signal_number
       AMDDevice.signal_number += 1
       if AMDDevice.signal_number == SIGNAL_COUNT: AMDDevice.signal_number = 16
     #print("signal", num)
     ret = hsa.amd_signal_t.from_address(AMDDevice.signals_page.va_addr + SIGNAL_SIZE*num)
-    ret.value = 0
+    ret.value = value
     ret.kind = hsa.AMD_SIGNAL_KIND_USER
     if sync_event is not None:
       ret.event_mailbox_ptr = AMDDevice.event_page.va_addr + sync_event.event_slot_index*8
       ret.event_id = sync_event.event_id
     return ret
 
   @classmethod
-  def _wait_signal(self, signal:hsa.amd_signal_t, timeout=10000, skip_check=False):
+  def _wait_signal(self, signal:hsa.amd_signal_t, value=0, timeout=10000):
     assert signal.event_id != 0, "can't wait on this signal"
-    evt_arr = (kfd.struct_kfd_event_data * 1)()
-    evt_arr[0].event_id = signal.event_id
-    ret = kio.wait_events(AMDDevice.kfd, events_ptr=ctypes.addressof(evt_arr), num_events=1, wait_for_all=1, timeout=timeout)
-    if ret.wait_result != 0: raise RuntimeError(f"wait_result: {ret.wait_result}, {timeout} ms TIMEOUT!")
-
-    #val = signal.value
-    #while val != 0: val = signal.value
-    assert skip_check or signal.value == 0, f"not set to 0, but {signal.value}"
+    evt_arr = (kfd.struct_kfd_event_data)(event_id=signal.event_id)
+
+    start_time = time.time() * 1000
+    while (time.time() * 1000 - start_time) < timeout:
+      if signal.value >= value: return
+      kio.wait_events(AMDDevice.kfd, events_ptr=ctypes.addressof(evt_arr), num_events=1, wait_for_all=1, timeout=100)
+    raise RuntimeError(f"wait_signal: not set to {value}, but {signal.value}, {timeout} ms TIMEOUT!")
 
   def __init__(self, device:str=""):
     if AMDDevice.kfd == -1:
       AMDDevice.kfd = os.open("/dev/kfd", os.O_RDWR)
       AMDDevice.gpus = [g.parent for g in pathlib.Path("/sys/devices/virtual/kfd/kfd/topology/nodes").glob("*/gpu_id") if is_usable_gpu(g)]
     self.device_id = int(device.split(":")[1]) if ":" in device else 0
     with open(f"{AMDDevice.gpus[self.device_id]}/gpu_id", "r") as f: self.gpu_id = int(f.read())
@@ -523,16 +488,17 @@
       AMDDevice.event_page = self._gpu_alloc(0x8000, kfd.KFD_IOC_ALLOC_MEM_FLAGS_GTT, uncached=True)
       sync_event = kio.create_event(AMDDevice.kfd, event_page_offset=AMDDevice.event_page.handle, auto_reset=1)
     else:
       self._gpu_map(AMDDevice.signals_page)
       self._gpu_map(AMDDevice.event_page)
       sync_event = kio.create_event(AMDDevice.kfd, auto_reset=1)
 
-    self.completion_signal = AMDDevice._get_signal(self.device_id*2, sync_event=sync_event)
-    self.signal_sdma = AMDDevice._get_signal(self.device_id*2+1, sync_event=kio.create_event(AMDDevice.kfd, auto_reset=1))
+    self.timeline_value: int = 1
+    self.timeline_signal = AMDDevice._get_signal(self.device_id*2, sync_event=sync_event)
+    self._shadow_timeline_signal = AMDDevice._get_signal(self.device_id*2+1, sync_event=kio.create_event(AMDDevice.kfd, auto_reset=1))
 
     self.kernargs = self._gpu_alloc(0x1000000, kfd.KFD_IOC_ALLOC_MEM_FLAGS_VRAM)
     self.kernargs_ptr = self.kernargs.va_addr
 
     # scratch setup
     max_cu_id = self.properties['simd_count'] // self.properties['simd_per_cu'] - 1
     max_wave_id = self.properties['max_waves_per_simd'] * self.properties['simd_per_cu'] - 1
@@ -550,15 +516,15 @@
 
     # doorbell page
     self.doorbells_base = self.sdma_queue.doorbell_offset & (~0x1fff)  # doorbell is two pages
     self.doorbells = libc.mmap(0, 0x2000, mmap.PROT_READ|mmap.PROT_WRITE, mmap.MAP_SHARED, AMDDevice.kfd, self.doorbells_base)
 
     self.sdma_read_pointer = to_mv(self.sdma_queue.read_pointer_address, 8).cast("Q")
     self.sdma_write_pointer = to_mv(self.sdma_queue.write_pointer_address, 8).cast("Q")
-    self.sdma_doorbell = to_mv(self.doorbells + self.sdma_queue.doorbell_offset - self.doorbells_base, 4).cast("I")
+    self.sdma_doorbell = to_mv(self.doorbells + self.sdma_queue.doorbell_offset - self.doorbells_base, 8).cast("Q")
     self.sdma_doorbell_value = 0
 
     # PM4 Queue
     self.pm4_ctx_save_restore_address = self._gpu_alloc(0x2C02000, kfd.KFD_IOC_ALLOC_MEM_FLAGS_VRAM)
     self.eop_pm4_buffer = self._gpu_alloc(0x1000, kfd.KFD_IOC_ALLOC_MEM_FLAGS_VRAM)
     self.gart_pm4 = self._gpu_alloc(0x1000, kfd.KFD_IOC_ALLOC_MEM_FLAGS_GTT, uncached=True)
     self.pm4_ring = self._gpu_alloc(0x100000, kfd.KFD_IOC_ALLOC_MEM_FLAGS_GTT, uncached=True)
@@ -568,36 +534,23 @@
       # TODO: are these needed? (i know eop is)
       ctx_save_restore_address=self.pm4_ctx_save_restore_address.va_addr, ctx_save_restore_size=self.pm4_ctx_save_restore_address.size,
       ctl_stack_size = 0xa000,
       write_pointer_address=self.gart_pm4.va_addr, read_pointer_address=self.gart_pm4.va_addr+8)
 
     self.pm4_read_pointer = to_mv(self.pm4_queue.read_pointer_address, 8).cast("Q")
     self.pm4_write_pointer = to_mv(self.pm4_queue.write_pointer_address, 8).cast("Q")
-    self.pm4_doorbell = to_mv(self.doorbells + self.pm4_queue.doorbell_offset - self.doorbells_base, 4).cast("I")
-
-    super().__init__(device, AMDAllocator(self), AMDCompiler(self.arch), functools.partial(AMDProgram, self))
+    self.pm4_doorbell = to_mv(self.doorbells + self.pm4_queue.doorbell_offset - self.doorbells_base, 8).cast("Q")
 
-  def _submit_sdma(self, dest, src, copy_size, wait_signals=None, completion_signal=None):
-    q = HWCopyQueue()
-    if wait_signals is not None:
-      # NOTE: we check only low 32 bits to be zeroed, we don't use higher values for signals
-      for sig in wait_signals: q.wait(ctypes.addressof(sig) + getattr(hsa.amd_signal_t, 'value').offset)
-    if completion_signal is not None: q.timestamp(ctypes.addressof(completion_signal) + getattr(hsa.amd_signal_t, 'start_ts').offset)
-    q.copy(dest, src, copy_size)
-    if completion_signal is not None: q.timestamp(ctypes.addressof(completion_signal) + getattr(hsa.amd_signal_t, 'end_ts').offset)
-    if completion_signal is not None: q.signal(completion_signal)
-    q.submit(self)
-
-  def _submit_cache_inv(self, addr=0x0, sz=(1 << 64)-1, gli=0, glv=0, glk=0, gl1=0, gl2=0):
-    HWPM4Queue().invalidate_cache().signal(self.completion_signal).submit(self)
-    self._wait_signal(self.completion_signal)
-    assert (wp:=(self.pm4_write_pointer[0]%(self.pm4_ring.size//4))) == (rp:=self.pm4_read_pointer[0]), \
-      f"didn't run {wp} != {rp} len {self.pm4_ring.size//4}"
+    from tinygrad.runtime.graph.hcq import HCQGraph
+    super().__init__(device, AMDAllocator(self), HIPRenderer(), HSACompiler(self.arch),
+                     functools.partial(AMDProgram, self),
+                     functools.partial(HCQGraph, AMDDevice, HWPM4Queue, HWCopyQueue))
 
   def synchronize(self):
-    HWPM4Queue().signal(self.completion_signal).submit(self)
-    self._wait_signal(self.completion_signal)
-    assert (wp:=(self.pm4_write_pointer[0]%(self.pm4_ring.size//4))) == (rp:=self.pm4_read_pointer[0]), \
-      f"didn't run {wp} != {rp} len {self.pm4_ring.size//4}"
+    AMDDevice._wait_signal(self.timeline_signal, self.timeline_value - 1)
 
     # reset kernargs
     self.kernargs_ptr = self.kernargs.va_addr
+    if self.timeline_value > (1 << 31):
+      self.timeline_signal, self._shadow_timeline_signal = self._shadow_timeline_signal, self.timeline_signal
+      self.timeline_signal.value, self.timeline_value = 0, 1
+      cast(AMDAllocator, self.allocator).b_timeline = [0] * len(cast(AMDAllocator, self.allocator).b)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_clang.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_clang.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import ctypes, subprocess, pathlib, tempfile
-from tinygrad.device import Compiled, MallocAllocator, Compiler, CompilerOptions
-from tinygrad.helpers import cpu_time_execution
+from tinygrad.device import Compiled, Compiler, MallocAllocator
+from tinygrad.helpers import cpu_time_execution, DEBUG, cpu_objdump
 from tinygrad.renderer.cstyle import ClangRenderer
 
 class ClangCompiler(Compiler):
-  compiler_opts = CompilerOptions("CLANG", supports_float4=False, has_local=False)
-  def render(self, name:str, uops) -> str: return ClangRenderer(name, uops)
   def compile(self, src:str) -> bytes:
     # TODO: remove file write. sadly clang doesn't like the use of /dev/stdout here
     with tempfile.NamedTemporaryFile(delete=True) as output_file:
       subprocess.check_output(['clang', '-include', 'tgmath.h', '-shared', '-march=native', '-O2', '-Wall', '-Werror', '-x', 'c', '-fPIC', '-',
                                '-o', str(output_file.name)], input=src.encode('utf-8'))
       return pathlib.Path(output_file.name).read_bytes()
 
 class ClangProgram:
   def __init__(self, name:str, lib:bytes):
+    if DEBUG >= 6: cpu_objdump(lib)
     self.name, self.lib = name, lib
     # write to disk so we can load it
     with tempfile.NamedTemporaryFile(delete=True) as cached_file_path:
       pathlib.Path(cached_file_path.name).write_bytes(lib)
       self.fxn = ctypes.CDLL(str(cached_file_path.name))[name]
 
   def __call__(self, *bufs, vals=(), wait=False): return cpu_time_execution(lambda: self.fxn(*bufs, *vals), enable=wait)
 
 class ClangDevice(Compiled):
   def __init__(self, device:str):
     from tinygrad.runtime.graph.clang import ClangGraph
-    super().__init__(device, MallocAllocator, ClangCompiler("compile_clang"), ClangProgram, ClangGraph)
+    super().__init__(device, MallocAllocator, ClangRenderer(), ClangCompiler("compile_clang"), ClangProgram, ClangGraph)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_cuda.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_cuda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 import subprocess, hashlib, tempfile, ctypes, ctypes.util, functools, re
 from pathlib import Path
-from dataclasses import replace
 from typing import Tuple, Optional, List
 import tinygrad.runtime.autogen.cuda as cuda
 from tinygrad.helpers import DEBUG, getenv, from_mv, to_char_p_p, init_c_var, init_c_struct_t, colored, cpu_time_execution
-from tinygrad.device import Compiled, LRUAllocator, MallocAllocator, Compiler, CompilerOptions
-from tinygrad.buffer import BufferOptions
+from tinygrad.device import Compiled, Compiler, BufferOptions, LRUAllocator, MallocAllocator
 from tinygrad.renderer.cstyle import CUDARenderer
 from tinygrad.renderer.assembly import PTXRenderer
 if getenv("IOCTL"): import extra.nv_gpu_driver.nv_ioctl  # noqa: F401
 
 def pretty_ptx(s):
   # all expressions match `<valid_before><expr><valid_after>` and replace it with `<valid_before>color(<expr>)<valid_after>`
   s = re.sub(r'([!@<\[\s,\+\-;\n])((?:[_%$][\w%\$_]+(?:\.[xyz])?\:?)|(?:buf\d+))([<>\]\s,\+\-;\n\)])', lambda m:m[1]+colored(m[2], "blue")+m[3], s, flags=re.M) # identifiers  # noqa: E501
@@ -50,33 +48,29 @@
   return ret.value * 1e-3
 
 def _get_bytes(arg, get_str, get_sz, check) -> bytes:
   sz = init_c_var(ctypes.c_size_t(), lambda x: check(get_sz(arg, ctypes.byref(x))))
   return ctypes.string_at(init_c_var(ctypes.create_string_buffer(sz.value), lambda x: check(get_str(arg, x))), size=sz.value)
 
 class PTXCompiler(Compiler):
-  compiler_opts = CompilerOptions("CUDA", suffix="PTX", global_max=[65535, 65535, 2147483647], local_max=[64, 1024, 1024], shared_max=49152)
   def __init__(self, arch:str):
     self.arch = arch
     self.version = "7.8" if arch >= "sm_89" else "7.5"
-    PTXCompiler.compiler_opts = replace(PTXCompiler.compiler_opts, has_tensor_cores=int(arch[3:]) >= 80)
+    #PTXCompiler.compiler_opts = replace(PTXCompiler.compiler_opts, has_tensor_cores=int(arch[3:]) >= 80)
     super().__init__(f"compile_ptx_{self.arch}")
-  def render(self, name:str, uops) -> str: return PTXRenderer(name, uops).replace("TARGET", self.arch).replace("VERSION", self.version)
-  def compile(self, src:str) -> bytes: return src.encode()
+  def compile(self, src:str) -> bytes: return src.replace("TARGET", self.arch).replace("VERSION", self.version).encode()
 
 class CUDACompiler(Compiler):
-  compiler_opts = CompilerOptions("CUDA", global_max=[65535, 65535, 2147483647], local_max=[64, 1024, 1024], shared_max=49152)
   def __init__(self, arch:str):
     self.arch = arch
-    CUDACompiler.compiler_opts = replace(CUDACompiler.compiler_opts, has_tensor_cores=int(arch[3:]) >= 80)
+    #CUDACompiler.compiler_opts = replace(CUDACompiler.compiler_opts, has_tensor_cores=int(arch[3:]) >= 80)
     check(cuda.nvrtcVersion((nvrtcMajor := ctypes.c_int()), (nvrtcMinor := ctypes.c_int())))
     self.compile_options = [f'--gpu-architecture={arch}', "-I/usr/local/cuda/include", "-I/usr/include", "-I/opt/cuda/include/"]
     if (nvrtcMajor.value, nvrtcMinor.value) >= (12, 4): self.compile_options.append("--minimal")
     super().__init__(f"compile_cuda_{self.arch}")
-  def render(self, name:str, uops) -> str: return CUDARenderer(name, uops)
   def compile(self, src:str) -> bytes:
     check(cuda.nvrtcCreateProgram(ctypes.byref(prog := cuda.nvrtcProgram()), src.encode(), "<null>".encode(), 0, None, None))
     status = cuda.nvrtcCompileProgram(prog, len(self.compile_options), to_char_p_p([o.encode() for o in self.compile_options]))
 
     if status != 0: raise RuntimeError(f"compile failed: {_get_bytes(prog, cuda.nvrtcGetProgramLog, cuda.nvrtcGetProgramLogSize, check).decode()}")
     return _get_bytes(prog, cuda.nvrtcGetPTX, cuda.nvrtcGetPTXSize, check)
 
@@ -173,14 +167,15 @@
 
     self.arch = f"sm_{major.value}{minor.value}" if not CUDACPU else "sm_35"
     self.pending_copyin: List[Tuple[int, int, Optional[BufferOptions]]] = []
     CUDADevice.devices.append(self)
 
     from tinygrad.runtime.graph.cuda import CUDAGraph
     super().__init__(device, CUDAAllocator(self) if not CUDACPU else MallocAllocator,
+                     PTXRenderer(self.arch) if getenv("PTX") else CUDARenderer(self.arch),
                      PTXCompiler(self.arch) if getenv("PTX") else CUDACompiler(self.arch),
                      functools.partial(CUDAProgram, self), graph=CUDAGraph if not CUDACPU else None)
 
   def synchronize(self):
     if CUDACPU: return
     check(cuda.cuCtxSetCurrent(self.context))
     check(cuda.cuCtxSynchronize())
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_disk.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_disk.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       dest[:] = src._buf()
   def offset(self, buf:DiskBuffer, size:int, offset:int): return DiskBuffer(buf.device, size, offset)
 
 class DiskDevice(Compiled):
   def __init__(self, device:str):
     self.size: Optional[int] = None
     self.count = 0
-    super().__init__(device, DiskAllocator(self), None, None)
+    super().__init__(device, DiskAllocator(self), None, None, None)
   def _might_open(self, size):
     self.count += 1
     assert self.size is None or size <= self.size, f"can't reopen Disk tensor with larger size, opened with {self.size}, tried to open with {size}"
     if self.size is not None: return
     filename = self.dname[len("disk:"):]
     self.size = size
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_gpu.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from __future__ import annotations
 from typing import Tuple, Optional, List, cast
 import ctypes, functools, hashlib
 import tinygrad.runtime.autogen.opencl as cl
 from tinygrad.helpers import init_c_var, to_char_p_p, from_mv, OSX, DEBUG
 from tinygrad.renderer.cstyle import OpenCLRenderer
-from tinygrad.buffer import BufferOptions
-from tinygrad.device import Compiled, LRUAllocator, Compiler, CompilerOptions
+from tinygrad.device import BufferOptions, LRUAllocator, Compiled, Compiler
 
 # see test/external/external_osx_profiling.py to determine this ratio. it's in like GPU clocks or something
 OSX_TIMING_RATIO = (125/3) if OSX else 1.0
 
 def check(status):
   if status != 0: raise RuntimeError(f"OpenCL Error {status}")
 def checked(ret, status): return (check(status.value), ret)[1]
 
 class CLCompiler(Compiler):
-  compiler_opts = CompilerOptions("GPU")
   def __init__(self, device:CLDevice, compile_key:str):
     self.device = device
     super().__init__(f"compile_cl_{compile_key}")
-  def render(self, name:str, uops) -> str: return OpenCLRenderer(name, uops)
   def compile(self, src:str) -> bytes:
     program = checked(cl.clCreateProgramWithSource(self.device.context, 1, to_char_p_p([src.encode()]), None, status := ctypes.c_int32()), status)
     build_status: int = cl.clBuildProgram(program, 1, self.device.device_id, None, cl.clBuildProgram.argtypes[4](), None)
     if build_status != 0:
       cl.clGetProgramBuildInfo(program, self.device.device_id, cl.CL_PROGRAM_BUILD_LOG, 0, None, log_size := ctypes.c_size_t())
       cl.clGetProgramBuildInfo(program, self.device.device_id, cl.CL_PROGRAM_BUILD_LOG, log_size.value, mstr := ctypes.create_string_buffer(log_size.value), None)  # noqa: E501
       raise RuntimeError(f"OpenCL Compile Error\n\n{mstr.value.decode()}")
@@ -94,13 +91,13 @@
     self.device_name = (cl.clGetDeviceInfo(self.device_id, cl.CL_DEVICE_NAME, 256, buf := ctypes.create_string_buffer(256), None), buf.value.decode())[1]  # noqa: E501
     self.driver_version = (cl.clGetDeviceInfo(self.device_id, cl.CL_DRIVER_VERSION, 256, buf := ctypes.create_string_buffer(256), None), buf.value.decode())[1]  # noqa: E501
     self.context = checked(cl.clCreateContext(None, 1, self.device_id, cl.clCreateContext.argtypes[3](), None, status := ctypes.c_int32()), status)
     self.queue = checked(cl.clCreateCommandQueue(self.context, self.device_id, cl.CL_QUEUE_PROFILING_ENABLE, status), status)
     self.pending_copyin: List[memoryview] = []
 
     compile_key = hashlib.md5(self.device_name.encode() + self.driver_version.encode()).hexdigest()
-    super().__init__(device, CLAllocator(self), CLCompiler(self, f"compile_cl_{compile_key}"), functools.partial(CLProgram, self))
+    super().__init__(device, CLAllocator(self), OpenCLRenderer(), CLCompiler(self, f"compile_cl_{compile_key}"), functools.partial(CLProgram, self))
   def synchronize(self):
     check(cl.clFinish(self.queue))
     self.pending_copyin.clear()
 
 GPUDevice = CLDevice # for legacy reasons
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_hsa.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_hsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 import ctypes, functools, subprocess, io, atexit, collections, json
 from typing import Tuple, TypeVar, List, Dict, Any
 import tinygrad.runtime.autogen.hsa as hsa
 from tinygrad.helpers import DEBUG, init_c_var, from_mv, round_up, to_mv, init_c_struct_t, getenv
-from tinygrad.device import Compiled, LRUAllocator, Compiler, CompilerOptions
-from tinygrad.buffer import BufferOptions
+from tinygrad.device import Compiled, Compiler, BufferOptions, LRUAllocator
 from tinygrad.renderer.cstyle import HIPRenderer
 from tinygrad.runtime.driver.hsa import check, scan_agents, find_memory_pool, AQLQueue
 from tinygrad.runtime.driver.hip_comgr import compile_hip
 if getenv("IOCTL"): import extra.hip_gpu_driver.hip_ioctl  # noqa: F401
 
 PROFILE = getenv("PROFILE", 0)
 
@@ -39,19 +38,17 @@
       mjson.append({"name": name, "ph": "B", "pid": dev_id, "tid": queue_id, "ts": st*1e-3})
       mjson.append({"name": name, "ph": "E", "pid": dev_id, "tid": queue_id, "ts": et*1e-3})
     with open(path, "w") as f: f.write(json.dumps({"traceEvents": mjson}))
     print(f"Saved HSA profile to {path}")
 Profiler = HSAProfiler()
 
 class HSACompiler(Compiler):
-  compiler_opts = CompilerOptions("HSA", has_tensor_cores=True, shared_max=65536)
   def __init__(self, arch:str):
     self.arch = arch
     super().__init__(f"compile_hip_{self.arch}")
-  def render(self, name:str, uops) -> str: return HIPRenderer(name, uops)
   def compile(self, src:str) -> bytes: return compile_hip(src, self.arch)
 
 class HSAProgram:
   def __init__(self, device:HSADevice, name:str, lib:bytes):
     self.device, self.name, self.lib = device, name, lib
 
     if DEBUG >= 6:
@@ -217,15 +214,15 @@
     check(hsa.hsa_agent_get_info(self.agent, hsa.HSA_AMD_AGENT_INFO_HDP_FLUSH, ctypes.byref(hdp_flush := hsa.hsa_amd_hdp_flush_t())))
     self.hdp_flush = hdp_flush
 
     self.delayed_free: List[int] = []
     self.reusable_signals: List[hsa.hsa_signal_t] = []
 
     from tinygrad.runtime.graph.hsa import HSAGraph
-    super().__init__(device, HSAAllocator(self), HSACompiler(self.arch), functools.partial(HSAProgram, self), HSAGraph)
+    super().__init__(device, HSAAllocator(self), HIPRenderer(), HSACompiler(self.arch), functools.partial(HSAProgram, self), HSAGraph)
 
     # Finish init: preallocate some signals + space for kernargs
     self.signal_pool = [init_c_var(hsa.hsa_signal_t(), lambda x: check(hsa.hsa_signal_create(1, 0, None, ctypes.byref(x)))) for _ in range(4096)]
     self._new_kernargs_region(16 << 20) # initial region size is 16mb
 
   def synchronize(self):
     self.hw_queue.wait()
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_llvm.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_llvm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 import ctypes, functools
 from typing import Tuple
-from tinygrad.device import Compiled, MallocAllocator, Compiler, CompilerOptions
-from tinygrad.helpers import DEBUG, cpu_time_execution
-from tinygrad.renderer.llvmir import uops_to_llvm_ir
+from tinygrad.device import Compiled, Compiler, MallocAllocator
+from tinygrad.helpers import DEBUG, cpu_time_execution, cpu_objdump
+from tinygrad.renderer.llvmir import LLVMRenderer
 import llvmlite.binding as llvm
 
 class LLVMCompiler(Compiler):
-  compiler_opts = CompilerOptions("LLVM", supports_float4=False, has_local=False, has_shared=False)
   def __init__(self, device:LLVMDevice):
     self.device = device
     super().__init__("compile_llvm")
-  def render(self, name:str, uops) -> str: return uops_to_llvm_ir(name, uops)
   def compile(self, src:str) -> bytes:
     mod = llvm.parse_assembly(src)
     mod.verify()
     self.device.optimizer.run(mod)
     if DEBUG >= 5: print(self.device.target_machine.emit_assembly(mod))
     return self.device.target_machine.emit_object(mod)
 
 class LLVMProgram:
   def __init__(self, device:LLVMDevice, name:str, lib:bytes):
+    if DEBUG >= 6: cpu_objdump(lib)
     self.name, self.lib = name, lib
     device.engine.add_object_file(llvm.object_file.ObjectFileRef.from_data(lib))
     self.fxn = device.engine.get_function_address(name)
 
   def __call__(self, *bufs, vals:Tuple[int, ...]=(), wait=False):
     if not hasattr(self, 'cfunc'):
       self.cfunc = ctypes.CFUNCTYPE(ctypes.c_int, *([ctypes.c_void_p]*len(bufs)), *([ctypes.c_int32]*len(vals)))(self.fxn)
@@ -40,8 +39,8 @@
     # this opt actually can change things. ex: opt=3 means no FMA, opt=2 means FMA
     self.target_machine: llvm.targets.TargetMachine = llvm.Target.from_triple(llvm.get_process_triple()).create_target_machine(opt=2)
     self.target_machine.add_analysis_passes(self.optimizer)
     self.target_machine.set_asm_verbosity(True)
     backing_mod = llvm.parse_assembly(str())
     backing_mod.triple = llvm.get_process_triple()
     self.engine: llvm.executionengine.ExecutionEngine = llvm.create_mcjit_compiler(backing_mod, self.target_machine)
-    super().__init__(device, MallocAllocator, LLVMCompiler(self), functools.partial(LLVMProgram, self))
+    super().__init__(device, MallocAllocator, LLVMRenderer(), LLVMCompiler(self), functools.partial(LLVMProgram, self))
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_metal.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_metal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from __future__ import annotations
 import os, subprocess, pathlib, ctypes, tempfile, functools
 import Metal, libdispatch
 from typing import List, Set, Any, Tuple, Optional
 from tinygrad.helpers import prod, getenv, DEBUG, unwrap2
-from tinygrad.device import Compiled, LRUAllocator, Compiler, CompilerOptions
+from tinygrad.device import Compiled, Compiler, LRUAllocator
 from tinygrad.renderer.cstyle import MetalRenderer
 
 def wait_check(cbuf: Any):
   cbuf.waitUntilCompleted()
   if (error := cbuf.error()) is not None:
     raise RuntimeError(error)
 
 class MetalCompiler(Compiler):
-  compiler_opts = CompilerOptions("METAL", has_tensor_cores=os.uname().machine == "arm64", shared_max=32768)
   def __init__(self, device:Optional[MetalDevice]):
     self.device = device
     super().__init__("compile_metal")
-  def render(self, name:str, uops) -> str: return MetalRenderer(name, uops)
   def compile(self, src:str) -> bytes:
     if self.device is None:
       # NOTE: if you run llvm-dis on "air" you can see the llvm bytecode
       air = subprocess.check_output(['xcrun', '-sdk', 'macosx', 'metal', '-x', 'metal', '-c', '-', '-o', '-'], input=src.encode('utf-8'))
       return subprocess.check_output(['xcrun', '-sdk', 'macosx', 'metallib', '-', '-o', '-'], input=air)
     else:
       options = Metal.MTLCompileOptions.new()
@@ -31,15 +29,15 @@
 class MetalProgram:
   def __init__(self, device:MetalDevice, name:str, lib:bytes):
     self.device, self.name, self.lib = device, name, lib
     if DEBUG >= 6:
       with tempfile.NamedTemporaryFile(delete=True) as shader:
         shader.write(lib)
         shader.flush()
-        os.system(f"cd {pathlib.Path(__file__).parents[2]}/disassemblers/applegpu && python3 compiler_explorer.py {shader.name}")
+        os.system(f"cd {pathlib.Path(__file__).parents[2]}/extra/disassemblers/applegpu && python3 compiler_explorer.py {shader.name}")
     assert lib[:4] == b"MTLB", "Invalid Metal library. Could be due to using conda. Try system python or METAL_XCODE=1 DISABLE_COMPILER_CACHE=1."
     data = libdispatch.dispatch_data_create(lib, len(lib), None, None)
     self.library = unwrap2(self.device.device.newLibraryWithData_error_(data, None))
     self.fxn = self.library.newFunctionWithName_(name)
     self.pipeline_state = unwrap2(self.device.device.newComputePipelineStateWithFunction_error_(self.fxn, None))
 
   def __call__(self, *bufs, global_size:Tuple[int,int,int]=(1,1,1), local_size:Tuple[int,int,int]=(1,1,1), vals:Tuple[int, ...]=(), wait=False):
@@ -94,14 +92,14 @@
   def __init__(self, device:str):
     self.device = Metal.MTLCreateSystemDefaultDevice()
     self.mtl_queue = self.device.newCommandQueueWithMaxCommandBufferCount_(1024)
     self.mtl_buffers_in_flight: List[Any] = []
     self.mv_in_metal: List[memoryview] = []
     self.track_cross_buffer: List[Any] = []
     from tinygrad.runtime.graph.metal import MetalGraph
-    super().__init__(device, MetalAllocator(self), MetalCompiler(None if getenv("METAL_XCODE") else self),
+    super().__init__(device, MetalAllocator(self), MetalRenderer(), MetalCompiler(None if getenv("METAL_XCODE") else self),
                      functools.partial(MetalProgram, self), MetalGraph)
   def synchronize(self):
     for cbuf in self.mtl_buffers_in_flight: wait_check(cbuf)
     self.mv_in_metal.clear()
     self.mtl_buffers_in_flight.clear()
     self.track_cross_buffer.clear()
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_nv.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_nv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
-import os, ctypes, pathlib, re, fcntl, functools, mmap, struct, tempfile, hashlib, subprocess, time
-from typing import Tuple, List, Any
-from dataclasses import replace
-from tinygrad.device import Compiled, LRUAllocator, Compiler, BufferOptions, CompilerOptions
+import os, ctypes, pathlib, re, fcntl, functools, mmap, struct, tempfile, hashlib, subprocess, time, array
+from typing import Tuple, List, Any, cast
+from tinygrad.device import Compiled, Compiler, LRUAllocator, BufferOptions
 from tinygrad.helpers import getenv, from_mv, init_c_struct_t, to_mv, round_up, to_char_p_p, DEBUG, prod
 from tinygrad.renderer.cstyle import CUDARenderer
-from tinygrad.runtime.ops_cuda import check as cuda_check, _get_bytes
+from tinygrad.runtime.ops_cuda import check as cuda_check, _get_bytes, CUDACompiler
 import tinygrad.runtime.autogen.cuda as cuda
 import tinygrad.runtime.autogen.nv_gpu as nv_gpu
 if getenv("IOCTL"): import extra.nv_gpu_driver.nv_ioctl # noqa: F401
 
-libc = ctypes.CDLL("libc.so.6")
-libc.memset.argtypes = [ctypes.c_void_p, ctypes.c_char, ctypes.c_int]
+libc = ctypes.CDLL(ctypes.util.find_library("c"))
 libc.mmap.argtypes = [ctypes.c_void_p, ctypes.c_size_t, ctypes.c_int, ctypes.c_int, ctypes.c_int, ctypes.c_long]
 libc.mmap.restype = ctypes.c_void_p
 libc.munmap.argtypes = [ctypes.c_void_p, ctypes.c_size_t]
 libc.munmap.restype = ctypes.c_int
 
-QMD_SIZE = (8 << 8)
+if MOCKGPU:=getenv("MOCKGPU"):
+  import extra.mockgpu.mockgpu  # noqa: F401
+  libc.mmap = extra.mockgpu.mockgpu._mmap # type: ignore
+  libc.munmap = extra.mockgpu.mockgpu._munmap # type: ignore
 
 def nv_iowr(fd, nr, args):
   ret = fcntl.ioctl(fd, (3 << 30) | (ctypes.sizeof(args) & 0x1FFF) << 16 | (ord('F') & 0xFF) << 8 | (nr & 0xFF), args)
   if ret != 0: raise RuntimeError(f"ioctl returned {ret}")
 
 def rm_alloc(fd, clss, root, parant, params):
   made = nv_gpu.NVOS21_PARAMETERS(hRoot=root, hObjectParent=parant, hClass=clss,
@@ -63,23 +64,21 @@
 assert ctypes.sizeof(qmd_struct_t) == 0x40 * 4
 
 def nvmethod(subc, mthd, size, typ=2): return (typ << 28) | (size << 16) | (subc << 13) | (mthd >> 2)
 def nvdata64(data): return (data >> 32, data & 0xFFFFFFFF)
 def nvdata64_le(data): return (data & 0xFFFFFFFF, data >> 32)
 
 class NVCompiler(Compiler):
-  compiler_opts = CompilerOptions("NV", global_max=[65535, 65535, 2147483647], local_max=[64, 1024, 1024], shared_max=49152)
   def __init__(self, arch:str):
     self.arch = arch
-    NVCompiler.compiler_opts = replace(NVCompiler.compiler_opts, has_tensor_cores=int(arch[3:]) >= 80)
+    #NVCompiler.compiler_opts = replace(NVCompiler.compiler_opts, has_tensor_cores=int(arch[3:]) >= 80)
     cuda_check(cuda.nvrtcVersion((nvrtcMajor := ctypes.c_int()), (nvrtcMinor := ctypes.c_int())))
     self.compile_options = [f'--gpu-architecture={arch}', "-I/usr/local/cuda/include", "-I/usr/include", "-I/opt/cuda/include/"]
     if (nvrtcMajor.value, nvrtcMinor.value) >= (12, 4): self.compile_options.append("--minimal")
     super().__init__(f"compile_nv_{self.arch}")
-  def render(self, name:str, uops) -> str: return CUDARenderer(name, uops)
   def compile(self, src:str) -> bytes:
     cuda_check(cuda.nvrtcCreateProgram(ctypes.byref(prog := cuda.nvrtcProgram()), src.encode(), "<null>".encode(), 0, None, None))
     status = cuda.nvrtcCompileProgram(prog, len(self.compile_options), to_char_p_p([o.encode() for o in self.compile_options]))
 
     if status != 0:
       raise RuntimeError(f"compile failed: {_get_bytes(prog, cuda.nvrtcGetProgramLog, cuda.nvrtcGetProgramLogSize, cuda_check).decode()}")
     return _get_bytes(prog, cuda.nvrtcGetCUBIN, cuda.nvrtcGetCUBINSize, cuda_check)
@@ -89,41 +88,39 @@
   def copy_from_cpu(self, gpuaddr, data):
     self.q += [nvmethod(1, nv_gpu.NVC6C0_OFFSET_OUT_UPPER, 2), *nvdata64(gpuaddr)]
     self.q += [nvmethod(1, nv_gpu.NVC6C0_LINE_LENGTH_IN, 2), len(data)*4, 0x1]
     self.q += [nvmethod(1, nv_gpu.NVC6C0_LAUNCH_DMA, 1), 0x41]
     self.q += [nvmethod(1, nv_gpu.NVC6C0_LOAD_INLINE_DATA, len(data), typ=6)] + [x for x in data]
     return self
 
-  def exec(self, prg, kernargs, global_size:Tuple[int,int,int]=(1,1,1), local_size:Tuple[int,int,int]=(1,1,1), completion_signal=None):
+  def exec(self, prg, kernargs, global_size:Tuple[int,int,int]=(1,1,1), local_size:Tuple[int,int,int]=(1,1,1)):
     prg.qmd.cta_raster_width, prg.qmd.cta_raster_height, prg.qmd.cta_raster_depth = global_size
     prg.qmd.cta_thread_dimension0, prg.qmd.cta_thread_dimension1, prg.qmd.cta_thread_dimension2 = local_size
-    prg.qmd.constant_buffer_addr_lower_0 = (kernargs + QMD_SIZE) & 0xffffffff
-    prg.qmd.constant_buffer_addr_upper_0 = (kernargs + QMD_SIZE) >> 32
+    prg.qmd.constant_buffer_addr_lower_0 = kernargs & 0xffffffff
+    prg.qmd.constant_buffer_addr_upper_0 = kernargs >> 32
     self.q += [nvmethod(1, nv_gpu.NVC6C0_INVALIDATE_SHADER_CACHES_NO_WFI, 1), (1 << 12) | (1 << 4) | (1 << 0)]
-    self.q += [nvmethod(1, nv_gpu.NVC6C0_SET_INLINE_QMD_ADDRESS_A, 0x42), *nvdata64(kernargs >> 8)]
+    self.q += [nvmethod(1, nv_gpu.NVC6C0_SET_INLINE_QMD_ADDRESS_A, 0x42), *nvdata64((kernargs + round_up(prg.constbuf_0_size, 1 << 8)) >> 8)]
     self.q += [x for x in to_mv(ctypes.addressof(prg.qmd), ctypes.sizeof(prg.qmd)).cast("I")]
-
-    if completion_signal is not None: self.signal(completion_signal)
     return self
 
   def wait(self, signal, value=0):
     self.q += [nvmethod(0, nv_gpu.NVC56F_SEM_ADDR_LO, 5), *nvdata64_le(ctypes.addressof(from_mv(signal))), *nvdata64_le(value),
                (3 << 0) | (1 << 12) | (1 << 24)] # ACQUIRE | ACQUIRE_SWITCH_TSG | PAYLOAD_SIZE_64BIT
     return self
 
   def signal(self, signal, value=0, timestamp=False):
     self.q += [nvmethod(0, nv_gpu.NVC56F_SEM_ADDR_LO, 5), *nvdata64_le(ctypes.addressof(from_mv(signal))), *nvdata64_le(value),
                (1 << 0) | (1 << 20) | (1 << 24) | ((1 << 25) if timestamp else 0)] # RELEASE | RELEASE_WFI | PAYLOAD_SIZE_64BIT | RELEASE_TIMESTAMP
     self.q += [nvmethod(0, nv_gpu.NVC56F_NON_STALL_INTERRUPT, 1), 0x0]
     return self
 
   def submit(self, dev:NVDevice):
+    if len(self.q) == 0: return
     assert len(self.q) < (1 << 21)
-    self.signal(dev.compute_progress_signal, dev.compute_put_value + 1)
-    for i,packet in enumerate(self.q): dev.cmdq[dev.cmdq_wptr//4 + i] = packet
+    dev.cmdq[dev.cmdq_wptr//4:dev.cmdq_wptr//4+len(self.q)] = array.array('I', self.q)
     fifo_entry = dev.compute_put_value % dev.compute_gpfifo_entries
     dev.compute_gpu_ring[fifo_entry] = ((dev.cmdq_page.base+dev.cmdq_wptr)//4 << 2) | (len(self.q) << 42) | (1 << 41)
     dev.compute_gpu_ring_controls.GPPut = (dev.compute_put_value + 1) % dev.compute_gpfifo_entries
     dev.compute_put_value += 1
     dev.gpu_mmio[0x90 // 4] = dev.compute_gpfifo_token
     dev.cmdq_wptr += len(self.q) * 4
 
@@ -133,27 +130,27 @@
   def copy(self, dest, src, copy_size):
     self.q += [nvmethod(4, nv_gpu.NVC6B5_OFFSET_IN_UPPER, 4), *nvdata64(src), *nvdata64(dest)]
     self.q += [nvmethod(4, nv_gpu.NVC6B5_LINE_LENGTH_IN, 1), copy_size]
     self.q += [nvmethod(4, nv_gpu.NVC6B5_LAUNCH_DMA, 1), 0x182] # TRANSFER_TYPE_NON_PIPELINED | DST_MEMORY_LAYOUT_PITCH | SRC_MEMORY_LAYOUT_PITCH
     return self
 
   def wait(self, signal, value=0):
-    self.q += [nvmethod(0, nv_gpu.NVC56F_SEM_ADDR_LO, 5), *nvdata64_le(ctypes.addressof(from_mv(signal))), value, 0x0,
+    self.q += [nvmethod(0, nv_gpu.NVC56F_SEM_ADDR_LO, 5), *nvdata64_le(ctypes.addressof(from_mv(signal))), *nvdata64_le(value),
                (3 << 0) | (1 << 12) | (1 << 24)] # ACQUIRE | ACQUIRE_SWITCH_TSG | PAYLOAD_SIZE_64BIT
     return self
 
   def signal(self, signal, value=0, timestamp=False):
     self.q += [nvmethod(0, nv_gpu.NVC56F_SEM_ADDR_LO, 5), *nvdata64_le(ctypes.addressof(from_mv(signal))), *nvdata64_le(value),
                (1 << 0) | (1 << 20) | (1 << 24) | ((1 << 25) if timestamp else 0)] # RELEASE | RELEASE_WFI | PAYLOAD_SIZE_64BIT | RELEASE_TIMESTAMP
     self.q += [nvmethod(0, nv_gpu.NVC56F_NON_STALL_INTERRUPT, 1), 0x0]
     return self
 
   def submit(self, dev:NVDevice):
-    self.signal(dev.dma_progress_signal, dev.dma_put_value + 1)
-    for i,packet in enumerate(self.q): dev.cmdq[dev.cmdq_wptr//4 + i] = packet
+    if len(self.q) == 0: return
+    dev.cmdq[dev.cmdq_wptr//4:dev.cmdq_wptr//4+len(self.q)] = array.array('I', self.q)
     fifo_entry = dev.dma_put_value % dev.dma_gpfifo_entries
     dev.dma_gpu_ring[fifo_entry] = ((dev.cmdq_page.base+dev.cmdq_wptr)//4 << 2) | (len(self.q) << 42)
     dev.dma_gpu_ring_controls.GPPut = (dev.dma_put_value + 1) % dev.dma_gpfifo_entries
     dev.dma_put_value += 1
     dev.gpu_mmio[0x90 // 4] = dev.dma_gpfifo_token
     dev.cmdq_wptr += len(self.q) * 4
 
@@ -164,133 +161,169 @@
     if DEBUG >= 6:
       try:
         fn = (pathlib.Path(tempfile.gettempdir()) / f"tinycuda_{hashlib.md5(lib).hexdigest()}").as_posix()
         with open(fn + ".cubin", "wb") as f: f.write(lib)
         print(subprocess.check_output(["nvdisasm", fn+".cubin"]).decode('utf-8'))
       except Exception as e: print("failed to disasm cubin", str(e))
 
-    _phoff, _shoff, _flags, _ehsize, _phentsize, _phnum, _shentsize, _shnum, _shstrndx = struct.unpack_from("<QQIHHHHHH", self.lib, 0x20)
-    sections = [struct.unpack_from("<IIQQQQIIQ", self.lib, _shoff + i * _shentsize) for i in range(_shnum)]
-    shstrtab = memoryview(bytearray(self.lib[sections[_shstrndx][4]:sections[_shstrndx][4]+sections[_shstrndx][5]]))
-
-    self.shmem_usage = 0
+    self.global_init, self.shmem_usage = None, 0
     constant_buffers_data = {}
-    for sh_name, sh_type, sh_flags, _, sh_offset, sh_size, _, sh_info, _ in sections:
-      section_name = shstrtab[sh_name:].tobytes().split(b'\0', 1)[0].decode('utf-8')
-      if sh_type == SHT_NOBITS and sh_flags & SHF_ALLOC: self.shmem_usage = sh_size
-      elif sh_type == SHT_PROGBITS and sh_flags & SHF_ALLOC and sh_flags & SHF_EXECINSTR:
-        self.program = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
-        self.registers_usage = sh_info >> 24
-      if match := re.match(r'\.nv\.constant(\d+)', section_name):
-        constant_buffers_data[int(match.group(1))] = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
-      if section_name == ".nv.info":
-        section_data = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
-        for i in range(sh_size // 12):
-          if section_data[i * 3 + 0] & 0xffff == 0x1204 and section_data[i * 3 + 2] + 0x240 > self.device.slm_per_thread:
-            raise RuntimeError("too high local memory")
+
+    if MOCKGPU:
+      self.program, self.registers_usage = memoryview(bytearray(lib) + b'\x00' * (4 - len(lib)%4)).cast("I"), 0x10
+      constant_buffers_data[0] = memoryview(bytearray(0x190))
+    else:
+      _phoff, _shoff, _flags, _ehsize, _phentsize, _phnum, _shentsize, _shnum, _shstrndx = struct.unpack_from("<QQIHHHHHH", self.lib, 0x20)
+      sections = [struct.unpack_from("<IIQQQQIIQ", self.lib, _shoff + i * _shentsize) for i in range(_shnum)]
+      shstrtab = memoryview(bytearray(self.lib[sections[_shstrndx][4]:sections[_shstrndx][4]+sections[_shstrndx][5]]))
+      for sh_name, sh_type, sh_flags, _, sh_offset, sh_size, _, sh_info, _ in sections:
+        section_name = shstrtab[sh_name:].tobytes().split(b'\0', 1)[0].decode('utf-8')
+        if sh_type == SHT_NOBITS and sh_flags & SHF_ALLOC: self.shmem_usage = sh_size
+        elif sh_type == SHT_PROGBITS and sh_flags & SHF_ALLOC and sh_flags & SHF_EXECINSTR:
+          self.program = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
+          self.registers_usage = sh_info >> 24
+        if match := re.match(r'\.nv\.constant(\d+)', section_name):
+          constant_buffers_data[int(match.group(1))] = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
+        if section_name == ".nv.global.init": self.global_init = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
+        elif section_name == ".nv.info":
+          section_data = memoryview(bytearray(self.lib[sh_offset:sh_offset+sh_size])).cast("I")
+          for i in range(sh_size // 12):
+            if section_data[i * 3 + 0] & 0xffff == 0x1204 and section_data[i * 3 + 2] + 0x240 > self.device.slm_per_thread:
+              raise RuntimeError("too high local memory")
+
+    # Registers allocation granularity per warp is 256, warp allocaiton granularity is 4. Register file size is 65536.
+    self.max_threads = ((65536 // round_up(self.registers_usage * 32, 256)) // 4) * 4 * 32
 
     # Load program and constant buffers (if any)
-    self.lib_sz = round_up(round_up(self.program.nbytes, 128) + sum([round_up(x.nbytes, 128) for i,x in constant_buffers_data.items()]), 0x1000)
+    self.lib_sz = round_up(round_up(self.program.nbytes, 128) + round_up(0 if self.global_init is None else self.global_init.nbytes, 128) +
+                           sum([round_up(x.nbytes, 128) for i,x in constant_buffers_data.items()]), 0x1000)
     self.lib_gpu = self.device.allocator.alloc(self.lib_sz)
-    for st in range(0, len(self.program), 4096):
-      HWComputeQueue().copy_from_cpu(self.lib_gpu.base+st*4, self.program[st:st+4096]).submit(self.device)
+    for st in range(0, len(self.program), 4095):
+      HWComputeQueue().copy_from_cpu(self.lib_gpu.base+st*4, self.program[st:st+4095]).submit(self.device)
 
     self.constbuffer_0 = [0] * 88
     self.constbuffer_0[6:12] = [*nvdata64_le(self.device.shared_mem_window), *nvdata64_le(self.device.local_mem_window), *nvdata64_le(0xfffdc0)]
 
-    smem_config = min(shmem_conf * 1024 for shmem_conf in [8, 16, 32, 64, 96] if shmem_conf * 1024 >= self.shmem_usage) // 4096 + 1
+    smem_config = min(shmem_conf * 1024 for shmem_conf in [32, 64, 100] if shmem_conf * 1024 >= self.shmem_usage) // 4096 + 1
     self.qmd = qmd_struct_t(qmd_group_id=0x3f, sm_global_caching_enable=1, invalidate_texture_header_cache=1, invalidate_texture_sampler_cache=1,
                             invalidate_texture_data_cache=1, invalidate_shader_data_cache=1, api_visible_call_limit=1, sampler_index=1,
                             cwd_membar_type=nv_gpu.NVC6C0_QMDV03_00_CWD_MEMBAR_TYPE_L1_SYSMEMBAR, qmd_major_version=3,
                             shared_memory_size=max(0x400, round_up(self.shmem_usage, 0x100)), min_sm_config_shared_mem_size=smem_config,
                             max_sm_config_shared_mem_size=0x1a, register_count_v=self.registers_usage, target_sm_config_shared_mem_size=smem_config,
                             barrier_count=1, shader_local_memory_high_size=self.device.slm_per_thread, program_prefetch_size=0x10, sass_version=0x89,
                             program_address_lower=self.lib_gpu.base&0xffffffff, program_address_upper=self.lib_gpu.base>>32,
                             program_prefetch_addr_lower_shifted=self.lib_gpu.base>>8, program_prefetch_addr_upper_shifted=self.lib_gpu.base>>40,
                             constant_buffer_size_shifted4_0=0x190, constant_buffer_valid_0=1, constant_buffer_invalidate_0=1)
 
+    # NV's kernargs is constbuffer (size 0x160), then arguments to the kernel follows. Kernargs also appends QMD at the end of the kernel.
+    self.constbuf_0_size = constant_buffers_data[0].nbytes if 0 in constant_buffers_data else 0
+    self.kernargs_segment_size = round_up(self.constbuf_0_size, 1 << 8) + (8 << 8)
+    self.kernargs_offset = 0x160
+
     # constant buffer 0 is filled for each program, no need to copy it from elf (it's just zeroes)
     if 0 in constant_buffers_data: constant_buffers_data.pop(0)
 
     off = round_up(self.program.nbytes, 128)
+    if self.global_init is not None:
+      # Constbuffer 4 contains a pointer to nv.global.init, load section and set up the pointer.
+      assert 4 in constant_buffers_data and constant_buffers_data[4].nbytes == 8
+      HWComputeQueue().copy_from_cpu(load_addr:=(self.lib_gpu.base + off), self.global_init).submit(self.device)
+      constant_buffers_data[4][0:2] = memoryview(struct.pack('Q', load_addr)).cast('I')
+      off += round_up(self.global_init.nbytes, 128)
+
     for i,data in constant_buffers_data.items():
       self.qmd.__setattr__(f'constant_buffer_addr_upper_{i}', (self.lib_gpu.base + off) >> 32)
       self.qmd.__setattr__(f'constant_buffer_addr_lower_{i}', (self.lib_gpu.base + off) & 0xffffffff)
       self.qmd.__setattr__(f'constant_buffer_size_shifted4_{i}', data.nbytes)
       self.qmd.__setattr__(f'constant_buffer_valid_{i}', 1)
 
       HWComputeQueue().copy_from_cpu(self.lib_gpu.base + off, data).submit(self.device)
       off += round_up(data.nbytes, 128)
+
+    HWComputeQueue().signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+    self.device.timeline_value += 1
     self.device.synchronize()
 
   def __del__(self):
     if hasattr(self, 'lib_gpu'): self.device.allocator.free(self.lib_gpu, self.lib_sz)
 
   def __call__(self, *args, global_size:Tuple[int,int,int]=(1,1,1), local_size:Tuple[int,int,int]=(1,1,1), vals:Tuple[int, ...]=(), wait=False):
-    if prod(local_size) > 1024 or self.registers_usage * prod(local_size) > 65536: raise RuntimeError("Too many resources requsted for launch")
+    if prod(local_size) > 1024 or self.max_threads < prod(local_size): raise RuntimeError("Too many resources requsted for launch")
+    if not hasattr(self, "args_struct_t"):
+      self.args_struct_t = init_c_struct_t(tuple([(f'f{i}', ctypes.c_void_p) for i in range(len(args))] +
+                                                 [(f'v{i}', ctypes.c_int) for i in range(len(vals))]))
 
-    kernargs_size = round_up(QMD_SIZE + 0x160 + len(args) * 8 + len(vals) * 4, 1 << 8)
-    if self.device.kernargs_ptr >= (self.device.kernargs_page.base + self.device.kernargs_page.length - kernargs_size):
+    if self.device.kernargs_ptr >= (self.device.kernargs_page.base + self.device.kernargs_page.length - self.kernargs_segment_size):
       self.device.kernargs_ptr = self.device.kernargs_page.base
 
+    # HACK: Save counts of args and vars to "unused" constbuffer for later extraction in mockgpu to pass into gpuocelot.
+    if MOCKGPU: self.constbuffer_0[0:2] = [len(args), len(vals)]
     kernargs = [arg_half for arg in args for arg_half in nvdata64_le(arg.base)] + [val for val in vals]
-    kernargs_ptr = self.device.kernargs_ptr
-    self.device.kernargs_ptr += kernargs_size
 
-    if wait: st, en = self.device._get_signal(), self.device._get_signal()
     queue = HWComputeQueue()
-    queue.wait(self.device.dma_progress_signal, self.device.dma_put_value)
-    queue.wait(self.device.compute_progress_signal, self.device.compute_put_value)
-    if wait: queue.signal(st, timestamp=True)
-    queue.copy_from_cpu(kernargs_ptr + QMD_SIZE, self.constbuffer_0 + kernargs)
-    queue.exec(self, kernargs_ptr, global_size, local_size)
-    if wait: queue.signal(en, timestamp=True)
-    queue.submit(self.device)
+    queue.wait(self.device.timeline_signal, self.device.timeline_value - 1)
+    if wait: queue.signal(self.device.time_event_st, timestamp=True)
+    queue.copy_from_cpu(self.device.kernargs_ptr, self.constbuffer_0 + kernargs)
+    queue.exec(self, self.device.kernargs_ptr, global_size, local_size)
+    if wait: queue.signal(self.device.time_event_en, timestamp=True)
+    queue.signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+    self.device.timeline_value += 1
+    self.device.kernargs_ptr += self.kernargs_segment_size
+
     if wait:
-      self.device._wait_signal(self.device.compute_progress_signal, self.device.compute_put_value)
-      return (en[1]-st[1]) / 1e9
+      self.device._wait_signal(self.device.timeline_signal, self.device.timeline_value - 1)
+      return (self.device.time_event_en[1] - self.device.time_event_st[1]) / 1e9
 
 class NVAllocator(LRUAllocator):
   def __init__(self, device:NVDevice):
     self.device = device
+    self.b = [self.device._gpu_host_alloc(2 << 20) for _ in range(16)]
+    self.b_timeline = [0] * len(self.b)
+    self.b_next = 0
     super().__init__()
 
   def _alloc(self, size:int, options:BufferOptions):
     if options.host: return self.device._gpu_host_alloc(size)
-    else: return self.device._gpu_alloc(size, map_to_all_gpus=True)
+    else: return self.device._gpu_alloc(size, map_to_cpu=options.cpu_access)
 
   def _free(self, gpumem, options:BufferOptions):
     NVDevice.synchronize_system()
     if options.host: self.device._gpu_host_free(gpumem)
     else: self.device._gpu_free(gpumem)
 
   def copyin(self, dest, src: memoryview):
-    host_mem = self.alloc(src.nbytes, BufferOptions(host=True))
-    self.device.pending_copyin.append((host_mem, src.nbytes, BufferOptions(host=True)))
-    ctypes.memmove(host_mem.base, from_mv(src), src.nbytes)
-    HWCopyQueue().copy(dest.base, host_mem.base, src.nbytes).submit(self.device)
-    self.device.synchronize()
+    for i in range(0, src.nbytes, self.b[0].length):
+      self.b_next = (self.b_next + 1) % len(self.b)
+      NVDevice._wait_signal(self.device.timeline_signal, self.b_timeline[self.b_next])
+      ctypes.memmove(self.b[self.b_next].va_addr, from_mv(src[i:]), lsize:=min(self.b[self.b_next].length, src.nbytes-i))
+      HWCopyQueue().wait(self.device.timeline_signal, self.device.timeline_value - 1) \
+                   .copy(dest.va_addr+i, self.b[self.b_next].va_addr, lsize) \
+                   .signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+      self.b_timeline[self.b_next] = self.device.timeline_value
+      self.device.timeline_value += 1
 
   def copyout(self, dest:memoryview, src):
     NVDevice.synchronize_system()
-    host_mem = self.alloc(dest.nbytes, BufferOptions(host=True))
-    self.device.pending_copyin.append((host_mem, dest.nbytes, BufferOptions(host=True)))
-    HWCopyQueue().copy(host_mem.base, src.base, dest.nbytes).submit(self.device)
-    self.device.synchronize()
-    ctypes.memmove(from_mv(dest), host_mem.base, dest.nbytes)
+    for i in range(0, dest.nbytes, self.b[0].length):
+      HWCopyQueue().wait(self.device.timeline_signal, self.device.timeline_value - 1) \
+                   .copy(self.b[0].va_addr, src.va_addr+i, lsize:=min(self.b[0].length, dest.nbytes-i)) \
+                   .signal(self.device.timeline_signal, self.device.timeline_value).submit(self.device)
+      NVDevice._wait_signal(self.device.timeline_signal, self.device.timeline_value)
+      self.device.timeline_value += 1
+
+      ctypes.memmove(from_mv(dest[i:]), self.b[0].va_addr, lsize)
 
   def transfer(self, dest, src, sz:int, src_dev=None, dest_dev=None):
-    queue = HWCopyQueue()
-    queue.wait(src_dev.dma_progress_signal, src_dev.dma_put_value)
-    queue.wait(src_dev.compute_progress_signal, src_dev.compute_put_value)
-    queue.wait(dest_dev.dma_progress_signal, dest_dev.dma_put_value)
-    queue.wait(dest_dev.compute_progress_signal, dest_dev.compute_put_value)
-    queue.copy(dest.base, src.base, sz).submit(src_dev)
-    HWCopyQueue().wait(src_dev.dma_progress_signal, src_dev.dma_put_value).submit(dest_dev)
-    dest_dev.synchronize()
+    src_dev._gpu_map(dest)
+    HWCopyQueue().wait(src_dev.timeline_signal, src_dev.timeline_value - 1) \
+                 .wait(dest_dev.timeline_signal, dest_dev.timeline_value - 1) \
+                 .copy(dest.va_addr, src.va_addr, sz) \
+                 .signal(src_dev.timeline_signal, src_dev.timeline_value).submit(src_dev)
+    HWComputeQueue().wait(src_dev.timeline_signal, src_dev.timeline_value).submit(dest_dev)
+    src_dev.timeline_value += 1
 
 MAP_FIXED, MAP_NORESERVE = 0x10, 0x400
 class NVDevice(Compiled):
   root = None
   fd_ctl: int = -1
   fd_uvm: int = -1
   gpus_info = None
@@ -309,33 +342,28 @@
     fd_dev = self._new_gpu_fd() if not system else os.open("/dev/nvidiactl", os.O_RDWR | os.O_CLOEXEC)
     made = nv_gpu.nv_ioctl_nvos33_parameters_with_fd(fd=fd_dev,
       params=nv_gpu.NVOS33_PARAMETERS(hClient=self.root, hDevice=self.device, hMemory=memory_handle, length=size, flags=flags))
     nv_iowr(self.fd_ctl, nv_gpu.NV_ESC_RM_MAP_MEMORY, made)
     if made.params.status != 0: raise RuntimeError(f"_gpu_map_to_cpu returned {made.params.status}")
     return libc.mmap(target, size, mmap.PROT_READ|mmap.PROT_WRITE, mmap.MAP_SHARED | (MAP_FIXED if target is not None else 0), fd_dev, 0)
 
-  def _gpu_alloc(self, size:int, contig=False, huge_page=False, va_addr=None, map_to_cpu=False, map_to_all_gpus=False, map_flags=0):
+  def _gpu_alloc(self, size:int, contig=False, huge_page=False, va_addr=None, map_to_cpu=False, map_flags=0):
     size = round_up(size, align:=((4 << 10) if huge_page else (2 << 20))) # TODO: need hugepage option, any speedup?
     alloc_params = nv_gpu.NV_MEMORY_ALLOCATION_PARAMS(owner=self.root, alignment=align, offset=0, limit=size-1, format=6, size=size,
       attr=(((nv_gpu.NVOS32_ATTR_PAGE_SIZE_HUGE << 23) if huge_page else 0) |
             ((nv_gpu.NVOS32_ATTR_PHYSICALITY_CONTIGUOUS if contig else nv_gpu.NVOS32_ATTR_PHYSICALITY_ALLOW_NONCONTIGUOUS) << 27)),
       attr2=((nv_gpu.NVOS32_ATTR2_ZBC_PREFER_NO_ZBC << 0) | (nv_gpu.NVOS32_ATTR2_GPU_CACHEABLE_YES << 2) |
              ((nv_gpu.NVOS32_ATTR2_PAGE_SIZE_HUGE_2MB << 20) if huge_page else 0)),
       flags=(nv_gpu.NVOS32_ALLOC_FLAGS_ALIGNMENT_FORCE | nv_gpu.NVOS32_ALLOC_FLAGS_PERSISTENT_VIDMEM | nv_gpu.NVOS32_ALLOC_FLAGS_MAP_NOT_REQUIRED |
              nv_gpu.NVOS32_ALLOC_FLAGS_IGNORE_BANK_PLACEMENT | nv_gpu.NVOS32_ALLOC_FLAGS_MEMORY_HANDLE_PROVIDED))
     mem_handle = rm_alloc(self.fd_ctl, nv_gpu.NV1_MEMORY_USER, self.root, self.device, alloc_params).hObjectNew
 
     if va_addr is None: va_addr = self._alloc_gpu_vaddr(size, alignment=align)
     if map_to_cpu: va_addr = self._gpu_map_to_cpu(mem_handle, size, target=va_addr, flags=map_flags)
-
-    handle = self._gpu_uvm_map(va_addr, size, mem_handle)
-    if map_to_all_gpus:
-      for dev in NVDevice.devices:
-        if dev != self: dev._gpu_uvm_map(handle.base, handle.length, handle.hMemory, create_range=False)
-    return handle
+    return self._gpu_uvm_map(va_addr, size, mem_handle)
 
   def _gpu_system_alloc(self, size:int, va_addr=None, map_to_cpu=False, map_flags=0):
     alloc_params = nv_gpu.NV_MEMORY_ALLOCATION_PARAMS(owner=self.root, type=13,
       attr=(nv_gpu.NVOS32_ATTR_PHYSICALITY_ALLOW_NONCONTIGUOUS << 27) | (nv_gpu.NVOS32_ATTR_LOCATION_PCI << 25),
       attr2=(nv_gpu.NVOS32_ATTR2_ZBC_PREFER_NO_ZBC << 0) | (nv_gpu.NVOS32_ATTR2_GPU_CACHEABLE_NO << 2),
       flags=(nv_gpu.NVOS32_ALLOC_FLAGS_IGNORE_BANK_PLACEMENT | nv_gpu.NVOS32_ALLOC_FLAGS_MEMORY_HANDLE_PROVIDED |
              nv_gpu.NVOS32_ALLOC_FLAGS_MAP_NOT_REQUIRED), format=6, size=size, alignment=(4<<10), offset=0, limit=size-1)
@@ -371,16 +399,23 @@
     if made.params.status != 0: raise RuntimeError(f"_map_to_gpu returned {made.params.status}")
     return self._gpu_uvm_map(va_base, size, made.params.hObjectNew)
 
   def _gpu_uvm_map(self, va_base, size, mem_handle, create_range=True) -> nv_gpu.UVM_MAP_EXTERNAL_ALLOCATION_PARAMS:
     if create_range: uvm.create_external_range(self.fd_uvm, base=va_base, length=size)
     gpu_attrs = (nv_gpu.struct_c__SA_UvmGpuMappingAttributes*256)(
       nv_gpu.struct_c__SA_UvmGpuMappingAttributes(gpuUuid=nv_gpu.struct_nv_uuid(uuid=self.gpu_uuid), gpuMappingType = 1))
+
+    # NOTE: va_addr is set to make rawbufs compatable with AMD.
     return uvm.map_external_allocation(self.fd_uvm, base=va_base, length=size, rmCtrlFd=self.fd_ctl, hClient=self.root, hMemory=mem_handle,
-                                       gpuAttributesCount=1, perGpuAttributes=gpu_attrs)
+                                       gpuAttributesCount=1, perGpuAttributes=gpu_attrs, va_addr=va_base)
+
+  def _gpu_map(self, mem):
+    if self.gpu_uuid in getattr(mem, "mapped_gpu_ids", []): return
+    mem.__setattr__("mapped_gpu_ids", getattr(mem, "mapped_gpu_ids", []) + [self.gpu_uuid])
+    return self._gpu_uvm_map(mem.base, mem.length, mem.hMemory, create_range=False)
 
   def _alloc_gpu_vaddr(self, size, alignment=(4 << 10)):
     NVDevice.uvm_vaddr = (res_va:=round_up(NVDevice.uvm_vaddr, alignment)) + size
     return res_va
 
   def __init__(self, device:str=""):
     if NVDevice.root is None:
@@ -411,14 +446,18 @@
                                                    vaMode=nv_gpu.NV_DEVICE_ALLOCATION_VAMODE_MULTIPLE_VASPACES)
     self.device = rm_alloc(self.fd_ctl, nv_gpu.NV01_DEVICE_0, self.root, self.root, device_params).hObjectNew
     self.subdevice = rm_alloc(self.fd_ctl, nv_gpu.NV20_SUBDEVICE_0, self.root, self.device, None).hObjectNew
     self.usermode = rm_alloc(self.fd_ctl, nv_gpu.TURING_USERMODE_A, self.root, self.subdevice, None).hObjectNew
     gpu_mmio_ptr = self._gpu_map_to_cpu(self.usermode, 0x10000, flags=2)
     self.gpu_mmio = to_mv(gpu_mmio_ptr, 0x10000).cast("I")
 
+    boost_params = nv_gpu.struct_NV2080_CTRL_PERF_BOOST_PARAMS(duration=0xffffffff, flags=((nv_gpu.NV2080_CTRL_PERF_BOOST_FLAGS_CUDA_YES << 4) | \
+      (nv_gpu.NV2080_CTRL_PERF_BOOST_FLAGS_CUDA_PRIORITY_HIGH << 6) | (nv_gpu.NV2080_CTRL_PERF_BOOST_FLAGS_CMD_BOOST_TO_MAX << 0)))
+    rm_control(self.fd_ctl, nv_gpu.NV2080_CTRL_CMD_PERF_BOOST, self.root, self.subdevice, boost_params)
+
     vaspace_params = nv_gpu.NV_VASPACE_ALLOCATION_PARAMETERS(vaBase=0x1000, vaSize=0x1fffffb000000,
       flags=nv_gpu.NV_VASPACE_ALLOCATION_FLAGS_ENABLE_PAGE_FAULTING | nv_gpu.NV_VASPACE_ALLOCATION_FLAGS_IS_EXTERNALLY_OWNED)
     vaspace = rm_alloc(self.fd_ctl, nv_gpu.FERMI_VASPACE_A, self.root, self.device, vaspace_params).hObjectNew
 
     gpu_uuid_params = nv_gpu.NV2080_CTRL_GPU_GET_GID_INFO_PARAMS(flags=nv_gpu.NV2080_GPU_CMD_GPU_GET_GID_FLAGS_FORMAT_BINARY, length=16)
     rm_control(self.fd_ctl, nv_gpu.NV2080_CTRL_CMD_GPU_GET_GID_INFO, self.root, self.subdevice, gpu_uuid_params)
     self.gpu_uuid = (ctypes.c_ubyte*16)(*[gpu_uuid_params.data[i] for i in range(16)])
@@ -427,87 +466,95 @@
     uvm.register_gpu_vaspace(self.fd_uvm, gpuUuid=nv_gpu.struct_nv_uuid(uuid=self.gpu_uuid), rmCtrlFd=self.fd_ctl,
                              hClient=self.root, hVaSpace=vaspace)
 
     for dev in self.devices:
       uvm.enable_peer_access(self.fd_uvm, gpuUuidA=nv_gpu.struct_nv_uuid(uuid=self.gpu_uuid), gpuUuidB=nv_gpu.struct_nv_uuid(uuid=dev.gpu_uuid))
 
     if NVDevice.signals_page is None: NVDevice.signals_page = self._gpu_system_alloc(0x10000, map_to_cpu=True)
-    else: self._gpu_uvm_map(NVDevice.signals_page.base, NVDevice.signals_page.length, NVDevice.signals_page.hMemory, create_range=False)
+    else: self._gpu_map(NVDevice.signals_page)
 
     channel_params = nv_gpu.NV_CHANNEL_GROUP_ALLOCATION_PARAMETERS(engineType=nv_gpu.NV2080_ENGINE_TYPE_GRAPHICS)
     channel_group = rm_alloc(self.fd_ctl, nv_gpu.KEPLER_CHANNEL_GROUP_A, self.root, self.device, channel_params).hObjectNew
 
     gpfifo = self._gpu_alloc(0x200000, contig=True, huge_page=True, map_to_cpu=True, map_flags=0x10d0000)
 
     ctxshare_params = nv_gpu.NV_CTXSHARE_ALLOCATION_PARAMETERS(hVASpace=vaspace, flags=nv_gpu.NV_CTXSHARE_ALLOCATION_FLAGS_SUBCONTEXT_ASYNC)
     ctxshare = rm_alloc(self.fd_ctl, nv_gpu.FERMI_CONTEXT_SHARE_A, self.root, channel_group, ctxshare_params).hObjectNew
 
     self.compute_gpfifo_entries: int = 0x10000
     self.compute_gpfifo_token: int = self._gpu_fifo_setup(gpfifo, ctxshare, channel_group, offset=0, entries=self.compute_gpfifo_entries)
     self.compute_gpu_ring: memoryview = to_mv(gpfifo.base, self.compute_gpfifo_entries * 8).cast("Q")
     self.compute_gpu_ring_controls = nv_gpu.AmpereAControlGPFifo.from_address(gpfifo.base + self.compute_gpfifo_entries * 8)
     self.compute_put_value: int = 0
-    self.compute_progress_signal = NVDevice._get_signal(self.device_id * 2)
 
     self.dma_gpfifo_entries: int = 0x10000
     self.dma_gpfifo_token: int = self._gpu_fifo_setup(gpfifo, ctxshare, channel_group, offset=0x100000, entries=self.dma_gpfifo_entries)
     self.dma_gpu_ring: memoryview = to_mv(gpfifo.base + 0x100000, self.dma_gpfifo_entries * 8).cast("Q")
     self.dma_gpu_ring_controls = nv_gpu.AmpereAControlGPFifo.from_address(gpfifo.base + 0x100000 + self.dma_gpfifo_entries * 8)
     self.dma_put_value: int = 0
-    self.dma_progress_signal = NVDevice._get_signal(self.device_id * 2 + 1)
 
     en_fifo_params = nv_gpu.NVA06C_CTRL_GPFIFO_SCHEDULE_PARAMS(bEnable=1)
     rm_control(self.fd_ctl, nv_gpu.NVA06C_CTRL_CMD_GPFIFO_SCHEDULE, self.root, channel_group, en_fifo_params)
 
+    self.timeline_value: int = 1
+    self.timeline_signal = NVDevice._get_signal(self.device_id * 2)
+    self._shadow_timeline_signal = NVDevice._get_signal(self.device_id * 2 + 1)
+    self.time_event_st, self.time_event_en = NVDevice._get_signal(), NVDevice._get_signal()
+
     self.cmdq_page: nv_gpu.UVM_MAP_EXTERNAL_ALLOCATION_PARAMS = self._gpu_alloc(0x200000, map_to_cpu=True, huge_page=True)
     self.cmdq: memoryview = to_mv(self.cmdq_page.base, 0x200000).cast("I")
     self.cmdq_wptr: int = 0 # in bytes
 
     self.kernargs_page: nv_gpu.UVM_MAP_EXTERNAL_ALLOCATION_PARAMS = self._gpu_alloc(0x4000000, map_to_cpu=True)
     self.kernargs_ptr: int = self.kernargs_page.base
 
-    self.arch: str = 'sm_89' # TODO: fix
-    self.pending_copyin: List[Any] = []
+    self.arch: str = "sm_89" if not MOCKGPU else "sm_35" # TODO: fix
 
-    super().__init__(device, NVAllocator(self), NVCompiler(self.arch), functools.partial(NVProgram, self))
+    from tinygrad.runtime.graph.hcq import HCQGraph
+    super().__init__(device, NVAllocator(self), CUDARenderer(self.arch), CUDACompiler(self.arch) if MOCKGPU else NVCompiler(self.arch),
+                     functools.partial(NVProgram, self), functools.partial(HCQGraph, NVDevice, HWComputeQueue, HWCopyQueue))
 
     self._cmdq_setup_compute_gpfifo()
     self._cmdq_setup_dma_gpfifo()
 
     NVDevice.devices.append(self)
 
   def synchronize(self):
-    self._wait_signal(self.compute_progress_signal, self.compute_put_value)
-    self._wait_signal(self.dma_progress_signal, self.dma_put_value)
+    NVDevice._wait_signal(self.timeline_signal, self.timeline_value - 1)
     self.cmdq_wptr = 0
 
-    for opaque,sz,options in self.pending_copyin: self.allocator.free(opaque, sz, options)
-    self.pending_copyin.clear()
+    if self.timeline_value > (1 << 63):
+      self.timeline_signal, self._shadow_timeline_signal = self._shadow_timeline_signal, self.timeline_signal
+      self.timeline_signal[0], self.timeline_value = 0, 1
+      cast(NVAllocator, self.allocator).b_timeline = [0] * len(cast(NVAllocator, self.allocator).b)
 
   @staticmethod
   def synchronize_system():
     for d in NVDevice.devices: d.synchronize()
 
   @classmethod
-  def _get_signal(self, num=None) -> memoryview:
+  def _set_signal(self, sig, value): sig[0] = value
+
+  @classmethod
+  def _get_signal(self, num=None, value=0) -> memoryview:
     if num is None:
       self.signal_number += 1
       if self.signals_page and self.signal_number * 16 >= self.signals_page.length: self.signal_number = 32
       num = self.signal_number
     sig = to_mv(self.signals_page.base + num * 16, 16).cast("Q")
-    sig[0] = 0
+    sig[0] = value
     return sig
 
   @classmethod
   def _wait_signal(self, signal, value=0, timeout=10000):
-    start_time = time.time()
+    start_time = time.time() * 1000
     sem_value = signal[0]
-    while sem_value != value:
+    while sem_value < value:
       sem_value = signal[0]
-      if time.time() - start_time > timeout // 1000: raise RuntimeError(f"wait_result: {timeout} ms TIMEOUT!")
+      if time.time() * 1000 - start_time > timeout: raise RuntimeError(f"wait_result: {timeout} ms TIMEOUT!")
 
   def _gpu_fifo_setup(self, gpfifo, ctxshare, channel_group, offset, entries=0x400):
     notifier = self._gpu_system_alloc(48 << 20)
     params = nv_gpu.NV_CHANNELGPFIFO_ALLOCATION_PARAMETERS(hObjectError=notifier.hMemory, hObjectBuffer=gpfifo.hMemory,
       gpFifoOffset=gpfifo.base+offset, gpFifoEntries=entries, hContextShare=ctxshare,
       hUserdMemory=(ctypes.c_uint32*8)(gpfifo.hMemory), userdOffset=(ctypes.c_uint64*8)(entries*8+offset))
     gpfifo = rm_alloc(self.fd_ctl, nv_gpu.AMPERE_CHANNEL_GPFIFO_A, self.root, channel_group, params).hObjectNew
@@ -535,15 +582,17 @@
 
     queue = HWComputeQueue()
     queue.q += [nvmethod(1, nv_gpu.NVC6C0_SET_OBJECT, 1), self.compute_type]
     queue.q += [nvmethod(1, nv_gpu.NVC6C0_SET_SHADER_LOCAL_MEMORY_A, 2), *nvdata64(self.shader_local_mem)]
     queue.q += [nvmethod(1, nv_gpu.NVC6C0_SET_SHADER_LOCAL_MEMORY_NON_THROTTLED_A, 3), *nvdata64(bytes_per_tpc), 0x40]
     queue.q += [nvmethod(1, nv_gpu.NVC6C0_SET_SHADER_LOCAL_MEMORY_WINDOW_A, 2), *nvdata64(self.local_mem_window)]
     queue.q += [nvmethod(1, nv_gpu.NVC6C0_SET_SHADER_SHARED_MEMORY_WINDOW_A, 2), *nvdata64(self.shared_mem_window)]
-    queue.submit(self)
+    queue.signal(self.timeline_signal, self.timeline_value).submit(self)
+    self.timeline_value += 1
     self.synchronize()
 
   def _cmdq_setup_dma_gpfifo(self):
     queue = HWCopyQueue()
     queue.q += [nvmethod(4, nv_gpu.NVC6C0_SET_OBJECT, 1), nv_gpu.AMPERE_DMA_COPY_B]
-    queue.submit(self)
+    queue.signal(self.timeline_signal, self.timeline_value).submit(self)
+    self.timeline_value += 1
     self.synchronize()
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/runtime/ops_python.py` & `tinygrad_tools-0.8.2/tinygrad/runtime/ops_python.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # a python uops emulator
 # works to test the tensor cores, and all the uops in general
 # this is the (living) definition of uops
 from typing import Tuple, List, Optional, Any, Dict
 import pickle, base64, itertools, time, struct
 from tinygrad.dtype import DType, dtypes, ImageDType
 from tinygrad.helpers import all_same, getenv, flatten
-from tinygrad.device import Compiled, Allocator, Compiler, CompilerOptions
+from tinygrad.device import Compiled, Compiler, Allocator
 from tinygrad.codegen.uops import UOpGraph, UOps
 from tinygrad.ops import BinaryOps, TernaryOps, exec_alu
+from tinygrad.renderer import Renderer
 
 def _load(m, i):
   if i < 0 or i >= len(m): raise IndexError(f"load out of bounds, size is {len(m)} and access is {i}")
   return m[i]
 
 def load(inp, j=0):
   if len(inp) == 4: return [_load(m, x+j) if gate else default for m,x,gate,default in zip(*inp)]
@@ -82,15 +83,15 @@
           if arg[1][0] == 'g':
             ul[i] = [idxs[2-arg[0]]] * warp_size
           elif arg[1][0] == 'l':
             ul[i] = [x[2-arg[0]] for x in warp]
         elif uop is UOps.CONST:
           ul[i] = [[arg] * warp_size for _ in range(dtype.count)] if dtype.count > 1 else [arg] * warp_size
         elif uop is UOps.DEFINE_ACC:
-          ul[i] = [[arg] * warp_size for _ in range(dtype.count)] if dtype.count > 1 else [arg] * warp_size
+          ul[i] = [[arg[0]] * warp_size for _ in range(dtype.count)] if dtype.count > 1 else [arg[0]] * warp_size
         elif uop is UOps.LOOP:
           if i not in ul: ul[i] = [inp[0][0]] * warp_size
           else:
             for j in range(len(ul[i])):
               ul[i][j] += 1
             if ul[i][0] == inp[1][0]:
               del ul[i]
@@ -173,24 +174,29 @@
           assert all_same([len(x) for x in inp]), f"{[len(x) for x in inp]} doesn't match on {arg}"
           assert all_same([dtype] + dtp) or arg in {BinaryOps.CMPEQ, BinaryOps.CMPLT, TernaryOps.WHERE}, f"dtype mismatch on {arg}"
           ul[i] = [exec_alu(arg, dtype, p) for p in zip(*inp)]
         assert i in ul, (uop, dtype, idp, arg)
         i += 1
     return time.perf_counter() - st
 
-class PythonCompiler(Compiler):
-  compiler_opts = CompilerOptions("METAL", has_tensor_cores=True) if getenv("EMULATE_METAL") else \
-    (CompilerOptions("HSA", has_tensor_cores=True) if getenv("EMULATE_HSA") else \
-    (CompilerOptions("CUDA", has_tensor_cores=True) if getenv("EMULATE_CUDA") else CompilerOptions("PYTHON")))
+class PythonRenderer(Renderer):
+  device = "PYTHON"
+  def __init__(self):
+    if getenv("EMULATE_METAL"): self.device, self.has_tensor_cores = "METAL", True
+    if getenv("EMULATE_HSA"): self.device, self.has_tensor_cores = "HSA", True
+    if getenv("EMULATE_CUDA"): self.device, self.has_tensor_cores = "CUDA", True
+
   def render(self, name:str, uops:UOpGraph) -> str:
     lops = [(u.uop, u.dtype, [uops.uops.index(v) for v in u.vin], u.arg) for u in uops]
     return base64.b64encode(pickle.dumps(lops)).decode()
+
+class PythonCompiler(Compiler):
   def compile(self, src:str) -> bytes: return base64.b64decode(src)
 
 class PythonAllocator(Allocator):
   def _alloc(self, size, options): return memoryview(bytearray(size))
   def copyin(self, dest, src:memoryview): dest[:] = src
   def copyout(self, dest:memoryview, src): dest[:] = src
 
 class PythonDevice(Compiled):
   def __init__(self, device:str):
-    super().__init__(device, PythonAllocator(), PythonCompiler(), PythonProgram)
+    super().__init__(device, PythonAllocator(), PythonRenderer(), PythonCompiler(), PythonProgram)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad/shape/shapetracker.py` & `tinygrad_tools-0.8.2/tinygrad/shape/shapetracker.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/shape/symbolic.py` & `tinygrad_tools-0.8.2/tinygrad/shape/symbolic.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/shape/view.py` & `tinygrad_tools-0.8.2/tinygrad/shape/view.py`

 * *Files identical despite different names*

### Comparing `tinygrad_tools-0.8.1/tinygrad/tensor.py` & `tinygrad_tools-0.8.2/tinygrad/tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from __future__ import annotations
 import time, math, itertools, functools
 from contextlib import ContextDecorator
 from typing import List, Tuple, Callable, Optional, ClassVar, Type, Union, Sequence, Dict, DefaultDict, cast, get_args, Set
 from collections import defaultdict
 import numpy as np
 
-from tinygrad.dtype import DType, dtypes, ImageDType, ConstType, least_upper_float, least_upper_dtype
+from tinygrad.dtype import DType, dtypes, ImageDType, ConstType, least_upper_float, least_upper_dtype, sum_acc_dtype
 from tinygrad.helpers import argfix, make_pair, flatten, prod, all_int, round_up, merge_dicts, fully_flatten, argsort, IMAGE, DEBUG, WINO, THREEFRY
 from tinygrad.helpers import getenv
 from tinygrad.lazy import LazyBuffer
-from tinygrad.features.multi import MultiLazyBuffer
-from tinygrad.ops import LoadOps, ScheduleItem
-from tinygrad.buffer import Buffer, BufferOptions
+from tinygrad.multi import MultiLazyBuffer
+from tinygrad.ops import LoadOps
+from tinygrad.device import Buffer, BufferOptions
 from tinygrad.device import Device
 from tinygrad.shape.symbolic import sint, Variable, MulNode, Node
-from tinygrad.engine.realize import run_schedule, memory_planner
-from tinygrad.engine.schedule import create_schedule_with_vars
+from tinygrad.engine.realize import run_schedule
+from tinygrad.engine.schedule import ScheduleItem, create_schedule_with_vars, memory_planner
 
 # **** start with two base classes, Tensor and Function ****
 
 class Function:
   def __init__(self, device:Union[str, Tuple[str, ...]], *tensors:Tensor):
     self.device = device
     self.needs_input_grad = [t.requires_grad for t in tensors]
@@ -106,17 +106,17 @@
     self._ctx: Optional[Function] = None
     if isinstance(data, LazyBuffer): assert dtype is None or dtype == data.dtype, "dtype doesn't match, and casting isn't supported"
     elif isinstance(data, get_args(ConstType)): data = _loadop(LoadOps.CONST, tuple(), dtype or dtypes.from_py(data), device, data)
     elif isinstance(data, Variable): data = _loadop(LoadOps.CONST, tuple(), dtype or dtypes.from_py(data.unbind()[1]), device, data)
     elif isinstance(data, bytes): data = _fromcpu(np.frombuffer(data, np.uint8))
     elif data is None: data = _loadop(LoadOps.EMPTY, (0,), dtype or dtypes.default_float, device)
     elif isinstance(data, list):
-      if (d := fully_flatten(data)) and all(isinstance(s, bool) for s in d): dtype = dtype or dtypes.bool
-      elif d and all_int(d): dtype = dtype or dtypes.default_int
-      else: dtype = dtype or dtypes.default_float
+      if dtype is None:
+        if (d := fully_flatten(data)) and all(isinstance(s, bool) for s in d): dtype = dtypes.bool
+        else: dtype = dtypes.default_int if d and all_int(d) else dtypes.default_float
       if dtype == dtypes.bfloat16: data = Tensor(_fromcpu(np.array(data, np.float32)), device=device).cast(dtypes.bfloat16).lazydata
       else: data = _fromcpu(np.array(data, dtype.np))
     elif isinstance(data, np.ndarray):
       if data.shape == (): data = _loadop(LoadOps.CONST, tuple(), dtype or dtypes.from_np(data.dtype), device, data.item())
       else: data = _fromcpu(data.astype(dtype.np) if dtype is not None and dtype.np is not None else data)
 
     # data is a LazyBuffer, but it might be on the wrong device
@@ -331,25 +331,26 @@
       # for bfloat16, numpy rand passes buffer in float
       if (dtype or dtypes.default_float) == dtypes.bfloat16:
         return Tensor.rand(*shape, **kwargs, device=device, dtype=dtypes.float).cast(dtypes.bfloat16)
       return Tensor._loadop(LoadOps.CUSTOM, argfix(*shape), arg=custom_random, device=device, dtype=dtype, **kwargs)
 
     # threefry
     if (num := prod((shape:=argfix(*shape)))) == 0: return Tensor.zeros(shape, device=device, dtype=dtype, **kwargs)
-    counts = (Tensor.arange(num, device=device, dtype=dtypes.uint32, requires_grad=False)+Tensor._rng_counter.to(device)).realize().pad(((0,num%2),))
+    counts1 = (Tensor.arange(math.ceil(num / 2), device=device, dtype=dtypes.uint32, requires_grad=False)+Tensor._rng_counter.to(device)).realize()
+    counts2 = counts1 + math.ceil(num / 2)
     Tensor._rng_counter.assign(Tensor._rng_counter + num).realize()
 
     rotations = [[13, 15, 26, 6], [17, 29, 16, 24]]
     ks = [0x0, Tensor._seed ^ 0x0 ^ 0x1BD11BDA, Tensor._seed]
 
-    x = [(c := counts.chunk(2))[0] + ks[-1], c[1] + ks[0]]
+    x = [counts1 + ks[-1], counts2 + ks[0]]
     for i in range(5):
-      for r in rotations[i % 2]: x[0], x[1] = (x0 := x[0] + x[1]), x0 ^ ((x[1] * (2 ** r)) + (x[1].div(2 ** (32 - r), upcast=False)))
+      for r in rotations[i % 2]: x[0], x[1] = (x0 := x[0] + x[1]), x0 ^ ((x[1] << r) + (x[1] >> (32 - r)))
       x = [(x[0] + ks[i % 3]), (x[1] + ks[(i + 1) % 3] + i + 1)]
-    out = x[0].cat(x[1])[:num].div(2 ** 8, upcast=False).cast(dtypes.float32).div(2 ** 24)
+    out = x[0].cat(x[1]).rshift(8).cast(dtypes.float32).div(2 ** 24)[:num]
     out = out.reshape(shape).cast(dtypes.default_float if dtype is None else dtype)
     out.requires_grad = kwargs.get("requires_grad")
     return out.contiguous()
 
   # ***** creation helper functions *****
 
   @staticmethod
@@ -793,15 +794,15 @@
 
       masks, first_dim, last_dim = [], min(idx.keys()), max(idx.keys())
       pre_reduce_shape = ret.shape[:first_dim] + (big_shape := broadcast_shape(*(t.shape for t in idx.values()))) + ret.shape[first_dim:]
 
       # create masks
       for dim, i in idx.items():
         try: i = i.reshape(i.shape + (1,)*(ret.ndim - first_dim)).expand(pre_reduce_shape)
-        except ValueError as exc: raise IndexError("cannot broadcast indices") from exc
+        except ValueError as e: raise IndexError(f"cannot broadcast indices: {e}") from e
         a = Tensor.arange(ret.shape[dim], device=self.device, requires_grad=False).reshape((ret.shape[dim],) + (1,)*(ret.ndim - dim - 1))
         masks.append(i == a)
 
       # reduce masks to 1 mask
       mask: Tensor = functools.reduce(lambda x,y: x.mul(y), masks)
 
       # inject 1's for the extra dims added in create masks
@@ -818,14 +819,18 @@
     if isinstance(self.device, str) and self.device.startswith("DISK"):
       self.__getitem__(indices).assign(v)
       return
     # NOTE: check that setitem target is valid first
     assert all(lb.st.contiguous for lb in self.lazydata.lbs), "setitem target needs to be contiguous"
     if not isinstance(v, (Tensor, float, int, bool)): raise TypeError(f"can't set a {type(v).__name__} to a Tensor")
     if not isinstance(v, Tensor): v = Tensor(v, device=self.device, dtype=self.dtype)
+    if self.requires_grad or v.requires_grad: raise NotImplementedError("setitem with requires_grad is not supported")
+    if isinstance(indices, (Tensor, list)) or (isinstance(indices, tuple) and any(isinstance(i, (Tensor, list)) for i in indices)):
+      raise NotImplementedError("Advanced indexing setitem is not currently supported")
+
     assign_to = self.realize().__getitem__(indices)
     # NOTE: contiguous to prevent const folding.
     v = v.cast(assign_to.dtype)._broadcast_to(broadcast_shape(assign_to.shape, v.shape)).contiguous()
     assign_to.assign(v).realize()
 
   # NOTE: using slice is discouraged and things should migrate to pad and shrink
   def slice(self, arg:Sequence[Optional[Tuple[int, sint]]], value:float=0) -> Tensor:
@@ -909,63 +914,69 @@
     return self.reshape(self.shape[:start_dim] + (prod(self.shape[start_dim:end_dim+1]), ) + self.shape[end_dim+1:])
   def unflatten(self, dim:int, sizes:Tuple[int,...]):
     dim = self._resolve_dim(dim)
     return self.reshape(self.shape[:dim] + sizes + self.shape[dim+1:])
 
   # ***** reduce ops *****
 
-  def _reduce(self, fxn:Type[Function], axis:Optional[Union[int, Tuple[int, ...]]]=None, keepdim=False, acc_dtype:Optional[DType]=None) -> Tensor:
+  def _reduce(self, fxn:Type[Function], axis:Optional[Union[int, Tuple[int, ...]]]=None, keepdim=False) -> Tensor:
+    if self.ndim == 0:
+      if axis is not None and axis not in [-1, 0]: raise IndexError(f"{axis=} out of range of [-1, 0]")
+      axis = None
     axis_: Tuple[int, ...] = tuple(range(len(self.shape))) if axis is None else ((axis,) if isinstance(axis, int) else tuple(axis))
-    axis_ = tuple(x if x >= 0 else x+len(self.shape) for x in axis_)
-    shape = tuple(s for i,s in enumerate(self.shape) if i not in axis_)
-    ret = fxn.apply(self, axis=axis_, acc_dtype=acc_dtype)
-    return ret if keepdim else ret.reshape(shape)
-
-  def sum(self, axis=None, keepdim=False, acc_dtype:Optional[DType]=None): return self._reduce(F.Sum, axis, keepdim, acc_dtype)
+    axis_ = tuple(self._resolve_dim(x) for x in axis_)
+    ret = fxn.apply(self, axis=axis_)
+    return ret if keepdim else ret.reshape(tuple(s for i,s in enumerate(self.shape) if i not in axis_))
+
+  def sum(self, axis=None, keepdim=False, acc_dtype:Optional[DType]=None):
+    ret = self.cast(acc_dtype or sum_acc_dtype(self.dtype))._reduce(F.Sum, axis, keepdim)
+    return ret.cast(self.dtype) if self.dtype in {dtypes.float16, dtypes.bfloat16} else ret
   def max(self, axis=None, keepdim=False): return self._reduce(F.Max, axis, keepdim)
   def min(self, axis=None, keepdim=False): return -((-self).max(axis=axis, keepdim=keepdim))
 
   def mean(self, axis=None, keepdim=False):
-    out = self.sum(axis=axis, keepdim=keepdim)
-    return out.div(prod([si for si, so in zip(self.shape, self.sum(axis=axis, keepdim=True).shape) if si != so]))
+    output_dtype = self.dtype if dtypes.is_float(self.dtype) else dtypes.float32
+    numerator = self.cast(sum_acc_dtype(self.dtype)).sum(axis=axis, keepdim=keepdim)
+    return numerator.div(prod([si for si, so in zip(self.shape, self.sum(axis=axis, keepdim=True).shape) if si != so])).cast(output_dtype)
   def var(self, axis=None, keepdim=False, correction=1):
     assert all_int(self.shape), "does not support symbolic shape"
     square_sum = ((self - self.mean(axis=axis, keepdim=True)).square()).sum(axis=axis, keepdim=keepdim)
     return square_sum.div(max(0, prod(self.shape)/prod(square_sum.shape)-correction))
   def std(self, axis=None, keepdim=False, correction=1): return self.var(axis, keepdim, correction).sqrt()
 
   def _softmax(self, axis):
-    if len(self.shape) == 0:
-      assert axis in [-1, 0], f"{axis=} out of range of [-1, 0]"
-      axis = None
     m = self - self.max(axis=axis, keepdim=True)
     e = m.exp()
     return m, e, e.sum(axis=axis, keepdim=True)
 
   def softmax(self, axis=-1):
     _, e, ss = self._softmax(axis)
     return e.div(ss)
 
   def log_softmax(self, axis=-1):
     m, _, ss = self._softmax(axis)
     return m - ss.log()
 
+  def logsumexp(self, axis=None, keepdim=False):
+    m = self.max(axis=axis, keepdim=True)
+    return (self - m).exp().sum(axis=axis, keepdim=keepdim).log() + m.squeeze(axis)
+
   def argmax(self, axis=None, keepdim=False):
     # NOTE: return the first index if there are multiple occurrences of the maximum values
     if axis is None:
       idx = (self == self.max(axis)) * Tensor.arange(prod(self.shape)-1,-1,-1, requires_grad=False, device=self.device).reshape(self.shape)
       return (prod(self.shape) - idx.max() - 1).cast(dtypes.int32)
     axis = self._resolve_dim(axis)
     m = self == self.max(axis=axis, keepdim=True)
     idx = m * Tensor.arange(self.shape[axis]-1,-1,-1, requires_grad=False, device=self.device).reshape(self.shape[axis], *[1]*(self.ndim-axis-1))
     return (self.shape[axis]-idx.max(axis=axis, keepdim=keepdim)-1).cast(dtypes.int32)
   def argmin(self, axis=None, keepdim=False): return (-self).argmax(axis=axis, keepdim=keepdim)
 
   @staticmethod
-  def einsum(formula:str, *raw_xs) -> Tensor:
+  def einsum(formula:str, *raw_xs, acc_dtype:Optional[DType]=None) -> Tensor:
     xs:Tuple[Tensor] = argfix(*raw_xs)
     formula = formula.replace(" ", "")
     inputs_str, output = formula.split("->") if "->" in formula else (formula, sorted(formula))
     inputs = [x for x in cast(str,inputs_str).split(',')]
     assert len(xs) == len(inputs), f"number of inputs doesn't match number of operands in formula, expected {len(inputs)}, got {len(xs)}"
 
     # map the value of each letter in the formula
@@ -979,15 +990,15 @@
 
     # determine the inverse permutation to revert back to original order
     rhs_letter_order = argsort(list(output))
     rhs_order = argsort(rhs_letter_order)
 
     # sum over all axes that's not in the output, then permute to the output order
     return functools.reduce(lambda a,b:a*b, xs_) \
-      .sum(axis=[axis for axis,(letter,_) in enumerate(letter_val) if letter not in output]).permute(rhs_order)
+      .sum(axis=[axis for axis,(letter,_) in enumerate(letter_val) if letter not in output],acc_dtype=acc_dtype).permute(rhs_order)
 
   # ***** processing ops *****
 
   def _pool(self, k_:Tuple[sint, ...], stride:Union[Tuple[int, ...], int]=1, dilation:Union[Tuple[int, ...], int]=1) -> Tensor:
     assert len(self.shape) >= len(k_), f"can't pool {self.shape} with {k_}"
     assert all_int(self.shape) and all_int(k_), f"does not support symbolic {self.shape=}, {k_=}"
     s_, d_ = make_pair(stride, len(k_)), make_pair(dilation, len(k_))
@@ -1136,24 +1147,24 @@
   def ceil(self: Tensor) -> Tensor: return (self > (b := self.trunc())).where(b+1, b)
   def floor(self: Tensor) -> Tensor: return (self < (b := self.trunc())).where(b-1, b)
   def round(self: Tensor) -> Tensor:
     return ((self > 0) == ((b := self.cast(dtypes.int32) / 2.0).cast(dtypes.int32) == b)).where((self - 0.5).ceil(), (self + 0.5).floor())
   def lerp(self, end: Tensor, weight: Union[Tensor, float]) -> Tensor: return self + (end - self) * weight
   def square(self): return self*self
   def clip(self, min_, max_): return self.maximum(min_).minimum(max_)
-  def abs(self): return self.relu() + (-self).relu()
-  def sign(self): return ((self.float()) / (self.float().abs() + 1e-12)).cast(self.dtype)
+  def sign(self): return F.Sign.apply(self)
+  def abs(self): return self * self.sign()
   def reciprocal(self): return F.Reciprocal.apply(self.cast(least_upper_float(self.dtype)))
 
   # ***** activation functions (unary) *****
 
   def elu(self, alpha=1.0): return self.relu() - alpha*(1-self.exp()).relu()
   def celu(self, alpha=1.0): return self.maximum(0) + (alpha * ((self / alpha).exp() - 1)).minimum(0)
   def swish(self): return self * self.sigmoid()
-  def silu(self): return self.swish()   # The SiLU function is also known as the swish F.
+  def silu(self): return self.swish()   # The SiLU function is also known as the swish function.
   def relu6(self): return self.relu() - (self-6).relu()
   def hardswish(self): return self * (self+3).relu6() * (1/6)
   def tanh(self): return 2.0 * ((2.0 * self).sigmoid()) - 1.0
   def sinh(self): return (self.exp() - self.neg().exp()) / 2
   def cosh(self): return (self.exp() + self.neg().exp()) / 2
   def atanh(self): return ((1 + self)/(1 - self)).log() / 2
   def asinh(self): return (self + (self.square() + 1).sqrt()).log()
@@ -1203,14 +1214,22 @@
   def mul(self, x:Union[Tensor, ConstType], reverse=False) -> Tensor: return F.Mul.apply(*self._broadcasted(x, reverse))
   def div(self, x:Union[Tensor, ConstType], reverse=False, upcast=True) -> Tensor:
     numerator, denominator = self._broadcasted(x, reverse)
     if upcast: numerator, denominator = numerator.cast(least_upper_float(numerator.dtype)), denominator.cast(least_upper_float(denominator.dtype))
     return F.Div.apply(numerator, denominator)
   def xor(self, x:Union[Tensor, ConstType], reverse=False) -> Tensor: return F.Xor.apply(*self._broadcasted(x, reverse))
 
+  def lshift(self, x:int):
+    assert dtypes.is_unsigned(self.dtype) and isinstance(x, int) and x >= 0, f"not supported {self.dtype=} {x=}"
+    return self.mul(2 ** x)
+
+  def rshift(self, x:int):
+    assert dtypes.is_unsigned(self.dtype) and isinstance(x, int) and x >= 0, f"not supported {self.dtype=} {x=}"
+    return self.div(2 ** x, upcast=False)
+
   def pow(self, x:Union[Tensor, ConstType], reverse=False) -> Tensor:
     x = self._to_const_val(x)
     if not isinstance(x, Tensor) and not reverse:
       # simple pow identities
       if x < 0: return self.reciprocal().pow(-x)
       if x == 0: return 1 + self * 0
       if x in [3,2,1]: return functools.reduce(lambda acc,_: acc * self, range(int(x)-1), self)
@@ -1249,14 +1268,16 @@
   def __add__(self, x) -> Tensor: return self.add(x)
   def __sub__(self, x) -> Tensor: return self.sub(x)
   def __mul__(self, x) -> Tensor: return self.mul(x)
   def __pow__(self, x) -> Tensor: return self.pow(x)
   def __truediv__(self, x) -> Tensor: return self.div(x)
   def __matmul__(self, x) -> Tensor: return self.matmul(x)
   def __xor__(self, x) -> Tensor: return self.xor(x)
+  def __lshift__(self, x) -> Tensor: return self.lshift(x)
+  def __rshift__(self, x) -> Tensor: return self.rshift(x)
 
   def __radd__(self, x) -> Tensor: return self.add(x, True)
   def __rsub__(self, x) -> Tensor: return self.sub(x, True)
   def __rmul__(self, x) -> Tensor: return self.mul(x, True)
   def __rpow__(self, x) -> Tensor: return self.pow(x, True)
   def __rtruediv__(self, x) -> Tensor: return self.div(x, True)
   def __rmatmul__(self, x) -> Tensor: return self.matmul(x, True)
@@ -1265,14 +1286,16 @@
   def __iadd__(self, x) -> Tensor: return self.assign(self.add(x))
   def __isub__(self, x) -> Tensor: return self.assign(self.sub(x))
   def __imul__(self, x) -> Tensor: return self.assign(self.mul(x))
   def __ipow__(self, x) -> Tensor: return self.assign(self.pow(x))
   def __itruediv__(self, x) -> Tensor: return self.assign(self.div(x))
   def __imatmul__(self, x) -> Tensor: return self.assign(self.matmul(x))
   def __ixor__(self, x) -> Tensor: return self.assign(self.xor(x))
+  def __ilshift__(self, x) -> Tensor: return self.assign(self.lshift(x))
+  def __irshift__(self, x) -> Tensor: return self.assign(self.rshift(x))
 
   def __lt__(self, x) -> Tensor: return F.Less.apply(*self._broadcasted(x, False))
   def __gt__(self, x) -> Tensor: return F.Less.apply(*self._broadcasted(x, True))
   def __ge__(self, x) -> Tensor: return (self<x).logical_not()
   def __le__(self, x) -> Tensor: return (self>x).logical_not()
   def __eq__(self, x) -> Tensor: return F.Eq.apply(*self._broadcasted(x, True))       # type: ignore[override]
   def __ne__(self, x) -> Tensor: return (self==x).logical_not()                       # type: ignore[override]
@@ -1320,17 +1343,17 @@
     return (self.maximum(0) - y * self + (1 + self.abs().neg().exp()).log()).mean()
 
   def sparse_categorical_crossentropy(self, Y:Tensor, ignore_index=-1, label_smoothing=0.0) -> Tensor:
     assert 0.0 <= label_smoothing <= 1.0, "label_smoothing must be in [0.0, 1.0]"
     # NOTE: self is a logits input
     log_probs, loss_mask = self.log_softmax(), (Y != ignore_index)
     y_counter = Tensor.arange(self.shape[-1], requires_grad=False, device=self.device).unsqueeze(0).expand(Y.numel(), self.shape[-1])
-    y = ((y_counter == Y.flatten().reshape(-1, 1)).where(-1, 0) * loss_mask.reshape(-1, 1)).reshape(*Y.shape, self.shape[-1])
-    smoothing = -1 * label_smoothing * (log_probs.mean(-1) * loss_mask).sum() / loss_mask.sum()
-    return (1 - label_smoothing) * (log_probs * y).sum() / loss_mask.sum() + smoothing
+    y = ((y_counter == Y.flatten().reshape(-1, 1)) * loss_mask.reshape(-1, 1)).reshape(*Y.shape, self.shape[-1])
+    smoothing = label_smoothing * (log_probs.mean(-1) * loss_mask).sum()
+    return -((1 - label_smoothing) * (log_probs * y).sum() + smoothing) / loss_mask.sum()
 
   # ***** cast ops *****
 
   def llvm_bf16_cast(self, dtype:DType):
     # hack for devices that don't support bfloat16
     assert self.dtype == dtypes.bfloat16
     return self.to("LLVM").bitcast(dtypes.uint16).cast(dtypes.uint32).mul(1<<16).bitcast(dtypes.float32).cast(dtype)
@@ -1347,22 +1370,102 @@
   def ndim(self) -> int: return len(self.shape)
   def numel(self) -> sint: return prod(self.shape)
   def element_size(self) -> int: return self.dtype.itemsize
   def nbytes(self) -> int: return self.numel() * self.element_size()
   def is_floating_point(self) -> bool: return dtypes.is_float(self.dtype)
   def size(self, dim=None) -> Union[sint, Tuple[sint, ...]]: return self.shape if dim is None else self.shape[dim]
 
+  # *** image Tensor function replacements ***
+
+  def image_dot(self, w:Tensor, acc_dtype=None):
+    # NOTE: we use a 1x1 conv2d to do the matmul. mxk @ kxn = (1,k,m,1).conv2d(n,k,1,1)
+    n1, n2 = len(self.shape), len(w.shape)
+    assert n1 != 0 and n2 != 0, f"both arguments to matmul need to be at least 1D, but they are {n1}D and {n2}D"
+    assert self.shape[-1] == w.shape[-min(n2, 2)], f"Input Tensor shapes {self.shape} and {w.shape} cannot be multiplied ({self.shape[-1]} != {w.shape[-min(n2, 2)]})"  # noqa: E501
+    bs, groups, cin, cout = prod(self.shape[0:-2]), prod(w.shape[0:-2]), w.shape[-2], w.shape[-1]
+    out_shape_t = self.shape[0:-2] + (cout,-1) if len(self.shape) > 1 else (cout, )
+
+    # NOTE: with NHWC we can remove the transposes
+    # bs x groups*cin x H x W
+    cx = self.transpose(self.ndim-1, self.ndim-2).reshape((bs//groups, groups*cin, -1, 1))
+    # groups*cout x cin x H, W
+    cw = w.transpose(w.ndim-1, w.ndim-2).reshape((groups*cout, cin, 1, 1))
+    return cx.image_conv2d(cw, groups=groups, acc_dtype=acc_dtype).reshape(out_shape_t).transpose(self.ndim-1, self.ndim-2)
+
+  def image_conv2d(self, weight:Tensor, bias:Optional[Tensor]=None, groups=1, stride=1, dilation=1, padding=0, acc_dtype=None):
+    base_image_type = dtypes.imageh if getenv("FLOAT16", 0) else dtypes.imagef
+
+    (bs,_,iy,ix), (cout,cin,H,W) = self.shape, weight.shape
+    x, w = self, weight.reshape(groups, (rcout := cout//groups), cin, H, W)
+
+    # hack for non multiples of 4 on cin
+    if cin % 4 != 0 and not (cin == 1 and groups%4 == 0):
+      x = x.reshape(bs, groups, cin, iy, ix)   # do this always?
+      added_input_channels = 4 - (cin % 4)
+      w = w.pad(tuple((0, added_input_channels) if i == 2 else None for i in range(w.ndim)))
+      x = x.pad(tuple((0, added_input_channels) if i == 2 else None for i in range(x.ndim)))
+      cin = cin + added_input_channels
+      x = x.reshape(bs, groups*cin, iy, ix)
+
+    # hack for non multiples of 4 on rcout
+    added_output_channels = 0
+    if rcout % 4 != 0 and not (rcout == 1 and groups%4 == 0):
+      added_output_channels = 4 - (rcout % 4)
+      rcout += added_output_channels
+      cout = groups * rcout
+      w = w.pad(tuple((0, added_output_channels) if i == 1 else None for i in range(w.ndim)))
+
+    # packed (note: flipping bs and iy would make the auto-padding work)
+    x = x.permute(0,2,3,1)
+    cin_last = iy == 1 and ix == 1
+    if cin == 1: w = w.reshape(cout//4,4,H,W).permute(0,2,3,1)
+    elif cin_last: w = w.reshape(cout//4,4,cin//4,4,H,W).permute(0,4,2,5,1,3)
+    else: w = w.reshape(cout//4,4,cin//4,4,H,W).permute(0,4,2,5,3,1)
+
+    # contiguous creates the image, and early realize static weights (TODO: test for the static weight)
+    if IMAGE >= 2: x,w = x.cast(base_image_type((bs*iy, ix*groups*cin//4, 4))), w.cast(base_image_type((cout//4, H*W*cin, 4)))
+    x, w = x.contiguous(), w.contiguous()
+
+    # expand out
+    rcin_hi, rcin_lo = cin//4 if cin >= 4 else 1, 4 if cin >= 4 else 1
+    cout_expand = [groups//4 if cin == 1 else groups, 4 if cin == 1 else 1, rcout//4 if rcout >= 4 else 1, 4 if rcout >= 4 else 1]
+    x = x.reshape(bs, iy, ix, groups, rcin_hi, rcin_lo)
+    if cin_last: w = w.reshape(cout//4, H, rcin_hi, W, 4, rcin_lo)
+    else: w = w.reshape(cout//4, H, rcin_hi, W, rcin_lo, 4).permute(0,1,2,3,5,4)
+
+    # padding
+    padding_ = [padding]*4 if isinstance(padding, int) else (padding if len(padding) == 4 else [padding[1], padding[1], padding[0], padding[0]])
+    x = x.slice((None, (-padding_[2], x.shape[1]+padding_[3]), (-padding_[0], x.shape[2]+padding_[1]), None, None, None))
+
+    # prepare input
+    x = x.permute(0,3,4,5,1,2)._pool((H, W), stride, dilation) # -> (bs, groups, rcin_hi, rcin_lo, oy, ox, H, W)
+    x = x.permute(0,4,5,1,2,3,6,7).reshape(bs, (oy := x.shape[4]), (ox := x.shape[5]), *cout_expand[0:2], 1, 1, rcin_hi, rcin_lo, H, W)
+
+    # prepare weights
+    w = w.permute(0,4,2,5,1,3).reshape((1, 1, 1, *cout_expand, rcin_hi, rcin_lo, H, W))
+
+    # the conv!
+    ret = (x*w).cast(base_image_type((bs*oy, ox*cout//4, 4)) if IMAGE >= 2 else dtypes.float32).sum((-4, -3, -2, -1), acc_dtype=acc_dtype)
+
+    # undo hack for non multiples of 4 on C.rcout
+    if added_output_channels != 0:
+      ret = ret.reshape(bs, oy, ox, groups, rcout)[:, :, :, :, :-added_output_channels]
+      cout = groups * (rcout - added_output_channels)
+
+    # NCHW output
+    ret = ret.reshape(bs, oy, ox, cout).permute(0,3,1,2)
+    return ret if bias is None else ret.add(bias.reshape(1, -1, 1, 1))
+
 # register functions to move between devices
 for device in Device._devices: setattr(Tensor, f"{device.lower()}", functools.partialmethod(Tensor.to, device))
 
 if IMAGE:
   # if IMAGE>0 we install these replacement functions in Tensor (hack!)
-  from tinygrad.features.image import image_conv2d, image_dot
-  setattr(Tensor, "conv2d", image_conv2d)
-  setattr(Tensor, "dot", image_dot)
+  setattr(Tensor, "conv2d", Tensor.image_conv2d)
+  setattr(Tensor, "dot", Tensor.image_dot)
 
 # TODO: eventually remove this
 def custom_random(out:Buffer):
   Tensor._seed += 1
   rng = np.random.default_rng(Tensor._seed)
   if out.dtype == dtypes.half: rng_np_buffer = (rng.integers(low=0, high=2047, size=out.size) / 2048).astype(np.half, copy=False)
   else: rng_np_buffer = rng.random(size=out.size, dtype=np.float32).astype(dtype=out.dtype.np, copy=False)
```

### Comparing `tinygrad_tools-0.8.1/tinygrad_tools.egg-info/PKG-INFO` & `tinygrad_tools-0.8.2/tinygrad_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinygrad-tools
-Version: 0.8.1
+Version: 0.8.2
 Summary: You like pytorch? You like micrograd? You love tinygrad! <3
 Author: George Hotz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -44,24 +44,24 @@
 Requires-Dist: hypothesis; extra == "testing"
 Requires-Dist: nibabel; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: markdown-callouts; extra == "docs"
 Requires-Dist: markdown-exec[ansi]; extra == "docs"
+Requires-Dist: black; extra == "docs"
 Provides-Extra: testing-tf
 Requires-Dist: tensorflow==2.15.1; extra == "testing-tf"
 Requires-Dist: tensorflow_addons; extra == "testing-tf"
 
 <div align="center">
 
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="/docs-legacy/logo_tiny_dark.svg">
-  <source media="(prefers-color-scheme: light)" srcset="/docs-legacy/logo_tiny_light.svg">
-  <img alt="tiny corp logo" src="/docs-legacy/logo_tiny_light.svg" width="50%" height="50%">
+  <source media="(prefers-color-scheme: light)" srcset="/docs/logo_tiny_light.svg">
+  <img alt="tiny corp logo" src="/docs/logo_tiny_dark.svg" width="50%" height="50%">
 </picture>
 
 tinygrad: For something between [PyTorch](https://github.com/pytorch/pytorch) and [karpathy/micrograd](https://github.com/karpathy/micrograd). Maintained by [tiny corp](https://tinygrad.org).
 
 <h3>
 
 [Homepage](https://github.com/tinygrad/tinygrad) | [Documentation](/docs) | [Examples](/examples) | [Showcase](/docs/showcase.md) | [Discord](https://discord.gg/ZjZadyC7PK)
@@ -138,15 +138,15 @@
 - [x] [C Code (Clang)](tinygrad/runtime/ops_clang.py)
 - [x] [LLVM](tinygrad/runtime/ops_llvm.py)
 - [x] [METAL](tinygrad/runtime/ops_metal.py)
 - [x] [CUDA](tinygrad/runtime/ops_cuda.py)
 - [x] [HSA](tinygrad/runtime/ops_hsa.py)
 
 And it is easy to add more! Your accelerator of choice only needs to support a total of ~25 low level ops.
-More information can be found in the [documentation for adding new accelerators](/docs-legacy/adding_new_accelerators.md).
+More information can be found in the [documentation for adding new accelerators](/docs/adding_new_accelerators.md).
 
 ## Installation
 
 The current recommended way to install tinygrad is from source.
 
 ### From source
```

### Comparing `tinygrad_tools-0.8.1/tinygrad_tools.egg-info/SOURCES.txt` & `tinygrad_tools-0.8.2/tinygrad_tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -48,64 +48,63 @@
 test/test_to_numpy.py
 test/test_uop_graph.py
 test/test_uops.py
 test/test_uops_stats.py
 test/test_winograd.py
 test/test_zero_copy.py
 tinygrad/__init__.py
-tinygrad/buffer.py
 tinygrad/device.py
 tinygrad/dtype.py
 tinygrad/function.py
 tinygrad/helpers.py
 tinygrad/lazy.py
+tinygrad/multi.py
 tinygrad/ops.py
 tinygrad/tensor.py
 tinygrad/codegen/kernel.py
 tinygrad/codegen/linearizer.py
 tinygrad/codegen/uops.py
 tinygrad/engine/__init__.py
+tinygrad/engine/graph.py
 tinygrad/engine/jit.py
 tinygrad/engine/realize.py
 tinygrad/engine/schedule.py
-tinygrad/features/graph.py
-tinygrad/features/image.py
-tinygrad/features/multi.py
-tinygrad/features/search.py
+tinygrad/engine/search.py
 tinygrad/nn/__init__.py
 tinygrad/nn/datasets.py
 tinygrad/nn/optim.py
 tinygrad/nn/state.py
+tinygrad/renderer/__init__.py
 tinygrad/renderer/assembly.py
 tinygrad/renderer/cstyle.py
 tinygrad/renderer/llvmir.py
 tinygrad/runtime/ops_amd.py
 tinygrad/runtime/ops_clang.py
 tinygrad/runtime/ops_cuda.py
 tinygrad/runtime/ops_disk.py
 tinygrad/runtime/ops_gpu.py
 tinygrad/runtime/ops_hsa.py
 tinygrad/runtime/ops_llvm.py
 tinygrad/runtime/ops_metal.py
 tinygrad/runtime/ops_npy.py
 tinygrad/runtime/ops_nv.py
 tinygrad/runtime/ops_python.py
-tinygrad/runtime/ops_rhip.py
 tinygrad/runtime/autogen/amd_gpu.py
 tinygrad/runtime/autogen/comgr.py
 tinygrad/runtime/autogen/cuda.py
 tinygrad/runtime/autogen/hip.py
 tinygrad/runtime/autogen/hsa.py
 tinygrad/runtime/autogen/kfd.py
 tinygrad/runtime/autogen/nv_gpu.py
 tinygrad/runtime/autogen/opencl.py
 tinygrad/runtime/driver/hip_comgr.py
 tinygrad/runtime/driver/hsa.py
 tinygrad/runtime/graph/clang.py
 tinygrad/runtime/graph/cuda.py
+tinygrad/runtime/graph/hcq.py
 tinygrad/runtime/graph/hsa.py
 tinygrad/runtime/graph/metal.py
 tinygrad/shape/shapetracker.py
 tinygrad/shape/symbolic.py
 tinygrad/shape/view.py
 tinygrad_tools.egg-info/PKG-INFO
 tinygrad_tools.egg-info/SOURCES.txt
```

### Comparing `tinygrad_tools-0.8.1/tinygrad_tools.egg-info/requires.txt` & `tinygrad_tools-0.8.2/tinygrad_tools.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 unicorn
 
 [docs]
 mkdocs-material
 mkdocstrings[python]
 markdown-callouts
 markdown-exec[ansi]
+black
 
 [linting]
 pylint
 mypy
 typing-extensions
 pre-commit
 ruff
```

