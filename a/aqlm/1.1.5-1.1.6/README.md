# Comparing `tmp/aqlm-1.1.5.tar.gz` & `tmp/aqlm-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqlm-1.1.5.tar", last modified: Sat Apr 20 17:16:12 2024, max compression
+gzip compressed data, was "aqlm-1.1.6.tar", last modified: Fri May 31 14:10:00 2024, max compression
```

## Comparing `aqlm-1.1.5.tar` & `aqlm-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.263104 aqlm-1.1.5/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)       81 2024-02-16 15:38:52.000000 aqlm-1.1.5/MANIFEST.in
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-20 17:16:12.263104 aqlm-1.1.5/PKG-INFO
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      333 2024-02-16 15:38:52.000000 aqlm-1.1.5/pyproject.toml
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1418 2024-04-20 17:16:12.267104 aqlm-1.1.5/setup.cfg
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.239104 aqlm-1.1.5/src/
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.243104 aqlm-1.1.5/src/aqlm/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      130 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/__init__.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4747 2024-04-02 21:27:23.000000 aqlm-1.1.5/src/aqlm/inference.py
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.251104 aqlm-1.1.5/src/aqlm/inference_kernels/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      102 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/inference_kernels/__init__.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    10906 2024-04-20 14:40:20.000000 aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cpp
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    14569 2024-04-20 14:12:20.000000 aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cu
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3350 2024-04-02 21:27:23.000000 aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      716 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/inference_kernels/dequantization.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4334 2024-04-02 21:27:23.000000 aqlm-1.1.5/src/aqlm/inference_kernels/kernel_selector.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     2499 2024-03-06 14:39:27.000000 aqlm-1.1.5/src/aqlm/inference_kernels/numba_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     7238 2024-02-22 09:29:16.000000 aqlm-1.1.5/src/aqlm/inference_kernels/triton_kernel.py
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3022 2024-02-16 15:38:52.000000 aqlm-1.1.5/src/aqlm/utils.py
-drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-04-20 17:16:12.259104 aqlm-1.1.5/src/aqlm.egg-info/
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/PKG-INFO
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      600 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/SOURCES.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        1 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/dependency_links.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      199 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/requires.txt
--rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        5 2024-04-20 17:16:12.000000 aqlm-1.1.5/src/aqlm.egg-info/top_level.txt
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-05-31 14:10:00.978397 aqlm-1.1.6/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)       81 2024-02-16 15:38:52.000000 aqlm-1.1.6/MANIFEST.in
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-05-31 14:10:00.978397 aqlm-1.1.6/PKG-INFO
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      333 2024-02-16 15:38:52.000000 aqlm-1.1.6/pyproject.toml
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1418 2024-05-31 14:10:00.982397 aqlm-1.1.6/setup.cfg
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-05-31 14:10:00.962397 aqlm-1.1.6/src/
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-05-31 14:10:00.966397 aqlm-1.1.6/src/aqlm/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      130 2024-02-22 09:29:16.000000 aqlm-1.1.6/src/aqlm/__init__.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4747 2024-05-30 22:07:56.000000 aqlm-1.1.6/src/aqlm/inference.py
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-05-31 14:10:00.974397 aqlm-1.1.6/src/aqlm/inference_kernels/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      102 2024-02-22 09:29:16.000000 aqlm-1.1.6/src/aqlm/inference_kernels/__init__.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    14274 2024-05-30 21:22:10.000000 aqlm-1.1.6/src/aqlm/inference_kernels/cuda_kernel.cpp
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)    15718 2024-05-30 21:50:15.000000 aqlm-1.1.6/src/aqlm/inference_kernels/cuda_kernel.cu
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3350 2024-04-02 21:27:23.000000 aqlm-1.1.6/src/aqlm/inference_kernels/cuda_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      716 2024-05-30 22:08:12.000000 aqlm-1.1.6/src/aqlm/inference_kernels/dequantization.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     4289 2024-05-30 22:07:24.000000 aqlm-1.1.6/src/aqlm/inference_kernels/kernel_selector.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     2499 2024-03-06 14:39:27.000000 aqlm-1.1.6/src/aqlm/inference_kernels/numba_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     7238 2024-02-22 09:29:16.000000 aqlm-1.1.6/src/aqlm/inference_kernels/triton_kernel.py
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     3022 2024-02-16 15:38:52.000000 aqlm-1.1.6/src/aqlm/utils.py
+drwxr-xr-x   0 apanfero (1105122) alistgrp (1000941)        0 2024-05-31 14:10:00.974397 aqlm-1.1.6/src/aqlm.egg-info/
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)     1679 2024-05-31 14:10:00.000000 aqlm-1.1.6/src/aqlm.egg-info/PKG-INFO
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      600 2024-05-31 14:10:00.000000 aqlm-1.1.6/src/aqlm.egg-info/SOURCES.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        1 2024-05-31 14:10:00.000000 aqlm-1.1.6/src/aqlm.egg-info/dependency_links.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)      199 2024-05-31 14:10:00.000000 aqlm-1.1.6/src/aqlm.egg-info/requires.txt
+-rw-r--r--   0 apanfero (1105122) alistgrp (1000941)        5 2024-05-31 14:10:00.000000 aqlm-1.1.6/src/aqlm.egg-info/top_level.txt
```

### Comparing `aqlm-1.1.5/PKG-INFO` & `aqlm-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqlm
-Version: 1.1.5
+Version: 1.1.6
 Summary: Efficiently run models quantized with AQLM
 Home-page: https://github.com/Vahe1994/AQLM
 Author: AQLM paper authors
 Author-email: vahe527887@yandex.ru
 Project-URL: Bug Tracker, https://github.com/Vahe1994/AQLM/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aqlm-1.1.5/setup.cfg` & `aqlm-1.1.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aqlm
-version = 1.1.5
+version = 1.1.6
 author = AQLM paper authors
 author_email = vahe527887@yandex.ru
 description = Efficiently run models quantized with AQLM
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Vahe1994/AQLM
 project_urls =
```

### Comparing `aqlm-1.1.5/src/aqlm/inference.py` & `aqlm-1.1.6/src/aqlm/inference.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.cpp` & `aqlm-1.1.6/src/aqlm/inference_kernels/cuda_kernel.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -20,41 +20,51 @@
         dtype.name(),
         ". Please specify the correct `torch_dtype` when loading the model."
       )
     );
   }
 }
 
-void code1x16_matvec_cuda(
+
+template <bool use_bfloat16, size_t group_size>
+void  code1x16_matvec_cuda(
   const void* A,
   const void* B,
         void* C,
   const void* codebook,
   int prob_m,
-  int prob_k,
-  bool use_bfloat16
+  int prob_k
 );
+extern template void code1x16_matvec_cuda<false, 8>(const void*, const void*, void*, const void*, int, int);
+extern template void code1x16_matvec_cuda<true, 8>(const void*, const void*, void*, const void*, int, int); 
+extern template void code1x16_matvec_cuda<false, 16>(const void*, const void*, void*, const void*, int, int);
+extern template void code1x16_matvec_cuda<true, 16>(const void*, const void*, void*, const void*, int, int);
 
+template <size_t group_size>
 void code1x16_dequant_cuda(
   const void* A,
         void* C,
   const void* codebook,
   int prob_m,
   int prob_k
 );
+extern template void code1x16_dequant_cuda<8>(const void*, void*, const void*, int, int);
+extern template void code1x16_dequant_cuda<16>(const void*, void*, const void*, int, int);
 
+template <bool use_bfloat16>
 void code2x8_matvec_cuda(
   const void* A,
   const void* B,
         void* C,
   const void* codebook,
   int prob_m,
-  int prob_k,
-  bool use_bfloat16
+  int prob_k
 );
+extern template void code2x8_matvec_cuda<false>(const void*, const void*, void*, const void*, int, int);
+extern template void code2x8_matvec_cuda<true>(const void*, const void*, void*, const void*, int, int);
 
 void code2x8_dequant_cuda(
   const void* A,
         void* C,
   const void* codebook,
   int prob_m,
   int prob_k,
@@ -85,23 +95,37 @@
         torch::Tensor& C,
   const torch::Tensor& codebook,
   const bool use_bfloat16
 ) {
   const at::cuda::OptionalCUDAGuard device_guard(device_of(A));
   int prob_m = C.size(0);
   int prob_k = B.size(0);
-  code1x16_matvec_cuda(
-    A.data_ptr(),
-    B.data_ptr(),
-    C.data_ptr(),
-    codebook.data_ptr(),
-    prob_m,
-    prob_k,
-    use_bfloat16
-  );
+
+  if (codebook.size(3) == 8) {
+    if (use_bfloat16) {
+      code1x16_matvec_cuda<true, 8>(A.data_ptr(), B.data_ptr(), C.data_ptr(), codebook.data_ptr(), prob_m, prob_k);
+    } else {
+      code1x16_matvec_cuda<false, 8>(A.data_ptr(), B.data_ptr(), C.data_ptr(), codebook.data_ptr(), prob_m, prob_k);
+    }
+  } else if (codebook.size(3) == 16) {
+    if (use_bfloat16) {
+      code1x16_matvec_cuda<true, 16>(A.data_ptr(), B.data_ptr(), C.data_ptr(), codebook.data_ptr(), prob_m, prob_k);
+    } else {
+      code1x16_matvec_cuda<false, 16>(A.data_ptr(), B.data_ptr(), C.data_ptr(), codebook.data_ptr(), prob_m, prob_k);
+    }
+  } else {
+    throw c10::NotImplementedError(
+      {__func__, __FILE__, static_cast<uint32_t>(__LINE__)},
+      c10::str(
+        "AQLM CUDA kernels only support codebooks with 8 or 16 features. Got ",
+        codebook.size(3),
+        "."
+      )
+    );
+  }
 }
 
 torch::Tensor code1x16_matmat(
   const torch::Tensor& input,
   const torch::Tensor& codes,
   const torch::Tensor& codebooks,
   const torch::Tensor& scales,
@@ -138,29 +162,48 @@
 
 torch::Tensor code1x16_dequant(
   const torch::Tensor& codes,
   const torch::Tensor& codebooks,
   const torch::Tensor& scales
 ) {
   check_use_bfloat16(codebooks);
-  auto in_features = codes.size(1) * 8;
+  auto in_features = codes.size(1) * codebooks.size(3);
   auto out_features = scales.size(0);
 
   auto weight = torch::empty({out_features, in_features},
     torch::TensorOptions()
       .dtype(codebooks.dtype())
       .device(codebooks.device())
   );
-  code1x16_dequant_cuda(
-    codes.data_ptr(),
-    weight.data_ptr(),
-    codebooks.data_ptr(),
-    out_features,
-    in_features
-  );
+  if (codebooks.size(3) == 8) {
+    code1x16_dequant_cuda<8>(
+      codes.data_ptr(),
+      weight.data_ptr(),
+      codebooks.data_ptr(),
+      out_features,
+      in_features
+    );
+  } else if (codebooks.size(3) == 16) {
+    code1x16_dequant_cuda<16>(
+      codes.data_ptr(),
+      weight.data_ptr(),
+      codebooks.data_ptr(),
+      out_features,
+      in_features
+    );
+  } else {
+    throw c10::NotImplementedError(
+      {__func__, __FILE__, static_cast<uint32_t>(__LINE__)},
+      c10::str(
+        "AQLM CUDA kernels only support codebooks with 8 or 16 features. Got ",
+        codebooks.size(3),
+        "."
+      )
+    );
+  }
   weight *= scales.index({"...", 0, 0});
 
   return weight;
 }
 
 int4 accumulate_sizes(const torch::Tensor& codebook_partition_sizes)
 {
@@ -187,30 +230,49 @@
   const torch::Tensor& codes,
   const torch::Tensor& codebooks,
   const torch::Tensor& scales,
   const std::optional<torch::Tensor>& bias
 ) {
   bool use_bfloat16 = check_use_bfloat16(input);
   auto input_sizes = input.sizes();
-  auto in_features = codes.size(1) * 8;
+  auto in_features = codes.size(1) * codebooks.size(3);
   auto out_features = codes.size(0) * codebooks.size(2);
   auto flat_input = input.reshape({-1, input.size(-1)});
 
   auto weight = torch::empty({out_features, in_features},
     torch::TensorOptions()
       .dtype(codebooks.dtype())
       .device(codebooks.device())
   );
-  code1x16_dequant_cuda(
-    codes.data_ptr(),
-    weight.data_ptr(),
-    codebooks.data_ptr(),
-    out_features,
-    in_features
-  );
+  if (codebooks.size(3) == 8) {
+    code1x16_dequant_cuda<8>(
+      codes.data_ptr(),
+      weight.data_ptr(),
+      codebooks.data_ptr(),
+      out_features,
+      in_features
+    );
+  } else if (codebooks.size(3) == 16) {
+    code1x16_dequant_cuda<16>(
+      codes.data_ptr(),
+      weight.data_ptr(),
+      codebooks.data_ptr(),
+      out_features,
+      in_features
+    );
+  } else {
+    throw c10::NotImplementedError(
+      {__func__, __FILE__, static_cast<uint32_t>(__LINE__)},
+      c10::str(
+        "AQLM CUDA kernels only support codebooks with 8 or 16 features. Got ",
+        codebooks.size(3),
+        "."
+      )
+    );
+  }
 
   auto flat_output = F::linear(flat_input, weight);
   return scale_bias_unflatten_output(
     flat_output,
     scales,
     bias,
     input_sizes
@@ -231,21 +293,40 @@
   auto scaled_input = (input.reshape({-1, input.size(-1)}) * scales.flatten().unsqueeze(0)).reshape(input_sizes);
 
   auto weight = torch::empty({out_features, in_features},
     torch::TensorOptions()
       .dtype(codebooks.dtype())
       .device(codebooks.device())
   );
-  code1x16_dequant_cuda(
-    codes.data_ptr(),
-    weight.data_ptr(),
-    codebooks.data_ptr(),
-    out_features,
-    in_features
-  );
+  if (codebooks.size(3) == 8) {
+    code1x16_dequant_cuda<8>(
+      codes.data_ptr(),
+      weight.data_ptr(),
+      codebooks.data_ptr(),
+      out_features,
+      in_features
+    );
+  } else if (codebooks.size(3) == 16) {
+    code1x16_dequant_cuda<16>(
+      codes.data_ptr(),
+      weight.data_ptr(),
+      codebooks.data_ptr(),
+      out_features,
+      in_features
+    );
+  } else {
+    throw c10::NotImplementedError(
+      {__func__, __FILE__, static_cast<uint32_t>(__LINE__)},
+      c10::str(
+        "AQLM CUDA kernels only support codebooks with 8 or 16 features. Got ",
+        codebooks.size(3),
+        "."
+      )
+    );
+  }
 
   torch::Tensor bias_2{};
   if (bias.has_value()) {
     bias_2 = bias.value();
   }
 
   return F::linear(scaled_input, weight.transpose(0, 1), bias_2);
@@ -257,23 +338,33 @@
         torch::Tensor& C,
   const torch::Tensor& codebook,
   bool use_bfloat16
 ) {
   const at::cuda::OptionalCUDAGuard device_guard(device_of(A));
   int prob_m = C.size(0);
   int prob_k = B.size(0);
-  code2x8_matvec_cuda(
-    A.data_ptr(),
-    B.data_ptr(),
-    C.data_ptr(),
-    codebook.data_ptr(),
-    prob_m,
-    prob_k,
-    use_bfloat16
-  );
+  if (use_bfloat16) {
+    code2x8_matvec_cuda<true>(
+      A.data_ptr(),
+      B.data_ptr(),
+      C.data_ptr(),
+      codebook.data_ptr(),
+      prob_m,
+      prob_k
+    );
+  } else {
+    code2x8_matvec_cuda<false>(
+      A.data_ptr(),
+      B.data_ptr(),
+      C.data_ptr(),
+      codebook.data_ptr(),
+      prob_m,
+      prob_k
+    );
+  }
 }
 
 torch::Tensor code2x8_matmat(
   const torch::Tensor& input,
   const torch::Tensor& codes,
   const torch::Tensor& codebooks,
   const torch::Tensor& scales,
```

### Comparing `aqlm-1.1.5/src/aqlm/inference_kernels/cuda_kernel.py` & `aqlm-1.1.6/src/aqlm/inference_kernels/cuda_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.5/src/aqlm/inference_kernels/dequantization.py` & `aqlm-1.1.6/src/aqlm/inference_kernels/dequantization.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.5/src/aqlm/inference_kernels/kernel_selector.py` & `aqlm-1.1.6/src/aqlm/inference_kernels/kernel_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,40 +20,31 @@
 
 def get_forward_pass_kernel(
     codebooks: torch.Tensor,
     optimize_for_training: bool,
 ) -> Callable[[torch.Tensor, torch.IntTensor, torch.Tensor, torch.Tensor, Optional[torch.Tensor]], torch.Tensor]:
     num_codebooks, codebook_size, out_group_size, in_group_size = codebooks.shape
 
-    if (optimize_for_training, codebooks.device.type, num_codebooks, codebook_size, out_group_size, in_group_size) == (
+    if (optimize_for_training, codebooks.device.type, num_codebooks, codebook_size, out_group_size) == (
         False,
         "cuda",
         1,
         65536,
         1,
-        8,
-    ):
+    ) and in_group_size in [8, 16]:
         from .cuda_kernel import CUDA_FOLDER
 
         return torch.ops.aqlm.code1x16_matmat
-    elif (
-        optimize_for_training,
-        codebooks.device.type,
-        num_codebooks,
-        codebook_size,
-        out_group_size,
-        in_group_size,
-    ) == (
+    elif (optimize_for_training, codebooks.device.type, num_codebooks, codebook_size, out_group_size,) == (
         True,
         "cuda",
         1,
         65536,
         1,
-        8,
-    ):
+    ) and in_group_size in [8, 16]:
         from .cuda_kernel import CUDA_FOLDER
 
         return torch.ops.aqlm.code1x16_matmat_dequant
     elif (
         optimize_for_training,
         codebooks.device.type,
         num_codebooks,
@@ -91,22 +82,21 @@
 
 def get_backward_pass_kernel(
     codebooks: torch.Tensor,
     optimize_for_training: bool,
 ) -> torch.Tensor:
     num_codebooks, codebook_size, out_group_size, in_group_size = codebooks.shape
 
-    if (optimize_for_training, codebooks.device.type, num_codebooks, codebook_size, out_group_size, in_group_size,) == (
+    if (optimize_for_training, codebooks.device.type, num_codebooks, codebook_size, out_group_size,) == (
         True,
         "cuda",
         1,
         65536,
         1,
-        8,
-    ):
+    ) and in_group_size in [8, 16]:
         from .cuda_kernel import CUDA_FOLDER
 
         return torch.ops.aqlm.code1x16_matmat_dequant_transposed
     elif (
         optimize_for_training,
         codebooks.device.type,
         num_codebooks,
```

### Comparing `aqlm-1.1.5/src/aqlm/inference_kernels/numba_kernel.py` & `aqlm-1.1.6/src/aqlm/inference_kernels/numba_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.5/src/aqlm/inference_kernels/triton_kernel.py` & `aqlm-1.1.6/src/aqlm/inference_kernels/triton_kernel.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.5/src/aqlm/utils.py` & `aqlm-1.1.6/src/aqlm/utils.py`

 * *Files identical despite different names*

### Comparing `aqlm-1.1.5/src/aqlm.egg-info/PKG-INFO` & `aqlm-1.1.6/src/aqlm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqlm
-Version: 1.1.5
+Version: 1.1.6
 Summary: Efficiently run models quantized with AQLM
 Home-page: https://github.com/Vahe1994/AQLM
 Author: AQLM paper authors
 Author-email: vahe527887@yandex.ru
 Project-URL: Bug Tracker, https://github.com/Vahe1994/AQLM/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `aqlm-1.1.5/src/aqlm.egg-info/SOURCES.txt` & `aqlm-1.1.6/src/aqlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

