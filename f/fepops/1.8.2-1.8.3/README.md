# Comparing `tmp/fepops-1.8.2.tar.gz` & `tmp/fepops-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fepops-1.8.2.tar", last modified: Thu Nov  2 09:21:23 2023, max compression
+gzip compressed data, was "fepops-1.8.3.tar", last modified: Fri May 31 00:35:14 2024, max compression
```

## Comparing `fepops-1.8.2.tar` & `fepops-1.8.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.517123 fepops-1.8.2/
--rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.8.2/LICENSE.md
--rw-r--r--   0 justin    (1002) justin    (1002)    14406 2023-11-02 09:21:23.517123 fepops-1.8.2/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)    13588 2023-11-02 09:14:05.000000 fepops-1.8.2/README.md
--rw-rw-r--   0 justin    (1002) justin    (1002)     1158 2023-11-02 09:14:05.000000 fepops-1.8.2/pyproject.toml
--rw-rw-r--   0 justin    (1002) justin    (1002)       38 2023-11-02 09:21:23.517123 fepops-1.8.2/setup.cfg
--rw-rw-r--   0 justin    (1002) justin    (1002)       38 2023-08-06 20:41:37.000000 fepops-1.8.2/setup.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.397125 fepops-1.8.2/src/
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.477124 fepops-1.8.2/src/fepops/
--rw-rw-r--   0 justin    (1002) justin    (1002)       84 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/__init__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)     6489 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/__main__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)    41896 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/fepops.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.497124 fepops-1.8.2/src/fepops/fepops_persistent/
--rwxrwxr-x   0 justin    (1002) justin    (1002)      241 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/fepops_persistent/__init__.py
--rwxrwxr-x   0 justin    (1002) justin    (1002)    18945 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/fepops_persistent/fepops_persistent_abc.py
--rwxrwxr-x   0 justin    (1002) justin    (1002)     5870 2023-09-03 23:46:11.000000 fepops-1.8.2/src/fepops/fepops_persistent/fepopsdb_json.py
--rwxrwxr-x   0 justin    (1002) justin    (1002)     7690 2023-09-03 23:46:11.000000 fepops-1.8.2/src/fepops/fepops_persistent/fepopsdb_sqlite.py
--rw-rw-r--   0 justin    (1002) justin    (1002)      713 2023-10-10 11:27:29.000000 fepops-1.8.2/src/fepops/fepops_persistent/utils.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.505123 fepops-1.8.2/src/fepops/utils/
--rw-rw-r--   0 justin    (1002) justin    (1002)      158 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/utils/__init__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)     6425 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/utils/dude_preprocessor.py
--rw-rw-r--   0 justin    (1002) justin    (1002)     5627 2023-09-13 21:40:38.000000 fepops-1.8.2/src/fepops/utils/mol_filter.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.481124 fepops-1.8.2/src/fepops.egg-info/
--rw-r--r--   0 justin    (1002) justin    (1002)    14406 2023-11-02 09:21:23.000000 fepops-1.8.2/src/fepops.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)      657 2023-11-02 09:21:23.000000 fepops-1.8.2/src/fepops.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-11-02 09:21:23.000000 fepops-1.8.2/src/fepops.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)       61 2023-11-02 09:21:23.000000 fepops-1.8.2/src/fepops.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      194 2023-11-02 09:21:23.000000 fepops-1.8.2/src/fepops.egg-info/requires.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-11-02 09:21:23.000000 fepops-1.8.2/src/fepops.egg-info/top_level.txt
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-11-02 09:21:23.505123 fepops-1.8.2/tests/
--rw-rw-r--   0 justin    (1002) justin    (1002)     2305 2023-09-13 21:40:38.000000 fepops-1.8.2/tests/tests.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.969290 fepops-1.8.3/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.8.3/LICENSE.md
+-rw-r--r--   0 justin    (1002) justin    (1002)    14406 2024-05-31 00:35:14.969290 fepops-1.8.3/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)    13588 2023-11-02 09:14:05.000000 fepops-1.8.3/README.md
+-rw-rw-r--   0 justin    (1002) justin    (1002)     1158 2024-05-31 00:34:58.000000 fepops-1.8.3/pyproject.toml
+-rw-rw-r--   0 justin    (1002) justin    (1002)       38 2024-05-31 00:35:14.969290 fepops-1.8.3/setup.cfg
+-rw-rw-r--   0 justin    (1002) justin    (1002)       38 2023-08-06 20:41:37.000000 fepops-1.8.3/setup.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.965290 fepops-1.8.3/src/
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.965290 fepops-1.8.3/src/fepops/
+-rw-rw-r--   0 justin    (1002) justin    (1002)       84 2023-09-13 21:40:38.000000 fepops-1.8.3/src/fepops/__init__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     6493 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/__main__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)    42113 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/fepops.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.969290 fepops-1.8.3/src/fepops/fepops_persistent/
+-rwxrwxr-x   0 justin    (1002) justin    (1002)      241 2023-09-13 21:40:38.000000 fepops-1.8.3/src/fepops/fepops_persistent/__init__.py
+-rwxrwxr-x   0 justin    (1002) justin    (1002)    18949 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/fepops_persistent/fepops_persistent_abc.py
+-rwxrwxr-x   0 justin    (1002) justin    (1002)     5870 2023-09-03 23:46:11.000000 fepops-1.8.3/src/fepops/fepops_persistent/fepopsdb_json.py
+-rwxrwxr-x   0 justin    (1002) justin    (1002)     7696 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/fepops_persistent/fepopsdb_sqlite.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)      714 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/fepops_persistent/utils.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.969290 fepops-1.8.3/src/fepops/utils/
+-rw-rw-r--   0 justin    (1002) justin    (1002)      158 2023-09-13 21:40:38.000000 fepops-1.8.3/src/fepops/utils/__init__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     6441 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/utils/dude_preprocessor.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     5628 2024-05-31 00:13:58.000000 fepops-1.8.3/src/fepops/utils/mol_filter.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.969290 fepops-1.8.3/src/fepops.egg-info/
+-rw-r--r--   0 justin    (1002) justin    (1002)    14406 2024-05-31 00:35:14.000000 fepops-1.8.3/src/fepops.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)      657 2024-05-31 00:35:14.000000 fepops-1.8.3/src/fepops.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        1 2024-05-31 00:35:14.000000 fepops-1.8.3/src/fepops.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)       61 2024-05-31 00:35:14.000000 fepops-1.8.3/src/fepops.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)      194 2024-05-31 00:35:14.000000 fepops-1.8.3/src/fepops.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        7 2024-05-31 00:35:14.000000 fepops-1.8.3/src/fepops.egg-info/top_level.txt
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2024-05-31 00:35:14.969290 fepops-1.8.3/tests/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     2305 2023-09-13 21:40:38.000000 fepops-1.8.3/tests/tests.py
```

### Comparing `fepops-1.8.2/LICENSE.md` & `fepops-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fepops-1.8.2/PKG-INFO` & `fepops-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fepops
-Version: 1.8.2
+Version: 1.8.3
 Summary: OpenFEPOPS; A Python implementation of the FEPOPS molecular similarity method
 Author: Yan-Kai Chen, Steven Shave
 Project-URL: Homepage, https://github.com/JustinYKC/FEPOPS
 Keywords: molecular similarity,ligand based virtual screening
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `fepops-1.8.2/README.md` & `fepops-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `fepops-1.8.2/pyproject.toml` & `fepops-1.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="fepops"
-version="1.8.2"
+version="1.8.3"
 description="OpenFEPOPS; A Python implementation of the FEPOPS molecular similarity method"
 authors = [
     {name = "Yan-Kai Chen"},
     {name = "Steven Shave"},
 ]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `fepops-1.8.2/src/fepops/__main__.py` & `fepops-1.8.3/src/fepops/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import numpy as np
-import fire
 import json
 from pathlib import Path
 from typing import Optional
-from .fepops import OpenFEPOPS, GetFepopStatusCode
+
+import fire
+import numpy as np
+
+from .fepops import GetFepopStatusCode, OpenFEPOPS
 from .fepops_persistent import get_persistent_fepops_storage_object
 
 
 class FepopsCMDLineInterface:
     """Object to organise the command line interface to FEPOPS
 
     Used as an entrypoint to allow use of simply 'fepops' on the command line
```

### Comparing `fepops-1.8.2/src/fepops/fepops.py` & `fepops-1.8.3/src/fepops/fepops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from rdkit import Chem
-from rdkit.Chem import AllChem
-from rdkit.Chem import MolStandardize
-from rdkit.Chem import Crippen, Lipinski
-from rdkit.Chem import rdMolTransforms
-from sklearn.cluster import KMeans as _SKLearnKMeans
-from fast_pytorch_kmeans import KMeans as _FastPTKMeans
-from scipy.spatial.distance import cdist, squareform, pdist
-from scipy.special import softmax
-import numpy as np
-import itertools, zlib
-import torch
-from typing import Union, Optional, Tuple, Literal
-from enum import Enum
+import itertools
+import logging
 import multiprocessing as mp
+import zlib
+from enum import Enum
 from multiprocessing import SimpleQueue
-import logging
+from typing import Literal, Tuple, Union
+
+import numpy as np
+import torch
+from fast_pytorch_kmeans import KMeans as _FastPTKMeans
+from rdkit import Chem
+from rdkit.Chem import AllChem, Crippen, Lipinski, rdMolTransforms
+from rdkit.Chem.MolStandardize import rdMolStandardize
+from scipy.spatial.distance import cdist, pdist, squareform
+from scipy.special import softmax
+from sklearn.cluster import KMeans as _SKLearnKMeans
 
 GetFepopStatusCode = Enum(
     "GetFepopStatusCode",
     ["SUCCESS", "FAILED_TO_GENERATE", "FAILED_TO_RETRIEVE", "FAILED_RETRIEVED_NONE"],
 )
 
 
@@ -40,22 +40,22 @@
         "sklearn" is passed then Scikit-learn's kmeans implementation is used.
         However a faster implementation from the fast_pytorch_kmeans package can
         also be used if Pytorch is available and may be run in cpu-only mode, or
         GPU accelerated mode. Note: GPU accelerated mode should only be used if
         you are stretching the capabilities in terms of feature points for large
         molecules.  Small molecules will not benefit at all from GPU
         acceleration due to overheads.  By default "sklearn"
-    max_tautomers : Optional[int], optional
+    max_tautomers : Union[int, None], optional
         Maximum number of tautomers which should be generated. Internally, this
         implementation of FEPOPS relies upon RDKit's TautomerEnumerator to
-        generate tautomers and may optionally pass in a limit to the number of
-        Tautomers to generate. Unless the molecules (or macromolecules) you are
-        working with generate massive numbers of tautomers, this should be None
-        implying that no limit should be placed on tautomer generation. By
-        default None
+        generate tautomers and pass 5 to the number of tautomers to generate 
+        based on original FEPOPS paper. Unless the molecules (or macromolecules) 
+        you areworking with generate massive numbers of tautomers, this may 
+        optionally set as None implying that no limit should be placed on 
+        tautomer generation. By default 5
     num_fepops_per_mol : int, optional
         Number of feature points to use in the representation of a molecule.
         Literature notes that 7 has been empirically found to be a good number
         of feature points for performant representations of small molecules.
         This might be increased if you are dealing with large and very flexible
         molecules, by default 7
     num_centroids_per_fepop : int, optional
@@ -95,15 +95,15 @@
 
     """
 
     def __init__(
         self,
         *,
         kmeans_method: Literal['sklearn', 'pytorchcpu', 'pytorchgpu'] = 'sklearn',
-        max_tautomers: Optional[int] = None,
+        max_tautomers: Union[int, None] = 5,
         num_fepops_per_mol: int = 7,
         num_centroids_per_fepop: int = 4,
         descriptor_means: Tuple[float, ...] = (
             -0.28971602,
             0.5181022,
             0.37487135,
             0.99922747,
@@ -247,18 +247,19 @@
         self.donor_mol_from_smarts = Chem.MolFromSmarts("[!H0;#7,#8,#9]")
         self.acceptor_mol_from_smarts = Chem.MolFromSmarts(
             "[!$([#6,F,Cl,Br,I,o,s,nX3,#7v5,#15v5,#16v4,#16v6,*+1,*+2,*+3])]"
         )
         self.rotatable_bond_from_smarts = Chem.MolFromSmarts(
             "[!$(*#*)&!D1]-&!@[!$(*#*)&!D1]"
         )
-
-        self.tautomer_enumerator = MolStandardize.tautomer.TautomerEnumerator(
-            **{"max_tautomers": max_tautomers} if max_tautomers is not None else {}
-        )
+        self.tautomer_enumerator = rdMolStandardize.TautomerEnumerator()
+        if isinstance(max_tautomers, int):
+            self.tautomer_enumerator.SetMaxTautomers(max_tautomers)
+        if max_tautomers is None:
+            self.tautomer_enumerator.GetMaxTautomers()
 
     def _get_k_medoids(
         self, input_x: np.ndarray, k: int = 7, random_state: int = 42
     ) -> np.ndarray:
         """Select k FEPOPS from conformers and tautomers
 
         Gets k mediods from conformers (and tautomers) which are representative
@@ -849,17 +850,20 @@
             )
             return GetFepopStatusCode.FAILED_TO_GENERATE, None
         if Lipinski.HeavyAtomCount(mol) < self.num_centroids_per_fepop:
             logging.error(
                 f"Number of heavy atoms ({Lipinski.HeavyAtomCount(mol)}) below requested feature points ({self.num_centroids_per_fepop}) for molecule {original_smiles if original_smiles is not None else ''}"
             )
             return GetFepopStatusCode.FAILED_TO_GENERATE, None
-        mol = Chem.AddHs(mol)
+        mol = Chem.RemoveAllHs(mol)
 
-        tautomers_list = self.tautomer_enumerator.enumerate(mol)
+        tautomers_list = [
+            tautomer for tautomer in self.tautomer_enumerator.Enumerate(mol)
+        ]
+        tautomers_list = [Chem.AddHs(m_) for m_ in tautomers_list]
         each_mol_with_all_confs_list = []
         for index, t_mol in enumerate(tautomers_list):
             conf_list = self.generate_conformers(t_mol)
             each_mol_with_all_confs_list.extend(conf_list)
         if each_mol_with_all_confs_list == []:
             logging.error(
                 f"Failed to generate conformers/tautomers {' for '+original_smiles if original_smiles is not None else ''}"
```

### Comparing `fepops-1.8.2/src/fepops/fepops_persistent/fepops_persistent_abc.py` & `fepops-1.8.3/src/fepops/fepops_persistent/fepops_persistent_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import logging
+import multiprocessing as mp
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 from rdkit import Chem
 from scipy.spatial.distance import cdist, pdist, squareform
 from tqdm import tqdm
+
 from fepops.fepops import GetFepopStatusCode
+
 from ..fepops import OpenFEPOPS
-import multiprocessing as mp
-import logging
 
 
 class FepopsPersistentAbstractBaseClass(metaclass=ABCMeta):
     """Abstract base class for persistent fepops storage
 
     New storage methods may be implemented as demonstrated in fepopsdb_json.py
     or in fepopsdb_sqlite.py by extending this abstract base class which
```

### Comparing `fepops-1.8.2/src/fepops/fepops_persistent/fepopsdb_json.py` & `fepops-1.8.3/src/fepops/fepops_persistent/fepopsdb_json.py`

 * *Files identical despite different names*

### Comparing `fepops-1.8.2/src/fepops/fepops_persistent/fepopsdb_sqlite.py` & `fepops-1.8.3/src/fepops/fepops_persistent/fepopsdb_sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import bz2
 import sqlite3
 from pathlib import Path
 from typing import Union
-from rdkit import Chem
+
 import numpy as np
+from rdkit import Chem
+
 from fepops.fepops import GetFepopStatusCode
+
 from .fepops_persistent_abc import FepopsPersistentAbstractBaseClass
 
 
 class FepopsDBSqlite(FepopsPersistentAbstractBaseClass):
     """FepopsDBSqlite - allows reading and writing to a sqlite cache/database"""
 
     def __init__(
```

### Comparing `fepops-1.8.2/src/fepops/fepops_persistent/utils.py` & `fepops-1.8.3/src/fepops/fepops_persistent/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from . import FepopsDBSqlite, FepopsDBJSON
-from typing import Union
 from pathlib import Path
+from typing import Union
+
+from . import FepopsDBJSON, FepopsDBSqlite
 
 
 def get_persistent_fepops_storage_object(
     database_file: Union[str, Path],
     kmeans_method: str = "sklearn",
     parallel: bool = True,
     n_jobs: int = -1,
```

### Comparing `fepops-1.8.2/src/fepops/utils/dude_preprocessor.py` & `fepops-1.8.3/src/fepops/utils/dude_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Union, Optional
+import logging
+import multiprocessing as mp
 from pathlib import Path
-from tqdm import tqdm
-from fepops import OpenFEPOPS
+from typing import Optional, Union
+
 import pandas as pd
-import multiprocessing as mp
 from rdkit import Chem
-import logging
+from tqdm import tqdm
+
+from fepops import OpenFEPOPS
 
 
 class DudePreprocessor:
     def __init__(
         self,
         *,
         dude_directory: Union[Path, str] = "data/dude/",
@@ -144,15 +146,16 @@
         csv_path : Union[Path, str]
             Path of CSV file. If None, then all CSV files in the DUDE datasets
             processed path are used.
         rdkit_canonical_smiles_column_header : str, optional
             Column header containing RDKit canonical SMILES, by default
             "rdkit_canonical_smiles"
         """
-        from ...fepops.fepops_persistent import get_persistent_fepops_storage_object
+        from ...fepops.fepops_persistent import \
+            get_persistent_fepops_storage_object
 
         for csv_path in (
             [Path(csv_path)]
             if csv_path is not None
             else self.dude_processed_path.glob("dude_target_*.csv")
         ):
             df = pd.read_csv(csv_path)
```

### Comparing `fepops-1.8.2/src/fepops/utils/mol_filter.py` & `fepops-1.8.3/src/fepops/utils/mol_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Optional
+
 from rdkit import Chem
 from rdkit.Chem import rdMolDescriptors
 from rdkit.Chem.MolStandardize import rdMolStandardize
-from typing import Optional
 
 
 class Filter:
     """Filter molecules by property
 
     Filter object allows filtering by min atoms, max rings, and max rotatable
     bonds present within a molecule.
```

### Comparing `fepops-1.8.2/src/fepops.egg-info/PKG-INFO` & `fepops-1.8.3/src/fepops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fepops
-Version: 1.8.2
+Version: 1.8.3
 Summary: OpenFEPOPS; A Python implementation of the FEPOPS molecular similarity method
 Author: Yan-Kai Chen, Steven Shave
 Project-URL: Homepage, https://github.com/JustinYKC/FEPOPS
 Keywords: molecular similarity,ligand based virtual screening
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `fepops-1.8.2/src/fepops.egg-info/SOURCES.txt` & `fepops-1.8.3/src/fepops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fepops-1.8.2/tests/tests.py` & `fepops-1.8.3/tests/tests.py`

 * *Files identical despite different names*

