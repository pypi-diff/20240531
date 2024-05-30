# Comparing `tmp/ensemble_networkx-2024.2.5.tar.gz` & `tmp/ensemble_networkx-2024.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_networkx-2024.2.5.tar", last modified: Tue Feb  6 01:49:23 2024, max compression
+gzip compressed data, was "ensemble_networkx-2024.5.30.tar", last modified: Thu May 30 22:23:04 2024, max compression
```

## Comparing `ensemble_networkx-2024.2.5.tar` & `ensemble_networkx-2024.5.30.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2024-02-06 01:49:23.415560 ensemble_networkx-2024.2.5/
--rw-r--r--   0 jespinoz  (3456) staff       (20)     1563 2023-08-15 22:05:31.000000 ensemble_networkx-2024.2.5/LICENSE
--rw-r--r--   0 jespinoz  (3456) staff       (20)      252 2024-02-06 01:49:23.415123 ensemble_networkx-2024.2.5/PKG-INFO
--rw-r--r--   0 jespinoz  (3456) staff       (20)    26226 2023-09-05 21:01:45.000000 ensemble_networkx-2024.2.5/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2024-02-06 01:49:23.409516 ensemble_networkx-2024.2.5/ensemble_networkx/
--rw-r--r--   0 jespinoz  (3456) staff       (20)     1099 2024-02-06 01:45:19.000000 ensemble_networkx-2024.2.5/ensemble_networkx/__init__.py
--rw-r--r--   0 jespinoz  (3456) staff       (20)   161001 2024-02-06 01:48:29.000000 ensemble_networkx-2024.2.5/ensemble_networkx/ensemble_networkx.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2024-02-06 01:49:23.414440 ensemble_networkx-2024.2.5/ensemble_networkx.egg-info/
--rw-------   0 jespinoz  (3456) staff       (20)      252 2024-02-06 01:49:22.000000 ensemble_networkx-2024.2.5/ensemble_networkx.egg-info/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)      299 2024-02-06 01:49:22.000000 ensemble_networkx-2024.2.5/ensemble_networkx.egg-info/SOURCES.txt
--rw-------   0 jespinoz  (3456) staff       (20)        1 2024-02-06 01:49:22.000000 ensemble_networkx-2024.2.5/ensemble_networkx.egg-info/dependency_links.txt
--rw-------   0 jespinoz  (3456) staff       (20)      134 2024-02-06 01:49:22.000000 ensemble_networkx-2024.2.5/ensemble_networkx.egg-info/requires.txt
--rw-------   0 jespinoz  (3456) staff       (20)       18 2024-02-06 01:49:22.000000 ensemble_networkx-2024.2.5/ensemble_networkx.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2024-02-06 01:49:23.415697 ensemble_networkx-2024.2.5/setup.cfg
--rw-r--r--   0 jespinoz  (3456) staff       (20)      917 2023-09-26 00:33:32.000000 ensemble_networkx-2024.2.5/setup.py
+drwxr-xr-x   0 jolespin   (501) staff       (20)        0 2024-05-30 22:23:04.455750 ensemble_networkx-2024.5.30/
+-rw-------   0 jolespin   (501) staff       (20)     1563 2023-08-15 22:05:37.000000 ensemble_networkx-2024.5.30/LICENSE
+-rw-r--r--   0 jolespin   (501) staff       (20)      522 2024-05-30 22:23:04.455537 ensemble_networkx-2024.5.30/PKG-INFO
+-rw-------   0 jolespin   (501) staff       (20)    26227 2024-02-06 21:03:54.000000 ensemble_networkx-2024.5.30/README.md
+drwxr-xr-x   0 jolespin   (501) staff       (20)        0 2024-05-30 22:23:04.454590 ensemble_networkx-2024.5.30/ensemble_networkx/
+-rw-------   0 jolespin   (501) staff       (20)     1287 2024-05-30 22:22:35.000000 ensemble_networkx-2024.5.30/ensemble_networkx/__init__.py
+-rw-------   0 jolespin   (501) staff       (20)   168124 2024-05-30 22:18:23.000000 ensemble_networkx-2024.5.30/ensemble_networkx/ensemble_networkx.py
+drwxr-xr-x   0 jolespin   (501) staff       (20)        0 2024-05-30 22:23:04.455284 ensemble_networkx-2024.5.30/ensemble_networkx.egg-info/
+-rw-r--r--   0 jolespin   (501) staff       (20)      522 2024-05-30 22:23:04.000000 ensemble_networkx-2024.5.30/ensemble_networkx.egg-info/PKG-INFO
+-rw-------   0 jolespin   (501) staff       (20)      299 2024-05-30 22:23:04.000000 ensemble_networkx-2024.5.30/ensemble_networkx.egg-info/SOURCES.txt
+-rw-------   0 jolespin   (501) staff       (20)        1 2024-05-30 22:23:04.000000 ensemble_networkx-2024.5.30/ensemble_networkx.egg-info/dependency_links.txt
+-rw-------   0 jolespin   (501) staff       (20)      134 2024-05-30 22:23:04.000000 ensemble_networkx-2024.5.30/ensemble_networkx.egg-info/requires.txt
+-rw-------   0 jolespin   (501) staff       (20)       18 2024-05-30 22:23:04.000000 ensemble_networkx-2024.5.30/ensemble_networkx.egg-info/top_level.txt
+-rw-r--r--   0 jolespin   (501) staff       (20)       38 2024-05-30 22:23:04.455805 ensemble_networkx-2024.5.30/setup.cfg
+-rw-------   0 jolespin   (501) staff       (20)      917 2023-09-26 00:33:40.000000 ensemble_networkx-2024.5.30/setup.py
```

### Comparing `ensemble_networkx-2024.2.5/LICENSE` & `ensemble_networkx-2024.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemble_networkx-2024.2.5/README.md` & `ensemble_networkx-2024.5.30/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 ### Ensemble NetworkX
 High-level [Ensemble](https://en.wikipedia.org/wiki/Ensemble_averaging_(machine_learning)) Network implementations in Python.  Built on top of [NetworkX](https://github.com/networkx/networkx) and [Pandas](https://pandas.pydata.org/).  
 
 #### Dependencies:
 Compatible for Python 3.
 
-    panda
+    pandas
     numpy
     scipy
     networkx
     matplotlib
     soothsayer_utils
     compositional
```

### Comparing `ensemble_networkx-2024.2.5/ensemble_networkx/__init__.py` & `ensemble_networkx-2024.5.30/ensemble_networkx/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/usr/env python
 #
 # =======
 # Version
 # =======
-__version__= "2024.2.5"
+__version__= "2024.5.30"
 __author__ = "Josh L. Espinoza"
 __email__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"
 __url__ = "https://github.com/jolespin/ensemble_networkx"
 __license__ = "BSD-3"
 __developmental__ = True
 
 # =======
@@ -20,14 +20,18 @@
 ] + [
     "get_symmetric_category",
     "redundant_to_condensed",
     "condensed_to_redundant",
     "convert_network",
 ] + [
     "connectivity",
+    "grouped_node_connectivity_from_numpy", 
+    "grouped_node_connectivity_from_pandas_dataframe", 
+    "group_connectivity_from_numpy", 
+    "group_connectivity_from_pandas_dataframe",
     "density",
     "centralization",
     "heterogeneity",
     "entropy",
     "evenness",
     "topological_overlap_measure",
     "community_detection",
```

### Comparing `ensemble_networkx-2024.2.5/ensemble_networkx/ensemble_networkx.py` & `ensemble_networkx-2024.5.30/ensemble_networkx/ensemble_networkx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, division
 
 # ==============================================================================
 # Modules
 # ==============================================================================
 # Built-ins
-import os, sys, time, datetime, copy, warnings
+import os, sys, time, datetime, copy, warnings, itertools
 from typing import Dict, Union, Any
 from collections import defaultdict, OrderedDict
 from collections.abc import Mapping, Hashable
 from itertools import combinations, product
 
 # Packages
 import pandas as pd
 import numpy as np
 import networkx as nx
 import igraph as ig
-import xarray as xr
+# import xarray as xr
 from scipy import stats
 from scipy.special import comb
 from scipy.spatial.distance import squareform, pdist
 from sklearn.base import clone, is_classifier, is_regressor
 from sklearn.exceptions import ConvergenceWarning, UndefinedMetricWarning
 
 # Compositional
 from compositional import pairwise_rho, pairwise_phi, pairwise_partial_correlation_with_basis_shrinkage
 
 # soothsayer_utils
-from soothsayer_utils import pv, flatten, assert_acceptable_arguments, is_symmetrical, is_graph, write_object, format_memory, format_header, format_path, is_nonstring_iterable, Suppress, dict_build, dict_filter, is_dict, is_dict_like, is_color, is_number, check_packages, is_query_class
+from soothsayer_utils import pv, flatten, assert_acceptable_arguments, is_symmetrical, is_graph, write_object, format_memory, format_header, format_path, is_nonstring_iterable, Suppress, dict_build, is_dict, is_dict_like, is_number, check_packages, is_query_class
 
 try:
     from . import __version__
 except ImportError:
     __version__ = "ImportError: attempted relative import with no known parent package"
 
 
@@ -54,15 +54,15 @@
     return pd.Series(data, index=index, name=name)
 
 # pd.Series to pd.DataFrame 2D
 def condensed_to_redundant(y:pd.Series, fill_diagonal=None, index=None):
 
     # Need to optimize this
     data = defaultdict(dict)
-    for edge, w in y.iteritems():
+    for edge, w in y.items():
         number_of_unique_nodes = len(edge)
         if len(edge) == 2:
             node_a, node_b = tuple(edge)
         else:
             node_a = node_b = list(edge)[0]
             
         data[node_a][node_b] = data[node_b][node_a] = w
@@ -110,14 +110,15 @@
     # I/O
     data, 
     into, 
     
     # Subgraphs
     node_subgraph:list=None, 
     edge_subgraph:list=None, 
+    nodes_ordering=None, # Only applies to pd.DataFrame
         
     # Symmetry
     remove_self_interactions:bool=True,
     assert_symmetry=True, 
     tol=None, 
 
     # Missing values
@@ -144,27 +145,43 @@
     input_category = get_symmetric_category(data)
     output_category = get_symmetric_category(into)
 
     assert output_category in {("pandas", "Series"), ("pandas", "DataFrame"), "Symmetric", "networkx", "igraph"}, "`data` must be either a pandas[Series, DataFrame], ensemble_networkx[Symmetric], networkx[Graph, DiGraph, OrdereredGraph, DiOrderedGraph], igraph[Graph]"
     assert isinstance(into, type), "`into` must be an instantiated object: a pandas[Series, DataFrame], ensemble_networkx[Symmetric], networkx[Graph, DiGraph, OrdereredGraph, DiOrderedGraph], igraph[Graph]"
     assert into not in {nx.MultiGraph, nx.MultiDiGraph},  "`into` cannot be a `Multi[Di]Graph`"
     
-    
     assert not (node_subgraph is not None) & (edge_subgraph is not None), "Cannot create subgraph from `node_subgraph` and `edge_subgraph`"
+    if (nodes_ordering is not None) & (node_subgraph is not None):
+        assert set(nodes_ordering) == set(node_subgraph), "nodes_ordering elements must be the same as node_subgraph"
+        
+    if all([
+        input_category == "Symmetric",
+        output_category == ("pandas", "DataFrame"),
+        nodes_ordering is None,
+        ]):
+        raise Exception("Please provide `nodes_ordering` if input_type is Symmetric and output_type is pd.DataFrame.  Alternatively, use Symmetric's .to_pandas_dataframe() method")
+    
+    if all([
+        input_category == ("pandas", "DataFrame"),
+        output_category == "Symmetric",
+        ]):
+        raise Exception("Please provide instantiate a Symmetric object from a pd.DataFrame directly via `Symmetric(df)`")
     
     if all([
         input_category == output_category,
         node_subgraph is None, 
         edge_subgraph is None, 
         remove_self_interactions == False,
         ]):
         return data.copy()
     
     _attrs = dict()
     
+    
+
     # Convert to pd.Series
     if input_category == "igraph":
         # iGraph -> NetworkX
         if all([
             output_category == "network",
             node_subgraph is None, 
             edge_subgraph is None, 
@@ -256,15 +273,20 @@
             
     # Output
     if output_category == ("pandas", "Series"):
         data.name = _attrs.get("name", None)
         return data
     
     if output_category == ("pandas", "DataFrame"):
-        return condensed_to_redundant(data, fill_diagonal=fill_diagonal)
+        df = condensed_to_redundant(data, fill_diagonal=fill_diagonal)
+        if nodes_ordering is not None:
+            nodes_ordering = pd.Index(nodes_ordering)
+            if not np.all(df.index == nodes_ordering):
+                df = df.loc[nodes_ordering, nodes_ordering]
+        return df
     
     if output_category == "networkx":
         graph = into(**_attrs)
         for edge, w in data.items():
             if len(edge) == 1:
                 node_a = node_b = list(edge)[0]
             else:
@@ -290,74 +312,205 @@
     if output_category == "Symmetric":
         return Symmetric(data=data, **_attrs)
     
 # ===================
 # Network Statistics
 # ===================
 # Connectivity
-def connectivity(data, groups:pd.Series=None, remove_self_interactions=True, tol=1e-10):
+def grouped_node_connectivity_from_numpy(data:np.ndarray, groups:np.ndarray, labels=None, preserve_order=True):
+    """
+    Get grouped node connectivity from a symmetric matrix
+
+    Input:
+        data: symmetric matrix of connectivities (n,n)
+        groups: array of groups (n,)
+    Output:
+        pd.DataFrame of connectivities
+    """
+    index_sorted = np.argsort(groups)
+    groups = groups[index_sorted]
+    data = data[index_sorted,:][:,index_sorted]
+    if labels is not None:
+        number_of_labels = len(labels)
+        assert number_of_labels == data.shape[0], "labels must be same size as data.shape[0]"
+        assert number_of_labels == data.shape[1], "labels must be same size as data.shape[1]"
+        assert number_of_labels == groups.size, "labels must be same size as group.size"
+        labels_unsorted = np.asarray(labels)
+        labels_sorted = np.asarray(labels_unsorted)[index_sorted]
+    
+    # Group by the values in y and track the positions
+    data_connectivity = OrderedDict()
+    for id_group, index_group in itertools.groupby(enumerate(groups), key=lambda x: x[1]):
+        # Get boolean mask for clustres
+        positions = list(map(lambda x: x[0], index_group))
+        mask = np.zeros(groups.size, dtype=bool)
+        mask[positions] = True
+        
+        # Subset data by query group
+        data_group = data[mask,:]
+
+        n_intra_cluster = np.sum(mask)
+        n_inter_cluster = np.sum(~mask)
+
+        for _i, connectivities in enumerate(data_group):
+            i = positions[_i]
+
+            intra_group_connectivities_sum = connectivities[mask].sum()
+            inter_group_connectivities_sum = connectivities[~mask].sum()
+            data_connectivity[i] = OrderedDict([
+        # Unscaled
+         ("total_connectivity",  intra_group_connectivities_sum + inter_group_connectivities_sum),
+         ("intra-group_connectivity",  intra_group_connectivities_sum),
+         ("inter-group_connectivity",  inter_group_connectivities_sum),
+        # Scaled
+         ("total_connectivity(scaled)",  (intra_group_connectivities_sum + inter_group_connectivities_sum)/(n_intra_cluster + n_inter_cluster)),
+         ("intra-group_connectivity(scaled)",  intra_group_connectivities_sum/n_intra_cluster),
+         ("inter-group_connectivity(scaled)",  inter_group_connectivities_sum/n_inter_cluster),
+        ])
+    df_connectivity = pd.DataFrame(data_connectivity).T
+    if labels is not None:
+        df_connectivity.index = labels_sorted
+        if preserve_order:
+            df_connectivity = df_connectivity.loc[labels_unsorted]
+    else:
+        if preserve_order:
+            df_connectivity = df_connectivity.sort_index()
+    df_connectivity.index.name = "id_node"
+    return df_connectivity
+
+def grouped_node_connectivity_from_pandas_dataframe(data:pd.DataFrame, groups:pd.Series, preserve_order=True, checks=True):
+        """
+        Get grouped node connectivity from a symmetric pd.DataFrame
+    
+        Input:
+            data: symmetric pd.DataFrame of connectivities (n,n)
+            groups: pd.Series of groups (n,)
+        Output:
+            pd.DataFrame of connectivities
+        """
+        if checks:
+            assert np.all(data.index == groups.index), "data.index must be the same as groups.index"
+        df_connectivity = grouped_node_connectivity_from_numpy(data.values, groups.values, labels=data.index, preserve_order=preserve_order)
+        return df_connectivity
+
+
+def group_connectivity_from_numpy(data:np.ndarray, groups:np.ndarray) -> pd.DataFrame:
+    """
+    Get grouped connectivity from a symmetric matrix
+
+    Input:
+        data: symmetric matrix of connectivities (n,n)
+        groups: array of groups (n,)
+    Output:
+        pd.DataFrame of connectivities
+    """
+    index_sorted = np.argsort(groups)
+    groups = groups[index_sorted]
+    data = data[index_sorted,:][:,index_sorted]
+    
+    # Group by the values in y and track the positions
+    data_connectivity = OrderedDict()
+    for id_group, index_group in itertools.groupby(enumerate(groups), key=lambda x: x[1]):
+        # Get boolean mask for clustres
+        positions = list(map(lambda x: x[0], index_group))
+        mask = np.zeros(groups.size, dtype=bool)
+        mask[positions] = True
+        
+        # Subset data by query group
+        data_group = data[mask,:]
+        
+        # Triangle of intra-group connectivities
+        intra_group_connectivities = squareform(data_group[:,mask])
+        intra_group_connectivities_sum = intra_group_connectivities.sum()
+        
+        # Flatten inter-group connectivities
+        inter_group_connectivities = data_group[:,~mask]
+        inter_group_connectivities_sum = inter_group_connectivities.sum()
+
+        # Build output table
+        data_connectivity[id_group] = OrderedDict([
+        # Unscaled
+         ("total_connectivity",  intra_group_connectivities_sum + inter_group_connectivities_sum),
+         ("intra-group_connectivity",  intra_group_connectivities_sum),
+         ("inter-group_connectivity",  inter_group_connectivities_sum),
+        # Scaled
+         ("total_connectivity(scaled)",  (intra_group_connectivities_sum + inter_group_connectivities_sum)/(intra_group_connectivities.size + inter_group_connectivities.size)),
+         ("intra-group_connectivity(scaled)",  intra_group_connectivities_sum/intra_group_connectivities.size),
+         ("inter-group_connectivity(scaled)",  inter_group_connectivities_sum/inter_group_connectivities.size),
+        ])
+    df_connectivity = pd.DataFrame(data_connectivity).T
+    df_connectivity.index.name = "id_group"
+    return df_connectivity
+
+def group_connectivity_from_pandas_dataframe(data:pd.DataFrame, groups:pd.Series, checks=True) -> pd.DataFrame:
+    """
+    Get grouped connectivity from a symmetric matrix
+
+    Input:
+        data: symmetric pd.DataFrame of connectivities (n,n)
+        groups: pd.Series of groups (n,)
+    Output:
+        pd.DataFrame of connectivities
+    """
+    if checks:
+        assert np.all(data.index == groups.index), "data.index must be the same as groups.index"
+    df_connectivity = group_connectivity_from_numpy(data.values, groups.values)
+    return df_connectivity
+
+def connectivity(data, groups:pd.Series=None, return_type="nodes", outlier_group=None, preserve_order=True, remove_self_interactions=True,  tol=1e-10):
     """
     Calculate connectivity from pd.DataFrame (must be symmetric), Symmetric, Hive, or NetworkX graph
+    Input: 
+        data: symmetric pd.DataFrame of connectivities (n,n)
+        groups: pd.Series of groups (n,)
+        return_type: Connectivities on nodes or groups 
+        outlier_group: Group value for outliers (e.g., -1)
+    Output: 
+        pd.DataFrame of connectivities if groups are provided else pd.Series of connectivities
+    
     
-    groups must be dict-like: {node:group}
     """
+    # Return type
+    assert_acceptable_arguments(return_type, {"nodes", "groups"})
+    if return_type == "groups":
+        assert groups is not None, "Must provide groups if return_type=groups"
+        
     # This is a hack to allow Hives from hive_networkx
     if is_query_class(data, "Hive"):
         data = data.weights
-    # assert isinstance(data, (pd.DataFrame, Symmetric, nx.Graph, nx.DiGraph, nx.OrderedGraph, nx.OrderedDiGraph)), "Must be either a symmetric pd.DataFrame, Symmetric, nx.Graph, or hx.Hive object"
-#     if is_graph(data):
-#         weights = dict()
-#         for edge_data in data.edges(data=True):
-#             edge = frozenset(edge_data[:-1])
-#             weight = edge_data[-1]["weight"]
-#             weights[edge] = weight
-#         weights = pd.Series(weights, name="Weights")#.sort_index()
-#         data = Symmetric(weights)
-#     if isinstance(data, Symmetric):
-#         df_redundant = condensed_to_redundant(data.weights)
-
-#     if isinstance(data, pd.DataFrame):
-#         assert is_symmetrical(data, tol=tol)
-#         df_redundant = data
 
     if not isinstance(data, pd.DataFrame):
         df_redundant = convert_network(data=data, into=pd.DataFrame, remove_missing_values=False, remove_self_interactions=False, tol=tol)
     else:
         assert is_symmetrical(X=data, tol=tol, nans_ok=True)
         df_redundant = data.copy()
         
     if remove_self_interactions:
         np.fill_diagonal(df_redundant.values, 0)
 
     #kTotal
-    k_total = df_redundant.sum(axis=1)
+    number_of_nodes = df_redundant.shape[0]
+    
     
     if groups is None:
+        k_total = df_redundant.sum(axis=1)
+        k_total.name = "total_connectivity"
         return k_total
     else:
-        groups = pd.Series(groups)
-        data_connectivity = OrderedDict()
-        
-        data_connectivity["kTotal"] = k_total
-        
-        #kWithin
-        k_within = list()
-        for group in groups.unique():
-            index_nodes = pd.Index(sorted(set(groups[lambda x: x == group].index) & set(df_redundant.index)))
-            k_group = df_redundant.loc[index_nodes,index_nodes].sum(axis=1)
-            k_within.append(k_group)
-        data_connectivity["kWithin"] = pd.concat(k_within)
-        
-        #kOut
-        data_connectivity["kOut"] = data_connectivity["kTotal"] - data_connectivity["kWithin"]
-
-        #kDiff
-        data_connectivity["kDiff"] = data_connectivity["kWithin"] - data_connectivity["kOut"]
-
-        return pd.DataFrame(data_connectivity)
+        # Remove outlier group if any exist
+        groups = pd.Series(groups).loc[data.index]
+        if outlier_group is not None:
+            inverse_mask = groups.map(lambda x: x != outlier_group).values
+            df_redundant = df_redundant.iloc[inverse_mask, inverse_mask]
+            groups = groups.iloc[inverse_mask]
+        
+        if return_type == "nodes":
+            return grouped_node_connectivity_from_pandas_dataframe(df_redundant, groups, preserve_order=preserve_order)
+        if return_type == "groups":
+            return group_connectivity_from_pandas_dataframe(df_redundant, groups)
 
 def density(k:pd.Series):
     """
     Density = sum(khelp)/(nGenes * (nGenes - 1))
     https://github.com/cran/WGCNA/blob/15de0a1fe2b214f7047b887e6f8ccbb1c681e39e/R/Functions.R#L1963
     """
     k_total = k.sum()
@@ -891,14 +1044,17 @@
     #     (iris_149, iris_146)    0.986481
     #     (iris_147, iris_148)    0.995708
     #     (iris_149, iris_147)    0.994460
     #     (iris_149, iris_148)    0.999916
     =====
     devel
     =====
+    2024-May-28
+    * Removed .iteritems method
+    
     2022-Feb-12
     * Completely rewrote Symmetric to clean it up. A little slower but much easier to prototype
     
     2022-Feb-08
     * Added support for iGraph
     * Added support for non-fully-connected graphs
     
@@ -976,14 +1132,21 @@
                 tol=tol, 
                 remove_missing_values=remove_missing_values, 
                 fill_missing_values_with=fill_missing_values_with,
                 name="Weights",
             )
             self.edges = pd.Index(self.weights.index, name="Edges")
             self.nodes = pd.Index(sorted(frozenset.union(*self.weights.index)), name="Nodes")
+
+            if isinstance(data, pd.DataFrame):
+                self.nodes_ordering = data.index
+            else:
+                if hasattr(data, "nodes_ordering"):
+                    self.nodes_ordering = getattr(data, "nodes_ordering")
+                self.nodes_ordering = self.nodes
             
             # Set keywords
             for k, v in kwargs.items():
                 setattr(self, k, v)
 
         # If there's still no `edge_type` and `func_metric` is not empty, then use this the name of `func_metric`
         if (self.edge_type is None) and (self.func_metric is not None):
@@ -1074,16 +1237,14 @@
     def __len__(self):
         return self.number_of_edges
     def __iter__(self):
         for v in self.weights:
             yield v
     def items(self):
         return self.weights.items()
-    def iteritems(self):
-        return self.weights.iteritems()
     def keys(self):
         return self.weights.keys()
     def apply(self, func):
         return func(self.weights)
     def mean(self):
         return self.weights.mean()
     def median(self):
@@ -1173,27 +1334,31 @@
     # def to_redundant(self, node_subgraph=None, fill_diagonal=None):
     #     if fill_diagonal is None:
     #         fill_diagonal = self.diagonal
     #     if node_subgraph is None:
     #         node_subgraph = self.nodes
     #     return condensed_to_redundant(y=self.weights, fill_diagonal=fill_diagonal, index=node_subgraph)
     
-    def to_pandas_dataframe(self, node_subgraph=None, edge_subgraph=None, fill_diagonal=None, vertical=False, **convert_network_kws):
+    def to_pandas_dataframe(self, node_subgraph=None, edge_subgraph=None, fill_diagonal=None, vertical=False,  **convert_network_kws):
+        
         # df = self.to_redundant(node_subgraph=node_subgraph, fill_diagonal=fill_diagonal)
         if fill_diagonal is None:
             fill_diagonal = self.diagonal
         if (node_subgraph is None) & (edge_subgraph is None):
-            node_subgraph = self.nodes
-        
+            # assert edge_subgraph is None, "Cannot provide both node_subgraph and edge_subgraph"
+            node_subgraph = self.nodes_ordering
+        # if edge_subgraph is None:
+        #     assert node_subgraph is None, "Cannot provide both node_subgraph and edge_subgraph"
         df = convert_network(
             data=self.weights, 
             into=pd.DataFrame,
             node_subgraph=node_subgraph,
             edge_subgraph=edge_subgraph,
             fill_diagonal=fill_diagonal,
+            nodes_ordering=self.nodes_ordering,
             **convert_network_kws,
         )
             
         if vertical:
             df = df.stack().to_frame().reset_index()
             df.columns = ["Node_A", "Node_B", "Weight"]
             df.index.name = "Edge_Index"
@@ -1571,17 +1736,15 @@
     def __len__(self):
         return len(self.engineered_to_initial_features_)
     def __iter__(self):
         for v in self.engineered_to_initial_features_.items():
             yield v
     def items(self):
         return self.engineered_to_initial_features_.items()
-    def iteritems(self):
-        for v in self.engineered_to_initial_features_.items():
-            yield v
+
             
     def to_file(self, path, **kwargs):
         write_object(obj=self, path=path, **kwargs)
 
     def copy(self):
         return copy.deepcopy(self)
 
@@ -3253,23 +3416,14 @@
         assert level in {"nodes", "edges"}
         if level == "edges":
             weights = self.edge_weights_.copy()
         if level == "nodes":
             weights = self.node_weights_.copy()
         return weights.items()
         
-    def iteritems(self, level="edges"):
-
-        assert level in {"nodes", "edges"}
-        if level == "edges":
-            weights = self.edge_weights_.copy()
-        if level == "nodes":
-            weights = self.node_weights_.copy()
-        return weights.iteritems()
-        
     def keys(self, level="edges"):
 
         assert level in {"nodes", "edges"}
         if level == "edges":
             weights = self.edge_weights_.copy()
         if level == "nodes":
             weights = self.node_weights_.copy()
```

### Comparing `ensemble_networkx-2024.2.5/setup.py` & `ensemble_networkx-2024.5.30/setup.py`

 * *Files identical despite different names*

