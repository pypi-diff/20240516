# Comparing `tmp/acetone_nnet-0.2.3.dev3.tar.gz` & `tmp/acetone_nnet-0.2.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.2.3.dev3.tar", last modified: Wed May 15 13:40:43 2024, max compression
+gzip compressed data, was "acetone_nnet-0.2.3.dev4.tar", last modified: Thu May 16 14:43:28 2024, max compression
```

## Comparing `acetone_nnet-0.2.3.dev3.tar` & `acetone_nnet-0.2.3.dev4.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.114323 acetone_nnet-0.2.3.dev3/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.3.dev3/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev3/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev3/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-15 13:40:43.114323 acetone_nnet-0.2.3.dev3/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.2.3.dev3/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-15 13:40:13.000000 acetone_nnet-0.2.3.dev3/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-15 13:40:43.114323 acetone_nnet-0.2.3.dev3/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.092322 acetone_nnet-0.2.3.dev3/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.096323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1801 2024-05-13 12:52:48.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.097323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-15 12:06:29.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.098322 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-15 06:49:54.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4946 2024-05-15 06:49:14.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.100323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2874 2024-05-15 07:11:48.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3371 2024-05-15 07:10:42.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.102323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1708 2024-05-15 08:12:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5004 2024-05-15 08:12:08.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1713 2024-05-15 08:12:54.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1724 2024-05-15 08:13:23.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1723 2024-05-15 08:13:39.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4095 2024-05-15 07:08:03.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.103323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3891 2024-05-15 08:07:41.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-05-15 08:09:29.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3063 2024-05-15 07:07:25.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4691 2024-05-15 07:06:26.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2401 2024-05-15 07:05:22.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4046 2024-05-15 07:04:47.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8308 2024-05-15 07:02:42.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2313 2024-05-15 06:57:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3290 2024-05-15 06:56:35.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.104323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2705 2024-05-15 08:01:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.104323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5096 2024-05-15 07:56:21.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.105323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10875 2024-05-15 07:49:14.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6712 2024-05-15 07:39:10.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5193 2024-05-15 07:37:13.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2193 2024-05-15 06:51:30.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    27890 2024-05-15 13:39:40.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.105323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.105323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18659 2024-05-15 06:28:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.106323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14558 2024-05-14 15:18:40.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.106323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.106323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    31813 2024-05-14 15:14:48.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.107323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.108323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.109323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.111323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.111323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-05-13 08:47:21.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-05-13 08:47:14.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-05-13 13:12:23.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-05-13 08:47:28.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.112323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.113323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.113323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.114323 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1634 2024-05-15 13:39:16.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-15 13:40:43.114323 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-15 13:40:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6926 2024-05-15 13:40:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-15 13:40:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-15 13:40:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-15 13:40:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-15 13:40:43.000000 acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.294291 acetone_nnet-0.2.3.dev4/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.3.dev4/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev4/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3.dev4/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-16 14:43:28.294291 acetone_nnet-0.2.3.dev4/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.2.3.dev4/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-16 14:43:24.000000 acetone_nnet-0.2.3.dev4/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-16 14:43:28.294291 acetone_nnet-0.2.3.dev4/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.263291 acetone_nnet-0.2.3.dev4/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.269291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1801 2024-05-13 12:52:48.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.270290 acetone_nnet-0.2.3.dev4/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-15 12:06:29.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.271291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4946 2024-05-15 06:49:14.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.274291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3281 2024-05-16 12:23:11.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4494 2024-05-16 12:12:33.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.276291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1708 2024-05-15 08:12:43.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6103 2024-05-16 14:22:43.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1713 2024-05-15 08:12:54.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1724 2024-05-15 08:13:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1723 2024-05-15 08:13:39.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5069 2024-05-16 14:03:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.277291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5680 2024-05-16 14:40:47.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3541 2024-05-16 11:41:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4691 2024-05-15 07:06:26.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2859 2024-05-16 11:46:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-05-16 11:34:22.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     9683 2024-05-16 08:45:22.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2934 2024-05-16 08:03:06.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3861 2024-05-16 07:57:35.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.278291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3503 2024-05-16 13:28:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.279291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6129 2024-05-16 14:39:59.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.280291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    12486 2024-05-16 12:52:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6895 2024-05-16 12:47:31.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5476 2024-05-16 12:48:31.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2359 2024-05-16 08:00:32.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29244 2024-05-16 14:36:20.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.280291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.281291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18659 2024-05-15 06:28:43.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.281291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14558 2024-05-14 15:18:40.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.282291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.282291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    32109 2024-05-16 13:20:29.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.282291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.284291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.287291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.289291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.290291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-05-13 08:47:21.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-05-13 08:47:14.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-05-13 13:12:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-05-13 08:47:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.291291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.292291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.292291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.293291 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-16 14:43:28.293291 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6926 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-16 14:43:28.000000 acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.2.3.dev3/AUTHORS.md` & `acetone_nnet-0.2.3.dev4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/COPYING` & `acetone_nnet-0.2.3.dev4/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/LICENSE` & `acetone_nnet-0.2.3.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/PKG-INFO` & `acetone_nnet-0.2.3.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.3.dev3
+Version: 0.2.3.dev4
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.2.3.dev3/README.md` & `acetone_nnet-0.2.3.dev4/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/pyproject.toml` & `acetone_nnet-0.2.3.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.2.3.dev3"
+version = "0.2.3.dev4"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,34 @@
 from ..Layer import Layer
 from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 class Add_Bias(Layer):
 
-    def __init__(self, idx:int, size:int, biases:int, activation_function:ActivationFunctions):
+    def __init__(self, idx:int, size:int, biases:np.ndarray, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Add_Biass'
-        self.biases = np.asarray(biases)
+        self.biases = biases
         self.nb_biases = self.count_elements_array(self.biases)
         self.activation_function = activation_function
+
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.biases) == np.ndarray
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert  len(self.biases.shape) == 1 and self.biases.shape[0] == self.size
     
     #Go through all the indices and do the operation
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str#if the value is in a road or saved eslewhere
 
         mustach_hash = {}
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,62 +14,62 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from ..Layer import Layer
-from ..activation_functions import ActivationFunctions
+from ...Layer import Layer
+from ...activation_functions import ActivationFunctions
 import numpy as np
-import pystache
+from abc import abstractmethod
 
-class BatchNormalization(Layer):
-
-    def __init__(self, idx:int, size:int, input_shape:list, epsilon:float|int, scale:np.ndarray, biases:np.ndarray, mean:np.ndarray, var:np.ndarray, activation_function:ActivationFunctions):
+#The Pad Layers
+#Pad alongside each dimmensions
+#attribut: the mode of padding required
+#input: a tensor to be padded, the desired pads, the value of teh constant if mode == constant
+#output:the resized tensor
+######################### cf https://onnx.ai/onnx/operators/onnx__Pad.html for the doc
+class Pad(Layer):
+    
+    def __init__(self, idx:int, size:int, pads:np.ndarray, constant_value:float, axes:np.ndarray|list, input_shape:list, activation_function:ActivationFunctions):
         super().__init__()
         self.idx = idx
         self.size = size
-        self.name = 'BatchNormalization'
-        self.output_channels = input_shape[1]
-        self.output_height = input_shape[2]
-        self.output_width = input_shape[3]
-        self.epsilon = epsilon
-        self.scale = scale
-        self.mean = mean
-        self.var = var
-        self.biases = biases
-        self.nb_biases = self.count_elements_array(self.biases)
-
+        self.pads = pads
+        self.constant_value = constant_value
+        self.axes = axes
+        self.name = 'Pad'
+        self.input_shape = input_shape
+        self.output_channels = input_shape[1] + pads[1] + pads[5]
+        self.output_height = input_shape[2] + pads[2] + pads[6]
+        self.output_width = input_shape[3] + pads[3] + pads[7]
+        self.mode = ''
         self.activation_function = activation_function
 
-    def generate_inference_code_layer(self):
-        #Variable indicating under which name the input tensor is
-        output_str = self.previous_layer[0].output_str
-
-        mustach_hash = {}
-
-        mustach_hash['name'] = self.name
-        mustach_hash['idx'] = "{:02d}".format(self.idx)
-        mustach_hash['comment'] = self.activation_function.comment
-        mustach_hash['output_str'] = output_str
-        mustach_hash['path'] = self.path
-        
-        if(self.activation_function.name != 'linear'):
-            mustach_hash['activation_function'] = self.activation_function.write_activation_str('output_'+str(self.path)+'[k + '+str(self.output_height*self.output_width)+'*f]')
-
-        mustach_hash['input_channels'] = self.output_channels
-        mustach_hash['channel_size'] = self.output_height*self.output_width
-        mustach_hash['epsilon'] = self.epsilon
-
-        with open(self.template_path+'layers/template_BatchNormalization.c.tpl','r') as template_file:
-            template = template_file.read()
-        template_file.close()
-
-        return pystache.render(template, mustach_hash)
+        ####### Checking the instantiation#######
 
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert all(type(pad) == int for pad in self.pads)
+        assert type(self.constant_value) == float or type(self.constant_value) == int
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert all(type(shape) == int for shape in self.input_shape)
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert all(0 <= axe and axe < 4 for axe in self.axes)
+    
     def forward_path_layer(self, input:np.ndarray):
-        input = np.reshape(input, (self.output_channels, self.output_height, self.output_width))
-        output = []
-        for i in range(self.output_channels):
-            output.append((input[i] - self.mean[i])/np.sqrt(self.var[i] + self.epsilon)*self.scale[i] + self.biases[i])
-        return np.array(output)
+        input = input.reshape(self.input_shape[1], self.input_shape[2], self.input_shape[3])
+        nb_dim = len(self.pads)//2
+        pad_width = [(self.pads[i],self.pads[i+nb_dim]) for i in range(1,nb_dim)] #Constructing the pads accordingly to the numpy nomenclature
+        return self.activation_function.compute(np.pad(input,pad_width=pad_width,mode=self.mode,constant_values=self.constant_value,))
+    
+    @abstractmethod
+    def generate_inference_code_layer(self):
+        pass
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,102 +14,77 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from ...Layer import Layer
-from ...activation_functions import ActivationFunctions
+from .Pad import Pad
 
-from abc import abstractmethod
 import pystache
-import numpy as np
 
-#The class of the Layers which compute operation with broadcast numpy style
-#attribut: none
-#input: a list of tensor
-#output: the resultant tensor
-class Broadcast(Layer):
-    def __init__(self, idx:int, size:int, input_shapes:list, output_shape:list, activation_function:ActivationFunctions, constant:np.ndarray|float|int|None=None):
-        super().__init__()
-        self.idx = idx
-        self.size = size
-        self.name = ''
-        self.input_shapes = input_shapes
+#The Wrap mode of the Pad layers
+#Pads with the wrap of the vector along the axis. 
+#The first values are used to pad the end and the end values are used to pad the beginning.
+class Wrap_pad(Pad):
+    
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.mode = 'wrap'
+    
+    def write_padding(self):
+        mustach_hash = {}
+
+        mustach_hash['pads_front'] = self.pads[1]
+        mustach_hash['pads_top'] = self.pads[2]
+        mustach_hash['pads_left'] = self.pads[3]
+        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
+        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
+        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
+        mustach_hash['input_channels'] = self.input_shape[1]
+        mustach_hash['input_width'] = self.input_shape[3]
+        mustach_hash['input_height'] = self.input_shape[2]
         
-        self.output_height = output_shape[2]
-        self.output_width = output_shape[3]
-        self.output_channels = output_shape[1]
-        self.specific_operator = ''
-        self.activation_function = activation_function
-        self.constant = constant
-        if(constant is not None):
-            self.constant_size = self.count_elements_array(self.constant)
+        with open(self.template_path+'layers/Pad/template_Wrap_Pad.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template, mustach_hash)
+    
 
-    #Go through all the indices and do the operation
     def generate_inference_code_layer(self):
+        
+        output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
-        mustach_hash['road'] = self.path
         mustach_hash['size'] = self.size
+        mustach_hash['output_str'] = output_str
+        mustach_hash['road'] = self.path
 
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[k]')
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
 
         mustach_hash['output_channels'] = self.output_channels
         mustach_hash['output_height'] = self.output_height
         mustach_hash['output_width'] = self.output_width
+        mustach_hash['pads_front'] = self.pads[1]
+        mustach_hash['pads_top'] = self.pads[2]
+        mustach_hash['pads_left'] = self.pads[3]
+        mustach_hash['input_width'] = self.input_shape[3]
+        mustach_hash['input_height'] = self.input_shape[2]
 
-        start = 0
-        if(self.name == 'Maximum'):
-            start = 1
-            mustach_hash['output_str0'] = self.previous_layer[0].output_str
-            mustach_hash['input_width0'] = self.input_shapes[0][3]
-            mustach_hash['input_height0'] = self.input_shapes[0][2]
-            mustach_hash['input_channels0'] = self.input_shapes[0][1]
-            mustach_hash['max'] = True
-        elif(self.name == 'Minimum'):
-            start = 1
-            mustach_hash['output_str0'] = self.previous_layer[0].output_str
-            mustach_hash['input_width0'] = self.input_shapes[0][3]
-            mustach_hash['input_height0'] = self.input_shapes[0][2]
-            mustach_hash['input_channels0'] = self.input_shapes[0][1]
-            mustach_hash['min'] = True
-        elif(self.name == 'Average'):
-            mustach_hash['Average'] = True
-            mustach_hash['prev_size'] = len(self.previous_layer)
-        else:
-            mustach_hash['other'] = True
-        
-        mustach_hash['broadcast'] = []
-        for k in range(start, len(self.previous_layer)):
-            previous_dict = {}
-            previous_dict['output_str'] = self.previous_layer[k].output_str
-            previous_dict['input_width'] = self.input_shapes[k][3]
-            previous_dict['input_height'] = self.input_shapes[k][2]
-            previous_dict['input_channels'] = self.input_shapes[k][1]
-            if(k != len(self.previous_layer) -1):
-                previous_dict['operator'] = self.specific_operator
-            mustach_hash['broadcast'].append(previous_dict)
-        
-        if(self.constant is not None):
-            constant_dict = {}
-            constant_dict['cst_width'] = self.input_shapes[-1][3]
-            constant_dict['cst_height'] = self.input_shapes[-1][2]
-            constant_dict['cst_channels'] = self.input_shapes[-1][1]
-            constant_dict['operator'] = self.specific_operator
-            mustach_hash['constant'] = [constant_dict]
+        mustach_hash['change_indice'] = self.write_padding()
 
+        if(self.activation_function.name == 'linear'):
+            mustach_hash['linear'] = True
         
-        with open(self.template_path+'layers/template_Broadcast.c.tpl','r') as template_file:
+        if(self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
+
+        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
-        return pystache.render(template, mustach_hash)
-
-    @abstractmethod
-    def forward_path_layer(self, inputs:np.ndarray):
-        pass
+        return pystache.render(template, mustach_hash)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,33 @@
         self.size = size
         self.input_shapes = input_shapes
         self.name = 'Concatenate'
         self.axis = axis
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
         self.output_channels = output_shape[1]
-        self.activation_function = activation_function            
+        self.activation_function = activation_function
+
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert all((type(shape) == int for shape in input_shape) for input_shape in self.input_shapes)
+        assert self.axis in [1,2,3]
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert self.axis == 1 or all(self.output_channels == input_shape[1] for input_shape in self.input_shapes)
+        assert self.axis == 2 or all(self.output_height== input_shape[2] for input_shape in self.input_shapes)
+        assert self.axis == 3 or all(self.output_width == input_shape[3] for input_shape in self.input_shapes)
     
     def generate_inference_code_layer(self):
         borne_sup = 0
         borne_inf = 0
 
         mustach_hash = {}
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,69 +13,73 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
+from .Pad import Pad
 
-from ...Layer import Layer
-from ...activation_functions import ActivationFunctions
-import numpy as np
-from abc import abstractmethod
+import pystache
 
-class Conv2D(Layer):
+#The Edge mode of the Pad layers
+#Pads with the edge values of array.
+class Edge_pad(Pad):
     
-    def __init__(self, idx:int, conv_algorithm:str, size:int, padding:str|list, strides:int, kernel_h:int, kernel_w:int, dilation_rate:int, nb_filters:int, input_shape:list, output_shape:list, weights:np.ndarray, biases:np.ndarray, activation_function:ActivationFunctions):
-        super().__init__()
-        self.conv_algorithm = conv_algorithm
-        self.idx = idx
-        self.size = size
-        self.name = 'Conv2D'
-        self.padding = padding
-        self.strides = strides
-        self.kernel_h = kernel_h
-        self.kernel_w = kernel_w
-        self.dilation_rate = dilation_rate
-        self.nb_filters = nb_filters
-    
-        self.input_channels = input_shape[1]
-        self.input_height = input_shape[2]
-        self.input_width = input_shape[3]
-        self.output_height = output_shape[2]
-        self.output_width = output_shape[3]
-
-        self.input_shape = [self.input_channels, self.input_height, self.input_width]
-        self.output_channels = self.nb_filters
-
-        self.weights = weights
-        self.biases = biases
-        self.activation_function = activation_function
-        self.local_var = 'sum'
-
-        self.nb_weights = self.count_elements_array(self.weights)
-        self.nb_biases = self.count_elements_array(self.biases)
-        self.pad_right, self.pad_left, self.pad_bottom, self.pad_top = self.compute_padding(self.padding,self.input_height, self.input_width, self.kernel_h, self.kernel_w, self.strides, self.dilation_rate)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.mode = 'edge'
+
+    def write_padding(self):
+        mustach_hash = {}
+
+        mustach_hash['pads_front'] = self.pads[1]
+        mustach_hash['pads_top'] = self.pads[2]
+        mustach_hash['pads_left'] = self.pads[3]
+        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
+        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
+        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
+
+        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template, mustach_hash)
     
-    @abstractmethod
+
     def generate_inference_code_layer(self):
-        pass
+        
+        output_str = self.previous_layer[0].output_str
 
-    def forward_path_layer(self, input:np.ndarray):
-        # Conv for chw
-        input = input.reshape(self.input_channels, self.input_height, self.input_width)
+        mustach_hash = {}
+
+        mustach_hash['name'] = self.name
+        mustach_hash['idx'] = "{:02d}".format(self.idx)
+        mustach_hash['comment'] = self.activation_function.comment
+        mustach_hash['size'] = self.size
+        mustach_hash['output_str'] = output_str
+        mustach_hash['road'] = self.path
+
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
+
+        mustach_hash['output_channels'] = self.output_channels
+        mustach_hash['output_height'] = self.output_height
+        mustach_hash['output_width'] = self.output_width
+        mustach_hash['pads_front'] = self.pads[1]
+        mustach_hash['pads_top'] = self.pads[2]
+        mustach_hash['pads_left'] = self.pads[3]
+        mustach_hash['input_width'] = self.input_shape[3]
+        mustach_hash['input_height'] = self.input_shape[2]
+
+        mustach_hash['change_indice'] = self.write_padding()
+
+        if(self.activation_function.name == 'linear'):
+            mustach_hash['linear'] = True
         
-        output = np.zeros((self.nb_filters, self.output_height, self.output_width))
-        print(self.weights.shape)
+        if(self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
+
+        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
 
-        if self.pad_right and self.pad_left and self.pad_top and self.pad_bottom:
-            input_padded = np.zeros((self.input_channels, self.input_height + self.pad_top + self.pad_bottom, self.input_width + self.pad_left + self.pad_right))
-            input_padded[:, self.pad_top:-self.pad_bottom, self.pad_left:-self.pad_right] = input
-        else:
-            input_padded = input
-            
-        for f in range(self.nb_filters):
-            for i in range(self.output_height):
-                for j in range(self.output_width):
-                        output[f,i,j]=np.sum(input_padded[:, i*self.strides:i*self.strides+self.kernel_h, j*self.strides:j*self.strides+self.kernel_w] 
-                                            * self.weights[:,:,:,f]) + self.biases[f]
-        return self.activation_function.compute(output)
+        return pystache.render(template, mustach_hash)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,24 +22,14 @@
 
 import pystache
 
 class Conv2D_std_gemm(Conv2D_gemm):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-
-        self.patches_height = self.input_channels * self.kernel_h * self.kernel_w
-        self.patches_width = self.output_height * self.output_width
-        self.patches_size = self.patches_height * self.patches_width
-
-        self.conv_algorithm = self.conv_algorithm[-7:]
-        self.algo_gemm_mapping = { 'gemm_nn' : self.write_gemm_nn,
-                                   'gemm_nt' : self.write_gemm_nt,
-                                   'gemm_tn' : self.write_gemm_tn,
-                                   'gemm_tt' : self.write_gemm_tt}
         
         self.algo_patch_building_mapping = { 'gemm_nn' : self.write_im2col,
                                              'gemm_nt' : self.write_im2row,
                                              'gemm_tn' : self.write_im2col,
                                              'gemm_tt' : self.write_im2row}
 
     def write_im2col(self):
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,27 @@
         self.biases = biases
         self.activation_function = activation_function
         self.local_var = 'dotproduct'
         
         self.nb_weights = self.count_elements_array(self.weights)
         self.nb_biases = self.count_elements_array(self.biases)
 
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.weights) == np.ndarray
+        assert type(self.biases) == np.ndarray
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert self.size == self.weights.shape[-1]
+        assert self.size == self.biases.shape[0]
+
         
     def generate_inference_code_layer(self):
         #Variable indicating under which name the input tensor is
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,25 @@
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shape = input_shape
         self.data_format = data_format
         self.name = 'Flatten'
 
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert all(type(shape) == int for shape in self.input_shape)
+        assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
+
+        ### Checking value consistency ###
+        assert self.size == self.input_shape[1]*self.input_shape[2]*self.input_shape[3]
+
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
         if(self.data_format == 'channels_last'):
             mustach_hash['channels_last'] = True
             mustach_hash['input_channels'] = self.input_shape[1]
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,28 +25,47 @@
 
 #extract a list of subtensor from a given tensor
 #attribut: axis alongside of which the submatrix will be extracted (if the desired submatrix must have the height, width or channels of the parent tensor)
 #input: a tensor
 #output: a list of tensor
 class Gather(Layer):
     
-    def __init__(self, idx:int, size:int, axis:int,  indices:list, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
+    def __init__(self, idx:int, size:int, axis:int,  indices:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Gather'
         self.indices = indices
         self.axis = axis
-        self.input_channels = input_shape[1]
+        self.output_channels = input_shape[1]
         self.input_height = input_shape[2]
         self.input_width = input_shape[3]
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
         self.activation_function = activation_function
+
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.axis) == int
+        assert type(self.indices) == np.ndarray
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert type(self.input_height) == int
+        assert type(self.input_width) == int
+        assert isinstance(self.activation_function,ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert axis in [1,2,3]
+        assert all(indice >= 0 and indice < input_shape[axis] for indice in self.indices.flatten())
         
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
@@ -64,19 +83,19 @@
 
         if(self.axis == 1):
             mustach_hash['channels'] = True
             mustach_hash['output_height'] = self.output_height
             mustach_hash['output_width'] = self.output_width
         elif(self.axis == 2):
             mustach_hash['heights'] = True
-            mustach_hash['output_channels'] = self.input_channels
+            mustach_hash['output_channels'] = self.output_channels
             mustach_hash['output_width'] = self.output_width
         elif(self.axis == 3):
             mustach_hash['widths'] = True
-            mustach_hash['output_channels'] = self.input_channels
+            mustach_hash['output_channels'] = self.output_channels
             mustach_hash['output_height'] = self.output_height
 
         if(self.activation_function.name == 'linear'):
             mustach_hash['linear'] = True
 
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tensor_temp[position]',self.idx,'position')
@@ -84,9 +103,9 @@
         with open(self.template_path+'layers/template_Gather.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
     def forward_path_layer(self, input:np.ndarray):
-        input = input.reshape(self.input_channels,self.input_height,self.input_width)
+        input = input.reshape(self.output_channels,self.input_height,self.input_width)
         return np.take(input, indices=self.indices, axis=self.axis-1)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import pystache
 
 #The layer which compute the general matrix multiplication
 #input: weight tesnsor W and bias tensor B, input tensor T. The tensor must be of 2D
 #data: alpha and beta constante used in the operation, transpo un tuple saying if the tensor T or W must be transposed before the operation
 #output: The result of the operation """alpha*T*W + beta*B"""
 class Gemm(Layer):
-    def __init__(self, idx:int, size:int, alpha:float|int, beta:float|int, transA:bool, transB:bool, weights:np.ndarray, bias:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
+    def __init__(self, idx:int, size:int, alpha:float|int, beta:float|int, transA:bool|int, transB:bool|int, weights:np.ndarray, bias:np.ndarray, input_shape:list, output_shape:list, activation_function:ActivationFunctions):
         super().__init__() 
         self.name = 'Gemm'
         self.idx = idx
         self.size = size
         
         self.alpha = [alpha]
         self.beta =  [beta]
@@ -41,29 +41,49 @@
                              (0,1):self.write_gemm_nt,
                              (1,1):self.write_gemm_tt,
                              (1,0):self.write_gemm_tn}
         
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
         if(input_shape):
-            if(transA):
-                self.input_height = input_shape[3]
-                self.input_width = input_shape[2]
-            else:
-                self.input_height = input_shape[2]
-                self.input_width = input_shape[3]
+            self.input_height = input_shape[2]
+            self.input_width = input_shape[3]
         else:
             self.input_height = 1
             self.input_width = 1
         
         self.weights = weights
         self.biases = bias
         self.activation_function = activation_function
         self.nb_weights = self.count_elements_array(self.weights)
         self.nb_biases = self.count_elements_array(self.biases)
+
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.alpha) == float or type(self.alpha) == int
+        assert type(self.beta) == float or type(self.beta) == int
+        assert type(self.transpo) == tuple[int] or type(self.transpo) == tuple[bool]
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert type(self.input_height) == int
+        assert type(self.input_width) == int
+        assert type(self.weights) == np.ndarray
+        assert type(self.biases) == np.ndarray
+        assert isinstance(self.activation_function,ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert self.size == self.output_height*self.output_width
+        assert self.weights.shape[2 + self.transpo[1]] == self.input_height if self.transpo[0] else self.input_width
+        assert self.output_height == self.input_width if self.transpo[0] else self.input_height
+        assert self.output_width == self.weights.shape[3 - self.transpo[1]]
+        assert (self.biases.shape[0] == 1 or self.biases.shape[0] == self.output_height) and (self.biases.shape[1] == 1 or self.biases.shape[1] == self.output_width)
+
         
     #The various ways to compute the operation: 
     
     #None of the tensor ar transposed
     def write_gemm_nn(self, m, n, k, A, B):
 
         mustach_hash = {}
@@ -165,18 +185,17 @@
         with open(self.template_path+'layers/Gemm/template_gemm_tt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self, input:np.ndarray):
+        input = input.reshape(self.input_height,self.input_width)
         if(self.transpo[0]):
-            input = input.reshape(self.input_width,self.input_height).transpose()
-        else:
-            input = input.reshape(self.input_height,self.input_width)
+            input = input.transpose()
             
         if(self.transpo[1]):
             self.weights = self.weights.transpose()
         
         return self.activation_function.compute(self.alpha * np.dot(input,self.weights) + self.beta * self.biases)
     
     def generate_inference_code_layer(self):
@@ -186,14 +205,17 @@
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['size'] = self.size
         mustach_hash['road'] = self.path
 
         mustach_hash['patches_size'] = self.output_width*self.output_height
-        mustach_hash['gemm_code'] = self.algo_gemm_mapping[self.transpo](self.output_height, self.output_width, self.input_width, 'weights_' + self.name + '_' + str("{:02d}".format(self.idx)), self.previous_layer[0].output_str)
+        if self.transpo[0]:
+            mustach_hash['gemm_code'] = self.algo_gemm_mapping[self.transpo](self.output_height, self.output_width, self.input_height, 'weights_' + self.name + '_' + str("{:02d}".format(self.idx)), self.previous_layer[0].output_str)
+        else:
+            mustach_hash['gemm_code'] = self.algo_gemm_mapping[self.transpo](self.output_height, self.output_width, self.input_width, 'weights_' + self.name + '_' + str("{:02d}".format(self.idx)), self.previous_layer[0].output_str)
 
         with open(self.template_path+'layers/Gemm/template_Gemm.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,31 +25,46 @@
 class InputLayer(Layer):
 
     def __init__(self, idx:int, size:int, input_shape:list, data_format:str):
        
         super().__init__()
         self.idx = idx
         self.size = size
-        self.input_shape = input_shape
+        self.output_channels = input_shape[1]
+        self.output_height = input_shape[2]
+        self.output_width = input_shape[3]
         self.data_format = data_format
         self.name = 'Input_layer'
 
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert self.data_format == 'channels_last' or self.data_format == 'channels_first'
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['road'] = self.path
 
         if(self.data_format == 'channels_last' and len(self.input_shape) == 4):
             mustach_hash['channels_last'] = True
-            mustach_hash['input_channels'] = self.input_shape[1]
-            mustach_hash['input_height'] = self.input_shape[2]
-            mustach_hash['input_width'] = self.input_shape[3]
+            mustach_hash['input_channels'] = self.output_channels
+            mustach_hash['input_height'] = self.output_height
+            mustach_hash['input_width'] = self.output_width
         else:
             mustach_hash['size'] = self.size
 
 
 
 
         with open(self.template_path+'layers/template_Input_Layer.c.tpl','r') as template_file:
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,27 +21,45 @@
 from ..Layer import Layer
 from ..activation_functions import ActivationFunctions
 import numpy as np
 import pystache
 
 class MatMul(Layer):
 
-    def __init__(self, idx:int, size:int, input_shape:list, weights:list, side:bool, activation_function:ActivationFunctions):
+    def __init__(self, idx:int, size:int, input_shape:list, weights:np.ndarray, side:bool, activation_function:ActivationFunctions):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'MatMul'
-        self.weights = np.asarray(weights)
+        self.weights = weights
         self.activation_function = activation_function
         self.local_var = 'dotproduct'
         self.side = side
         self.input_shape = input_shape
         self.nb_weights = self.count_elements_array(self.weights)
 
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.input_shape) == list[int]
+        assert type(self.weights) == np.ndarray
+        assert type(side) == bool
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+        ### Checking value consistency ###
+        if self.side:
+            assert self.weights.shape[-1] == self.input_shape[-2]
+            assert self.size == self.weights.shape[-2] * self.input_shape[-1]
+        else:
+            assert self.weights.shape[-2] == self.input_shape[-1]
+            assert self.size == self.weights.shape[-1] * self.input_shape[-2]
+
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
@@ -66,13 +84,11 @@
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
     def forward_path_layer(self, input):
         
         input = input.reshape(self.previous_layer[0].size)
-        if (self.side):
-            weights = np.moveaxis(self.weights, 3,0)
-            weights = np.reshape(weights, (weights.shape[1],weights.shape[2],weights.shape[3],weights.shape[0]))
-            return self.activation_function.compute(np.matmul(weights,input))
+        if self.side:
+            return self.activation_function.compute(np.matmul(self.weights,input))
         else:
             return self.activation_function.compute(np.matmul(input,self.weights))
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,37 +13,38 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
+
 from .Pad import Pad
 
 import pystache
 
-#The Edge mode of the Pad layers
-#Pads with the edge values of array.
-class Edge_pad(Pad):
+#The Reflect mode of the Pad layers
+#Pads with the reflection of the vector mirrored on the first and last values of the vector along each axis.
+class Reflect_pad(Pad):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.mode = 'edge'
-
+        self.mode = 'reflect'
+    
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
-        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
-        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
-        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
-
-        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
+        mustach_hash['channels_max'] = self.input_shape[1] - 1
+        mustach_hash['height_max'] = self.input_shape[2] - 1
+        mustach_hash['width_max'] = self.input_shape[3] - 1
+        
+        with open(self.template_path+'layers/Pad/template_Reflect_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,77 +14,84 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from .Pad import Pad
-
 import pystache
+import numpy as np
+from abc import ABC
+from ... import templates
+
+class Normalizer(ABC):
+
+    def __init__(self, input_size:int, output_size:int, mins:list, maxes:list, means:list, ranges:list):
+        self.input_size = input_size
+        self.output_size = output_size
+        self.mins = mins
+        self.maxes = maxes
+        self.means = means
+        self.ranges = ranges
+        self.template_path = templates.__file__[:-11]
+        super().__init__()
+
+    def array_to_str(self, array:list):
+        s = "{"
+        for element in array:
+            s += str(element) + ", "
+        s = s[:-2] + "}"
+        return s
+
+    def write_pre_processing(self):
+        with open(self.template_path+'normalization/template_pre_processing.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template,{'input_size':self.input_size})
 
-#The Wrap mode of the Pad layers
-#Pads with the wrap of the vector along the axis. 
-#The first values are used to pad the end and the end values are used to pad the beginning.
-class Wrap_pad(Pad):
-    
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.mode = 'wrap'
-    
-    def write_padding(self):
-        mustach_hash = {}
 
-        mustach_hash['pads_front'] = self.pads[1]
-        mustach_hash['pads_top'] = self.pads[2]
-        mustach_hash['pads_left'] = self.pads[3]
-        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
-        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
-        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
-        mustach_hash['input_channels'] = self.input_shape[1]
-        mustach_hash['input_width'] = self.input_shape[3]
-        mustach_hash['input_height'] = self.input_shape[2]
-        
-        with open(self.template_path+'layers/Pad/template_Wrap_Pad.c.tpl','r') as template_file:
+    def write_post_processing(self):
+        with open(self.template_path+'normalization/template_post_processing.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template,{'output_size':self.output_size})
+
+    def write_normalization_cst_in_header_file(self):
+        mustach_hash= {}
+
+        mustach_hash['input_size'] = self.input_size
+
+        with open(self.template_path+'normalization/template_normalization_cst_in_header_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
+    def write_normalization_cst_in_globalvars_file(self):
+        mustach_hash= {}
 
-    def generate_inference_code_layer(self):
-        
-        output_str = self.previous_layer[0].output_str
-
-        mustach_hash = {}
-
-        mustach_hash['name'] = self.name
-        mustach_hash['idx'] = "{:02d}".format(self.idx)
-        mustach_hash['comment'] = self.activation_function.comment
-        mustach_hash['size'] = self.size
-        mustach_hash['output_str'] = output_str
-        mustach_hash['road'] = self.path
-
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
-
-        mustach_hash['output_channels'] = self.output_channels
-        mustach_hash['output_height'] = self.output_height
-        mustach_hash['output_width'] = self.output_width
-        mustach_hash['pads_front'] = self.pads[1]
-        mustach_hash['pads_top'] = self.pads[2]
-        mustach_hash['pads_left'] = self.pads[3]
-        mustach_hash['input_width'] = self.input_shape[3]
-        mustach_hash['input_height'] = self.input_shape[2]
-
-        mustach_hash['change_indice'] = self.write_padding()
-
-        if(self.activation_function.name == 'linear'):
-            mustach_hash['linear'] = True
-        
-        if(self.fused_layer):
-            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
+        mustach_hash['input_size'] = self.input_size
+        mustach_hash['input_min'] = self.array_to_str(self.mins)
+        mustach_hash['input_max'] = self.array_to_str(self.maxes)
+        mustach_hash['input_mean'] = self.array_to_str(self.means[:-1])
+        mustach_hash['input_range'] = self.array_to_str(self.ranges[:-1])
+        mustach_hash['output_mean'] = self.means[-1]
+        mustach_hash['output_range'] = self.ranges[-1]
 
-        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
+        with open(self.template_path+'normalization/template_normalization_cst_in_global_var_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
-        return pystache.render(template, mustach_hash)
+        return  pystache.render(template, mustach_hash)
+
+    def pre_processing(self, nn_input:np.ndarray):
+        inputs = nn_input.flatten()
+        for i in range(self.input_size):
+            inputs[i] = (max(self.mins[i],min(self.maxes[i],inputs[i])) - self.means[i]) / self.ranges[i]
+        return np.reshape(inputs, nn_input.shape)
+
+    def post_processing(self, nn_output:np.ndarray):
+        for i in range(len(nn_output)):
+            nn_output[i] = nn_output[i]*self.ranges[-1] + self.means[-1]
+        return nn_output
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,20 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from ...Layer import Layer
 from ...activation_functions import ActivationFunctions
 import numpy as np
+import math
 import pystache
 from abc import abstractmethod
 
 class Pooling2D(Layer):
-    def __init__(self, idx:int, size:int, padding:str|list, strides:int, pool_size:int, input_shape:list, output_shape:list, activation_function:ActivationFunctions, **kwargs):
+    def __init__(self, idx:int, size:int, padding:str|np.ndarray, strides:int, pool_size:int, input_shape:list, output_shape:list, activation_function:ActivationFunctions, **kwargs):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = ''
         self.padding = padding
         self.strides = strides
@@ -39,23 +40,45 @@
         self.input_height = input_shape[2]
         self.input_width = input_shape[3]
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
 
         self.output_channels = self.input_channels
 
-        self.pooling_funtion = ''
+        self.pooling_function = ''
         self.local_var = ''
         self.local_var_2 = ''
         self.output_var = ''
 
         self.activation_function = activation_function
 
         self.pad_right, self.pad_left, self.pad_bottom, self.pad_top = self.compute_padding(self.padding,self.input_height, self.input_width, self.pool_size,self.pool_size, self.strides)
 
+
+    ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.padding) == str or type(self.padding) == np.ndarray
+        assert type(self.strides) == int
+        assert type(self.pool_size) == int
+        assert type(self.input_channels) == int
+        assert type(self.input_height) == int
+        assert type(self.input_width) == int
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert self.output_height == math.ceil((self.input_height - self.pool_size)/self.strides) + 1
+        assert self.output_width == math.ceil((self.input_width - self.pool_size)/self.strides) + 1
+    
     @abstractmethod    
     def specific_function(self, index:str, input_of_layer:str):
         pass
 
     @abstractmethod    
     def update_local_vars(self):
         pass
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 #input: a tensor to be resized, the desired size or a scale to multiply the size by, the region of interest
 #output:the resized tensor
 ##############  https://onnx.ai/onnx/operators/onnx__Resize.html for more informations
 #The strategie is always to go throught the elements, find the coordinate in the original tensor 
 # and apply a transformation to the value in the original tensor to find the value to enter in the new tensor
 class Resize(Layer):
     
-    def __init__(self, idx:int, size:int, input_shape:list, activation_function:ActivationFunctions, axes:list=[], coordinate_transformation_mode:str='half_pixel', exclude_outside:int=0,
-                 keep_aspect_ratio_policy:str='stretch', boolean_resize:None|bool=None, target_size:list=[], roi:list=[], extrapolation_value:float=0, 
+    def __init__(self, idx:int, size:int, input_shape:list, activation_function:ActivationFunctions, axes:np.ndarray|list=[], coordinate_transformation_mode:str='half_pixel', exclude_outside:int=0,
+                 keep_aspect_ratio_policy:str='stretch', boolean_resize:None|bool=None, target_size:np.ndarray|list=[], roi:np.ndarray|list=[], extrapolation_value:float|int=0., 
                  nearest_mode:str='round_prefer_floor', cubic_coeff_a:float=-0.75):
         super().__init__()
         self.idx = idx
         if(type(nearest_mode) == bytes):
             self.nearest_mode = str(nearest_mode)[2:-1]
         else: 
             self.nearest_mode = nearest_mode
@@ -69,28 +69,58 @@
                                                                 "align_corners":self.align_corners_implem,
                                                                 "asymmetric":self.asymmetric_implem,
                                                                 "tf_crop_and_resize":self.tf_crop_and_resize_implem}
         
         self.input_channels = input_shape[1]
         self.input_height = input_shape[2]
         self.input_width = input_shape[3]
-        self.scale = [1,0,0,0]
+        self.scale = [1.,0.,0.,0.]
         if (boolean_resize):
             self.scale = target_size
             self.output_channels = int(self.input_channels*target_size[1]) #should be equal to input_channels
             self.output_height = int(self.input_height*target_size[2])
             self.output_width = int(self.input_width*target_size[3])
         else:
             self.output_channels = target_size[1] #should be equal to input_channels
             self.output_height = target_size[2]
             self.output_width = target_size[3]
             self.scale[1] = self.output_channels / self.input_channels #should be 1
             self.scale[2] = self.output_height / self.input_height
             self.scale[3] = self.output_width / self.input_width
-            
+
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert type(self.input_channels) == int
+        assert type(self.input_height) == int
+        assert type(self.input_width) == int
+        assert type(self.coordinate_transformation_mode) == str
+        assert type(axes) == np.ndarray or type(axes) == list
+        assert type(self.exclude_outside) == int
+        assert type(self.keep_aspect_ratio_policy) == str
+        assert type(self.roi) == np.ndarray or type(self.roi) == list
+        assert type(self.extrapolation_value) == float or type(self.extrapolation_value) == int
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert self.coordinate_transformation_mode in ['half_pixel','half_pixel_symmetric','pytorch_half_pixel','align_corners','asymmetric','tf_crop_and_resize']
+        assert self.keep_aspect_ratio_policy in ['stretch','not_larger','not_smaller']
+        assert self.exclude_outside in [0,1]
+        assert all(axe >=0 and axe < 4 for axe in self.axes)
+        if self.roi:
+            assert len(self.roi) == 2*len(self.axes) if self.axes else len(self.roi) == 8
+            assert all(0 <= indice and indice <= 1 for indice in self.roi)
+        assert all(0 < coeff for coeff in self.scale)
+        
+
     @abstractmethod
     def forward_path_layer(self, input:np.ndarray):
         pass
     
     @abstractmethod
     def generate_inference_code_layer(self):
         pass
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 class ResizeCubic(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode = 'cubic'
         self.template_dict = {'1D':self.template_path+'layers/Resize/template_ResizeCubic1D.c.tpl',
                               '2D':self.template_path+'layers/Resize/template_ResizeCubic2D.c.tpl'}
+        
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.cubic_coeff_a) == float or type(self.cubic_coeff_a) == int
     
     def cubic_interpolation_1D(self, input:np.ndarray, f:int, x:int, y:int, s:float):
         col_index = max(0,min(self.input_width-1,y))
         f_1 = input[f,max(0,min(self.input_height-1,x-1)),col_index]
         f0 = input[f,max(0,min(self.input_height-1,x)),col_index]
         f1 = input[f,max(0,min(self.input_height-1,x+1)),col_index]
         f2 = input[f,max(0,min(self.input_height-1,x+2)),col_index]
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,22 @@
                                      "floor":self.floor,
                                      "ceil":self.ceil}
         
         self.nearest_mode_implem_mapping = {"round_prefer_floor":self.round_prefer_floor_implem,
                                             "round_prefer_ceil":self.round_prefer_ceil_implem,
                                             "floor":math.floor,
                                             "ceil":math.ceil}
+        
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.nearest_mode) == str
+
+        ### Checking value consistency ###
+        assert self.nearest_mode in ['round_prefer_floor','round_prefer_ceil','floor','ceil']
     
     #Defining the several method to chose the nearest
     def floor(self, x:str, y:str):
         return x+' = floor('+y+');'
     
     def ceil(self, x:str, y:str):
         return x+' = ceil('+y+');'
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,20 @@
     def __init__(self, idx:int, size:int):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Softmax'
 
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,19 @@
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
 )
 
 class CodeGenerator(ABC):
 
-    def __init__(self, file:str|onnx.ModelProto|Functional|Sequential, test_dataset_file:str=None, function_name:str='inference', nb_tests:int|str=None, conv_algorithm:str='std_gemm_nn', normalize:bool|str=False, debug_mode:str|None=None, debug_target:list|None=None,**kwargs):
+    def __init__(self, file:str|onnx.ModelProto|Functional|Sequential, test_dataset:str|np.ndarray|None=None, function_name:str='inference', nb_tests:int|str=None, conv_algorithm:str='std_gemm_nn', normalize:bool|str=False, debug_mode:str|None=None, debug_target:list|None=None,**kwargs):
 
         self.file = file
-        self.test_dataset_file = test_dataset_file
         self.function_name = function_name
-        self.nb_tests = nb_tests
+        self.nb_tests = int(nb_tests)
         self.conv_algorithm = conv_algorithm
         self.normalize = bool(normalize)
         self.template_path = templates.__file__[:-11]
 
         if (not self.normalize):
             l, dtype, dtype_py, data_format, maxpath, dict_cst = parser(self.file, self.conv_algorithm)
         elif(self.normalize):
@@ -60,29 +59,55 @@
         self.layers = l
         self.data_type = dtype
         self.data_type_py = dtype_py
         self.maxpath = maxpath
         self.data_format = data_format
         self.dict_cst = dict_cst
 
-        if test_dataset_file:
+        if type(test_dataset) == str:
+            self.test_dataset_file = test_dataset
             ds = self.load_test_dataset()
             self.test_dataset = ds
+        elif type(test_dataset) == np.ndarray:
+            self.test_dataset = test_dataset
         else:
             print("creating random dataset")
             ds = self.create_test_dataset()
             self.test_dataset = ds
 
         self.files_to_gen = ['inference.c', 'inference.h', 'global_vars.c', 'main.c', 'Makefile', 'test_dataset.h', 'test_dataset.c']
         
         ##### Debug Mode #####
         self.debug_mode = debug_mode
         if self.debug_mode:
             self.debug_target = self.load_debug_target(debug_mode, debug_target)
         ##### Debug Mode #####
+            
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.file) == str or type(self.file) == onnx.ModelProto or type(self.file) == Functional or type(self.file) == Sequential
+        assert type(test_dataset) == str or type(test_dataset) == np.ndarray or type(test_dataset) == None
+        assert type(self.test_dataset) == np.ndarray
+        assert type(self.function_name) == str
+        assert type(self.conv_algorithm) == str
+        assert type(self.debug_mode) == None or type(self.debug_mode) == str
+        if self.debug_mode:
+            assert type(self.debug_target) == list
+
+        ### Checking value consistency ###
+        assert self.conv_algorithm in ['6loops',
+                                       'indirect_gemm_nn','indirect_gemm_tn','indirect_gemm_nt','indirect_gemm_tt',
+                                       'std_gemm_nn','std_gemm_tn','std_gemm_nt','std_gemm_']
+        ##### Debug Mode #####
+        if self.debug_mode:
+            assert self.debug_mode in ['keras','onnx']
+            assert len(self.debug_target) <= len(self.layers)
+            assert all(target <= len(self.layers) for target in self.debug_target)
+        ##### Debug Mode #####
     
     def load_debug_target(self, debug_mode:str|None, debug_target:list|None):
         if debug_target == None:
             return debug_target
         
         else:
             targets = []
@@ -91,15 +116,15 @@
                     targets[-1] = layer.idx
                 else:
                     targets.append(layer.idx)
 
             return targets
         
     def create_test_dataset(self):
-        test_dataset = self.data_type_py(np.random.default_rng(seed=10).random((int(self.nb_tests),1,int(self.layers[0].size))))
+        test_dataset = self.data_type_py(np.random.default_rng(seed=10).random((self.nb_tests,1,int(self.layers[0].size))))
         return test_dataset 
      
     def load_test_dataset(self):
         
         test_dataset = []
         try:
             with open(self.test_dataset_file, 'r') as f:
@@ -108,15 +133,15 @@
                     if self.data_type == 'int':
                         line = list(map(int,line))
                     elif self.data_type == 'double':
                         line = list(map(float,line)) 
                     elif self.data_type == 'float':
                         line = list(map(np.float32,line))
                     test_dataset.append(line)
-                    if i == int(self.nb_tests)-1:
+                    if i == self.nb_tests-1:
                         break
             test_dataset = np.array(test_dataset)
             f.close()
        
         except TypeError:
             None
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,84 +14,85 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import pystache
+from ..Layer import Layer
+from ..activation_functions import ActivationFunctions
 import numpy as np
-from abc import ABC
-from ... import templates
+import pystache
 
-class Normalizer(ABC):
+class BatchNormalization(Layer):
 
-    def __init__(self, input_size:int, output_size:int, mins:list, maxes:list, means:list, ranges:list):
-        self.input_size = input_size
-        self.output_size = output_size
-        self.mins = mins
-        self.maxes = maxes
-        self.means = means
-        self.ranges = ranges
-        self.template_path = templates.__file__[:-11]
+    def __init__(self, idx:int, size:int, input_shape:list, epsilon:float|int, scale:np.ndarray, biases:np.ndarray, mean:np.ndarray, var:np.ndarray, activation_function:ActivationFunctions):
         super().__init__()
+        self.idx = idx
+        self.size = size
+        self.name = 'BatchNormalization'
+        self.output_channels = input_shape[1]
+        self.output_height = input_shape[2]
+        self.output_width = input_shape[3]
+        self.epsilon = epsilon
+        self.scale = scale
+        self.mean = mean
+        self.var = var
+        self.biases = biases
+        self.nb_biases = self.count_elements_array(self.biases)
+
+        self.activation_function = activation_function
+
+        ####### Checking the instantiation#######
+
+        ### Checking argument type ###
+        assert type(self.idx) == int
+        assert type(self.size) == int
+        assert type(self.output_channels) == int
+        assert type(self.output_height) == int
+        assert type(self.output_width) == int
+        assert type(self.epsilon) == float or type(self.epsilon) == int
+        assert type(self.scale) == np.ndarray
+        assert type(self.mean) == np.ndarray 
+        assert type(self.var) == np.ndarray
+        assert type(self.biases) == np.ndarray
+        assert isinstance(self.activation_function, ActivationFunctions)
+
+        ### Checking value consistency ###
+        assert self.size == self.output_channels*self.output_height*self.output_width
+        assert len(self.scale.shape) == 1 and self.scale.shape[0] == self.output_channels
+        assert len(self.mean.shape) == 1 and self.mean.shape[0] == self.output_channels
+        assert len(self.var.shape) == 1 and self.var.shape[0] == self.output_channels
+        assert len(self.biases.shape) == 1 and self.biases.shape[0] == self.output_channels
+
+
+    def generate_inference_code_layer(self):
+        #Variable indicating under which name the input tensor is
+        output_str = self.previous_layer[0].output_str
+
+        mustach_hash = {}
+
+        mustach_hash['name'] = self.name
+        mustach_hash['idx'] = "{:02d}".format(self.idx)
+        mustach_hash['comment'] = self.activation_function.comment
+        mustach_hash['output_str'] = output_str
+        mustach_hash['path'] = self.path
+        
+        if(self.activation_function.name != 'linear'):
+            mustach_hash['activation_function'] = self.activation_function.write_activation_str('output_'+str(self.path)+'[k + '+str(self.output_height*self.output_width)+'*f]')
+
+        mustach_hash['input_channels'] = self.output_channels
+        mustach_hash['channel_size'] = self.output_height*self.output_width
+        mustach_hash['epsilon'] = self.epsilon
 
-    def array_to_str(self, array:list):
-        s = "{"
-        for element in array:
-            s += str(element) + ", "
-        s = s[:-2] + "}"
-        return s
-
-    def write_pre_processing(self):
-        with open(self.template_path+'normalization/template_pre_processing.c.tpl','r') as template_file:
-            template = template_file.read()
-        template_file.close()
-
-        return pystache.render(template,{'input_size':self.input_size})
-
-
-    def write_post_processing(self):
-        with open(self.template_path+'normalization/template_post_processing.c.tpl','r') as template_file:
-            template = template_file.read()
-        template_file.close()
-
-        return pystache.render(template,{'output_size':self.output_size})
-
-    def write_normalization_cst_in_header_file(self):
-        mustach_hash= {}
-
-        mustach_hash['input_size'] = self.input_size
-
-        with open(self.template_path+'normalization/template_normalization_cst_in_header_file.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_BatchNormalization.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
-    
-    def write_normalization_cst_in_globalvars_file(self):
-        mustach_hash= {}
-
-        mustach_hash['input_size'] = self.input_size
-        mustach_hash['input_min'] = self.array_to_str(self.mins)
-        mustach_hash['input_max'] = self.array_to_str(self.maxes)
-        mustach_hash['input_mean'] = self.array_to_str(self.means[:-1])
-        mustach_hash['input_range'] = self.array_to_str(self.ranges[:-1])
-        mustach_hash['output_mean'] = self.means[-1]
-        mustach_hash['output_range'] = self.ranges[-1]
-
-        with open(self.template_path+'normalization/template_normalization_cst_in_global_var_file.c.tpl','r') as template_file:
-            template = template_file.read()
-        template_file.close()
-
-        return  pystache.render(template, mustach_hash)
 
-    def pre_processing(self, nn_input:np.ndarray):
-        inputs = nn_input.flatten()
-        for i in range(self.input_size):
-            inputs[i] = (max(self.mins[i],min(self.maxes[i],inputs[i])) - self.means[i]) / self.ranges[i]
-        return np.reshape(inputs, nn_input.shape)
-
-    def post_processing(self, nn_output:np.ndarray):
-        for i in range(len(nn_output)):
-            nn_output[i] = nn_output[i]*self.ranges[-1] + self.means[-1]
-        return nn_output
+    def forward_path_layer(self, input:np.ndarray):
+        input = np.reshape(input, (self.output_channels, self.output_height, self.output_width))
+        output = []
+        for i in range(self.output_channels):
+            output.append((input[i] - self.mean[i])/np.sqrt(self.var[i] + self.epsilon)*self.scale[i] + self.biases[i])
+        return np.array(output)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,18 @@
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     initializers = [look_for_initializer(initializer_name,model) for initializer_name in node.input[1:]]
     attributs = extract_attribut(node)
     if ('axes' not in attributs):
         attributs['axes'] = []
+    else:
+        for axe in attributs['axes']:
+            if axe < 0:
+                axe = len(input_shape) - axe
     if('coordinate_transformation_mode' not in attributs):
         attributs['coordinate_transformation_mode'] = 'half_pixel'
     if('exclude_outside' not in attributs):
         attributs['exclude_outside'] = 0
     if('keep_aspect_ratio_policy' not in attributs):
         attributs['keep_aspect_ratio_policy'] = 'stretch'
     if('extrapolation_value' not in attributs):
@@ -224,15 +228,15 @@
         #scale
         targ_size = onnx.numpy_helper.to_array(initializers[1])
         bool_resize = 1
         
     if(initializers[0]):
         roi = onnx.numpy_helper.to_array(initializers[0])
     else:
-        roi = initializers[0]
+        roi = []
     
     return create_resize_obj(mode = attributs['mode'],
                              idx = idx,
                              size = size,
                              input_shape = input_shape,
                              axes = attributs['axes'],
                              coordinate_transformation_mode = attributs['coordinate_transformation_mode'],
@@ -253,17 +257,20 @@
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     initializers = [look_for_initializer(initializer_name,model) for initializer_name in node.input[1:]]
     attributs = extract_attribut(node)
     if(len(initializers)==2):
-        initializers.append([])
-    if(initializers[2]):
+        axes = []
+    else:
         axes = onnx.numpy_helper.to_array(initializers[2])
+        for axe in axes:
+            if axe < 0:
+                axe = len(input_shape) - axe
     return create_pad_obj(mode = attributs['mode'],
                           idx = idx,
                           size = size,
                           pads = onnx.numpy_helper.to_array(initializers[0]),
                           constant_value = onnx.numpy_helper.to_array(initializers[1]),
                           axes = axes,
                           input_shape = input_shape,
@@ -274,19 +281,22 @@
 def create_Gather(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
-    initializer = look_for_initializer(node.input[1],model)
+    indices = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))
+    for indice in indices.flatten():
+        if indice < 0:
+            indice = input_shape[attributs['axis']] - indice
     return Gather(idx = idx,
                     size = size,
                     axis = attributs['axis'],
-                    indices = onnx.numpy_helper.to_array(initializer),
+                    indices = indices,
                     input_shape = input_shape,
                     output_shape = output_shape,
                     activation_function = Linear())
 
 #create a layer Gemm
 def create_Gemm(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
@@ -295,15 +305,15 @@
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     B_tensor = look_for_initializer(node.input[1],model)
     if(len(node.input) == 3):
         C_tensor = look_for_initializer(node.input[2],model)
     else:
-        C_tensor = 0
+        C_tensor = np.zeros((1,1))
     if('transA' not in attributs):
         attributs['transA'] = 0
     if('transB' not in attributs):
         attributs['transB'] = 0
     if('alpha' not in attributs):
         attributs['alpha'] = 1.0
     if('beta' not in attributs):
@@ -327,15 +337,15 @@
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
     if(left_tensor or right_tensor):
         if(right_tensor and not left_tensor):
             #the weigth is the right tensor:  MatMul(W,T)
             side = True
             weights = onnx.numpy_helper.to_array(right_tensor)
-            weights = np.reshape(weights, (get_shape(node.input[1],model)[-1],1,1,output_shape[-1]))
+            weights = np.reshape(weights, (get_shape(node.input[1],model)[-2],1,1,output_shape[-2]))
             weights = np.moveaxis(weights, 0,3)
             dict_input[idx] = [node.input[1]]
             input_shape = get_shape(node.input[1],model)
         if(left_tensor and not right_tensor):
             #the weigth is the right tensor:  MatMul(W,T)
             side = False
             weights = onnx.numpy_helper.to_array(left_tensor)
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     {{/indices}}
 {{/is_gather}}
 
 {{{pre_processing}}}
 {{#layers}}
 {{{inference_function}}}
 {{#debug_layer}}
-    fprintf(fp, "{{name}} {{idx}} {{to_transpose}} {{channels}} {{height}} {{width}} \n");
+    fprintf(fp, "{{name}} {{idx}} {{to_transpose}} {{channels}} {{height}} {{width}}\n");
     for (k = 0; k < {{size}}; ++k)
     {
         fprintf(fp,"%.9g ", output_{{path}}[k]);
         if (k == {{size}} - 1)
         {
             fprintf(fp, "\n");
         }
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.3.dev3
+Version: 0.2.3.dev4
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.2.3.dev3/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.2.3.dev4/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

