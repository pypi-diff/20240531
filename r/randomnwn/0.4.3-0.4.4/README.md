# Comparing `tmp/randomnwn-0.4.3.tar.gz` & `tmp/randomnwn-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randomnwn-0.4.3.tar", last modified: Thu May 23 20:53:21 2024, max compression
+gzip compressed data, was "randomnwn-0.4.4.tar", last modified: Fri May 31 18:22:05 2024, max compression
```

## Comparing `randomnwn-0.4.3.tar` & `randomnwn-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:21.283816 randomnwn-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 20:53:14.000000 randomnwn-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-23 20:53:21.283816 randomnwn-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-23 20:53:14.000000 randomnwn-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:21.279816 randomnwn-0.4.3/randomnwn/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/fromtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/line_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/nanowires.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/units.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 20:53:14.000000 randomnwn-0.4.3/randomnwn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:21.283816 randomnwn-0.4.3/randomnwn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-23 20:53:21.000000 randomnwn-0.4.3/randomnwn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 20:53:21.000000 randomnwn-0.4.3/randomnwn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:53:21.000000 randomnwn-0.4.3/randomnwn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 20:53:21.000000 randomnwn-0.4.3/randomnwn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 20:53:21.000000 randomnwn-0.4.3/randomnwn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:53:21.283816 randomnwn-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-23 20:53:14.000000 randomnwn-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:53:21.283816 randomnwn-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 20:53:14.000000 randomnwn-0.4.3/tests/test_nanowires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:22:05.617139 randomnwn-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 18:22:01.000000 randomnwn-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-31 18:22:05.617139 randomnwn-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-31 18:22:01.000000 randomnwn-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:22:05.617139 randomnwn-0.4.4/randomnwn/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/fromtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/line_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/nanowires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 18:22:01.000000 randomnwn-0.4.4/randomnwn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:22:05.617139 randomnwn-0.4.4/randomnwn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-31 18:22:05.000000 randomnwn-0.4.4/randomnwn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-31 18:22:05.000000 randomnwn-0.4.4/randomnwn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:22:05.000000 randomnwn-0.4.4/randomnwn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 18:22:05.000000 randomnwn-0.4.4/randomnwn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 18:22:05.000000 randomnwn-0.4.4/randomnwn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:22:05.617139 randomnwn-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-31 18:22:01.000000 randomnwn-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:22:05.617139 randomnwn-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-31 18:22:01.000000 randomnwn-0.4.4/tests/test_nanowires.py
```

### Comparing `randomnwn-0.4.3/LICENSE` & `randomnwn-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/PKG-INFO` & `randomnwn-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.4.3
+Version: 0.4.4
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: GNU General Public License v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `randomnwn-0.4.3/README.md` & `randomnwn-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/__init__.py` & `randomnwn-0.4.4/randomnwn/__init__.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/_models.py` & `randomnwn-0.4.4/randomnwn/_models.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/calculations.py` & `randomnwn-0.4.4/randomnwn/calculations.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/dynamics.py` & `randomnwn-0.4.4/randomnwn/dynamics.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from scipy.integrate import solve_ivp
 
 from numbers import Number
 from typing import Callable, List, Union, Tuple, Iterable
 from scipy.integrate._ivp.ivp import OdeResult
 
 from .nanowires import get_edge_indices
-from .calculations import solve_drain_current
+from .calculations import solve_drain_current, solve_network
 from ._models import (
     resist_func,
     _HP_model_no_decay,
     _HP_model_decay,
     _HP_model_chen,
 )
 
@@ -356,7 +356,79 @@
         # Set state variables and get drain currents
         input_V = voltage_func(sol.t[i])
         set_state_variables(NWN, sol.y.T[i], edge_list)
         current_array[i] = solve_drain_current(
             NWN, source_node, drain_node, input_V, scaled, solver, **kwargs)
     
     return current_array.squeeze()
+
+
+def get_evolution_node_voltages(
+    NWN: nx.Graph, 
+    sol: OdeResult, 
+    edge_list: list[tuple], 
+    source_node: tuple | list[tuple],
+    drain_node: tuple | list[tuple],
+    voltage_func: Callable,
+    solver: str = "spsolve",
+    **kwargs
+) -> np.ndarray:
+    """
+    To be used in conjunction with `solve_evolution`. Takes the output from
+    `solve_evolution` and finds the voltage of all nodes in the network at each
+    time step.
+
+    The appropriate parameters passed should be the same as `solve_evolution`.
+
+    Parameters
+    ----------
+    NWN : Graph
+        Nanowire network.
+
+    sol : OdeResult
+        Output from `solve_evolution`.
+
+    edge_list : list of tuples
+        Output from `solve_evolution`.
+
+    source_node : tuple, or list of tuples
+        Voltage source nodes.
+
+    drain_node : tuple, or list of tuples
+        Grounded output nodes.
+
+    voltage_func : Callable
+        The applied voltage with the calling signature `func(t)`. The voltage 
+        should have units of `v0`.
+
+    solver : str, optional
+        Name of sparse matrix solving algorithm to use. Default: "spsolve".
+
+    **kwargs
+        Keyword arguments passed to the solver.
+
+    Returns
+    -------
+    node_voltage_array: ndarray
+        An `n` x `m` array containing the voltage of each node in the network,
+        corresponding to the `n` time steps and `m` nodes in the network.
+
+    """
+    # Get lists of source and drain nodes
+    if isinstance(source_node, tuple):
+        source_node = [source_node]
+    if isinstance(drain_node, tuple):
+        drain_node = [drain_node]
+        
+    # Preallocate output
+    node_voltage_array = np.zeros((len(sol.t), len(NWN.nodes)))
+
+    # Loop through each time step
+    for i in range(len(sol.t)):
+        # Set state variables and get drain currents
+        input_V = voltage_func(sol.t[i])
+        set_state_variables(NWN, sol.y.T[i], edge_list)
+        *node_voltage_array[i], I = solve_network(
+            NWN, source_node, drain_node, input_V, "voltage", solver, **kwargs
+        )
+    
+    return node_voltage_array.squeeze()
```

### Comparing `randomnwn-0.4.3/randomnwn/fromtext.py` & `randomnwn-0.4.4/randomnwn/fromtext.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/line_functions.py` & `randomnwn-0.4.4/randomnwn/line_functions.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/nanowires.py` & `randomnwn-0.4.4/randomnwn/nanowires.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,16 +210,17 @@
             # Get old edge attributes
             old_attributes = NWN.edges[edge]
 
             # Create the replacing MNR node and edge
             NWN.add_node((i, j), loc=loc, electrode=False)
             NWN.add_edge((i, j), other_node, **old_attributes)
 
-        # Remove old JDA node
-        NWN.remove_node((i,))
+        # Remove old JDA node, only if it had connections
+        if len(junction_locs) >= 1:
+            NWN.remove_node((i,))
 
         # Add edges between subnodes
         for ind, next_ind in zip(ordering, ordering[1:]):
             # Find inner-wire resistance
             L = NWN.nodes[(i, ind)]["loc"].distance(NWN.nodes[(i, next_ind)]["loc"])
             wire_conductance = (Ron * A0 * A) / (rho0 * l0 * rho * L * 1e3)
```

### Comparing `randomnwn-0.4.3/randomnwn/plotting.py` & `randomnwn-0.4.4/randomnwn/plotting.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn/units.py` & `randomnwn-0.4.4/randomnwn/units.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/randomnwn.egg-info/PKG-INFO` & `randomnwn-0.4.4/randomnwn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.4.3
+Version: 0.4.4
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: GNU General Public License v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `randomnwn-0.4.3/setup.py` & `randomnwn-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.3/tests/test_nanowires.py` & `randomnwn-0.4.4/tests/test_nanowires.py`

 * *Files identical despite different names*

