# Comparing `tmp/schubmult-1.3.9.tar.gz` & `tmp/schubmult-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.9.tar", last modified: Wed May 22 10:54:39 2024, max compression
+gzip compressed data, was "schubmult-1.4.0.tar", last modified: Fri May 31 13:39:39 2024, max compression
```

## Comparing `schubmult-1.3.9.tar` & `schubmult-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:39.314000 schubmult-1.3.9/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-22 10:54:39.263000 schubmult-1.3.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5299 2024-05-12 18:38:20.000000 schubmult-1.3.9/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:36.625000 schubmult-1.3.9/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.9/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    18348 2024-05-20 18:10:32.000000 schubmult-1.3.9/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:37.410000 schubmult-1.3.9/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.9/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.9/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5027 2024-05-17 15:39:33.000000 schubmult-1.3.9/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:37.778000 schubmult-1.3.9/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.9/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.9/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5757 2024-05-17 15:05:46.000000 schubmult-1.3.9/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:38.138000 schubmult-1.3.9/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.9/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.9/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    10420 2024-05-17 14:57:50.000000 schubmult-1.3.9/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:38.504000 schubmult-1.3.9/schubmult/schubmult_q_double/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.9/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.9/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3456 2024-05-17 15:40:28.000000 schubmult-1.3.9/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:38.829000 schubmult-1.3.9/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.9/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.9/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    12623 2024-05-21 17:59:25.000000 schubmult-1.3.9/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:39.188000 schubmult-1.3.9/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.9/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.9/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    47692 2024-05-21 13:46:50.000000 schubmult-1.3.9/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:37.083000 schubmult-1.3.9/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-22 10:54:34.000000 schubmult-1.3.9/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-22 10:54:35.000000 schubmult-1.3.9/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-22 10:54:34.000000 schubmult-1.3.9/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-22 10:54:34.000000 schubmult-1.3.9/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-22 10:54:35.000000 schubmult-1.3.9/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-22 10:54:35.000000 schubmult-1.3.9/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-22 10:54:39.298000 schubmult-1.3.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-22 10:54:17.000000 schubmult-1.3.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:39.398000 schubmult-1.4.0/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.4.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5590 2024-05-31 13:39:39.356000 schubmult-1.4.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5208 2024-05-31 13:14:16.000000 schubmult-1.4.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:37.087000 schubmult-1.4.0/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.4.0/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20367 2024-05-30 11:18:20.000000 schubmult-1.4.0/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:37.802000 schubmult-1.4.0/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.4.0/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.4.0/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5027 2024-05-17 15:39:33.000000 schubmult-1.4.0/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:38.082000 schubmult-1.4.0/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.4.0/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.4.0/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5757 2024-05-17 15:05:46.000000 schubmult-1.4.0/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:38.394000 schubmult-1.4.0/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.4.0/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.4.0/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13618 2024-05-31 12:53:54.000000 schubmult-1.4.0/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:38.682000 schubmult-1.4.0/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.4.0/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.4.0/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3624 2024-05-31 13:19:38.000000 schubmult-1.4.0/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:38.967000 schubmult-1.4.0/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.4.0/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.4.0/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16474 2024-05-31 12:54:36.000000 schubmult-1.4.0/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:39.278000 schubmult-1.4.0/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.4.0/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.4.0/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    47692 2024-05-21 13:46:50.000000 schubmult-1.4.0/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 13:39:37.520000 schubmult-1.4.0/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5590 2024-05-31 13:39:35.000000 schubmult-1.4.0/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-31 13:39:36.000000 schubmult-1.4.0/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-31 13:39:35.000000 schubmult-1.4.0/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-31 13:39:35.000000 schubmult-1.4.0/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-31 13:39:35.000000 schubmult-1.4.0/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-31 13:39:35.000000 schubmult-1.4.0/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-31 13:39:39.391000 schubmult-1.4.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-31 13:14:49.000000 schubmult-1.4.0/setup.py
```

### Comparing `schubmult-1.3.9/LICENSE` & `schubmult-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.9/PKG-INFO` & `schubmult-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.9
+Version: 1.4.0
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.3, it also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing (equivariant, Molev-Sagan) Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. It also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
 schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6 --display-positive
 schubmult_q 5 1 4 3 2 - 5 1 3 4 2
 schubmult_q_double 5 1 4 3 2 - 5 1 3 4 2
@@ -46,24 +46,24 @@
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
 schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
-Since version 1.3.7, schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
+schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
 ```
 schubmult_q_yz -nil-hecke 6 -code 2 2 --display-positive
 ```
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
-New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
+schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for quantum). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6)) # outputs dictionary with results  
@@ -72,13 +72,13 @@
 
 ```
 from schubmult.schubmult_py import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6))
 ```
 
-Version 1.0.18 adds the command line argument --display-positive to schubmult_yz (and version 1.3.3 adds --display-positive to schubmult_q_yz), which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
+The command line argument --display-positive is available in schubmult_yz and schubmult_q_yz, which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
 
 ![](https://raw.githubusercontent.com/matthematics/schubmult/main/positive_image.png)
 
 [Homepage of schubmult](http://schubmult.org/)
```

### Comparing `schubmult-1.3.9/README.md` & `schubmult-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.3, it also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing (equivariant, Molev-Sagan) Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. It also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
 schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6 --display-positive
 schubmult_q 5 1 4 3 2 - 5 1 3 4 2
 schubmult_q_double 5 1 4 3 2 - 5 1 3 4 2
@@ -33,24 +33,24 @@
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
 schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
-Since version 1.3.7, schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
+schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
 ```
 schubmult_q_yz -nil-hecke 6 -code 2 2 --display-positive
 ```
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
-New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
+schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for quantum). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6)) # outputs dictionary with results  
@@ -59,12 +59,12 @@
 
 ```
 from schubmult.schubmult_py import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6))
 ```
 
-Version 1.0.18 adds the command line argument --display-positive to schubmult_yz (and version 1.3.3 adds --display-positive to schubmult_q_yz), which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
+The command line argument --display-positive is available in schubmult_yz and schubmult_q_yz, which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
 
 ![](https://raw.githubusercontent.com/matthematics/schubmult/main/positive_image.png)
 
 [Homepage of schubmult](http://schubmult.org/)
```

### Comparing `schubmult-1.3.9/schubmult/perm_lib.py` & `schubmult-1.4.0/schubmult/perm_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from bisect import bisect_left
 import numpy as np
 
 n = 100
 
 q_var = symarray("q",n)
 
+def getpermval(perm,index):
+	if index<len(perm):
+		return perm[index]
+	return index+1
+
 def inv(perm):
 	L = len(perm)
 	v = [i for i in range(1,L+1)]
 	ans = 0
 	for i in range(L):
 		itr = bisect_left(v, perm[i])
 		ans += itr
@@ -659,8 +664,84 @@
 		vpm_list = vpm_list2
 	for vpm, b in vpm_list:
 		if vpm[vnum-1]==len(v)+1:
 			vpm2 = [*vpm]
 			vpm2.pop(vnum-1)
 			vp = permtrim(vpm2)
 			ret_list += [[[v[i] for i in range(vnum,len(v)) if ((i>len(vp) and v[i]==i) or (i<=len(vp) and v[i]==vp[i-1]))],vp]]
-	return ret_list			
+	return ret_list			
+	
+def get_cycles(perm):
+	cycle_set = []
+	done_vals = set()
+	for i in range(len(perm)):
+		p = i + 1
+		if perm[i] == p:
+			continue
+		if p in done_vals:
+			continue
+		cycle = []
+		m = -1
+		max_index = -1
+		while p not in done_vals:
+			cycle += [p]
+			done_vals.add(p)
+			if p>m:
+				m = p
+				max_index = len(cycle) - 1
+			p = perm[p-1]
+		cycle = tuple(cycle[max_index+1:] + cycle[:max_index+1])
+		cycle_set += [cycle]
+	return cycle_set
+	
+def double_elem_sym_q(u,p1,p2,k):
+	ret_list = {}
+	perms1 = elem_sym_perms_q(u,p1,k)
+	iu = inverse(u)
+	for perm1, udiff1, mul_val1 in perms1:
+		perms2 = elem_sym_perms_q(perm1,p2,k)
+		cycles1 = get_cycles(tuple(permtrim(mulperm(iu,[*perm1]))))
+		cycles1_dict = {}
+		for c in cycles1:
+			if c[-1] not in cycles1_dict:
+				cycles1_dict[c[-1]] = []
+			cycles1_dict[c[-1]]+= [set(c)]
+		ip1 = inverse(perm1)
+		for perm2, udiff2, mul_val2 in perms2:
+			cycles2 = get_cycles(tuple(permtrim(mulperm(ip1,[*perm2]))))
+			good = True
+			for i in range(len(cycles2)):
+				c2 = cycles2[i]
+				if c2[-1] not in cycles1_dict:
+					continue
+				for c1_s in cycles1_dict[c2[-1]]:
+					for a in range(len(c2)-2,-1,-1):
+						if c2[a] in c1_s:
+							good = False
+							break
+					if not good:
+						break														
+				if not good:
+					break
+			
+			if good:				
+				if (perm1,udiff1,mul_val1) not in ret_list:
+					ret_list[(perm1,udiff1,mul_val1)] = []
+				ret_list[(perm1,udiff1,mul_val1)] += [(perm2,udiff2,mul_val2)]
+	return ret_list
+
+def medium_theta(perm):
+	cd = code(perm)
+	found_one = True
+	while found_one:
+		found_one = False
+		for i in range(len(cd)-1):
+			if cd[i]<cd[i+1]: 
+				found_one = True
+				cd[i], cd[i+1] = cd[i+1]+1, cd[i]
+				break
+			if cd[i]==cd[i+1] and cd[i]!=0 and i>0 and cd[i-1]<=cd[i]+1:
+			#if cd[i]==cd[i+1] and i>0 and cd[i-1]<=cd[i]+1:
+				cd[i]+=1
+				found_one = True
+				break
+	return cd
```

### Comparing `schubmult-1.3.9/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.4.0/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.9/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.4.0/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.9/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.4.0/schubmult/schubmult_q/schubmult_q.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,14 +59,100 @@
 
 for i in range(1,n):
 	sm = var_r[0]
 	for j in range(1,i):
 		sm += var_r[j]
 	subs_dict[var2[i]] = sm
 
+def schubmult_db(perm_dict,v,var2=var2,var3=var3):
+	if v == (1,2):
+		return perm_dict
+	th = medium_theta(inverse(v))
+	#print(f"{th=}")
+	while th[-1] == 0:
+		th.pop()
+	#if len(set(th))!=len(th):
+	#	print(f"medium theta {th=}")
+	mu = permtrim(uncode(th))
+	vmu = permtrim(mulperm([*v],mu))
+	inv_vmu = inv(vmu)
+	inv_mu = inv(mu)
+	ret_dict = {}
+	vpaths = [([(vmu,0)],1)]
+	
+	thL = len(th)
+	#if thL!=2 and len(set(thL))!=1:
+	#	raise ValueError("Not what I can do")
+	vpathdicts = compute_vpathdicts(th,vmu,True)
+	#print(f"{vpathdicts=}")
+	for u,val in perm_dict.items():
+		inv_u = inv(u)
+		vpathsums = {u: {(1,2): val}}
+		for index in range(thL):
+			if index>0 and th[index-1] == th[index]:
+				continue				
+			mx_th = 0
+			for vp in vpathdicts[index]:
+				for v2,vdiff,s in vpathdicts[index][vp]:
+					if th[index]-vdiff > mx_th:
+						mx_th = th[index] - vdiff
+			if index<len(th)-1 and th[index] == th[index+1]:
+				mx_th1 = 0
+				for vp in vpathdicts[index+1]:
+					for v2,vdiff,s in vpathdicts[index+1][vp]:
+						if th[index+1]-vdiff > mx_th1:
+							mx_th1 = th[index+1] - vdiff				
+				newpathsums = {}
+				for up in vpathsums:
+					newpathsums0 = {}
+					inv_up = inv(up)
+					newperms = double_elem_sym_q(up,mx_th,mx_th1,th[index])
+					for v in vpathdicts[index]:
+						sumval = vpathsums[up].get(v,zero)
+						if sumval == 0:
+							continue
+						for v2,vdiff2,s2 in vpathdicts[index][v]:
+							for up1, udiff1, mul_val1 in newperms:
+								if (up1,udiff1,mul_val1) not in newpathsums0:
+									newpathsums0[(up1,udiff1,mul_val1)] = {}
+								if udiff1 + vdiff2 == th[index]:
+									newpathsums0[(up1,udiff1,mul_val1)][v2] = newpathsums0[(up1,udiff1,mul_val1)].get(v2,zero)+s2*sumval*mul_val1
+					
+					for up1, udiff1, mul_val1 in newpathsums0:
+						for v in vpathdicts[index+1]:
+							sumval = newpathsums0[(up1,udiff1,mul_val1)].get(v,zero)
+							if sumval == 0:
+								continue
+							for v2,vdiff2,s2 in vpathdicts[index+1][v]:
+								for up2, udiff2, mul_val2 in newperms[(up1,udiff1,mul_val1)]:
+									if up2 not in newpathsums:
+										newpathsums[up2]={}
+									if udiff2 + vdiff2 == th[index+1]:
+										newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s2*sumval*mul_val2
+			else:
+				newpathsums = {}
+				for up in vpathsums:
+					inv_up = inv(up)
+					newperms = elem_sym_perms_q(up,min(mx_th,(inv_mu-(inv_up-inv_u))-inv_vmu),th[index])
+					for up2, udiff, mul_val in newperms:
+						if up2 not in newpathsums:
+							newpathsums[up2]={}
+						for v in vpathdicts[index]:
+							sumval = vpathsums[up].get(v,zero)
+							if sumval == 0:
+								continue
+							for v2,vdiff,s in vpathdicts[index][v]:
+								if udiff+vdiff==th[index]:
+									newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*mul_val
+			vpathsums = newpathsums
+		toget = tuple(vmu)
+		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
+	return ret_dict
+
+
 def schubmult(perm_dict,v):
 	th = strict_theta(inverse(v))
 	mu = permtrim(uncode(th))
 	vmu = permtrim(mulperm([*v],mu))
 	#print(f"{th=} {mu=} {vmu=}")
 	inv_vmu = inv(vmu)
 	inv_mu = inv(mu)
@@ -173,20 +259,24 @@
 		pr = True
 		ascode = False
 		grass = False
 		grass_q_n = 0
 		equiv = False
 		mult = False
 		mulstring = ""
+		slow = False
 		
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if s == "--slow":
+					slow = True
+					continue
 				if mult:
 					mulstring += s
 					continue
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "-grass":
@@ -340,16 +430,20 @@
 		else:		
 			if ascode:
 				for i in range(len(perms)):
 					perms[i] = uncode(perms[i])
 		
 			coeff_dict = {tuple(permtrim([*perms[0]])): 1}
 			
-			for perm in perms[1:]:
-				coeff_dict = schubmult(coeff_dict,tuple(permtrim([*perm])))
+			if not slow:
+				for perm in perms[1:]:
+					coeff_dict = schubmult_db(coeff_dict,tuple(permtrim([*perm])))
+			else:
+				for perm in perms[1:]:
+					coeff_dict = schubmult(coeff_dict,tuple(permtrim([*perm])))
 			
 			if mult:
 				mul_exp = sympify(mulstring)
 				coeff_dict = mult_poly(coeff_dict,mul_exp)
 				
 			if pr:
 				if ascode:
```

### Comparing `schubmult-1.3.9/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.4.0/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from schubmult.perm_lib import *
-from schubmult.schubmult_q_yz import schubmult, mult_poly
+from schubmult.schubmult_q_yz import schubmult, schubmult_db, mult_poly
 from symengine import *
 import sys
 
 
 q_var = symarray("q",100)
 
 var2 = symarray("y",100)
@@ -33,20 +33,24 @@
 		pr = True
 		display_positive = False
 		ascode = False
 		coprod = False
 		check = True
 		msg = False
 		mult = False
+		slow = False
 		mulstring = ""
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
+				if s == "--slow":
+					slow = True
+					continue
 				if mult:
 					mulstring += s
 					continue
 				if s == "-mult":
 					mult = True
 					continue
 				if s == "-nocheck":
@@ -92,15 +96,18 @@
 				perms[i] = tuple(permtrim([*perms[i]]))
 		
 		size = 0
 		L = len(perms)
 		
 		coeff_dict = {perms[0]: 1}
 		for perm in perms[1:]:
-			coeff_dict = schubmult(coeff_dict,perm,var2,var2)
+			if slow:
+				coeff_dict = schubmult(coeff_dict,perm,var2,var2)
+			else:
+				coeff_dict = schubmult_db(coeff_dict,perm,var2,var2)
 		if mult:
 			mul_exp = sympify(mulstring)
 			coeff_dict = mult_poly(coeff_dict,mul_exp)
 		
 		if pr:
 			if ascode:
 				width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(sympify(coeff_dict[perm]).subs(subs_dict))!=0])
```

### Comparing `schubmult-1.3.9/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.4.0/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 19% similar despite different names*

```diff
@@ -145,14 +145,107 @@
 							#print(f"{code(up2)=} {elem_sym_func_q(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)=} {mul_val=} {sumval=}")							
 							newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*elem_sym_func_q(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)
 			vpathsums = newpathsums
 		toget = tuple(vmu)
 		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
 	return ret_dict
 
+def schubmult_db(perm_dict,v,var2=var2,var3=var3):
+	if v == (1,2):
+		return perm_dict
+	th = medium_theta(inverse(v))
+	#print(f"{th=}")
+	while th[-1] == 0:
+		th.pop()
+	#if len(set(th))!=len(th):
+	#	print(f"medium theta {th=}")
+	mu = permtrim(uncode(th))
+	vmu = permtrim(mulperm([*v],mu))
+	inv_vmu = inv(vmu)
+	inv_mu = inv(mu)
+	ret_dict = {}
+	vpaths = [([(vmu,0)],1)]
+	
+	thL = len(th)
+	#if thL!=2 and len(set(thL))!=1:
+	#	raise ValueError("Not what I can do")
+	vpathdicts = compute_vpathdicts(th,vmu,True)
+	#print(f"{vpathdicts=}")
+	for u,val in perm_dict.items():
+		inv_u = inv(u)
+		vpathsums = {u: {(1,2): val}}
+		for index in range(thL):
+			if index>0 and th[index-1] == th[index]:
+				continue				
+			mx_th = 0
+			for vp in vpathdicts[index]:
+				for v2,vdiff,s in vpathdicts[index][vp]:
+					if th[index]-vdiff > mx_th:
+						mx_th = th[index] - vdiff
+			if index<len(th)-1 and th[index] == th[index+1]:
+				mx_th1 = 0
+				for vp in vpathdicts[index+1]:
+					for v2,vdiff,s in vpathdicts[index+1][vp]:
+						if th[index+1]-vdiff > mx_th1:
+							mx_th1 = th[index+1] - vdiff				
+				newpathsums = {}
+				for up in vpathsums:
+					newpathsums0 = {}
+					inv_up = inv(up)
+					newperms = double_elem_sym_q(up,mx_th,mx_th1,th[index])
+					#for up1, up2, udiff1,udiff2,mul_val1,mul_val2 in newperms:
+					for v in vpathdicts[index]:
+						sumval = vpathsums[up].get(v,zero)
+						if sumval == 0:
+							continue
+						for v2,vdiff2,s2 in vpathdicts[index][v]:
+							for up1, udiff1, mul_val1 in newperms:
+								esim1 = elem_sym_func_q(th[index],index+1,up,up1,v,v2,udiff1,vdiff2,var2,var3)*mul_val1*s2
+								mulfac = sumval*esim1
+								if (up1,udiff1,mul_val1) not in newpathsums0:
+									newpathsums0[(up1,udiff1,mul_val1)] = {}
+								#newpathsums0[(up1, udiff1, mul_val1
+								newpathsums0[(up1,udiff1,mul_val1)][v2] = newpathsums0[(up1,udiff1,mul_val1)].get(v2,0) + mulfac
+					
+					for up1, udiff1, mul_val1 in newpathsums0:
+						for v in vpathdicts[index+1]:
+							sumval = newpathsums0[(up1,udiff1,mul_val1)].get(v,zero)
+							if sumval == 0:
+								continue
+							for v2,vdiff2,s2 in vpathdicts[index+1][v]:
+								for up2, udiff2, mul_val2 in newperms[(up1,udiff1,mul_val1)]:
+									esim1 = elem_sym_func_q(th[index+1],index+2,up1,up2,v,v2,udiff2,vdiff2,var2,var3)*mul_val2*s2
+									mulfac = sumval*esim1
+									if up2 not in newpathsums:
+										newpathsums[up2] = {}
+									newpathsums[up2][v2] = newpathsums[up2].get(v2,0) + mulfac
+											#for up2, udiff2, mul_val2 in newperms[(up1,udiff1,mul_val1)]:
+											#	if up2 not in newpathsums:
+											#		newpathsums[up2]={}
+											#	for v3,vdiff3,s3 in vpathdicts[index+1][v2]:
+											#			newpathsums[up2][v3] = newpathsums[up2].get(v3,zero)+s3*mul_val2*mulfac*elem_sym_func_q(th[index+1],index+2,up1,up2,v2,v3,udiff2,vdiff3,var2,var3)
+			else:
+				newpathsums = {}
+				for up in vpathsums:
+					inv_up = inv(up)
+					newperms = elem_sym_perms_q(up,min(mx_th,(inv_mu-(inv_up-inv_u))-inv_vmu),th[index])
+					for up2, udiff,mul_val in newperms:
+						if up2 not in newpathsums:
+							newpathsums[up2]={}
+						for v in vpathdicts[index]:
+							sumval = vpathsums[up].get(v,zero)*mul_val
+							if sumval == 0:
+								continue
+							for v2,vdiff,s in vpathdicts[index][v]:
+								newpathsums[up2][v2] = newpathsums[up2].get(v2,zero)+s*sumval*elem_sym_func_q(th[index],index+1,up,up2,v,v2,udiff,vdiff,var2,var3)
+			vpathsums = newpathsums
+		toget = tuple(vmu)
+		ret_dict = add_perm_dict({ep: vpathsums[ep].get(toget,0) for ep in vpathsums},ret_dict)
+	return ret_dict
+
 q_var2 = q_var.tolist()
 
 def sum_q_dict(q_dict1,q_dict2):
 	ret = {**q_dict1}
 	for key in q_dict2:
 		ret[key] = ret.get(key,0) + q_dict2[key]
 	return ret
@@ -266,27 +359,31 @@
 		ascode = False
 		coprod = False
 		nilhecke = False
 		check = True
 		msg = False
 		just_nil = False
 		mult = False
+		slow = False
 		
 		nil_N = 0
 		
 		mulstring = ""
 		norep = False
 		expa = False
 		
 		try:
 			for s in sys.argv[1:]:
 				if just_nil:
 					just_nil = False
 					nil_N = int(s)
 					continue
+				if s == "--slow":
+					slow = True
+					continue
 				if s == "--norep":
 					norep = True
 					continue
 				if s == "--expand":
 					expa = True
 					continue
 				if s == "-np" or s == "--no-print":
@@ -346,31 +443,37 @@
 		
 		if nilhecke:
 			coeff_dict = nil_hecke({(1,2): 1},perms[0],nil_N)			
 			rep = ("y","x")		
 		else:
 			coeff_dict = {perms[0]: 1}
 			for perm in perms[1:]:
-				coeff_dict = schubmult(coeff_dict,perm)
+				if not slow:
+					coeff_dict = schubmult_db(coeff_dict,perm)
+				else:
+					coeff_dict = schubmult(coeff_dict,perm)
 			if mult:
 				for v in var2:
 					globals()[str(v)] = v
 				for v in var3:
 					globals()[str(v)] = v	
 				for v in var_x:
 					globals()[str(v)] = v	
+				for v in q_var:
+					globals()[str(v)] = v
+				q = q_var
 				mul_exp = eval(mulstring)
 				coeff_dict = mult_poly(coeff_dict,mul_exp)
 			rep = ("","")			
 		
 		if pr:
-			if ascode:
-				width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
-			else:
-				width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
+			#if ascode:
+			#	width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
+			#else:
+			#	width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			
 			coeff_perms = list(coeff_dict.keys())
 			coeff_perms.sort(key=lambda x: (inv(x),*x))
 			
 			for perm in coeff_perms:
 				val = coeff_dict[perm]
 				if expand(val) != 0:
@@ -421,20 +524,20 @@
 									exit(1)
 							val = val2
 					if expa:
 						val = expand(val)
 					if val!=0:
 						if ascode:
 							if norep:
-								print(f"{str(trimcode(perm)):>{width}}  {str(val).replace(*rep)}")	
+								print(f"{str(trimcode(perm))}  {str(val).replace(*rep)}")	
 							else:
-								print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
+								print(f"{str(trimcode(perm))}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 						else:
 							if norep:
-								print(f"{str(perm):>{width}}  {str(val).replace(*rep)}")	
+								print(f"{str(perm)}  {str(val).replace(*rep)}")	
 							else:
-								print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
+								print(f"{str(perm)}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 	except BrokenPipeError:
 		pass
 		
 if __name__ == "__main__":
 	main()
```

### Comparing `schubmult-1.3.9/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.4.0/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.9/schubmult.egg-info/PKG-INFO` & `schubmult-1.4.0/schubmult.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.9
+Version: 1.4.0
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # schubmult
 
 ## Program and package for computing Littlewood-Richardson coefficients of Schubert polynomials
 
-This is a set of python scripts written by Matt Samuel for computing Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. Since version 1.3.3, it also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
+This is a set of python scripts written by Matt Samuel for computing (equivariant, Molev-Sagan) Littlewood-Richardson coefficients of (ordinary or double) Schubert polynomials. It also handles (double) quantum Schubert polynomials, if double then either in the same set or different sets of coefficient variables; that is to say it compute the (equivariant/mixed) Gromov-Witten invariants of the complete flag variety. It has the same command line syntax as the program "schubmult" in lrcalc by Anders Buch. Example:
 
 ```
 schubmult_py 1 2 4 9 11 6 8 12 3 5 7 10 - 6 8 1 2 3 4 7 10 12 14 5 9 11 13  
 schubmult_double 1 3 4 6 2 5 - 2 1 5 7 3 4 6  
 schubmult_yz 1 3 4 6 2 5 - 2 1 5 7 3 4 6 --display-positive
 schubmult_q 5 1 4 3 2 - 5 1 3 4 2
 schubmult_q_double 5 1 4 3 2 - 5 1 3 4 2
@@ -46,24 +46,24 @@
 or
 ```
 schubmult_py -code -coprod 0 1 2 3 - 2 4
 schubmult_double -code -coprod 0 1 2 3 - 2 4
 schubmult_yz -code -coprod 0 1 2 3 - 2 4 --display-positive
 ```
 
-Since version 1.3.7, schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
+schubmult_q_yz has a feature for displaying the coefficients of the divided difference operators in the evaluation of the quantum double Schubert polynomials on the commuting difference operators of Fomin, Gelfand, and Postnikov. It is necessary to cap the value of n in the group S_n we are working in because as n increases the expression does not stabilize.
 ```
 schubmult_q_yz -nil-hecke 6 -code 2 2 --display-positive
 ```
 
 Runtime will vary tremendously by case. The general problem is #P-hard. Though the result is always nonnegative (which at least is known for schubmult_py, schubmult_q, schubmult_double, and schubmult_q_double) and the problem is in GapP, it is not known to be in #P at this time.
 
 schubmult_py is for multiplying ordinary Schubert polynomials. schubmult_yz is for multiplying double Schubert polynomials in different sets of coefficient variables (labeled y and z), and schubmult_double is for multiplying double Schubert polynomials in the same set of coefficient variables. Similarly, schubmult_q is for multiplying quantum Schubert polynomials, schubmult_q_double is for multiplying quantum double Schubert polynomials in the same set of coefficient variables, and schubmult_q_yz is for multiplying quantum double Schubert polynomials in different sets of coefficient variables, or in other words it computes the Gromov-Witten invariants, equivariant Gromov-Witten invariants, and (mixed?) equivariant Gromov-Witten invariants of the complete flag variety. All have the same command line syntax as schubmult, except when using the -code option. schubmult_double/schubmult_q_double display the result with nonnegative coefficients in terms of the negative simple roots (and the q variables), and schubmult_yz and schubmult_q_yz optionally display the result positively in terms of y_i-z_j (and q) with the --display-positive option.
 
-New in version 1.1.0, schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for schubmult_q). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
+schubmult_xx -coprod allows you to split (double) Schubert polynomials along certain indices (not available for quantum). It takes one permutation as an argument, followed by a dash -, then the set of indices you would like to split on. These coefficients are always nonnegative since they occur as product coefficients (this is actually how they are computed).
 
 When imported as a python package, the relevant packages are schubmult.perm_lib, which has various permutation manipulation functions, and three modules that have functions of the same name (function name is "schubmult"): schubmult.schubmult_py, schubmult.schubmult_yz, schubmult.schubmult_double. Function takes a permutation dictionary (keys are tuples of ints, which must be trimmed permutations, and values are either integers or symengine values, which can also be integers) as well as a permutation as its second argument, which is the (double) Schubert polynomial to multiply by. Returns a dictionary of the same form with the coefficients.
 
 ```
 from schubmult.schubmult_yz import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6)) # outputs dictionary with results  
@@ -72,13 +72,13 @@
 
 ```
 from schubmult.schubmult_py import schubmult  
   
 coeff_dict = schubmult({(1,3,4,6,2,5): 1},(2,1,5,7,3,4,6))
 ```
 
-Version 1.0.18 adds the command line argument --display-positive to schubmult_yz (and version 1.3.3 adds --display-positive to schubmult_q_yz), which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
+The command line argument --display-positive is available in schubmult_yz and schubmult_q_yz, which displays the result positively (if possible, this is still only always possible conjecturally). It will fail and print out the offending case if it finds a counterexample. This is highly processor intensive.
 
 ![](https://raw.githubusercontent.com/matthematics/schubmult/main/positive_image.png)
 
 [Homepage of schubmult](http://schubmult.org/)
```

### Comparing `schubmult-1.3.9/schubmult.egg-info/SOURCES.txt` & `schubmult-1.4.0/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.9/setup.py` & `schubmult-1.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.9",
+    version="1.4.0",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

