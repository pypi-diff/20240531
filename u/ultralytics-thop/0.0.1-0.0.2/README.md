# Comparing `tmp/ultralytics_thop-0.0.1.tar.gz` & `tmp/ultralytics_thop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics_thop-0.0.1.tar", last modified: Fri May 31 18:51:29 2024, max compression
+gzip compressed data, was "ultralytics_thop-0.0.2.tar", last modified: Fri May 31 19:00:18 2024, max compression
```

## Comparing `ultralytics_thop-0.0.1.tar` & `ultralytics_thop-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:51:29.660397 ultralytics_thop-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47843 2024-05-31 18:51:29.660397 ultralytics_thop-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:51:29.660397 ultralytics_thop-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:51:29.656397 ultralytics_thop-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/tests/test_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/tests/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/tests/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:51:29.656397 ultralytics_thop-0.0.1/thop/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6958 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/fx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/onnx_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/rnn_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:51:29.656397 ultralytics_thop-0.0.1/thop/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/vision/basic_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/vision/calc_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/vision/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-31 18:50:34.000000 ultralytics_thop-0.0.1/thop/vision/onnx_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:51:29.660397 ultralytics_thop-0.0.1/ultralytics_thop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47843 2024-05-31 18:51:29.000000 ultralytics_thop-0.0.1/ultralytics_thop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 18:51:29.000000 ultralytics_thop-0.0.1/ultralytics_thop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:51:29.000000 ultralytics_thop-0.0.1/ultralytics_thop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 18:51:29.000000 ultralytics_thop-0.0.1/ultralytics_thop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 18:51:29.000000 ultralytics_thop-0.0.1/ultralytics_thop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47843 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.699634 ultralytics_thop-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.699634 ultralytics_thop-0.0.2/thop/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/fx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/onnx_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/rnn_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.699634 ultralytics_thop-0.0.2/thop/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/basic_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/calc_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-05-31 18:59:26.000000 ultralytics_thop-0.0.2/thop/vision/onnx_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:18.703634 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47843 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 19:00:18.000000 ultralytics_thop-0.0.2/ultralytics_thop.egg-info/top_level.txt
```

### Comparing `ultralytics_thop-0.0.1/LICENSE` & `ultralytics_thop-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.1/PKG-INFO` & `ultralytics_thop-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to count the FLOPs of PyTorch model.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `ultralytics_thop-0.0.1/README.md` & `ultralytics_thop-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics_thop-0.0.1/pyproject.toml` & `ultralytics_thop-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ultralytics-thop"
-version = "0.0.1"  # Placeholder version, needs to be dynamically set
+version = "0.0.2"  # Placeholder version, needs to be dynamically set
 description = "A tool to count the FLOPs of PyTorch model."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["FLOPs", "PyTorch", "Model Analysis"]  # Optional
 authors = [
     { name = "Ligeng Zhu", email = "ligeng.zhu+github@gmail.com" }
```

### Comparing `ultralytics_thop-0.0.1/thop/fx_profile.py` & `ultralytics_thop-0.0.2/thop/fx_profile.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,41 +9,45 @@
     logging.warning(
         f"torch.fx requires version higher than 1.8.0. "
         f"But You are using an old version PyTorch {torch.__version__}. "
     )
 
 
 def count_clamp(input_shapes, output_shapes):
+    """Ensures proper array sizes for tensors by clamping input and output shapes."""
     return 0
 
 
 def count_mul(input_shapes, output_shapes):
-    # element-wise
+    """Returns the number of elements in the first output shape."""
     return output_shapes[0].numel()
 
 
 def count_matmul(input_shapes, output_shapes):
+    """Calculates the total number of operations for a matrix multiplication given input and output shapes."""
     in_shape = input_shapes[0]
     out_shape = output_shapes[0]
     in_features = in_shape[-1]
     num_elements = out_shape.numel()
     return in_features * num_elements
 
 
 def count_fn_linear(input_shapes, output_shapes, *args, **kwargs):
+    """Calculates total operations (FLOPs) for a linear layer given input and output shapes."""
     mul_flops = count_matmul(input_shapes, output_shapes)
     if "bias" in kwargs:
         add_flops = output_shapes[0].numel()
     return mul_flops
 
 
 from .vision.calc_func import calculate_conv
 
 
 def count_fn_conv2d(input_shapes, output_shapes, *args, **kwargs):
+    """Calculates total operations (FLOPs) for a 2D convolutional layer given input and output shapes."""
     inputs, weight, bias, stride, padding, dilation, groups = args
     if len(input_shapes) == 2:
         x_shape, k_shape = input_shapes
     elif len(input_shapes) == 3:
         x_shape, k_shape, b_shape = input_shapes
     out_shape = output_shapes[0]
 
@@ -52,33 +56,37 @@
     in_channel = x_shape[1]
 
     total_ops = calculate_conv(bias_op, kernel_parameters, out_shape.numel(), in_channel, groups).item()
     return int(total_ops)
 
 
 def count_nn_linear(module: nn.Module, input_shapes, output_shapes):
+    """Counts the FLOPs for a fully connected (linear) layer in a neural network module."""
     return count_matmul(input_shapes, output_shapes)
 
 
 def count_zero_ops(module: nn.Module, input_shapes, output_shapes, *args, **kwargs):
+    """Returns 0 for the given neural network module, input shapes, and output shapes."""
     return 0
 
 
 def count_nn_conv2d(module: nn.Conv2d, input_shapes, output_shapes):
+    """Calculates total operations for a 2D convolutional neural network layer in a given neural network module."""
     bias_op = 1 if module.bias is not None else 0
     out_shape = output_shapes[0]
 
     in_channel = module.in_channels
     groups = module.groups
     kernel_ops = module.weight.shape[2:].numel()
     total_ops = calculate_conv(bias_op, kernel_ops, out_shape.numel(), in_channel, groups).item()
     return int(total_ops)
 
 
 def count_nn_bn2d(module: nn.BatchNorm2d, input_shapes, output_shapes):
+    """Calculate the total operations for a given nn.BatchNorm2d module based on its output shape."""
     assert len(output_shapes) == 1, "nn.BatchNorm2d should only have one output"
     y = output_shapes[0]
     # y = (x - mean) / \sqrt{var + e} * weight + bias
     total_ops = 2 * y.numel()
     return total_ops
 
 
@@ -112,18 +120,22 @@
 from torch.fx import symbolic_trace
 from torch.fx.passes.shape_prop import ShapeProp
 
 from .utils import prGreen, prRed, prYellow
 
 
 def null_print(*args, **kwargs):
+    """A no-op print function that takes any arguments without performing any actions."""
     return
 
 
 def fx_profile(mod: nn.Module, input: th.Tensor, verbose=False):
+    """Profiles the given torch.nn Module to calculate total FLOPs for each operation and prints detailed node
+    information if verbose.
+    """
     gm: torch.fx.GraphModule = symbolic_trace(mod)
     g = gm.graph
     ShapeProp(gm).propagate(input)
 
     fprint = null_print
     if verbose:
         fprint = print
@@ -200,24 +212,29 @@
     return total_flops
 
 
 if __name__ == "__main__":
 
     class MyOP(nn.Module):
         def forward(self, input):
+            """Performs forward pass on given input data."""
             return input / 1
 
     class MyModule(torch.nn.Module):
         def __init__(self):
+            """Initializes MyModule with two linear layers and a custom MyOP operator."""
             super().__init__()
             self.linear1 = torch.nn.Linear(5, 3)
             self.linear2 = torch.nn.Linear(5, 3)
             self.myop = MyOP()
 
         def forward(self, x):
+            """Applies two linear transformations to the input tensor, clamps the second, then combines and processes
+            with MyOP operator.
+            """
             out1 = self.linear1(x)
             out2 = self.linear2(x).clamp(min=0.0, max=1.0)
             return self.myop(out1 + out2)
 
     net = MyModule()
     data = th.randn(20, 5)
     flops = fx_profile(net, data, verbose=False)
```

### Comparing `ultralytics_thop-0.0.1/thop/onnx_profile.py` & `ultralytics_thop-0.0.2/thop/onnx_profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 from onnx import numpy_helper
 
 from thop.vision.onnx_counter import onnx_operators
 
 
 class OnnxProfile:
     def __init__(self):
+        """Initialize the OnnxProfile class with necessary imports for ONNX profiling."""
         pass
 
     def calculate_params(self, model: onnx.ModelProto):
+        """Calculate the total number of parameters in an ONNX model."""
         onnx_weights = model.graph.initializer
         params = 0
 
         for onnx_w in onnx_weights:
             try:
                 weight = numpy_helper.to_array(onnx_w)
                 params += np.prod(weight.shape)
             except Exception as _:
                 pass
 
         return params
 
     def create_dict(self, weight, input, output):
+        """Create and return a dictionary mapping weight, input, and output names to their respective dimensions."""
         diction = {}
         for w in weight:
             dim = np.array(w.dims)
             diction[str(w.name)] = dim
             if dim.size == 1:
                 diction[str(w.name)] = np.append(1, dim)
         for i in input:
@@ -48,14 +51,17 @@
             dim = np.array(o.type.tensor_type.shape.dim[0].dim_value)
             diction[str(o.name)] = [dim]
             if dim.size == 1:
                 diction[str(o.name)] = np.append(1, dim)
         return diction
 
     def nodes_counter(self, diction, node):
+        """Count nodes of a specific type in an ONNX graph, returning the count and associated node operation
+        details.
+        """
         if node.op_type not in onnx_operators:
             print("Sorry, we haven't add ", node.op_type, "into dictionary.")
             return 0, None, None
         else:
             fn = onnx_operators[node.op_type]
             return fn(diction, node)
```

### Comparing `ultralytics_thop-0.0.1/thop/profile.py` & `ultralytics_thop-0.0.2/thop/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 }
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.1.0"):
     register_hooks.update({nn.SyncBatchNorm: count_normalization})
 
 
 def profile_origin(model, inputs, custom_ops=None, verbose=True, report_missing=False):
+    """Profiles a PyTorch model's operations and parameters by applying custom or default hooks and returns total
+    operations and parameters.
+    """
     handler_collection = []
     types_collection = set()
     if custom_ops is None:
         custom_ops = {}
     if report_missing:
         verbose = True
 
@@ -158,14 +161,15 @@
     if custom_ops is None:
         custom_ops = {}
     if report_missing:
         # overwrite `verbose` option when enable report_missing
         verbose = True
 
     def add_hooks(m: nn.Module):
+        """Registers hooks to a neural network module to track total operations and parameters."""
         m.register_buffer("total_ops", torch.zeros(1, dtype=torch.float64))
         m.register_buffer("total_params", torch.zeros(1, dtype=torch.float64))
 
         # for p in m.parameters():
         #     m.total_params += torch.DoubleTensor([p.numel()])
 
         m_type = type(m)
@@ -196,14 +200,15 @@
     model.eval()
     model.apply(add_hooks)
 
     with torch.no_grad():
         model(*inputs)
 
     def dfs_count(module: nn.Module, prefix="\t") -> (int, int):
+        """Recursively counts the total operations and parameters of the given PyTorch module and its submodules."""
         total_ops, total_params = module.total_ops.item(), 0
         ret_dict = {}
         for n, m in module.named_children():
             # if not hasattr(m, "total_ops") and not hasattr(m, "total_params"):  # and len(list(m.children())) > 0:
             #     m_ops, m_params = dfs_count(m, prefix=prefix + "\t")
             # else:
             #     m_ops, m_params = m.total_ops, m.total_params
```

### Comparing `ultralytics_thop-0.0.1/thop/rnn_hooks.py` & `ultralytics_thop-0.0.2/thop/rnn_hooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import torch
 import torch.nn as nn
 from torch.nn.utils.rnn import PackedSequence
 
 
 def _count_rnn_cell(input_size, hidden_size, bias=True):
-    # h' = \tanh(W_{ih} x + b_{ih}  +  W_{hh} h + b_{hh})
+    """Calculate the total operations for an RNN cell based on input size, hidden size, and bias configuration."""
     total_ops = hidden_size * (input_size + hidden_size) + hidden_size
     if bias:
         total_ops += hidden_size * 2
 
     return total_ops
 
 
 def count_rnn_cell(m: nn.RNNCell, x: torch.Tensor, y: torch.Tensor):
+    """Counts RNN cell operations based on input, hidden size, bias, and batch size."""
     total_ops = _count_rnn_cell(m.input_size, m.hidden_size, m.bias)
 
     batch_size = x[0].size(0)
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
 
 def _count_gru_cell(input_size, hidden_size, bias=True):
+    """Counts the total operations for a GRU cell based on input size, hidden size, and bias."""
     total_ops = 0
     # r = \sigma(W_{ir} x + b_{ir} + W_{hr} h + b_{hr}) \\
     # z = \sigma(W_{iz} x + b_{iz} + W_{hz} h + b_{hz}) \\
     state_ops = (hidden_size + input_size) * hidden_size + hidden_size
     if bias:
         state_ops += hidden_size * 2
     total_ops += state_ops * 2
@@ -41,23 +43,27 @@
     # hadamard hadamard add
     total_ops += hidden_size * 3
 
     return total_ops
 
 
 def count_gru_cell(m: nn.GRUCell, x: torch.Tensor, y: torch.Tensor):
+    """Calculates and updates the total operations for a GRU cell in a mini-batch during inference."""
     total_ops = _count_gru_cell(m.input_size, m.hidden_size, m.bias)
 
     batch_size = x[0].size(0)
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
 
 def _count_lstm_cell(input_size, hidden_size, bias=True):
+    """Calculates the total operations for an LSTM cell during inference given input size, hidden size, and optional
+    bias.
+    """
     total_ops = 0
 
     # i = \sigma(W_{ii} x + b_{ii} + W_{hi} h + b_{hi}) \\
     # f = \sigma(W_{if} x + b_{if} + W_{hf} h + b_{hf}) \\
     # o = \sigma(W_{io} x + b_{io} + W_{ho} h + b_{ho}) \\
     # g = \tanh(W_{ig} x + b_{ig} + W_{hg} h + b_{hg}) \\
     state_ops = (input_size + hidden_size) * hidden_size + hidden_size
@@ -72,23 +78,27 @@
     # h' = o * \tanh(c') \\
     total_ops += hidden_size
 
     return total_ops
 
 
 def count_lstm_cell(m: nn.LSTMCell, x: torch.Tensor, y: torch.Tensor):
+    """Count the number of operations for a single LSTM cell in a given batch, updating the model's total operations
+    count.
+    """
     total_ops = _count_lstm_cell(m.input_size, m.hidden_size, m.bias)
 
     batch_size = x[0].size(0)
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
 
 def count_rnn(m: nn.RNN, x, y):
+    """Calculate and update the total number of operations for a single RNN cell in a given batch."""
     bias = m.bias
     input_size = m.input_size
     hidden_size = m.hidden_size
     num_layers = m.num_layers
 
     if isinstance(x[0], PackedSequence):
         batch_size = torch.max(x[0].batch_sizes)
@@ -118,14 +128,15 @@
     # batch_size
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
 
 def count_gru(m: nn.GRU, x, y):
+    """Calculate the total number of operations for a GRU layer in a neural network model."""
     bias = m.bias
     input_size = m.input_size
     hidden_size = m.hidden_size
     num_layers = m.num_layers
 
     if isinstance(x[0], PackedSequence):
         batch_size = torch.max(x[0].batch_sizes)
@@ -155,14 +166,17 @@
     # batch_size
     total_ops *= batch_size
 
     m.total_ops += torch.DoubleTensor([int(total_ops)])
 
 
 def count_lstm(m: nn.LSTM, x, y):
+    """Calculate the total operations for LSTM layers in a network, accounting for input size, hidden size, bias, and
+    bidirectionality.
+    """
     bias = m.bias
     input_size = m.input_size
     hidden_size = m.hidden_size
     num_layers = m.num_layers
 
     if isinstance(x[0], PackedSequence):
         batch_size = torch.max(x[0].batch_sizes)
```

### Comparing `ultralytics_thop-0.0.1/thop/utils.py` & `ultralytics_thop-0.0.2/thop/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 COLOR_RED = "91m"
 COLOR_GREEN = "92m"
 COLOR_YELLOW = "93m"
 
 
 def colorful_print(fn_print, color=COLOR_RED):
+    """A decorator to print text in the specified terminal color by wrapping the given print function."""
+
     def actual_call(*args, **kwargs):
         print(f"\033[{color}", end="")
         fn_print(*args, **kwargs)
         print("\033[00m", end="")
 
     return actual_call
 
@@ -25,14 +27,15 @@
 #     print("\033[92m{}\033[00m".format(skk))
 
 # def prYellow(skk):
 #     print("\033[93m{}\033[00m".format(skk))
 
 
 def clever_format(nums, format="%.2f"):
+    """Formats numerical values into a more readable string with units (K, M, G, T) based on their magnitude."""
     if not isinstance(nums, Iterable):
         nums = [nums]
     clever_nums = []
 
     for num in nums:
         if num > 1e12:
             clever_nums.append(format % (num / 1e12) + "T")
```

### Comparing `ultralytics_thop-0.0.1/thop/vision/onnx_counter.py` & `ultralytics_thop-0.0.2/thop/vision/onnx_counter.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,38 +15,42 @@
     counter_mul,
     counter_pow,
     counter_sqrt,
 )
 
 
 def onnx_counter_matmul(diction, node):
+    """Calculates multiply-accumulate operations and output size for matrix multiplication in an ONNX model node."""
     input1 = node.input[0]
     input2 = node.input[1]
     input1_dim = diction[input1]
     input2_dim = diction[input2]
     out_size = np.append(input1_dim[0:-1], input2_dim[-1])
     output_name = node.output[0]
     macs = counter_matmul(input1_dim, out_size[-2:])
     return macs, out_size, output_name
 
 
 def onnx_counter_add(diction, node):
+    """Calculate multiply-accumulate operations (MACs), output size, and output name for ONNX addition nodes."""
     if np.array(diction[node.input[1]]).size >= np.array(diction[node.input[0]]).size:
         out_size = diction[node.input[1]]
     else:
         out_size = diction[node.input[0]]
     output_name = node.output[0]
     macs = calculate_zero_ops()
     # if '140' in diction:
     #     print(diction['140'],output_name)
     return macs, out_size, output_name
 
 
 def onnx_counter_conv(diction, node):
-    # print(node)
+    """Calculates MACs, output size, and name for an ONNX convolution node based on input tensor dimensions and node
+    attributes.
+    """
     # bias,kernelsize,outputsize
     dim_bias = 0
     input_count = 0
     for i in node.input:
         input_count += 1
     if input_count == 3:
         dim_bias = 1
@@ -77,53 +81,59 @@
 
     # if '140' in diction:
     #     print("conv",diction['140'],output_name)
     return macs, output_size, output_name
 
 
 def onnx_counter_constant(diction, node):
-    # print("constant",node)
+    """Calculate MACs, output size, and output name for a constant operation in an ONNX model."""
     macs = calculate_zero_ops()
     output_name = node.output[0]
     output_size = [1]
     # print(macs, output_size, output_name)
     return macs, output_size, output_name
 
 
 def onnx_counter_mul(diction, node):
+    """Calculate MACs, output size, and output name for a multiplication operation in an ONNX model."""
     if np.array(diction[node.input[1]]).size >= np.array(diction[node.input[0]]).size:
         input_size = diction[node.input[1]]
     else:
         input_size = diction[node.input[0]]
     macs = counter_mul(np.prod(input_size))
     output_size = diction[node.input[0]]
     output_name = node.output[0]
     return macs, output_size, output_name
 
 
 def onnx_counter_bn(diction, node):
+    """Calculates MACs, output size, and output name for batch normalization layers in an ONNX model."""
     input_size = diction[node.input[0]]
     macs = calculate_norm(np.prod(input_size))
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_relu(diction, node):
+    """Calculates MACs, output size, and output name for ReLU layers in an ONNX model."""
     input_size = diction[node.input[0]]
     macs = calculate_zero_ops()
     output_name = node.output[0]
     output_size = input_size
     # print(macs, output_size, output_name)
     # if '140' in diction:
     #     print("relu",diction['140'],output_name)
     return macs, output_size, output_name
 
 
 def onnx_counter_reducemean(diction, node):
+    """Compute MACs, output size, and name for the ReduceMean ONNX node, adjusting dimensions based on the 'axes' and
+    'keepdims' attributes.
+    """
     keep_dim = 0
     for attr in node.attribute:
         if "axes" in attr.name:
             dim_axis = np.array(attr.ints)
         elif "keepdims" in attr.name:
             keep_dim = attr.i
 
@@ -135,86 +145,92 @@
     else:
         output_size = np.delete(input_size, dim_axis)
     # output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_sub(diction, node):
+    """Computes MACs, output size, and output name for a given ONNX node with specified input size."""
     input_size = diction[node.input[0]]
     macs = calculate_zero_ops()
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_pow(diction, node):
+    """Calculates MACs, output size, and output name for a given ONNX 'Pow' node with specified input size."""
     if np.array(diction[node.input[1]]).size >= np.array(diction[node.input[0]]).size:
         input_size = diction[node.input[1]]
     else:
         input_size = diction[node.input[0]]
     macs = counter_pow(np.prod(input_size))
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_sqrt(diction, node):
+    """Calculate MACs and output information for the SQRT operation in an ONNX node."""
     input_size = diction[node.input[0]]
     macs = counter_sqrt(np.prod(input_size))
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_div(diction, node):
+    """Calculate MACs and output information for the DIV operation in an ONNX node."""
     if np.array(diction[node.input[1]]).size >= np.array(diction[node.input[0]]).size:
         input_size = diction[node.input[1]]
     else:
         input_size = diction[node.input[0]]
     macs = counter_div(np.prod(input_size))
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_instance(diction, node):
+    """Calculate MACs, output size, and name for an ONNX node instance."""
     input_size = diction[node.input[0]]
     macs = calculate_norm(np.prod(input_size))
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_softmax(diction, node):
+    """Calculate MACs, output size, and name for an ONNX softmax node instance."""
     input_size = diction[node.input[0]]
     dim = node.attribute[0].i
     nfeatures = input_size[dim]
     batch_size = np.prod(input_size) / nfeatures
     macs = calculate_softmax(nfeatures, batch_size)
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_pad(diction, node):
-    # # TODO add constant name and output real vector
+    """Compute memory access cost (MACs), output size, and output name for ONNX pad operation."""
     # if
     # if (np.array(diction[node.input[1]]).size >= np.array(diction[node.input[0]]).size):
     #     input_size = diction[node.input[1]]
     # else:
     #     input_size = diction[node.input[0]]
     input_size = diction[node.input[0]]
     macs = calculate_zero_ops()
     output_name = node.output[0]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_averagepool(diction, node):
-    # TODO add support of ceil_mode and floor
+    """Calculate MACs and output size for an AveragePool ONNX operation based on input dimensions and attributes."""
     macs = calculate_avgpool(np.prod(diction[node.input[0]]))
     output_name = node.output[0]
     dim_pad = None
     for attr in node.attribute:
         # print(attr)
         if attr.name == "kernel_shape":
             dim_kernel = attr.ints  # kw,kh
@@ -236,39 +252,39 @@
             hw[i] = int((hw[i] - dim_kernel[i]) / dim_stride[i] + 1)
         output_size = np.append(dim_input[0 : -np.array(dim_kernel).size], hw)
     # print(macs, output_size, output_name)
     return macs, output_size, output_name
 
 
 def onnx_counter_flatten(diction, node):
-    # print(node)
+    """Returns MACs, output size, and output name for an ONNX Flatten node."""
     macs = calculate_zero_ops()
     output_name = node.output[0]
     axis = node.attribute[0].i
     input_size = diction[node.input[0]]
     output_size = np.append(input_size[axis - 1], np.prod(input_size[axis:]))
     # print("flatten",output_size)
     return macs, output_size, output_name
 
 
 def onnx_counter_gemm(diction, node):
-    # print(node)
+    """Calculate multiply–accumulate operations (MACs), output size, and name for ONNX Gemm node."""
     # Compute Y = alpha * A' * B' + beta * C
     input_size = diction[node.input[0]]
     dim_weight = diction[node.input[1]]
     # print(input_size,dim_weight)
     macs = np.prod(input_size) * dim_weight[1] + dim_weight[0]
     output_size = np.append(input_size[0:-1], dim_weight[0])
     output_name = node.output[0]
     return macs, output_size, output_name
     pass
 
 
 def onnx_counter_maxpool(diction, node):
-    # TODO add support of ceil_mode and floor
+    """Calculate MACs and output size for ONNX MaxPool operation based on input node attributes and dimensions."""
     # print(node)
     macs = calculate_zero_ops()
     output_name = node.output[0]
     dim_pad = None
     for attr in node.attribute:
         # print(attr)
         if attr.name == "kernel_shape":
@@ -291,36 +307,40 @@
             hw[i] = int((hw[i] - dim_kernel[i]) / dim_stride[i] + 1)
         output_size = np.append(dim_input[0 : -np.array(dim_kernel).size], hw)
     # print(macs, output_size, output_name)
     return macs, output_size, output_name
 
 
 def onnx_counter_globalaveragepool(diction, node):
+    """Counts MACs and computes output size for a global average pooling layer in an ONNX model."""
     macs = calculate_zero_ops()
     output_name = node.output[0]
     input_size = diction[node.input[0]]
     output_size = input_size
     return macs, output_size, output_name
 
 
 def onnx_counter_concat(diction, node):
-    # print(node)
+    """Counts MACs and computes output size for a concatenation layer along a specified axis in an ONNX model."""
     # print(diction[node.input[0]])
     axis = node.attribute[0].i
     input_size = diction[node.input[0]]
     for i in node.input:
         dim_concat = diction[i][axis]
     output_size = input_size
     output_size[axis] = dim_concat
     output_name = node.output[0]
     macs = calculate_zero_ops()
     return macs, output_size, output_name
 
 
 def onnx_counter_clip(diction, node):
+    """Calculate MACs, output size, and output name for an ONNX node clip operation using provided dimensions and input
+    size.
+    """
     macs = calculate_zero_ops()
     output_name = node.output[0]
     input_size = diction[node.input[0]]
     output_size = input_size
     return macs, output_size, output_name
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ultralytics_thop-0.0.1/ultralytics_thop.egg-info/PKG-INFO` & `ultralytics_thop-0.0.2/ultralytics_thop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics-thop
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to count the FLOPs of PyTorch model.
 Author-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 Maintainer-email: Ligeng Zhu <ligeng.zhu+github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `ultralytics_thop-0.0.1/ultralytics_thop.egg-info/SOURCES.txt` & `ultralytics_thop-0.0.2/ultralytics_thop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

