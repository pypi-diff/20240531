# Comparing `tmp/alphafold3_pytorch-0.1.1.tar.gz` & `tmp/alphafold3_pytorch-0.1.4.tar.gz`

## Comparing `alphafold3_pytorch-0.1.1.tar` & `alphafold3_pytorch-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.env.sample
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/Dockerfile
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0   106105 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/life.py
--rw-r--r--   0        0        0    11211 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/trainer.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/tests/test_af3.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/tests/test_trainer.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/LICENSE
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.env.sample
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/Dockerfile
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0   105334 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0    11617 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/life.py
+-rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/trainer.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    16360 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/tests/test_af3.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/tests/test_trainer.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.1.4/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.1.1/Dockerfile` & `alphafold3_pytorch-0.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/alphafold3.png` & `alphafold3_pytorch-0.1.4/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/.github/workflows/publish.yml` & `alphafold3_pytorch-0.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/alphafold3_pytorch/__init__.py` & `alphafold3_pytorch-0.1.4/alphafold3_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.1.4/alphafold3_pytorch/alphafold3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,9 @@
 from __future__ import annotations
 
-"""
-global ein notation:
-
-b - batch
-ba - batch with augmentation
-h - heads
-n - residue sequence length
-i - residue sequence length (source)
-j - residue sequence length (target)
-m - atom sequence length
-nw - windowed sequence length
-d - feature dimension
-ds - feature dimension (single)
-dp - feature dimension (pairwise)
-dap - feature dimension (atompair)
-dapi - feature dimension (atompair input)
-da - feature dimension (atom)
-dai - feature dimension (atom input)
-t - templates
-s - msa
-r - registers
-"""
-
-"""
-additional_residue_feats: [*, 10]:
-
-0: residue_index
-1: token_index
-2: asym_id
-3: entity_id
-4: sym_id
-5: restype (must be one hot encoded to 32)
-6: is_protein
-7: is_rna
-8: is_dna
-9: is_ligand
-"""
-
 from math import pi, sqrt
 from pathlib import Path
 from functools import partial, wraps
 from collections import namedtuple
 
 import torch
 from torch import nn, sigmoid
@@ -66,29 +28,67 @@
 
 from alphafold3_pytorch.attention import (
     Attention,
     pad_at_dim,
     slice_at_dim,
     pad_or_slice_to,
     pad_to_multiple,
-    concat_neighboring_windows,
+    concat_previous_window,
     full_attn_bias_to_windowed,
     full_pairwise_repr_to_windowed
 )
 
 from taylor_series_linear_attention import TaylorSeriesLinearAttn
 
 import einx
 from einops import rearrange, repeat, reduce, einsum, pack, unpack
 from einops.layers.torch import Rearrange
 
 from tqdm import tqdm
 
 from importlib.metadata import version
 
+"""
+global ein notation:
+
+b - batch
+ba - batch with augmentation
+h - heads
+n - residue sequence length
+i - residue sequence length (source)
+j - residue sequence length (target)
+m - atom sequence length
+nw - windowed sequence length
+d - feature dimension
+ds - feature dimension (single)
+dp - feature dimension (pairwise)
+dap - feature dimension (atompair)
+dapi - feature dimension (atompair input)
+da - feature dimension (atom)
+dai - feature dimension (atom input)
+t - templates
+s - msa
+r - registers
+"""
+
+"""
+additional_residue_feats: [*, 10]:
+
+0: residue_index
+1: token_index
+2: asym_id
+3: entity_id
+4: sym_id
+5: restype (must be one hot encoded to 32)
+6: is_protein
+7: is_rna
+8: is_dna
+9: is_ligand
+"""
+
 # constants
 
 ADDITIONAL_RESIDUE_FEATS = 10
 
 LinearNoBias = partial(Linear, bias = False)
 
 # helper functions
@@ -237,32 +237,14 @@
     output = einx.where(
         'b n, b n ..., -> b n ...',
         output_mask, output, mask_value
     )
 
     return output
 
-def repeat_pairwise_consecutive_with_lens(
-    feats: Float['b n n dp'],
-    lens: Int['b n']
-) -> Float['b m m dp']:
-
-    repeated_lens = repeat(lens, 'b ... -> (b repeat) ...', repeat = feats.shape[1])
-    feats, ps = pack_one(feats, '* n dp')
-    feats = repeat_consecutive_with_lens(feats, repeated_lens)
-    feats = unpack_one(feats, ps, '* n dp')
-
-    feats = rearrange(feats, 'b i j dp -> b j i dp')
-    repeated_lens = repeat(lens, 'b ... -> (b repeat) ...', repeat = feats.shape[1])
-    feats, ps = pack_one(feats, '* n dp')
-    feats = repeat_consecutive_with_lens(feats, repeated_lens)
-    feats = unpack_one(feats, ps, '* n dp')
-    feats = rearrange(feats, 'b j i dp -> b i j dp')
-    return feats
-
 # linear and outer sum
 # for single repr -> pairwise pattern throughout this architecture
 
 class LinearNoBiasThenOuterSum(Module):
     def __init__(
         self,
         dim,
@@ -561,16 +543,16 @@
         )
 
     @typecheck
     def forward(
         self,
         single_repr: Float['b n ds'],
         *,
-        pairwise_repr: Float['b n n dp'] | Float['b nw w (w*3) dp'],
-        attn_bias: Float['b n n'] | Float['b nw w (w*3)'] | None = None,
+        pairwise_repr: Float['b n n dp'] | Float['b nw w (w*2) dp'],
+        attn_bias: Float['b n n'] | Float['b nw w (w*2)'] | None = None,
         **kwargs
     ) -> Float['b n ds']:
 
         w, has_window_size = self.window_size, exists(self.window_size)
 
         # take care of windowing logic
         # for sequence-local atom transformer
@@ -1464,15 +1446,15 @@
 
     @typecheck
     def forward(
         self,
         noised_repr: Float['b n d'],
         *,
         single_repr: Float['b n ds'],
-        pairwise_repr: Float['b n n dp'] | Float['b nw w (w*3) dp'],
+        pairwise_repr: Float['b n n dp'] | Float['b nw w (w*2) dp'],
         mask: Bool['b n'] | None = None
     ):
         w = self.attn_window_size
         has_windows = exists(w)
 
         serial = self.serial
 
@@ -1705,15 +1687,15 @@
 
     @typecheck
     def forward(
         self,
         noised_atom_pos: Float['b m 3'],
         *,
         atom_feats: Float['b m da'],
-        atompair_feats: Float['b m m dap'] | Float['b nw w (w*3) dap'],
+        atompair_feats: Float['b m m dap'] | Float['b nw w (w*2) dap'],
         atom_mask: Bool['b m'],
         times: Float[' b'],
         mask: Bool['b n'],
         single_trunk_repr: Float['b n dst'],
         single_inputs_repr: Float['b n dsi'],
         pairwise_trunk: Float['b n n dpt'],
         pairwise_rel_pos_feats: Float['b n n dpr'],
@@ -1771,29 +1753,29 @@
         indices = pad_or_slice_to(indices, atom_seq_len, dim = -1)
         indices = pad_and_window(indices, w)
 
         row_indices = col_indices = indices
         row_indices = rearrange(row_indices, 'b n w -> b n w 1', w = w)
         col_indices = rearrange(col_indices, 'b n w -> b n 1 w', w = w)
 
-        col_indices = concat_neighboring_windows(col_indices, dim_seq = 1, dim_window = -1)
+        col_indices = concat_previous_window(col_indices, dim_seq = 1, dim_window = -1)
         row_indices, col_indices = torch.broadcast_tensors(row_indices, col_indices)
 
         pairwise_repr_cond = einx.get_at('b [i j] dap, b nw w1 w2, b nw w1 w2 -> b nw w1 w2 dap', pairwise_repr_cond, row_indices, col_indices)
 
         atompair_feats = pairwise_repr_cond + atompair_feats
 
         # condition atompair feats further with single atom repr
 
         atom_repr_cond = self.atom_repr_to_atompair_feat_cond(atom_feats)
         atom_repr_cond = pad_and_window(atom_repr_cond, w)
 
         atom_repr_cond_row, atom_repr_cond_col = atom_repr_cond.chunk(2, dim = -1)
 
-        atom_repr_cond_col = concat_neighboring_windows(atom_repr_cond_col, dim_seq = 1, dim_window = 2)
+        atom_repr_cond_col = concat_previous_window(atom_repr_cond_col, dim_seq = 1, dim_window = 2)
 
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w1 dap -> b nw w1 w2 dap', atompair_feats, atom_repr_cond_row)
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w2 dap -> b nw w1 w2 dap', atompair_feats, atom_repr_cond_col)
 
         # furthermore, they did one more MLP on the atompair feats for attention biasing in atom transformer
 
         atompair_feats = self.atompair_feats_mlp(atompair_feats) + atompair_feats
@@ -2101,16 +2083,14 @@
 
         # if additional residue feats is provided
         # calculate the weights for mse loss (wl)
 
         align_weights = atom_pos_ground_truth.new_ones(atom_pos_ground_truth.shape[:2])
 
         if exists(additional_residue_feats):
-            w = self.net.atoms_per_window
-
             is_nucleotide_or_ligand_fields = (additional_residue_feats[..., 7:] != 0.).unbind(dim = -1)
 
             is_nucleotide_or_ligand_fields = tuple(repeat_consecutive_with_lens(t, residue_atom_lens) for t in is_nucleotide_or_ligand_fields)
             is_nucleotide_or_ligand_fields = tuple(pad_or_slice_to(t, length = align_weights.shape[-1], dim = -1) for t in is_nucleotide_or_ligand_fields)
 
             atom_is_dna, atom_is_rna, atom_is_ligand = is_nucleotide_or_ligand_fields
 
@@ -2572,15 +2552,15 @@
         # condition atompair with atom repr
 
         atom_feats_cond = self.atom_repr_to_atompair_feat_cond(atom_feats)
 
         atom_feats_cond = pad_and_window(atom_feats_cond, w)
 
         atom_feats_cond_row, atom_feats_cond_col = atom_feats_cond.chunk(2, dim = -1)
-        atom_feats_cond_col = concat_neighboring_windows(atom_feats_cond_col, dim_seq = 1, dim_window = -2)
+        atom_feats_cond_col = concat_previous_window(atom_feats_cond_col, dim_seq = 1, dim_window = -2)
 
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w1 dap',atompair_feats, atom_feats_cond_row)
         atompair_feats = einx.add('b nw w1 w2 dap, b nw w2 dap',atompair_feats, atom_feats_cond_col)
 
         # initial atom transformer
 
         atom_feats = self.atom_transformer(
```

### Comparing `alphafold3_pytorch-0.1.1/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.1.4/alphafold3_pytorch/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import NamedTuple, Tuple
 
 import torch
-from torch import nn
+from torch import nn, Tensor
 import torch.nn.functional as F
 from torch.nn import Module
 
 import einx
 from einops import einsum, repeat, rearrange, pack, unpack
 from einops.layers.torch import Rearrange
 
@@ -95,44 +95,43 @@
 
     if padding_needed == 0:
         return t
 
     return pad_at_dim(t, (0, padding_needed), dim = dim, value = value)
 
 @typecheck
-def concat_neighboring_windows(
+def concat_previous_window(
     t: Tensor,
     *,
     dim_seq: int,
     dim_window: int
 ):
-    t = pad_at_dim(t, (1, 1), dim = dim_seq, value = 0.)
+    t = pad_at_dim(t, (1, 0), dim = dim_seq, value = 0.)
 
     t = torch.cat((
-        slice_at_dim(t, slice(None, -2), dim = dim_seq),
-        slice_at_dim(t, slice(1, -1), dim = dim_seq),
-        slice_at_dim(t, slice(2, None), dim = dim_seq)
+        slice_at_dim(t, slice(None, -1), dim = dim_seq),
+        slice_at_dim(t, slice(1, None), dim = dim_seq),
     ), dim = dim_window)
 
     return t
 
 # for changing full attention bias matrix to a local windowed one for atom attention
 
 @typecheck
 def full_pairwise_repr_to_windowed(
     pairwise_repr: Float['... m m dp'],
     window_size: int
-) -> Float['... n w (w*3) dp']:
+) -> Float['... n w (w*2) dp']:
 
     seq_len, device = pairwise_repr.shape[-2], pairwise_repr.device
 
     padding_needed = (window_size - (seq_len % window_size)) % window_size
     pairwise_repr = F.pad(pairwise_repr, (0, 0, 0, padding_needed, 0, padding_needed), value = 0.)
     pairwise_repr = rearrange(pairwise_repr, '... (i w1) (j w2) d -> ... i j w1 w2 d', w1 = window_size, w2 = window_size)
-    pairwise_repr = concat_neighboring_windows(pairwise_repr, dim_seq = -4, dim_window = -2)
+    pairwise_repr = concat_previous_window(pairwise_repr, dim_seq = -4, dim_window = -2)
 
     # get the diagonal
 
     n = torch.arange(pairwise_repr.shape[-4], device = device)
 
     pairwise_repr = einx.get_at(
         '... [i j] w1 w2 d, n, n -> ... n w1 w2 d',
@@ -141,15 +140,15 @@
 
     return pairwise_repr
 
 @typecheck
 def full_attn_bias_to_windowed(
     attn_bias: Float['... m m'],
     window_size: int
-) -> Float['... n w (w*3)']:
+) -> Float['... n w (w*2)']:
 
     attn_bias = rearrange(attn_bias, '... -> ... 1')
     attn_bias = full_pairwise_repr_to_windowed(attn_bias, window_size = window_size)
     return rearrange(attn_bias, '... 1 -> ...')
 
 # multi-head attention
 
@@ -211,15 +210,15 @@
 
     @typecheck
     def forward(
         self,
         seq: Float['b i d'],
         mask: Bool['b n']| None = None,
         context: Float['b j d'] | None = None,
-        attn_bias: Float['... i j'] | Float['... nw w (w*3)'] | None = None
+        attn_bias: Float['... i j'] | Float['... nw w (w*2)'] | None = None
 
     ) -> Float['b i d']:
 
         q = self.to_q(seq)
 
         context_seq = default(context, seq)
         k, v = self.to_kv(context_seq).chunk(2, dim = -1)
@@ -312,15 +311,15 @@
     @typecheck
     def local_attn(
         self,
         q: Float['b h n d'],
         k: Float['b h n d'],
         v: Float['b h n d'],
         mask: Bool['b n'] | None = None,
-        attn_bias: Float['... n n'] | Float['... nw w (w*3)'] | None = None
+        attn_bias: Float['... n n'] | Float['... nw w (w*2)'] | None = None
     ) -> Float['b h n d']:
         """
         simple local attention with a radius of 1 window size
         """
 
         window_size, batch, seq_len, device = self.window_size, q.shape[0], q.shape[-2], q.device
 
@@ -341,19 +340,19 @@
 
         q, k, v = tuple(rearrange(t, 'b h (n w) d -> b h n w d', w = window_size) for t in (q, k, v))
         mask = rearrange(mask, 'b (n w) -> b n w', w = window_size)
 
         # just do radius of 1 for now
         # perhaps not even necessary, and could try shifted windows (a la Swin)
 
-        k, v = tuple(pad_at_dim(t, (1, 1), dim = -2) for t in (k, v))
-        mask = F.pad(mask, (1, 1), value = False)
+        k, v = tuple(pad_at_dim(t, (1, 0), dim = -2) for t in (k, v))
+        mask = F.pad(mask, (1, 0), value = False)
 
-        k, v = tuple(torch.cat((t[..., :-2, :], t[..., 1:-1, :], t[..., 2:, :]), dim = -2) for t in (k, v))
-        mask = torch.cat((mask[..., :-2], mask[..., 1:-1], mask[..., 2:]), dim = -1)
+        k, v = tuple(torch.cat((t[..., :-1, :], t[..., 1:, :]), dim = -2) for t in (k, v))
+        mask = torch.cat((mask[..., :-1], mask[..., 1:]), dim = -1)
 
         # handle attention bias (inefficiently)
 
         is_full_attn_bias = attn_bias.shape[-1] == attn_bias.shape[-2]
 
         if exists(attn_bias) and is_full_attn_bias:
             attn_bias = full_attn_bias_to_windowed(attn_bias, window_size = window_size)
@@ -395,15 +394,15 @@
     @typecheck
     def forward(
         self,
         q: Float['b h i d'],
         k: Float['b h j d'],
         v: Float['b h j d'],
         mask: Bool['b j'] | None = None,
-        attn_bias: Float['... i j'] | Float['... nw w (w*3)'] | None = None,
+        attn_bias: Float['... i j'] | Float['... nw w (w*2)'] | None = None,
     ) -> Float['b h i d']:
 
         is_windowed_attn_bias = None
 
         if exists(attn_bias):
             is_windowed_attn_bias = attn_bias.shape[-1] != attn_bias.shape[-2]
```

### Comparing `alphafold3_pytorch-0.1.1/alphafold3_pytorch/life.py` & `alphafold3_pytorch-0.1.4/alphafold3_pytorch/life.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/alphafold3_pytorch/trainer.py` & `alphafold3_pytorch-0.1.4/alphafold3_pytorch/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 # constants
 
 @typecheck
 class Alphafold3Input(TypedDict):
     atom_inputs:                Float['m dai']
     residue_atom_lens:          Int['n 2']
-    atompair_inputs:            Float['m m dap']
+    atompair_inputs:            Float['m m dapi'] | Float['nw w (w*2) dapi']
     additional_residue_feats:   Float['n 10']
     templates:                  Float['t n n dt']
-    template_mask:              Bool['t'] | None
     msa:                        Float['s n dm']
-    msa_mask:                   Bool['s'] | None
+    template_mask:              Bool[' t'] | None
+    msa_mask:                   Bool[' s'] | None
     atom_pos:                   Float['m 3'] | None
-    residue_atom_indices:       Int['n'] | None
+    residue_atom_indices:       Int[' n'] | None
     distance_labels:            Int['n n'] | None
     pae_labels:                 Int['n n'] | None
-    pde_labels:                 Int['n'] | None
-    resolved_labels:            Int['n'] | None
+    pde_labels:                 Int[' n'] | None
+    resolved_labels:            Int[' n'] | None
 
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(v, d):
@@ -402,8 +402,8 @@
 
             test_loss_breakdown = {f'test_{k}':v for k, v in test_loss_breakdown.items()}
 
             # log
 
             self.log(**test_loss_breakdown)
 
-        print(f'training complete')
+        print('training complete')
```

### Comparing `alphafold3_pytorch-0.1.1/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.1.4/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.1.4/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/tests/test_af3.py` & `alphafold3_pytorch-0.1.4/tests/test_af3.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/tests/test_trainer.py` & `alphafold3_pytorch-0.1.4/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/.gitignore` & `alphafold3_pytorch-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/LICENSE` & `alphafold3_pytorch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/README.md` & `alphafold3_pytorch-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.1.1/pyproject.toml` & `alphafold3_pytorch-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.1.1"
+version = "0.1.4"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
```

### Comparing `alphafold3_pytorch-0.1.1/PKG-INFO` & `alphafold3_pytorch-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.1.1
+Version: 0.1.4
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
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.1 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.1.4 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

