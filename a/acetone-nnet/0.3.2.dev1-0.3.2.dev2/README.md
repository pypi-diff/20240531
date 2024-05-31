# Comparing `tmp/acetone_nnet-0.3.2.dev1.tar.gz` & `tmp/acetone_nnet-0.3.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.3.2.dev1.tar", last modified: Thu May 30 11:57:20 2024, max compression
+gzip compressed data, was "acetone_nnet-0.3.2.dev2.tar", last modified: Fri May 31 07:32:58 2024, max compression
```

## Comparing `acetone_nnet-0.3.2.dev1.tar` & `acetone_nnet-0.3.2.dev2.tar`

### file list

```diff
@@ -1,155 +1,157 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:20.008391 acetone_nnet-0.3.2.dev1/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.2.dev1/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev1/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev1/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-30 11:57:20.008391 acetone_nnet-0.3.2.dev1/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5749 2024-05-27 09:13:18.000000 acetone_nnet-0.3.2.dev1/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-30 11:57:02.000000 acetone_nnet-0.3.2.dev1/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-30 11:57:20.008391 acetone_nnet-0.3.2.dev1/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.609386 acetone_nnet-0.3.2.dev1/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.648387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1861 2024-05-30 10:00:06.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.650387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2764 2024-05-29 09:10:29.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.651387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1912 2024-05-30 09:59:54.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5245 2024-05-24 08:55:18.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.653387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.655387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1972 2024-05-24 08:54:29.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7432 2024-05-24 08:55:08.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1958 2024-05-24 08:54:22.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:13.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:37.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7493 2024-05-24 08:55:41.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.656387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8516 2024-05-30 09:14:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3419 2024-05-24 08:55:24.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11596 2024-05-24 08:54:47.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3574 2024-05-24 08:55:32.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.657387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.658387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.658387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2799 2024-05-29 11:45:24.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5494 2024-05-30 11:54:16.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Transpose.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2274 2024-05-30 09:59:44.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29413 2024-05-27 11:46:21.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.659387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1370 2024-05-29 07:00:39.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-27 09:32:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_keras.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3744 2024-05-27 09:35:47.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_onnx.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4417 2024-05-29 06:27:31.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_tools.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.659387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.659387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.660387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.660387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5381 2024-05-29 07:48:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.661387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    33832 2024-05-30 11:56:07.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-28 14:07:15.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.661387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.734388 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.840389 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.887390 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.911390 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.914390 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.962391 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      656 2024-05-30 07:17:26.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      493 2024-05-30 09:52:09.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Transpose.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.981391 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-05-29 14:00:27.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.996391 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:20.007391 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7209 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:58.048530 acetone_nnet-0.3.2.dev2/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.2.dev2/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev2/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev2/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-31 07:32:58.047530 acetone_nnet-0.3.2.dev2/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5749 2024-05-27 09:13:18.000000 acetone_nnet-0.3.2.dev2/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-31 07:32:48.000000 acetone_nnet-0.3.2.dev2/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-31 07:32:58.048530 acetone_nnet-0.3.2.dev2/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.563524 acetone_nnet-0.3.2.dev2/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.608525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1876 2024-05-31 07:21:05.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.610525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2764 2024-05-29 09:10:29.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.610525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1927 2024-05-31 07:21:11.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5245 2024-05-24 08:55:18.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.613525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.615525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1972 2024-05-24 08:54:29.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7432 2024-05-24 08:55:08.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1958 2024-05-24 08:54:22.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:13.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:37.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7493 2024-05-24 08:55:41.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.617525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8516 2024-05-30 09:14:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3419 2024-05-24 08:55:24.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7438 2024-05-31 07:30:41.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/GatherElement.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11596 2024-05-24 08:54:47.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3574 2024-05-24 08:55:32.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.618525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.619525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.620525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2799 2024-05-29 11:45:24.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5504 2024-05-30 13:58:05.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Transpose.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2332 2024-05-31 07:20:55.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29505 2024-05-31 07:32:23.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.621525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1370 2024-05-29 07:00:39.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-27 09:32:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/debug_keras.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3744 2024-05-27 09:35:47.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/debug_onnx.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4417 2024-05-29 06:27:31.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/debug_tools.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.621525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.621525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.621525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.622525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5381 2024-05-29 07:48:10.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.622525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    34770 2024-05-31 07:21:26.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-28 14:07:15.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.623525 acetone_nnet-0.3.2.dev2/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.719526 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.808527 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.880528 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.933529 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.959529 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:57.995529 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1140 2024-05-31 07:30:51.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_GatherElement.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      656 2024-05-30 07:17:26.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      494 2024-05-30 13:58:10.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Transpose.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:58.008529 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-05-29 14:00:27.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:58.034530 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-31 07:32:58.047530 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-31 07:32:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7328 2024-05-31 07:32:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-31 07:32:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-31 07:32:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-31 07:32:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-31 07:32:57.000000 acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.3.2.dev1/AUTHORS.md` & `acetone_nnet-0.3.2.dev2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/COPYING` & `acetone_nnet-0.3.2.dev2/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/LICENSE` & `acetone_nnet-0.3.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/PKG-INFO` & `acetone_nnet-0.3.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3.2.dev1
+Version: 0.3.2.dev2
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.3.2.dev1/README.md` & `acetone_nnet-0.3.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/pyproject.toml` & `acetone_nnet-0.3.2.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.3.2.dev1"
+version = "0.3.2.dev2"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  ******************************************************************************
 """
 
 from . import code_generator
 from .code_generator import (
     CodeGenerator, Layer,
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, 
-    Softmax, BatchNormalization, Transpose,
+    Softmax, BatchNormalization, Transpose, GatherElement,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from . import layers
 from .layers import (
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, 
-    Softmax, BatchNormalization, Transpose,
+    Softmax, BatchNormalization, Transpose, GatherElement,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Transpose.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/Transpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,28 +83,28 @@
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['size'] = self.size
         mustach_hash['road'] = self.path
         mustach_hash['output_str'] = output_str
 
-        mustach_hash['activation_function'] = self.activation_function.write_activation_str(self.local_var)
+        mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[k]')
 
         mustach_hash['output_channels'] = self.output_channels
         mustach_hash['output_height'] = self.output_height
         mustach_hash['output_width'] = self.output_width
         mustach_hash['input_height'] = self.input_height
         mustach_hash['input_width'] = self.input_width
 
-        indices = ['f','i','j']
-        if self.perm[1:] == (2,3,1):
+        indices = ['Batch','f','i','j']
+        if self.perm[1:] == [2,3,1]:
             mustach_hash['a'] = indices[self.perm[1]]
             mustach_hash['b'] = indices[self.perm[3]]
             mustach_hash['c'] = indices[self.perm[2]]
-        elif self.perm[1:] == (3,1,2):
+        elif self.perm[1:] == [3,1,2]:
             mustach_hash['a'] = indices[self.perm[2]]
             mustach_hash['b'] = indices[self.perm[1]]
             mustach_hash['c'] = indices[self.perm[3]]
         else:
             mustach_hash['a'] = indices[self.perm[3]]
             mustach_hash['b'] = indices[self.perm[2]]
             mustach_hash['c'] = indices[self.perm[1]]
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .Gather import Gather
 from .Gemm import Gemm
 from .Input import InputLayer
 from .MatMul import MatMul
 from .Softmax import Softmax
 from .BatchNormalization import BatchNormalization
 from .Transpose import Transpose
+from .GatherElement import GatherElement
 
 from . import Broadcast_layers
 from .Broadcast_layers import Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract 
 
 from . import Conv_layers
 from .Conv_layers import Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm
 
@@ -45,14 +46,14 @@
 
 from . import Resize_layers
 from .Resize_layers import Resize, ResizeCubic, ResizeLinear, ResizeNearest
 
 
 __all__ = (
     "Add_Bias", "Concatenate", "Dense", "Dot", "Flatten", "Gather", "Gemm", "InputLayer", "MatMul", 
-    "Softmax", "BatchNormalization", "Transpose",
+    "Softmax", "BatchNormalization", "Transpose", "GatherElement",
     Broadcast_layers.__all__,
     Conv_layers.__all__,
     Pad_layers.__all__,
     Pooling_layers.__all__,
     Resize_layers.__all__
 )
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 import pystache
 
 from .. import templates
 
 from ..format_importer.parser import parser
 
 from .layers import (
-    Dense, Dot, Softmax, Gather, Gemm, MatMul, Concatenate, Pad, Broadcast, BatchNormalization,
+    Dense, Dot, Softmax, Gather, Gemm, MatMul, Concatenate, Pad, 
+    Broadcast, BatchNormalization, GatherElement,
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
 )
 
 class CodeGenerator(ABC):
 
@@ -365,18 +366,18 @@
 
         mustach_hash = {}
 
         mustach_hash['data_type'] = self.data_type
         mustach_hash['input_size'] = self.layers[0].size
         mustach_hash['output_size'] = self.layers[-1].size
 
-        if any((isinstance(layer, Gather)) for layer in self.layers):
+        if any((isinstance(layer, Gather) or isinstance(layer, GatherElement)) for layer in self.layers):
             mustach_hash['is_gather'] = True
             indices = []
-            for gather in [layer for layer in self.layers if (isinstance(layer,Gather))]:
+            for gather in [layer for layer in self.layers if (isinstance(layer,Gather) or isinstance(layer, GatherElement))]:
                 indices.append({'idx':"{:02d}".format(gather.idx), 'lenght':len(gather.indices.flatten()), 'list':self.flatten_array_orderc(gather.indices)})
             mustach_hash['indices'] = indices
 
         self.l_size_max = 1
         for layer in (self.layers):
             if layer.size > self.l_size_max : self.l_size_max = layer.size
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_keras.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/debug_keras.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_onnx.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/debug_onnx.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_tools.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/debug_tools/debug_tools.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 from ...code_generator.layers import (
     AveragePooling2D, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
-    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias, BatchNormalization, Transpose
+    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul,
+    Add_Bias, BatchNormalization, Transpose, GatherElement
 )
 
 from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm, LeakyReLu
 
 ###### Utility functions ######
 
 def create_conv2d_obj(algorithm:str, **kwargs):
@@ -308,14 +309,34 @@
                     size = size,
                     axis = attributs['axis'],
                     indices = indices,
                     input_shape = input_shape,
                     output_shape = output_shape,
                     activation_function = Linear())
 
+#create a layer Gather
+def create_GatherElement(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
+    input_shape = get_shape(node.input[0],model)
+    output_shape = get_shape(node.output[0],model)
+    size = find_size(output_shape)
+    dict_input[idx] = [node.input[0]]
+    dict_output[node.output[0]] = idx
+    attributs = extract_attribut(node)
+    indices = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))
+    for indice in indices.flatten():
+        if indice < 0:
+            indice = input_shape[attributs['axis']] - indice
+    return GatherElement(idx = idx,
+                        size = size,
+                        axis = attributs['axis'],
+                        indices = indices,
+                        input_shape = input_shape,
+                        output_shape = output_shape,
+                        activation_function = Linear())
+
 #create a layer Gemm
 def create_Gemm(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3.2.dev1
+Version: 0.3.2.dev2
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.3.2.dev2/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/acetone_nnet/code_generator/layers/AddBias.py
 src/acetone_nnet/code_generator/layers/BatchNormalization.py
 src/acetone_nnet/code_generator/layers/Concatenate.py
 src/acetone_nnet/code_generator/layers/Dense.py
 src/acetone_nnet/code_generator/layers/Dot.py
 src/acetone_nnet/code_generator/layers/Flatten.py
 src/acetone_nnet/code_generator/layers/Gather.py
+src/acetone_nnet/code_generator/layers/GatherElement.py
 src/acetone_nnet/code_generator/layers/Gemm.py
 src/acetone_nnet/code_generator/layers/Input.py
 src/acetone_nnet/code_generator/layers/MatMul.py
 src/acetone_nnet/code_generator/layers/Softmax.py
 src/acetone_nnet/code_generator/layers/Transpose.py
 src/acetone_nnet/code_generator/layers/__init__.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
@@ -85,14 +86,15 @@
 src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
 src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
 src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
 src/acetone_nnet/templates/layers/template_Dense.c.tpl
 src/acetone_nnet/templates/layers/template_Dot.c.tpl
 src/acetone_nnet/templates/layers/template_Flatten.c.tpl
 src/acetone_nnet/templates/layers/template_Gather.c.tpl
+src/acetone_nnet/templates/layers/template_GatherElement.c.tpl
 src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
 src/acetone_nnet/templates/layers/template_MatMul.c.tpl
 src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
 src/acetone_nnet/templates/layers/template_Softmax.c.tpl
 src/acetone_nnet/templates/layers/template_Transpose.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
```

