# Comparing `tmp/alphafold3_pytorch-0.1.0.tar.gz` & `tmp/alphafold3_pytorch-0.1.1.tar.gz`

## Comparing `alphafold3_pytorch-0.1.0.tar` & `alphafold3_pytorch-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.env.sample
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/Dockerfile
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0   106090 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/life.py
--rw-r--r--   0        0        0    11211 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/trainer.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/tests/test_af3.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/tests/test_trainer.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/LICENSE
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/README.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.env.sample
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/Dockerfile
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0   106105 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/life.py
+-rw-r--r--   0        0        0    11211 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/trainer.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/tests/test_af3.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/tests/test_trainer.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.1.0/Dockerfile` & `alphafold3_pytorch-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/alphafold3.png` & `alphafold3_pytorch-0.1.1/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/.github/workflows/publish.yml` & `alphafold3_pytorch-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.1.1/alphafold3_pytorch/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from alphafold3_pytorch.attention import (
     Attention,
-    Attend
+    Attend,
+    full_pairwise_repr_to_windowed
 )
 
 from alphafold3_pytorch.alphafold3 import (
     RelativePositionEncoding,
     SmoothLDDTLoss,
     WeightedRigidAlign,
     ExpressCoordinatesInFrame,
```

### Comparing `alphafold3_pytorch-0.1.0/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.1.1/alphafold3_pytorch/alphafold3.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,23 @@
     def inner(self, *args, **kwargs):
         self._args_and_kwargs = (args, kwargs)
         self._version = version('alphafold3_pytorch')
 
         return fn(self, *args, **kwargs)
     return inner
 
+@typecheck
+def pad_and_window(
+    t: Float['b n ...'] | Int['b n ...'],
+    window_size: int
+):
+    t = pad_to_multiple(t, window_size, dim = 1)
+    t = rearrange(t, 'b (n w) ... -> b n w ...', w = window_size)
+    return t
+
 # packed atom representation functions
 
 @typecheck
 def lens_to_mask(
     lens: Int['b ...'],
     max_len: int | None = None
 ) -> Bool['... m']:
@@ -1756,32 +1765,31 @@
         pairwise_repr_cond = self.pairwise_repr_to_atompair_feat_cond(conditioned_pairwise_repr)
 
         indices = torch.arange(seq_len, device = device)
         indices = repeat(indices, 'n -> b n', b = batch_size)
 
         indices = repeat_consecutive_with_lens(indices, residue_atom_lens)
         indices = pad_or_slice_to(indices, atom_seq_len, dim = -1)
-        indices = pad_to_multiple(indices, w, dim = -1)
+        indices = pad_and_window(indices, w)
 
         row_indices = col_indices = indices
-        row_indices = rearrange(row_indices, 'b (n w) -> b n w 1', w = w)
-        col_indices = rearrange(col_indices, 'b (n w) -> b n 1 w', w = w)
+        row_indices = rearrange(row_indices, 'b n w -> b n w 1', w = w)
+        col_indices = rearrange(col_indices, 'b n w -> b n 1 w', w = w)
 
         col_indices = concat_neighboring_windows(col_indices, dim_seq = 1, dim_window = -1)
         row_indices, col_indices = torch.broadcast_tensors(row_indices, col_indices)
 
         pairwise_repr_cond = einx.get_at('b [i j] dap, b nw w1 w2, b nw w1 w2 -> b nw w1 w2 dap', pairwise_repr_cond, row_indices, col_indices)
 
         atompair_feats = pairwise_repr_cond + atompair_feats
 
         # condition atompair feats further with single atom repr
 
         atom_repr_cond = self.atom_repr_to_atompair_feat_cond(atom_feats)
-        atom_repr_cond = pad_to_multiple(atom_repr_cond, w, dim = 1)
-        atom_repr_cond = rearrange(atom_repr_cond, 'b (n w) dap -> b n w dap', w = w)
+        atom_repr_cond = pad_and_window(atom_repr_cond, w)
 
         atom_repr_cond_row, atom_repr_cond_col = atom_repr_cond.chunk(2, dim = -1)
 
         atom_repr_cond_col = concat_neighboring_windows(atom_repr_cond_col, dim_seq = 1, dim_window = 2)
 
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w1 dap -> b nw w1 w2 dap', atompair_feats, atom_repr_cond_row)
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w2 dap -> b nw w1 w2 dap', atompair_feats, atom_repr_cond_col)
@@ -2561,16 +2569,15 @@
         if not is_windowed:
             atompair_feats = full_pairwise_repr_to_windowed(atompair_feats, window_size = w)
 
         # condition atompair with atom repr
 
         atom_feats_cond = self.atom_repr_to_atompair_feat_cond(atom_feats)
 
-        atom_feats_cond = pad_to_multiple(atom_feats_cond, w, dim = 1)
-        atom_feats_cond = rearrange(atom_feats_cond, 'b (nw w) dap -> b nw w dap', w = w)
+        atom_feats_cond = pad_and_window(atom_feats_cond, w)
 
         atom_feats_cond_row, atom_feats_cond_col = atom_feats_cond.chunk(2, dim = -1)
         atom_feats_cond_col = concat_neighboring_windows(atom_feats_cond_col, dim_seq = 1, dim_window = -2)
 
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w1 dap',atompair_feats, atom_feats_cond_row)
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w2 dap',atompair_feats, atom_feats_cond_col)
```

### Comparing `alphafold3_pytorch-0.1.0/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.1.1/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/alphafold3_pytorch/life.py` & `alphafold3_pytorch-0.1.1/alphafold3_pytorch/life.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/alphafold3_pytorch/trainer.py` & `alphafold3_pytorch-0.1.1/alphafold3_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.1.1/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.1.1/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/tests/test_af3.py` & `alphafold3_pytorch-0.1.1/tests/test_af3.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/tests/test_trainer.py` & `alphafold3_pytorch-0.1.1/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/.gitignore` & `alphafold3_pytorch-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/LICENSE` & `alphafold3_pytorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.0/README.md` & `alphafold3_pytorch-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 <img src="./alphafold3.png" width="500px"></img>
 
 ## Alphafold 3 - Pytorch
 
 Implementation of <a href="https://www.nature.com/articles/s41586-024-07487-w">Alphafold 3</a> in Pytorch
 
-Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
+You can chat with other researchers about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
 ## Appreciation
 
 - <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the Relative Positional Encoding and the Smooth LDDT Loss!
 
 - <a href="https://github.com/engelberger">Felipe</a> for contributing Weighted Rigid Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation modules!
 
 - <a href="https://github.com/amorehead">Alex</a> for fixing various issues in the transcribed algorithms
 
 - <a href="https://github.com/gitabtion">Heng</a> for pointing out inconsistencies with the paper and pull requesting the solutions
 
+- <a href="https://github.com/patrick-kidger">Patrick</a> for <a href="https://docs.kidger.site/jaxtyping/">jaxtyping</a>, <a href="https://github.com/fferflo">Florian</a> for <a href="https://github.com/fferflo/einx">einx</a>, and of course, <a href="https://github.com/arogozhnikov">Alex</a> for <a href="https://einops.rocks/">einops</a>
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
 [./alphafold3.png]## Alphafold 3 - Pytorch Implementation of _A_l_p_h_a_f_o_l_d_ _3 in
-Pytorch Getting a fair number of emails. You can chat with me about this work
-_h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the Relative Positional Encoding
-and the Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid Align,
-Express Coordinates In Frame, Compute Alignment Error, and Centre Random
-Augmentation modules! - _A_l_e_x for fixing various issues in the transcribed
-algorithms - _H_e_n_g for pointing out inconsistencies with the paper and pull
-requesting the solutions ## Install ```bash $ pip install alphafold3-pytorch
-``` ## Usage ```python import torch from alphafold3_pytorch import Alphafold3
-alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_template_feats = 44 ) # mock
-inputs seq_len = 16 residue_atom_lens = torch.randint(1, 3, (2, seq_len))
-atom_seq_len = residue_atom_lens.sum(dim = -1).amax() atom_inputs = torch.randn
-(2, atom_seq_len, 77) atompair_inputs = torch.randn(2, atom_seq_len,
-atom_seq_len, 5) additional_residue_feats = torch.randn(2, seq_len, 10)
-template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
-torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) msa_mask =
-torch.ones((2, 7)).bool() # required for training, but omitted on inference
-atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
-residue_atom_lens - 1 # last atom, as an example distance_labels =
-torch.randint(0, 37, (2, seq_len, seq_len)) pae_labels = torch.randint(0, 64,
-(2, seq_len, seq_len)) pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
-plddt_labels = torch.randint(0, 50, (2, seq_len)) resolved_labels =
-torch.randint(0, 2, (2, seq_len)) # train loss = alphafold3
-( num_recycling_steps = 2, atom_inputs = atom_inputs, atompair_inputs =
-atompair_inputs, residue_atom_lens = residue_atom_lens,
+Pytorch You can chat with other researchers about this work _h_e_r_e ##
+Appreciation - _J_o_s_e_p_h for contributing the Relative Positional Encoding and the
+Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid Align, Express
+Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation
+modules! - _A_l_e_x for fixing various issues in the transcribed algorithms - _H_e_n_g
+for pointing out inconsistencies with the paper and pull requesting the
+solutions - _P_a_t_r_i_c_k for _j_a_x_t_y_p_i_n_g, _F_l_o_r_i_a_n for _e_i_n_x, and of course, _A_l_e_x for
+_e_i_n_o_p_s ## Install ```bash $ pip install alphafold3-pytorch ``` ## Usage
+```python import torch from alphafold3_pytorch import Alphafold3 alphafold3 =
+Alphafold3( dim_atom_inputs = 77, dim_template_feats = 44 ) # mock inputs
+seq_len = 16 residue_atom_lens = torch.randint(1, 3, (2, seq_len)) atom_seq_len
+= residue_atom_lens.sum(dim = -1).amax() atom_inputs = torch.randn(2,
+atom_seq_len, 77) atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len,
+5) additional_residue_feats = torch.randn(2, seq_len, 10) template_feats =
+torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
+() msa = torch.randn(2, 7, seq_len, 64) msa_mask = torch.ones((2, 7)).bool() #
+required for training, but omitted on inference atom_pos = torch.randn(2,
+atom_seq_len, 3) residue_atom_indices = residue_atom_lens - 1 # last atom, as
+an example distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
+pae_labels = torch.randint(0, 64, (2, seq_len, seq_len)) pde_labels =
+torch.randint(0, 64, (2, seq_len, seq_len)) plddt_labels = torch.randint(0, 50,
+(2, seq_len)) resolved_labels = torch.randint(0, 2, (2, seq_len)) # train loss
+= alphafold3( num_recycling_steps = 2, atom_inputs = atom_inputs,
+atompair_inputs = atompair_inputs, residue_atom_lens = residue_atom_lens,
 additional_residue_feats = additional_residue_feats, msa = msa, msa_mask =
 msa_mask, templates = template_feats, template_mask = template_mask, atom_pos =
 atom_pos, residue_atom_indices = residue_atom_indices, distance_labels =
 distance_labels, pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels
 = plddt_labels, resolved_labels = resolved_labels ) loss.backward() # after
 much training ... sampled_atom_pos = alphafold3( num_recycling_steps = 4,
 num_sample_steps = 16, atom_inputs = atom_inputs, atompair_inputs =
```

### Comparing `alphafold3_pytorch-0.1.0/pyproject.toml` & `alphafold3_pytorch-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.1.0"
+version = "0.1.1"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
@@ -24,16 +24,18 @@
 
 dependencies = [
     "beartype",
     "einops>=0.8.0",
     "einx>=0.2.2",
     "ema-pytorch>=0.4.8",
     "environs",
+    "hydra-core",
     "jaxtyping>=0.2.28",
     "lightning>=2.2.5",
+    "omegaconf",
     "taylor-series-linear-attention>=0.1.9",
     "torch>=2.1",
     "tqdm",
 ]
 
 [project.urls]
 Homepage = "https://pypi.org/project/alphafold3-pytorch/"
```

### Comparing `alphafold3_pytorch-0.1.0/PKG-INFO` & `alphafold3_pytorch-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -35,42 +35,46 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Requires-Dist: beartype
 Requires-Dist: einops>=0.8.0
 Requires-Dist: einx>=0.2.2
 Requires-Dist: ema-pytorch>=0.4.8
 Requires-Dist: environs
+Requires-Dist: hydra-core
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: lightning>=2.2.5
+Requires-Dist: omegaconf
 Requires-Dist: taylor-series-linear-attention>=0.1.9
 Requires-Dist: torch>=2.1
 Requires-Dist: tqdm
 Provides-Extra: examples
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 <img src="./alphafold3.png" width="500px"></img>
 
 ## Alphafold 3 - Pytorch
 
 Implementation of <a href="https://www.nature.com/articles/s41586-024-07487-w">Alphafold 3</a> in Pytorch
 
-Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
+You can chat with other researchers about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
 ## Appreciation
 
 - <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the Relative Positional Encoding and the Smooth LDDT Loss!
 
 - <a href="https://github.com/engelberger">Felipe</a> for contributing Weighted Rigid Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation modules!
 
 - <a href="https://github.com/amorehead">Alex</a> for fixing various issues in the transcribed algorithms
 
 - <a href="https://github.com/gitabtion">Heng</a> for pointing out inconsistencies with the paper and pull requesting the solutions
 
+- <a href="https://github.com/patrick-kidger">Patrick</a> for <a href="https://docs.kidger.site/jaxtyping/">jaxtyping</a>, <a href="https://github.com/fferflo">Florian</a> for <a href="https://github.com/fferflo/einx">einx</a>, and of course, <a href="https://github.com/arogozhnikov">Alex</a> for <a href="https://einops.rocks/">einops</a>
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.0 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.1 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -19,43 +19,44 @@
 DEALINGS IN THE SOFTWARE. License-File: LICENSE Keywords: artificial
 intelligence,deep learning,protein structure prediction Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8 Requires-Dist: beartype Requires-Dist:
 einops>=0.8.0 Requires-Dist: einx>=0.2.2 Requires-Dist: ema-pytorch>=0.4.8
-Requires-Dist: environs Requires-Dist: jaxtyping>=0.2.28 Requires-Dist:
-lightning>=2.2.5 Requires-Dist: taylor-series-linear-attention>=0.1.9 Requires-
-Dist: torch>=2.1 Requires-Dist: tqdm Provides-Extra: examples Provides-Extra:
-test Requires-Dist: pytest; extra == 'test' Description-Content-Type: text/
-markdown [./alphafold3.png]## Alphafold 3 - Pytorch Implementation of _A_l_p_h_a_f_o_l_d
-_3 in Pytorch Getting a fair number of emails. You can chat with me about this
-work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the Relative Positional
-Encoding and the Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid
-Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random
-Augmentation modules! - _A_l_e_x for fixing various issues in the transcribed
-algorithms - _H_e_n_g for pointing out inconsistencies with the paper and pull
-requesting the solutions ## Install ```bash $ pip install alphafold3-pytorch
-``` ## Usage ```python import torch from alphafold3_pytorch import Alphafold3
-alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_template_feats = 44 ) # mock
-inputs seq_len = 16 residue_atom_lens = torch.randint(1, 3, (2, seq_len))
-atom_seq_len = residue_atom_lens.sum(dim = -1).amax() atom_inputs = torch.randn
-(2, atom_seq_len, 77) atompair_inputs = torch.randn(2, atom_seq_len,
-atom_seq_len, 5) additional_residue_feats = torch.randn(2, seq_len, 10)
-template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
-torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) msa_mask =
-torch.ones((2, 7)).bool() # required for training, but omitted on inference
-atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
-residue_atom_lens - 1 # last atom, as an example distance_labels =
-torch.randint(0, 37, (2, seq_len, seq_len)) pae_labels = torch.randint(0, 64,
-(2, seq_len, seq_len)) pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
-plddt_labels = torch.randint(0, 50, (2, seq_len)) resolved_labels =
-torch.randint(0, 2, (2, seq_len)) # train loss = alphafold3
-( num_recycling_steps = 2, atom_inputs = atom_inputs, atompair_inputs =
-atompair_inputs, residue_atom_lens = residue_atom_lens,
+Requires-Dist: environs Requires-Dist: hydra-core Requires-Dist:
+jaxtyping>=0.2.28 Requires-Dist: lightning>=2.2.5 Requires-Dist: omegaconf
+Requires-Dist: taylor-series-linear-attention>=0.1.9 Requires-Dist: torch>=2.1
+Requires-Dist: tqdm Provides-Extra: examples Provides-Extra: test Requires-
+Dist: pytest; extra == 'test' Description-Content-Type: text/markdown [./
+alphafold3.png]## Alphafold 3 - Pytorch Implementation of _A_l_p_h_a_f_o_l_d_ _3 in
+Pytorch You can chat with other researchers about this work _h_e_r_e ##
+Appreciation - _J_o_s_e_p_h for contributing the Relative Positional Encoding and the
+Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid Align, Express
+Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation
+modules! - _A_l_e_x for fixing various issues in the transcribed algorithms - _H_e_n_g
+for pointing out inconsistencies with the paper and pull requesting the
+solutions - _P_a_t_r_i_c_k for _j_a_x_t_y_p_i_n_g, _F_l_o_r_i_a_n for _e_i_n_x, and of course, _A_l_e_x for
+_e_i_n_o_p_s ## Install ```bash $ pip install alphafold3-pytorch ``` ## Usage
+```python import torch from alphafold3_pytorch import Alphafold3 alphafold3 =
+Alphafold3( dim_atom_inputs = 77, dim_template_feats = 44 ) # mock inputs
+seq_len = 16 residue_atom_lens = torch.randint(1, 3, (2, seq_len)) atom_seq_len
+= residue_atom_lens.sum(dim = -1).amax() atom_inputs = torch.randn(2,
+atom_seq_len, 77) atompair_inputs = torch.randn(2, atom_seq_len, atom_seq_len,
+5) additional_residue_feats = torch.randn(2, seq_len, 10) template_feats =
+torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
+() msa = torch.randn(2, 7, seq_len, 64) msa_mask = torch.ones((2, 7)).bool() #
+required for training, but omitted on inference atom_pos = torch.randn(2,
+atom_seq_len, 3) residue_atom_indices = residue_atom_lens - 1 # last atom, as
+an example distance_labels = torch.randint(0, 37, (2, seq_len, seq_len))
+pae_labels = torch.randint(0, 64, (2, seq_len, seq_len)) pde_labels =
+torch.randint(0, 64, (2, seq_len, seq_len)) plddt_labels = torch.randint(0, 50,
+(2, seq_len)) resolved_labels = torch.randint(0, 2, (2, seq_len)) # train loss
+= alphafold3( num_recycling_steps = 2, atom_inputs = atom_inputs,
+atompair_inputs = atompair_inputs, residue_atom_lens = residue_atom_lens,
 additional_residue_feats = additional_residue_feats, msa = msa, msa_mask =
 msa_mask, templates = template_feats, template_mask = template_mask, atom_pos =
 atom_pos, residue_atom_indices = residue_atom_indices, distance_labels =
 distance_labels, pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels
 = plddt_labels, resolved_labels = resolved_labels ) loss.backward() # after
 much training ... sampled_atom_pos = alphafold3( num_recycling_steps = 4,
 num_sample_steps = 16, atom_inputs = atom_inputs, atompair_inputs =
```

