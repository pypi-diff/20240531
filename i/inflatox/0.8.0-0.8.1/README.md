# Comparing `tmp/inflatox-0.8.0-cp37-abi3-win_amd64.whl.zip` & `tmp/inflatox-0.8.1-cp37-abi3-win32.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 495606 bytes, number of entries: 11
--rw-r--r--  4.6 unx     6011 b- defN 24-Mar-18 09:50 inflatox-0.8.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Mar-18 09:50 inflatox-0.8.0.dist-info/WHEEL
--rw-r--r--  4.6 unx    14114 b- defN 24-Mar-18 09:50 inflatox-0.8.0.dist-info/license_files/LICENSE-EN.txt
--rw-r--r--  4.6 unx   377429 b- defN 24-Mar-18 09:50 inflatox-0.8.0.dist-info/license_files/LICENSE-EUPL.md
--rw-r--r--  4.6 unx    12860 b- defN 24-Mar-18 09:50 inflatox/compiler.py
--rw-r--r--  4.6 unx    22131 b- defN 24-Mar-18 09:50 inflatox/consistency_conditions.py
--rw-r--r--  4.6 unx    22319 b- defN 24-Mar-18 09:50 inflatox/symbolic.py
--rw-r--r--  4.6 unx      935 b- defN 24-Mar-18 09:50 inflatox/version.py
--rw-r--r--  4.6 unx     1195 b- defN 24-Mar-18 09:50 inflatox/__init__.py
--rwxr-xr-x  4.6 unx   912896 b- defN 24-Mar-18 09:50 inflatox/libinflx_rs.pyd
--rw-r--r--  4.6 unx      916 b- defN 24-Mar-18 09:50 inflatox-0.8.0.dist-info/RECORD
-11 files, 1370900 bytes uncompressed, 494072 bytes compressed:  64.0%
+Zip file size: 497354 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     6036 b- defN 24-May-31 08:11 inflatox-0.8.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       90 b- defN 24-May-31 08:11 inflatox-0.8.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx    14114 b- defN 24-May-31 08:11 inflatox-0.8.1.dist-info/license_files/LICENSE-EN.txt
+-rw-r--r--  4.6 unx   377429 b- defN 24-May-31 08:11 inflatox-0.8.1.dist-info/license_files/LICENSE-EUPL.md
+-rw-r--r--  4.6 unx    12860 b- defN 24-May-31 08:11 inflatox/compiler.py
+-rw-r--r--  4.6 unx    27785 b- defN 24-May-31 08:11 inflatox/consistency_conditions.py
+-rw-r--r--  4.6 unx    22823 b- defN 24-May-31 08:11 inflatox/symbolic.py
+-rw-r--r--  4.6 unx      935 b- defN 24-May-31 08:11 inflatox/version.py
+-rw-r--r--  4.6 unx     1195 b- defN 24-May-31 08:11 inflatox/__init__.py
+-rwxr-xr-x  4.6 unx   857600 b- defN 24-May-31 08:11 inflatox/libinflx_rs.pyd
+-rw-r--r--  4.6 unx      916 b- defN 24-May-31 08:11 inflatox-0.8.1.dist-info/RECORD
+11 files, 1321783 bytes uncompressed, 495820 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
-Filename: inflatox-0.8.0.dist-info/METADATA
+Filename: inflatox-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: inflatox-0.8.0.dist-info/WHEEL
+Filename: inflatox-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: inflatox-0.8.0.dist-info/license_files/LICENSE-EN.txt
+Filename: inflatox-0.8.1.dist-info/license_files/LICENSE-EN.txt
 Comment: 
 
-Filename: inflatox-0.8.0.dist-info/license_files/LICENSE-EUPL.md
+Filename: inflatox-0.8.1.dist-info/license_files/LICENSE-EUPL.md
 Comment: 
 
 Filename: inflatox/compiler.py
 Comment: 
 
 Filename: inflatox/consistency_conditions.py
 Comment: 
@@ -24,11 +24,11 @@
 
 Filename: inflatox/__init__.py
 Comment: 
 
 Filename: inflatox/libinflx_rs.pyd
 Comment: 
 
-Filename: inflatox-0.8.0.dist-info/RECORD
+Filename: inflatox-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inflatox/consistency_conditions.py

```diff
@@ -22,15 +22,15 @@
 import numpy as np
 
 #Internal imports
 from .compiler import CompilationArtifact
 from .libinflx_rs import *
 
 #Limit exports to these items
-__all__ = ['InflationCondition', 'AnguelovaLazaroiuCondition']
+__all__ = ['InflationCondition', 'GeneralisedAL']
 
 class InflationCondition():
   """Base class for all inflation conditions. Provides native methods to evaluate
   the potential and projected Hesse matrix. This base-class may be extended either
   by using these native methods, or by including your own native code that hooks
   into the Rust API or C ABI.
   """
@@ -103,16 +103,18 @@
     `np.ndarray`: Components of the projected covariant hesse matrix with
       parameters `args` at coordinates `x`.
     """
     return self.dylib.hesse(x, args)
   
   def calc_H_array(self,
     args: list[float] | np.ndarray,
-    start: list[float] | np.ndarray,
-    stop: list[float] | np.ndarray,
+    x0_start: float,
+    x0_stop: float,
+    x1_start: float,
+    x1_stop: float,
     N: list[int] | None = None
   ) -> np.ndarray:
     """constructs an array of field space coordinates and fills it with the
     value of the projected Hesse matrix at those field space coordinates.
     The start and stop values of each axis in field-space can be specified with
     the `start` and `stop` arguments. The number of samples along each axis can
     be set with the `N` argument. It defaults to `8000` per axis.
@@ -131,22 +133,29 @@
 
     ### Returns
     `np.ndarray`: (d+2)-dimensional array for a d-dimensional field-space. The
       first two axes of this array represent the axes of the Hesse matrix itself.
       The other axes correspond to the field-space components. 
     """
     n_fields = self.artifact.n_fields
-    start_stop = np.array([[start, stop] for (start, stop) in zip(start, stop)])
+    start_stop = np.array([
+      [x0_start, x0_stop],
+      [x1_start, x1_stop]
+    ])
     N = N if N is not None else (8000 for _ in range(n_fields))
-    return self.dylib.hesse_array(N, args, start_stop)
+    return self.dylib.hesse_array(np.array(n_fields, dtype=np.int64), args, start_stop)
 
-class AnguelovaLazaroiuCondition(InflationCondition):
-  """This class extends the generic `InflationCondition` with the potential
-  consistency condition from Anguelova and Lazaroiu 2022 paper
-  (`arXiv:2210.00031v2`) for rapid-turn, slow-roll (RTSL) inflationary models.
+class GeneralisedAL(InflationCondition):
+  """This class extends the generic `InflationCondition` with the generalised rapid-turn (ω>>ε^½)
+  consistency condition from (`arXiv:2405.11628`).
+
+  In addition, related quantities that may be estimated from the potential and field-space metric,
+  such as the slow-roll parameters εH, η_||, the angle δ and turn-rate ω can also be computed.
+  The rapid-turn limit of the consistency condition derived in the 2022 Anguelova and Lazaroiu 2022
+  (`arXiv:2210.00031v2`) is also available.
 
   ### Usage
   To construct an instance of this class, a `CompilationArtifact` is required.
   Such an artifact can be obtained by running an instance of `inflatox.Compiler`
   with a specific model (fieldspace metric + scalar potential). For more info on
   how to use the `Compiler`, see its documentation.
   
@@ -181,20 +190,27 @@
         difference between the rhs and lhs:
           out = ||lhs| - |rhs||/(|lhs| + |rhs|)
         Note that out = 0 corresponds to the consistency condition holding
         perfectly. Values larger than zero indicate it does not hold perfectly.
       2. ε_V (first potential slow-roll parameter)
       3. ε_H (first dynamical slow-roll parameter), calculated assuming that the
         AL condition holds.
-      4. η_H (second dynamical slow-roll parameter), calculated assuming that the
+      4. η_|| (second dynamical slow-roll parameter), calculated assuming that the
         AL condition holds.
       5. δ (characteristic angle), calculated assuming that the AL condition holds.
       6. ω (relative turn rate), calculated assuming that the AL condition holds.
-    Using (1) and (3), slow-roll trajectories with |ε_H|, |η_H| << 1 can be
+    Using (1) and (3), slow-roll trajectories with |ε_H|, |η_||| << 1 can be
     identified. See (paper) for a more complete discussion.
+
+    ### *NOTE*
+    The consistency condition or ε_H *on their own* are usually insufficient to discriminate
+    determine the location of the rapid-turn attractor. Always verify that:
+    1. The consistency condition holds AND
+    2. ε_H << 1 AND
+    3. ε_H > 0 
     
     ### Args:
     - `args` (`np.ndarray`): values of the model-dependent parameters. 
     - `x0_start` (`float`): minimum value of first field `x[0]`.
     - `x0_stop` (`float`): maximum value of first field `x[0]`.
     - `x1_start` (`float`): minimum value of second field `x[1]`.
     - `y_stop` (`float`): maximum value of second field `x[1]`.
@@ -208,15 +224,15 @@
       will be used. 
 
     ### Returns:
     `np.ndarray` (✕6): arrays filled with the following quantities (in order):
       1. Consistency condition ||lhs| - |rhs||/(|lhs| + |rhs|)
       2. ε_V (first potential slow-roll parameter)
       3. ε_H (first dynamical slow-roll parameter)
-      4. η_H (second dynamical slow-roll parameter)
+      4. η_|| (speed-up parameter)
       5. δ (characteristic angle)
       6. ω (relative turn rate)
     """
     
     #set up args for anguelova's condition
     out = np.zeros((N_x0, N_x1, 6), dtype=float)
     
@@ -228,15 +244,15 @@
     #calculate 
     threads = threads if threads is not None else 0
     
     #evaluate and return
     complete_analysis(self.dylib, args, out, start_stop, progress, threads)
     return (out[:,:,0], out[:,:,1], out[:,:,2], out[:,:,3], out[:,:,4], out[:,:,5])
 
-  def consistency_only(self,
+  def consistency(self,
       args: np.ndarray,
       x0_start: float,
       x0_stop: float,
       x1_start: float,
       x1_stop: float,
       N_x0: int = 1_000,
       N_x1: int = 1_000,
@@ -285,15 +301,15 @@
     #calculate 
     threads = threads if threads is not None else 0
     
     #evaluate and return
     consistency_only(self.dylib, args, out, start_stop, progress, threads)
     return out
 
-  def epsilon_v_only(self,
+  def epsilon_v(self,
       args: np.ndarray,
       x0_start: float,
       x0_stop: float,
       x1_start: float,
       x1_stop: float,
       N_x0: int = 1_000,
       N_x1: int = 1_000,
@@ -338,15 +354,15 @@
     #calculate 
     threads = threads if threads is not None else 0
     
     #evaluate and return
     epsilon_v_only(self.dylib, args, out, start_stop, progress, threads)
     return out
 
-  def consistency_only_old(self,
+  def consistency_rapidturn(self,
       args: np.ndarray,
       x0_start: float,
       x0_stop: float,
       x1_start: float,
       x1_stop: float,
       N_x0: int = 1_000,
       N_x1: int = 1_000,
@@ -447,15 +463,15 @@
     flag_quantum_dif_py(self.dylib, args, x, start_stop, progress, accuracy)
     return x
 
   #########################
   # On_trajectory methods #
   #########################
 
-  def complete_analysis_on_trajectory(self,
+  def complete_analysis_ot(self,
       args: np.ndarray,
       x: np.ndarray,
       progress: bool = True,
       threads: None | int = None,
     ) -> np.ndarray:
     """This function performs a complete analysis of possible slow-roll (rapid)
     turn trajectories using the methods described in (paper), based on the AL
@@ -465,41 +481,169 @@
         difference between the rhs and lhs:
           out = ||lhs| - |rhs||/(|lhs| + |rhs|)
         Note that out = 0 corresponds to the consistency condition holding
         perfectly. Values larger than zero indicate it does not hold perfectly.
       2. ε_V (first potential slow-roll parameter)
       3. ε_H (first dynamical slow-roll parameter), calculated assuming that the
         AL condition holds.
-      4. η_H (second dynamical slow-roll parameter), calculated assuming that the
+      4. η_|| (second dynamical slow-roll parameter), calculated assuming that the
         AL condition holds.
       5. δ (characteristic angle), calculated assuming that the AL condition holds.
       6. ω (relative turn rate), calculated assuming that the AL condition holds.
-    Using (1) and (3), slow-roll trajectories with |ε_H|, |η_H| << 1 can be
+    Using (1) and (3), slow-roll trajectories with |ε_H|, |η_||| << 1 can be
     identified. See (paper) for a more complete discussion.
+
+    ### *NOTE*
+    The consistency condition or ε_H *on their own* are usually insufficient to discriminate
+    determine the location of the rapid-turn attractor. Always verify that:
+    1. The consistency condition holds AND
+    2. ε_H << 1 AND
+    3. ε_H > 0 
     
     ### Args:
     - `args` (`np.ndarray`): values of the model-dependent parameters. 
     - `progress` (`bool`, optional): whether to render a progressbar or not. Showing the
       progressbar may slightly degrade performance. Defaults to True.
     - `threads` (`None | int`, optional): number of threads to use for calculation.
       When set to `None`, inflatox will choose the optimum number (usually 1).
       When set to 1, a single-threaded implementation will be used. 
 
     ### Returns:
     `np.ndarray` (✕6): arrays filled with the following quantities (in order):
       1. Consistency condition ||lhs| - |rhs||/(|lhs| + |rhs|)
       2. ε_V (first potential slow-roll parameter)
       3. ε_H (first dynamical slow-roll parameter)
-      4. η_H (second dynamical slow-roll parameter)
+      4. η_|| (speed-up parameter)
       5. δ (characteristic angle)
       6. ω (relative turn rate)
     """
     
     #set up args for anguelova's condition
     out = np.zeros((x.shape[0], 6), dtype=float)
         
     # Single-threaded default is more appropriate for smaller number of iterations 
     threads = threads if threads is not None else 1
     
     #evaluate and return
     complete_analysis_on_trajectory(self.dylib, args, x, out, progress, threads)
     return np.split(out, 6, 1)
+
+  def consistency_ot(self,
+      args: np.ndarray,
+      x: np.ndarray,
+      progress: bool = True,
+      threads: None | int = None,
+    ) -> np.ndarray:
+    """returns array filled with the normalised difference between one and the
+    quotient of the left-hand-side (lhs) and right-hand-side (rhs) of the slow-
+    roll turn consistency condition.
+    
+    ### Exact formulation of calculated quantities
+    This function returns:
+      ||lhs| - |rhs||/(|lhs| + |rhs|)
+    Where
+      lhs = Vww/V
+      rhs = 3 + 3 (Vvw/Vvv)² + (Vvv/V) (Vvw/Vvv)² 
+      
+    ### Args:
+    - `args` (`np.ndarray`): values of the model-dependent parameters. 
+    - `progress` (`bool`, optional): whether to render a progressbar or not. Showing the
+      progressbar may slightly degrade performance. Defaults to True.
+    - `threads` (`None | int`, optional): number of threads to use for calculation.
+      When set to `None`, inflatox will choose the optimum number (usually equal
+      to the number of CPU's). When set to 1, a single-threaded implementation
+      will be used. 
+
+    ### Returns:
+    `np.ndarray`: array filled with slow-roll (intermediate) turn consistency
+      condition from (paper)
+    """
+    #set up args for anguelova's condition
+    out = np.zeros((x.shape[0]), dtype=float)
+        
+    # Single-threaded default is more appropriate for smaller number of iterations 
+    threads = threads if threads is not None else 1
+    
+    #evaluate and return
+    consistency_only_on_trajectory(self.dylib, args, x, out, progress, threads)
+    return out
+  
+  def consistency_rapidturn_ot(self,
+      args: np.ndarray,
+      x: np.ndarray,
+      progress: bool = True,
+      threads: None | int = None,
+    ) -> np.ndarray:
+    """returns array filled with the normalised difference between one and the
+    quotient of the left-hand-side (lhs) and right-hand-side (rhs) of the slow-
+    roll turn consistency condition.
+    
+    ### Exact formulation of calculated quantities
+    This function returns:
+      ||lhs| - |rhs||/(|lhs| + |rhs|)
+    Where
+      lhs = Vww/V
+      rhs = 3 + 3 (Vvw/Vvv)² + (Vvv/V) (Vvw/Vvv)² 
+      
+    ### Args:
+    - `args` (`np.ndarray`): values of the model-dependent parameters. 
+    - `progress` (`bool`, optional): whether to render a progressbar or not. Showing the
+      progressbar may slightly degrade performance. Defaults to True.
+    - `threads` (`None | int`, optional): number of threads to use for calculation.
+      When set to `None`, inflatox will choose the optimum number (usually equal
+      to the number of CPU's). When set to 1, a single-threaded implementation
+      will be used. 
+
+    ### Returns:
+    `np.ndarray`: array filled with slow-roll (intermediate) turn consistency
+      condition from (paper)
+    """
+    #set up args for anguelova's condition
+    out = np.zeros((x.shape[0]), dtype=float)
+        
+    # Single-threaded default is more appropriate for smaller number of iterations 
+    threads = threads if threads is not None else 1
+    
+    #evaluate and return
+    consistency_rapidturn_only_on_trajectory(self.dylib, args, x, out, progress, threads)
+    return out
+
+  def epsilon_v_ot(self,
+      args: np.ndarray,
+      x: np.ndarray,
+      progress: bool = True,
+      threads: None | int = None,
+    ) -> np.ndarray:
+    """returns array filled with the normalised difference between one and the
+    quotient of the left-hand-side (lhs) and right-hand-side (rhs) of
+    Anguelova & Lazaroiu's original consistency condition (`arXiv:2210.00031v2`).
+  
+    ### Exact formulation of calculated quantities
+    This function returns:
+      ||lhs| - |rhs||/(|lhs| + |rhs|)
+    Where
+      lhs = Vww/V
+      rhs = 3 (Vvw/Vvv)²
+    
+    ### Args:
+    - `args` (`np.ndarray`): values of the model-dependent parameters. 
+    - `x` (`np.ndarray`):
+    - `progress` (`bool`, optional): whether to render a progressbar or not. Showing the
+      progressbar may slightly degrade performance. Defaults to True.
+    - `threads` (`None | int`, optional): number of threads to use for calculation.
+      When set to `None`, inflatox will choose the optimum number (usually equal
+      to the number of CPU's). When set to 1, a single-threaded implementation
+      will be used. 
+
+    ### Returns:
+    `np.ndarray`: array filled with Anguelova & Lazaroiu's original consistency
+      condition.
+    """
+    #set up args for anguelova's condition
+    out = np.zeros((x.shape[0]), dtype=float)
+      
+    # Single-threaded default is more appropriate for smaller number of iterations 
+    threads = threads if threads is not None else 1
+  
+    #evaluate and return
+    epsilon_v_only_on_trajectory(self.dylib, args, x, out, progress, threads)
+    return out
```

## inflatox/symbolic.py

```diff
@@ -236,52 +236,60 @@
       lhs = expr
     """
     if not self.silent and lhs is not None:
       display(Math(f"{lhs}={expr}"))
     elif not self.silent:
       display(expr)
     
-  def execute(self, guesses: list[list[sympy.Expr]]) -> SymbolicOutput:
+  def execute(self, guesses: list[list[sympy.Expr]] | None = None) -> SymbolicOutput:
     """Performs fully symbolic calculation of the components of the covariant
     Hesse matrix of the potential with respect to the metric, which are then
     projected onto an orthonormal vielbein basis constructed (using the
     Gramm-Schmidt procedure) from:
       1. the gradient of the potential.
       2. the list of vectors supplied by the caller of this function.
     The details of this procedure are specified in the documentation of the
     individual methods of this class.
 
     ### Args
-    `guesses` (`list[list[sympy.Expr]]`): list of vectors to be used to calculate
+    `guesses` (`list[list[sympy.Expr]] | None`): list of vectors to be used to calculate
       an orthonormal vielbein basis onto which the components of the Hesse matrix
       will be projected. The supplied vectors *do not* have to be orthogonal, but
-      they *must be* linearly independent.
+      they *must be* linearly independent. If this argument equals `None` and the model under
+      consideration is only two-dimensional, the code is able to determine the basis on its own.
+      Otherwise, it will throw an error.
     
     ### Simplification
     If the simplification depth is set to 1 or higher, this function will
     simplify its output before returning. See the docs of the constructor of this
     class for more info.
 
     ### Returns
     `HesseMatrix`: object containing the components of the projected Hesse matrix,
       as well as information about the model that was used to calculate said components. 
     """
     dim = len(self.coords)
-    assert(len(guesses) == dim - 1)
+    if guesses is not None: assert(len(guesses) == dim - 1)
     
     #(1) Calculate an orthonormal basis
     #(1a)...starting with a vector parallel to the potential gradient
     self.print("Calculating orthonormal basis...")
     basis = [self.calc_v()]
     self.display(basis[0], lhs='v')
-    
-    #(1b) followed by other gramm-schmidt produced vectors
-    for (i, guess) in enumerate(guesses):
-      basis.append(self.gramm_schmidt(basis, guess))
-      self.display(basis[-1], lhs=f'w_{i+1}')
+
+    if guesses is None and dim == 2:
+      basis.append([-basis[0][1], basis[0][0]])
+      self.display(basis[-1], lhs=f'w_1')
+    elif guesses is None:
+      raise Exception("guesses argument cannot be None if model has more than two fields")
+    else:    
+      #(1b) followed by other gramm-schmidt produced vectors
+      for (i, guess) in enumerate(guesses):
+        basis.append(self.gramm_schmidt(basis, guess))
+        self.display(basis[-1], lhs=f'w_{i+1}')
     
     #(1b) make sure the basis is orthonormal
     if self.assertions:
       for a in range(dim):
         for b in range(dim):
           if a == b:
             assert(sympy.Eq(1, self.inner_prod(basis[a], basis[b])).simplify())
```

## inflatox/version.py

```diff
@@ -13,9 +13,9 @@
 #  You should have received a copy of the EUPL in an/all official language(s) of
 #  the European Union along with Inflatox.  If not, see 
 #  <https://ec.europa.eu/info/european-union-public-licence_en/>.
 #
 #  (1) Resident of the Kingdom of the Netherlands; agreement between licensor and
 #  licensee subject to Dutch law as per article 15 of the EUPL.
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 __abi_version__ = '3.0.0'
```

## Comparing `inflatox-0.8.0.dist-info/METADATA` & `inflatox-0.8.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.3
 Name: inflatox
-Version: 0.8.0
+Version: 0.8.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy >1
 Requires-Dist: sympy >1
 Requires-Dist: joblib >1
 Requires-Dist: einsteinpy >=0.4
 Requires-Dist: ziglang >=0.10
 License-File: LICENSE-EN.txt
 License-File: LICENSE-EUPL.md
 Summary: Framework for implementing high-performance numerical consistency conditions for multifield inflation models.
 Author-email: Raúl Wolters <r.wolters@uu.nl>
 License: EUPL-1.2
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/smups/inflatox
 Project-URL: Bug Tracker, https://github.com/smups/inflatox/issues
 
 ![inflatox_banner](https://raw.githubusercontent.com/smups/inflatox/dev/logos/banner.png)
 # Inflatox - multifield inflation consistency conditions in python
 [![License: EUPL v1.2](https://img.shields.io/badge/License-EUPLv1.2-blue.svg)](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
+[![arXiv](https://img.shields.io/badge/arXiv-2405.11628-b31b1b.svg)](https://arxiv.org/abs/2405.11628)
 [![PyPi](https://img.shields.io/pypi/v/inflatox)](https://pypi.org/project/inflatox)
 [![CI](https://github.com/smups/inflatox/actions/workflows/CI.yml/badge.svg)](https://github.com/smups/inflatox/actions/workflows/CI.yml)
 
 Inflatox provides utilities to compute slow-roll parameters and turn-rates for
-two-field inflation models, based on the consistency condition from Anguelova &
-Lazaroiu (2023)[^1]. These can be used in a parameter sweep of a two-field
-model to find possible inflation trajectories.
+two-field inflation models, based on the consistency condition from Generalised consistency condition
+first presented in Anguelova & Lazaroiu (2023)[^1] and later expanded for the purposes of this package
+in [arXiv:2405.11628](https://arxiv.org/abs/2405.11628). The consistency conditions can be used in a
+parameter sweep of a two-field model to find possible inflation trajectories.
 
-If this software has proven useful to your research, please consider citing
-(_paper in preparation_).
+> If this software has proven useful to your research, please consider citing
+[arXiv:2405.11628](https://arxiv.org/abs/2405.11628) (_paper in preparation_).
 
 ## Features
 - symbolic solver for components of the Hesse matrix of an inflationary model
   with non-canonical kinetic terms, powered by [`sympy`](https://www.sympy.org).
 - transpiler to transform `sympy` expressions into executable compiled (`C`) code.
 - built-in multithreaded `rust` module for high-performance calculations of
   consistency conditions that interfaces directly with `numpy` and python.
@@ -43,15 +45,15 @@
   quantity, which can be used to extend it with additional consistency conditions.
 - no need to read, write or compile any `rust` or `C` code manually
   (this is all done automatically behind the scenes).
 - no system dependencies, everything needed to run the package can be automatically
   installed by `pip`.
 
 ## Installation and Dependencies
-Inflatox requires at least python (ABI) version `3.7`. The latest version of
+Inflatox requires at least python (ABI) version `3.8`. The latest version of
 inflatox can be installed using pip:
 ```console
 pip install inflatox
 ```
 Inflatox can be updated using:
 ```console
 pip install --upgrade inflatox
@@ -84,16 +86,16 @@
 calc = inflatox.SymbolicCalculation.new_from_list(fields, g, V)
 hesse = calc.execute([[0,1]])
 
 #run the compiler
 out = inflatox.Compiler(hesse).compile()
 
 #evaluate the compiled potential and Hesse matrix
-from inflatox.consistency_conditions import AnguelovaLazaroiuCondition
-anguelova = AnguelovaLazaroiuCondition(out)
+from inflatox.consistency_conditions import GeneralisedAL
+anguelova = GeneralisedAL(out)
 
 p = np.array([1.0, 1.0, 1.0])
 x = np.array([2.0, 2.0])
 print(anguelova.calc_V(x, p))
 print(anguelova.calc_H(x, p))
 
 extent = (-1, 1, -1, 1)
@@ -110,25 +112,16 @@
 - Intel/AMD x86_64/amd64 (64 bit)
   - linux/gnu (glibc >= 2.17, kernel >= 3.2)
   - windows 7+ [^2]
   - macOS 10.12+ / Sierra+
 - ARM aarch64 (64 bit)
   - linux/gnu (glibc >= 2.17, kernel >= 4.1)
   - macOS 11.0+ / Big Sur+
-- PowerPC ppc64le (64 bit)
-  - linux/gnu (glibc >= 2.17, kernel >= 3.10)
-- IBM s390x (64 bit)
-  - linux/gnu (glibc >= 2.17, kernel >= 3.2)
 *Note: Apple silicon M-series chips are supported (aarch64)*
 
-## Citing
-If this software package contributed meaningfully to your research, please
-consider citing the following papers:
-- (in preparation)
-
 ## License
 [![License: EUPL v1.2](https://img.shields.io/badge/License-EUPLv1.2-blue.svg)](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)
 >**Inflatox is explicitly not licensed under the dual
 Apache/MIT license common to the Rust ecosystem. Instead it is licensed under
 the terms of the [European Union Public License v1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)**.
 
 Inflatox is a science project and embraces the values of open science and free
```

## Comparing `inflatox-0.8.0.dist-info/license_files/LICENSE-EN.txt` & `inflatox-0.8.1.dist-info/license_files/LICENSE-EN.txt`

 * *Files identical despite different names*

## Comparing `inflatox-0.8.0.dist-info/license_files/LICENSE-EUPL.md` & `inflatox-0.8.1.dist-info/license_files/LICENSE-EUPL.md`

 * *Files identical despite different names*

## Comparing `inflatox-0.8.0.dist-info/RECORD` & `inflatox-0.8.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-inflatox-0.8.0.dist-info/METADATA,sha256=PJjbNU6TDG9VXR2-9iwFceAmUq1t8yJgGcHOOW7UtPE,6011
-inflatox-0.8.0.dist-info/WHEEL,sha256=d40ZnTlPFCUsdXDb0X9563rVL9wMWbhpBmBuaD2xdkg,94
-inflatox-0.8.0.dist-info/license_files/LICENSE-EN.txt,sha256=Aif1zk6wdAUTw1KYZpRUC_cXUeVECcTDwYncAOS1DFI,14114
-inflatox-0.8.0.dist-info/license_files/LICENSE-EUPL.md,sha256=KmidoWBnFWjACK_7WlJKWKoQmwzCzFjn5L5V0wPtcyQ,377429
+inflatox-0.8.1.dist-info/METADATA,sha256=X1CL1H6_P_3kn4cESAtsTqWQwaB9xJ3dM6QD2ZSMQ-0,6036
+inflatox-0.8.1.dist-info/WHEEL,sha256=6OJYZIM2Dk4eAjI82h1dKfIeHAb4_0-YRQodIDqhP8I,90
+inflatox-0.8.1.dist-info/license_files/LICENSE-EN.txt,sha256=Aif1zk6wdAUTw1KYZpRUC_cXUeVECcTDwYncAOS1DFI,14114
+inflatox-0.8.1.dist-info/license_files/LICENSE-EUPL.md,sha256=KmidoWBnFWjACK_7WlJKWKoQmwzCzFjn5L5V0wPtcyQ,377429
 inflatox/compiler.py,sha256=zta6Ir2KIxW5OMvPp1AHN9cAX9DosF76srdMspH0K1w,12860
-inflatox/consistency_conditions.py,sha256=oxyNPCvrokPQWAUSNxqO_aFT10bmy578RdTq47E2UrE,22131
-inflatox/symbolic.py,sha256=i_djmrvqqIpmpPVYZ1G7UCr_OAhIOX0I1sY3gDjDERc,22319
-inflatox/version.py,sha256=ojlZRaBv6AfB3qCi3D6cCCYUzNSOcsKphO_yiz8WLKk,935
+inflatox/consistency_conditions.py,sha256=lPsc54VeQSCS74QtNkRi5H3mEPHtxh3coQd7zWfUMiA,27785
+inflatox/symbolic.py,sha256=ppT7E84mfE_Ii02hRrcoFw9UUcCt-eNJsVhR8AJWtXQ,22823
+inflatox/version.py,sha256=ZOKFW0-8H5kN6GHdMhQJMY_OKgyCA8-ECCJ-X9s-ZL8,935
 inflatox/__init__.py,sha256=RHx1BTYfX7SSBEXATKFnxX5SrZCB6BSBN1eEKbar040,1195
-inflatox/libinflx_rs.pyd,sha256=8byyHRVVzG8QZ8CegqazXIk8B1aShcEqYQ_6Idzl8HE,912896
-inflatox-0.8.0.dist-info/RECORD,,
+inflatox/libinflx_rs.pyd,sha256=m4qQTfpBgZtKW_3lL9AW425uAkMTkqC2TU4Ee4-_Fug,857600
+inflatox-0.8.1.dist-info/RECORD,,
```

