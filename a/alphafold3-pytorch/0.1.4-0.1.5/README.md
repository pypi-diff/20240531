# Comparing `tmp/alphafold3_pytorch-0.1.4.tar.gz` & `tmp/alphafold3_pytorch-0.1.5.tar.gz`

## Comparing `alphafold3_pytorch-0.1.4.tar` & `alphafold3_pytorch-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.env.sample
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/Dockerfile
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0   105334 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/life.py
--rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/trainer.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/tests/test_af3.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/tests/test_trainer.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/LICENSE
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/.env.sample
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/Dockerfile
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0   105338 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3_pytorch/life.py
+-rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3_pytorch/trainer.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/tests/test_af3.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/tests/test_trainer.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.5/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.1.4/Dockerfile` & `alphafold3_pytorch-0.1.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/alphafold3.png` & `alphafold3_pytorch-0.1.5/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/.github/workflows/publish.yml` & `alphafold3_pytorch-0.1.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.1.5/alphafold3_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.1.5/alphafold3_pytorch/alphafold3.py`

 * *Files 0% similar despite different names*

```diff
@@ -3319,15 +3319,15 @@
         should_call_confidence_head = any([*map(exists, confidence_head_labels)])
         return_pae_logits = exists(pae_labels)
 
         if calc_diffusion_loss and should_call_confidence_head:
 
             # rollout
 
-            pred_atom_pos = self.edm.sample(
+            denoised_atom_pos = self.edm.sample(
                 num_sample_steps = num_rollout_steps,
                 atom_feats = atom_feats,
                 atompair_feats = atompair_feats,
                 atom_mask = atom_mask,
                 mask = mask,
                 single_trunk_repr = single,
                 single_inputs_repr = single_inputs,
```

### Comparing `alphafold3_pytorch-0.1.4/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.1.5/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/alphafold3_pytorch/life.py` & `alphafold3_pytorch-0.1.5/alphafold3_pytorch/life.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/alphafold3_pytorch/trainer.py` & `alphafold3_pytorch-0.1.5/alphafold3_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.1.5/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.1.5/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/tests/test_af3.py` & `alphafold3_pytorch-0.1.5/tests/test_af3.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/tests/test_trainer.py` & `alphafold3_pytorch-0.1.5/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/.gitignore` & `alphafold3_pytorch-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/LICENSE` & `alphafold3_pytorch-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/README.md` & `alphafold3_pytorch-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.4/pyproject.toml` & `alphafold3_pytorch-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.1.4"
+version = "0.1.5"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
```

### Comparing `alphafold3_pytorch-0.1.4/PKG-INFO` & `alphafold3_pytorch-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.4 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.5 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

