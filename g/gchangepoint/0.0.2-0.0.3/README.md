# Comparing `tmp/gchangepoint-0.0.2.tar.gz` & `tmp/gchangepoint-0.0.3.tar.gz`

## Comparing `gchangepoint-0.0.2.tar` & `gchangepoint-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    33344 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/src/gchangepoint/MST.so
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/src/gchangepoint/__init__.py
--rw-r--r--   0        0        0    58590 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/src/gchangepoint/gchangepoint.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/src/gchangepoint/graphutilities.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/src/gchangepoint/.ipynb_checkpoints/GraphUtilities-checkpoint.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/LICENSE
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/README.md
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 gchangepoint-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    33344 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/src/gchangepoint/MST.so
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/src/gchangepoint/__init__.py
+-rw-r--r--   0        0        0    58649 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/src/gchangepoint/gchangepoint.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/src/gchangepoint/graphutilities.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/src/gchangepoint/.ipynb_checkpoints/GraphUtilities-checkpoint.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/LICENSE
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/README.md
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 gchangepoint-0.0.3/PKG-INFO
```

### Comparing `gchangepoint-0.0.2/src/gchangepoint/MST.so` & `gchangepoint-0.0.3/src/gchangepoint/MST.so`

 * *Files identical despite different names*

### Comparing `gchangepoint-0.0.2/src/gchangepoint/gchangepoint.py` & `gchangepoint-0.0.3/src/gchangepoint/gchangepoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,17 @@
                     def integrand(s):
                         x = rho1(N, s, n_edges, sum_degrees_squared)
                         return x*Nu(np.sqrt(2*b**2*x))
                     pval_original = norm.pdf(b)*b*integrate.quad(integrand, a=lower, b=upper)[0]
                     output["original"]=np.amin(np.concatenate(([pval_original], [1])))
         else:
             output["original"]=1
+            import
+            import
+            
     if statistic in ["all", "weighted", "wei", "w", "max", "m"]:
         t = np.arange(1, N, dtype="float")
         A1 = n_edges*t*(t-1)/(N*(N-1))+3*x1*t*(t-1)*(t-2)/(N*(N-1)*(N-2))+\
              (3*n_edges*(n_edges-1)-3*x1)*t*(t-1)*(t-2)*(t-3)/(N*(N-1)*(N-2)*(N-3))+\
              x2*t*(t-1)*(t-2)*(t-3)/(N*(N-1)*(N-2)*(N-3))+(6*x3-6*x5)*(t*(t-1)*(t-2)*(t-3))/(N*(N-1)*(N-2)*(N-3))+\
              2*x5*(t*(t-1)*(t-2))/(N*(N-1)*(N-2))+(3*x4+6*x5-12*x3)*t*(t-1)*(t-2)*(t-3)*(t-4)/(N*(N-1)*(N-2)*(N-3)*(N-4))+\
              (n_edges*(n_edges-1)*(n_edges-2)+6*x3-2*x5-x2-3*x4)*t*(t-1)*(t-2)*(t-3)*(t-4)*(t-5)/(N*(N-1)*(N-2)*(N-3)*(N-4)*(N-5))
@@ -860,19 +863,19 @@
         q = (N-t-1)/(N-2)
         p = (t-1)/(N-2)
         mu = n_edges*(q*t*(t-1)+p*(N-t)*(N-t-1))/(N*(N-1))
         sig1 = q**2*r1+2*q*p*r12+p**2*r2-mu**2
         sig = np.sqrt(sig1)
         ER3 = q**3*A1+3*q**2*p*B1+3*q*p**2*C1+p**3*D1
         r = np.float64((ER3-3*mu*sig**2-mu**3))/np.float64(sig**3)
-        b = scanZ["weighted"]["Zmax"]
-        result_u2 = pval2_sub2(N, b, r, x, lower, upper)
         r_Rw = r
         x_Rw = x
         if statistic in ["all", "weighted", "wei", "w"]:
+            b = scanZ["weighted"]["Zmax"]
+            result_u2 = pval2_sub2(N, b, r, x, lower, upper)
             if result_u2 > 0:
                 output["weighted"] = np.amin(np.concatenate(([result_u2], [1])))
             else:
                 if b > 0:
                     def integrand_W(t):
                         x = rho1_Rw(N, t)
                         return (b**2*x*Nu(np.sqrt(2*b**2*x)))**2*(N-t)
```

### Comparing `gchangepoint-0.0.2/src/gchangepoint/graphutilities.py` & `gchangepoint-0.0.3/src/gchangepoint/graphutilities.py`

 * *Files identical despite different names*

### Comparing `gchangepoint-0.0.2/src/gchangepoint/.ipynb_checkpoints/GraphUtilities-checkpoint.py` & `gchangepoint-0.0.3/src/gchangepoint/.ipynb_checkpoints/GraphUtilities-checkpoint.py`

 * *Files identical despite different names*

### Comparing `gchangepoint-0.0.2/LICENSE` & `gchangepoint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gchangepoint-0.0.2/README.md` & `gchangepoint-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gchangepoint-0.0.2/PKG-INFO` & `gchangepoint-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gchangepoint
-Version: 0.0.2
+Version: 0.0.3
 Summary: Graph-Based Changepoint Detection
 Author-email: Alexander Wold <alexwold@iastate.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
```

