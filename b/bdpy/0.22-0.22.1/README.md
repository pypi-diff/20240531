# Comparing `tmp/bdpy-0.22.tar.gz` & `tmp/bdpy-0.22.1.tar.gz`

## Comparing `bdpy-0.22.tar` & `bdpy-0.22.1.tar`

### file list

```diff
@@ -1,70 +1,69 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/__init__.py
--rw-r--r--   0        0        0    28717 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/bdata.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/featureselector.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/metadata.py
--rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/__init__.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/datastore.py
--rw-r--r--   0        0        0    18041 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/features.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/pd.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/sparse.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/utils.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataset/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataset/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/distcomp/__init__.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/distcomp/distcomp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/caffe.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/base.py
--rw-r--r--   0        0        0    33330 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/models.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/torch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/evals/__init__.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/evals/metrics.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/feature/__init__.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/feature/feature.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/__init__.py
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/draw_group_image_set.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/fig.py
--rw-r--r--   0        0        0    26579 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/makeplots.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/tile_images.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/__init__.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/crossvalidation.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/ensemble.py
--rw-r--r--   0        0        0    21455 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/learning.py
--rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/model.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/regress.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/searchlight.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/__init__.py
--rw-r--r--   0        0        0    35073 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/fmriprep.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/glm.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/image.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/load_epi.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/load_mri.py
--rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/roi.py
--rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/spm.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/opendata/__init__.py
--rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/opendata/openneuro.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/pipeline/config.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/interface.py
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/preprocessor.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/select_top.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/util.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/__init__.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/utils.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/torch/__init__.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/torch/deep.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/torch/icnn.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/stats/__init__.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/stats/corr.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/info.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/math.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bdpy-0.22/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bdpy-0.22/LICENSE
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bdpy-0.22/README.md
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 bdpy-0.22/pyproject.toml
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 bdpy-0.22/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/bdata/__init__.py
+-rw-r--r--   0        0        0    28717 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/bdata/bdata.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/bdata/featureselector.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/bdata/metadata.py
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/bdata/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataform/__init__.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataform/datastore.py
+-rw-r--r--   0        0        0    18041 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataform/features.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataform/pd.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataform/sparse.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataform/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataset/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dataset/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/distcomp/__init__.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/distcomp/distcomp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dl/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dl/caffe.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dl/torch/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dl/torch/base.py
+-rw-r--r--   0        0        0    33330 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dl/torch/models.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/dl/torch/torch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/evals/__init__.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/evals/metrics.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/feature/__init__.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/feature/feature.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/fig/__init__.py
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/fig/draw_group_image_set.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/fig/fig.py
+-rw-r--r--   0        0        0    26579 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/fig/makeplots.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/fig/tile_images.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/__init__.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/crossvalidation.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/ensemble.py
+-rw-r--r--   0        0        0    21455 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/learning.py
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/model.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/regress.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/ml/searchlight.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/__init__.py
+-rw-r--r--   0        0        0    35073 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/fmriprep.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/glm.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/image.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/load_epi.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/load_mri.py
+-rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/roi.py
+-rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/mri/spm.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/opendata/__init__.py
+-rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/opendata/openneuro.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/pipeline/config.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/preproc/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/preproc/interface.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/preproc/preprocessor.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/preproc/select_top.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/preproc/util.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/recon/__init__.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/recon/utils.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/recon/torch/__init__.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/recon/torch/icnn.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/stats/__init__.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/stats/corr.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/util/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/util/info.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/util/math.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 bdpy-0.22.1/bdpy/util/utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bdpy-0.22.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bdpy-0.22.1/LICENSE
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bdpy-0.22.1/README.md
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 bdpy-0.22.1/pyproject.toml
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 bdpy-0.22.1/PKG-INFO
```

### Comparing `bdpy-0.22/bdpy/bdata/bdata.py` & `bdpy-0.22.1/bdpy/bdata/bdata.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/bdata/featureselector.py` & `bdpy-0.22.1/bdpy/bdata/featureselector.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/bdata/metadata.py` & `bdpy-0.22.1/bdpy/bdata/metadata.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/bdata/utils.py` & `bdpy-0.22.1/bdpy/bdata/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dataform/datastore.py` & `bdpy-0.22.1/bdpy/dataform/datastore.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dataform/features.py` & `bdpy-0.22.1/bdpy/dataform/features.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dataform/pd.py` & `bdpy-0.22.1/bdpy/dataform/pd.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dataform/sparse.py` & `bdpy-0.22.1/bdpy/dataform/sparse.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dataform/utils.py` & `bdpy-0.22.1/bdpy/dataform/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dataset/utils.py` & `bdpy-0.22.1/bdpy/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/distcomp/distcomp.py` & `bdpy-0.22.1/bdpy/distcomp/distcomp.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dl/caffe.py` & `bdpy-0.22.1/bdpy/dl/caffe.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dl/torch/base.py` & `bdpy-0.22.1/bdpy/dl/torch/base.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dl/torch/models.py` & `bdpy-0.22.1/bdpy/dl/torch/models.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/dl/torch/torch.py` & `bdpy-0.22.1/bdpy/dl/torch/torch.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/evals/metrics.py` & `bdpy-0.22.1/bdpy/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/feature/feature.py` & `bdpy-0.22.1/bdpy/feature/feature.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/fig/draw_group_image_set.py` & `bdpy-0.22.1/bdpy/fig/draw_group_image_set.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/fig/fig.py` & `bdpy-0.22.1/bdpy/fig/fig.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/fig/makeplots.py` & `bdpy-0.22.1/bdpy/fig/makeplots.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/fig/tile_images.py` & `bdpy-0.22.1/bdpy/fig/tile_images.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/ml/crossvalidation.py` & `bdpy-0.22.1/bdpy/ml/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/ml/ensemble.py` & `bdpy-0.22.1/bdpy/ml/ensemble.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/ml/learning.py` & `bdpy-0.22.1/bdpy/ml/learning.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/ml/model.py` & `bdpy-0.22.1/bdpy/ml/model.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/ml/regress.py` & `bdpy-0.22.1/bdpy/ml/regress.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/ml/searchlight.py` & `bdpy-0.22.1/bdpy/ml/searchlight.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/fmriprep.py` & `bdpy-0.22.1/bdpy/mri/fmriprep.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/glm.py` & `bdpy-0.22.1/bdpy/mri/glm.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/image.py` & `bdpy-0.22.1/bdpy/mri/image.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/load_epi.py` & `bdpy-0.22.1/bdpy/mri/load_epi.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/load_mri.py` & `bdpy-0.22.1/bdpy/mri/load_mri.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/roi.py` & `bdpy-0.22.1/bdpy/mri/roi.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/mri/spm.py` & `bdpy-0.22.1/bdpy/mri/spm.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/opendata/openneuro.py` & `bdpy-0.22.1/bdpy/opendata/openneuro.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/pipeline/config.py` & `bdpy-0.22.1/bdpy/pipeline/config.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/preproc/interface.py` & `bdpy-0.22.1/bdpy/preproc/interface.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/preproc/preprocessor.py` & `bdpy-0.22.1/bdpy/preproc/preprocessor.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/preproc/select_top.py` & `bdpy-0.22.1/bdpy/preproc/select_top.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-"""
-select_top
+"""select_top.
 
 This file is a part of BdPy.
 """
 
 
 __all__ = ['select_top']
 
 
+from typing import Tuple, Optional
 import numpy as np
 from .util import print_start_msg, print_finish_msg
 
 
-def select_top(data, value, num, axis=0, verbose=True):
-    """
-    Select top `num` features of `value` from `data`
+def select_top(data: np.ndarray, value: np.ndarray, num: int, axis: Optional[int] = 0, verbose: Optional[bool] = True) -> Tuple[np.ndarray, np.ndarray]:
+    """Select top `num` features of `value` from `data`.
 
     Parameters
     ----------
     data : array
        Data matrix
     value : array_like
        Vector of values
@@ -27,35 +26,35 @@
 
     Returns
     -------
     selected_data : array
         Selected data matrix
     selected_index : array
         Index of selected data
-    """
 
+    """
     if verbose:
         print_start_msg()
 
     num_elem = data.shape[axis]
 
     value = np.array([-np.inf if np.isnan(a) else a for a in value])
     sorted_index = np.argsort(value)[::-1]
 
-    rank = np.zeros(num_elem, dtype=np.uint8)
+    rank = np.zeros(num_elem, dtype=int)
     rank[sorted_index] = np.array(range(0, num_elem))
 
     selected_index_bool = rank < num
 
     if axis == 0:
         selected_data = data[selected_index_bool, :]
-        selected_index = np.array(range(0, num_elem), dtype=np.uint8)[selected_index_bool]
+        selected_index = np.array(range(0, num_elem), dtype=int)[selected_index_bool]
     elif axis == 1:
         selected_data = data[:, selected_index_bool]
-        selected_index = np.array(range(0, num_elem), dtype=np.uint8)[selected_index_bool]
+        selected_index = np.array(range(0, num_elem), dtype=int)[selected_index_bool]
     else:
         raise ValueError('Invalid axis')
 
     if verbose:
         print_finish_msg()
 
     return selected_data, selected_index
```

### Comparing `bdpy-0.22/bdpy/recon/utils.py` & `bdpy-0.22.1/bdpy/recon/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/recon/torch/icnn.py` & `bdpy-0.22.1/bdpy/recon/torch/icnn.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/stats/corr.py` & `bdpy-0.22.1/bdpy/stats/corr.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/util/info.py` & `bdpy-0.22.1/bdpy/util/info.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/util/math.py` & `bdpy-0.22.1/bdpy/util/math.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/bdpy/util/utils.py` & `bdpy-0.22.1/bdpy/util/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/LICENSE` & `bdpy-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/README.md` & `bdpy-0.22.1/README.md`

 * *Files identical despite different names*

### Comparing `bdpy-0.22/pyproject.toml` & `bdpy-0.22.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bdpy"
-version = "0.22"
+version = "0.22.1"
 description = "Brain decoder toolbox for Python"
 authors = [
     { name = "Shuntaro C. Aoki", email = "s_aoki@i.kyoto-u.ac.jp" }
 ]
 readme = "README.md"
 requires-python = ">= 3.6, < 3.12"
 license = { file = "LICENSE" }
```

### Comparing `bdpy-0.22/PKG-INFO` & `bdpy-0.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bdpy
-Version: 0.22
+Version: 0.22.1
 Summary: Brain decoder toolbox for Python
 Project-URL: Homepage, https://github.com/KamitaniLab/bdpy
 Project-URL: Repository, https://github.com/KamitaniLab/bdpy
 Project-URL: Bug Tracker, https://github.com/KamitaniLab/bdpy/issues
 Author-email: "Shuntaro C. Aoki" <s_aoki@i.kyoto-u.ac.jp>
 License: MIT License
```

