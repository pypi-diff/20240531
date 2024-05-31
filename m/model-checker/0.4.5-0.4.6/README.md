# Comparing `tmp/model_checker-0.4.5.tar.gz` & `tmp/model_checker-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.4.5.tar", last modified: Tue May 28 17:34:47 2024, max compression
+gzip compressed data, was "model_checker-0.4.6.tar", last modified: Fri May 31 19:33:38 2024, max compression
```

## Comparing `model_checker-0.4.5.tar` & `model_checker-0.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.5/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-28 17:34:47.313779 model_checker-0.4.5/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     8817 2024-05-28 16:55:37.000000 model_checker-0.4.5/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-28 17:34:42.000000 model_checker-0.4.5/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-28 17:34:47.313779 model_checker-0.4.5/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.312779 model_checker-0.4.5/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)      595 2024-05-28 17:34:42.000000 model_checker-0.4.5/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    13743 2024-05-27 19:03:37.000000 model_checker-0.4.5/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    23866 2024-05-28 17:17:04.000000 model_checker-0.4.5/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    28248 2024-05-27 19:03:37.000000 model_checker-0.4.5/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    30661 2024-05-28 17:04:14.000000 model_checker-0.4.5/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7856 2024-05-25 01:29:18.000000 model_checker-0.4.5/src/model_checker/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     9602 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      492 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-28 17:34:47.000000 model_checker-0.4.5/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-28 17:34:47.313779 model_checker-0.4.5/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     7788 2024-05-28 17:34:02.000000 model_checker-0.4.5/test/test_sat.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-31 19:33:38.276641 model_checker-0.4.6/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.6/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)    10108 2024-05-31 19:33:38.276641 model_checker-0.4.6/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     9323 2024-05-31 15:53:22.000000 model_checker-0.4.6/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-31 19:33:34.000000 model_checker-0.4.6/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-31 19:33:38.276641 model_checker-0.4.6/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-31 19:33:38.275641 model_checker-0.4.6/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-31 19:33:38.275641 model_checker-0.4.6/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)      595 2024-05-31 19:33:34.000000 model_checker-0.4.6/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    13743 2024-05-27 19:03:37.000000 model_checker-0.4.6/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    24478 2024-05-31 18:12:36.000000 model_checker-0.4.6/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    28341 2024-05-30 22:15:13.000000 model_checker-0.4.6/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    37277 2024-05-31 19:32:26.000000 model_checker-0.4.6/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7884 2024-05-30 19:26:28.000000 model_checker-0.4.6/src/model_checker/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-31 19:33:38.276641 model_checker-0.4.6/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)    10108 2024-05-31 19:33:38.000000 model_checker-0.4.6/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      492 2024-05-31 19:33:38.000000 model_checker-0.4.6/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-31 19:33:38.000000 model_checker-0.4.6/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-31 19:33:38.000000 model_checker-0.4.6/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-31 19:33:38.000000 model_checker-0.4.6/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-31 19:33:38.000000 model_checker-0.4.6/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-31 19:33:38.276641 model_checker-0.4.6/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     7788 2024-05-28 17:34:02.000000 model_checker-0.4.6/test/test_sat.py
```

### Comparing `model_checker-0.4.5/LICENCE` & `model_checker-0.4.6/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.5/PKG-INFO` & `model_checker-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.5
+Version: 0.4.6
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -16,26 +16,27 @@
 
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 The language currently includes the following operators:
 
   - `neg` for _negation_
-  <!-- - `not` for _exclusion_ -->
   - `wedge` for _conjunction_
   - `vee` for _disjunction_
   - `rightarrow` for _material conditional_
   - `leftrightarrow` for _material biconditional_
   - `Box` for _necessity_
   - `Diamond` for _possibility_
   - `boxright` for the _must counterfactual conditional_
   - `circleright` for the _might counterfactual conditional_
   - `leq` for _ground_
   - `sqsubseteq` for _essence_
   - `equiv` for _propositional identity_
+  - `preceq` for _relevance_
+  <!-- - `not` for _exclusion_ -->
 
 Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
 To generate a test file run `model-checker` in the terminal without arguments.
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
@@ -99,19 +100,22 @@
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
 
 A _grounding sentence_ `A leq B` may be read '`A` is _sufficient for_ `B`' and an _essence sentence_ `A sqsubseteq B` may be read '`A` is _necessary for_ `B`'.
 A _propositional identity sentence_ `A equiv B` may be read '`A` _just is for_ `B`'.
+A _relevance sentence_ `A preceq B` may be read '`A` _is wholly relevant to_ `B`'.
 The semantics for ground requires every verifier for the antecedent to be a verifier for the consequent, any fusion of a falsifier for the antecedent and consequent to be a falsifier for the consequent, and any falsifier for the consequent to have a part that falsifies the antecedent.
 The semantics for essence requires every fusion of a verifier for the antecedent and consequent to be a verifier for the consequent, any verifier for the consequent must have a part that verifies the antecedent, and every falsifier for the antecedent to be a falsifier for the consequent.
 The semantics for propositional identity requires the two arguments to have the same verifiers and falsifiers.
-All three constitutive operators are interdefinable as indicated below: 
+The semantics for relevance requires any fusion of verifiers for the antecedent and consequent to be a verifier for the consequent and, similarly, any fusion of falsifiers for the antecedent and consequent to be a falsifier for the consequent.
+Whereas the first three constitutive operators are interdefinable, relevance is definable in terms of the other constitutive operators but not _vice versa_:
 
 - `A leq B  :=  neg A sqsubseteq neg B  :=  (A vee B) equiv B`.
 - `A sqsubseteq B  :=  neg A leq neg B  :=  (A wedge B) equiv B`.
 - `A equiv B  :=  (A leq B) wedge (B leq A)  :=  (A sqsubseteq B) wedge (B sqsubseteq A)`.
+- `A preceq B  :=  (A wedge B) leq B :=  (A vee B) sqsubseteq B`.
 
 Instead of a Boolean lattice as in extensional and intensional semantics theories, the space of hyperintensional propositions forms a non-interlaced bilattice as described in this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w), building on [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 
 More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.4.5/README.md` & `model_checker-0.4.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 The language currently includes the following operators:
 
   - `neg` for _negation_
-  <!-- - `not` for _exclusion_ -->
   - `wedge` for _conjunction_
   - `vee` for _disjunction_
   - `rightarrow` for _material conditional_
   - `leftrightarrow` for _material biconditional_
   - `Box` for _necessity_
   - `Diamond` for _possibility_
   - `boxright` for the _must counterfactual conditional_
   - `circleright` for the _might counterfactual conditional_
   - `leq` for _ground_
   - `sqsubseteq` for _essence_
   - `equiv` for _propositional identity_
+  - `preceq` for _relevance_
+  <!-- - `not` for _exclusion_ -->
 
 Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
 To generate a test file run `model-checker` in the terminal without arguments.
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
@@ -83,19 +84,22 @@
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
 
 A _grounding sentence_ `A leq B` may be read '`A` is _sufficient for_ `B`' and an _essence sentence_ `A sqsubseteq B` may be read '`A` is _necessary for_ `B`'.
 A _propositional identity sentence_ `A equiv B` may be read '`A` _just is for_ `B`'.
+A _relevance sentence_ `A preceq B` may be read '`A` _is wholly relevant to_ `B`'.
 The semantics for ground requires every verifier for the antecedent to be a verifier for the consequent, any fusion of a falsifier for the antecedent and consequent to be a falsifier for the consequent, and any falsifier for the consequent to have a part that falsifies the antecedent.
 The semantics for essence requires every fusion of a verifier for the antecedent and consequent to be a verifier for the consequent, any verifier for the consequent must have a part that verifies the antecedent, and every falsifier for the antecedent to be a falsifier for the consequent.
 The semantics for propositional identity requires the two arguments to have the same verifiers and falsifiers.
-All three constitutive operators are interdefinable as indicated below: 
+The semantics for relevance requires any fusion of verifiers for the antecedent and consequent to be a verifier for the consequent and, similarly, any fusion of falsifiers for the antecedent and consequent to be a falsifier for the consequent.
+Whereas the first three constitutive operators are interdefinable, relevance is definable in terms of the other constitutive operators but not _vice versa_:
 
 - `A leq B  :=  neg A sqsubseteq neg B  :=  (A vee B) equiv B`.
 - `A sqsubseteq B  :=  neg A leq neg B  :=  (A wedge B) equiv B`.
 - `A equiv B  :=  (A leq B) wedge (B leq A)  :=  (A sqsubseteq B) wedge (B sqsubseteq A)`.
+- `A preceq B  :=  (A wedge B) leq B :=  (A vee B) sqsubseteq B`.
 
 Instead of a Boolean lattice as in extensional and intensional semantics theories, the space of hyperintensional propositions forms a non-interlaced bilattice as described in this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w), building on [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 
 More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.4.5/pyproject.toml` & `model_checker-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.4.5"
+version = "0.4.6"
 description = "A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `model_checker-0.4.5/src/model_checker/__init__.py` & `model_checker-0.4.6/src/model_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.5/src/model_checker/__main__.py` & `model_checker-0.4.6/src/model_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.5/src/model_checker/model_definitions.py` & `model_checker-0.4.6/src/model_checker/model_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,17 +129,18 @@
             print_str += ", "
     print_str += "}"
     return print_str
 
 def product(set_A, set_B):
     """set of pairwise fusions of elements in set_A and set_B"""
     product_set = set()
-    for a in set_A:
-        for b in set_B:
-            product_set.add(bit_fusion(a,b))
+    for bit_a in set_A:
+        for bit_b in set_B:
+            bit_ab = bit_fusion(bit_a, bit_b)
+            product_set.add(bit_ab)
     return product_set
 
 def coproduct(set_A, set_B):
     """union closed under pairwise fusion"""
     A_U_B = set_A.union(set_B)
     return A_U_B.union(product(set_A, set_B))
 
@@ -481,14 +482,26 @@
                         break
         if not comp_state_parts and incomp_ver_parts:
             excluders.append(state)
     # TODO: would be nice to sort the excluders but they are bits
     # excluders_list = sorted(excluders)
     return excluders
 
+def all_has_part(set_A, set_B):
+    """checks whether every element in set_A has a part in set_B"""
+    for bit_z in set_A:
+        found = False
+        for bit_y in set_B:
+            if bit_part(bit_y, bit_z):
+                found = True
+                break
+        if not found:
+            return False
+    return True
+
 def find_complex_proposition(model_structure, complex_sentence, eval_world):
     """sentence is a sentence in prefix notation
     For a given complex proposition, returns the verifiers and falsifiers of that proposition
     given a solved model
     for a counterfactual, it'll just give the worlds it's true at and worlds it's not true at
     """
     if not model_structure.atomic_props_dict:
@@ -508,21 +521,21 @@
     if "not" in op:
         all_bits = model_structure.all_bits
         poss_bits = model_structure.poss_bits
         Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
         vers = find_excluders(Y_F, all_bits, poss_bits, null_singleton)
         fals = find_excluders(Y_V, all_bits, poss_bits, null_singleton)
         return (vers, fals)
-    if "pre" in op:
-        all_bits = model_structure.all_bits
-        poss_bits = model_structure.poss_bits
-        Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
-        vers = find_precluders(Y_F, all_bits, poss_bits)
-        fals = find_precluders(Y_V, all_bits, poss_bits)
-        return (vers, fals)
+    # if "pre" in op:
+    #     all_bits = model_structure.all_bits
+    #     poss_bits = model_structure.poss_bits
+    #     Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
+    #     vers = find_precluders(Y_F, all_bits, poss_bits)
+    #     fals = find_precluders(Y_V, all_bits, poss_bits)
+    #     return (vers, fals)
     if 'Box' in op or 'Diamond' in op:
         if evaluate_modal_expr(model_structure, complex_sentence, eval_world):
             return (null_singleton, set())
         return (set(), null_singleton)
     Z = complex_sentence[2]
     Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
     Z_V, Z_F = find_complex_proposition(model_structure, Z, eval_world)
@@ -544,19 +557,23 @@
             return (null_singleton, set())
         return (set(), null_singleton)
     if "circleright" in op:
         if evaluate_cf_expr(model_structure, complex_sentence, eval_world):
             return (null_singleton, set())
         return (set(), null_singleton)
     if "leq" in op:
-        if Y_V <= Z_V and product(Y_F, Z_F) == Z_F:
+        if Y_V <= Z_V and product(Y_F, Z_F) <= Z_F and all_has_part(Z_F, Y_F):
             return (null_singleton, set())
         return (set(), null_singleton)
     if "sqsubseteq" in op:
-        if product(Y_V, Z_V) == Z_V and Y_F <= Z_F:
+        if product(Y_V, Z_V) <= Z_V and all_has_part(Z_V, Y_V) and Y_F <= Z_F:
+            return (null_singleton, set())
+        return (set(), null_singleton)
+    if "preceq" in op:
+        if product(Y_V, Z_V) <= Z_V and product(Y_F, Z_F) <= Z_F:
             return (null_singleton, set())
         return (set(), null_singleton)
     if "equiv" in op:
         if Y_V == Z_V and Y_F == Z_F:
             return (null_singleton, set())
         return (set(), null_singleton)
     raise ValueError(f"Don't know how to handle {op} operator")
```

### Comparing `model_checker-0.4.5/src/model_checker/model_structure.py` & `model_checker-0.4.6/src/model_checker/model_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,19 +115,19 @@
         self.prefix_conclusions = [prefix(con) for con in infix_conclusions]
         find_constraints_func = define_N_semantics(
             self.verify,
             self.falsify,
             self.possible,
             self.assign,
             self.N,
-            self.w
         )
         frame_cons, prop_cons, premise_cons, conclusion_cons = find_constraints_func(
             self.prefix_premises,
-            self.prefix_conclusions
+            self.prefix_conclusions,
+            self.w,
         )
         self.frame_constraints = frame_cons
         self.prop_constraints = prop_cons
         self.premise_constraints = premise_cons
         self.conclusion_constraints = conclusion_cons
         prefix_sentences = self.prefix_premises + self.prefix_conclusions
         self.all_subsentences = find_subsentences(prefix_sentences)
@@ -444,15 +444,15 @@
         prop_obj.print_verifiers_and_falsifiers(world_bit, print_impossible, indent, output)
         if str(prop_obj) in [str(atom) for atom in sentence_letters]:
             return
         prefix_expr = prop_obj["prefix expression"]
         op = prefix_expr[0]
         first_subprop = self.find_proposition_object(prefix_expr[1])
         indent += 1 # begin subcases, so indent
-        if "neg" in op or "not" in op or "pre" in op:
+        if "neg" in op or "not" in op: # or "pre" in op:
             self.rec_print(first_subprop, world_bit, print_impossible, output, indent)
             return
         if 'Diamond' in op or 'Box' in op:
             for u in self.world_bits:
                 self.rec_print(first_subprop, u, print_impossible, output, indent)
             return
         left_subprop = first_subprop
@@ -524,14 +524,16 @@
         self.prop_dict = {}
         self.prop_dict["prefix expression"] = prefix_expr
         self.model_structure = model_structure
         verifiers, falsifiers = find_complex_proposition(model_structure, prefix_expr, eval_world)
         self.prop_dict["verifiers"] = verifiers
         self.prop_dict["falsifiers"] = falsifiers
         # TODO: can cf_sentences be treated in a more uniform way, avoiding the if clause below?
+        # if 'preceq' in str(prefix_expr[0]):
+        #     print(f"TEST: {verifiers}")
         if 'boxright' in str(prefix_expr[0]):
             # print(f"TEST: check condition")
             self.cf_world = eval_world
             true_worlds, false_worlds = true_and_false_worlds_for_cf(model_structure, prefix_expr)
             # print(f"TEST WORLDS: true {true_worlds}; false {false_worlds}")
             self['worlds cf true at'] = true_worlds
             self['worlds cf false at'] = false_worlds
```

### Comparing `model_checker-0.4.5/src/model_checker/semantics.py` & `model_checker-0.4.6/src/model_checker/semantics.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         sentence_letters_in_input = sentence_letters_in_compound(prefix_input)
         for sentence_letter in sentence_letters_in_input:
             sentence_letters.add(sentence_letter)
     return list(sentence_letters)
     # sort just to make every output the same, given sets aren't hashable
 
 
-def define_N_semantics(verify, falsify, possible, assign, N, w):
+def define_N_semantics(verify, falsify, possible, assign, N):
     # NOTE: just thought of this—we could make the options to do non_null or non_triv optional.
     # Like it coulld be an optional argument put into the model at the top level, just like
     # unsat_core is. Let me below know if you think that's a good idea or if it wouln't be useful.
     '''function that makes the function to make the constraints (and list of sentence letters
     and prefix sentences) This has to be done in order to define N in an input file—you'll see
     here that N is passed in as a variable to the function, after which these 'make' a semantics
     with that N (and the other inputs to this function also depend on N)
@@ -228,16 +228,16 @@
         """ext_sent is in prefix form. The state is the state that verifies ext_sent. 
         evaluate is an optional bool to evaluate something (now unused).
         returns a Z3 constraint"""
         if len(sentence) == 1:
             sentence_letter = sentence[0]
             return verify(state, sentence_letter)
         operator = sentence[0]
-        hyper_ops = ["Box", "Diamond", "boxright", "circleright", "leq", "sqsubseteq", "equiv"]
-        for choice in hyper_ops:
+        non_ext_ops = ["Box", "Diamond", "boxright", "circleright", "leq", "sqsubseteq", "equiv", "preceq"]
+        for choice in non_ext_ops:
             if choice in operator:
                 return true_at(sentence, eval_world)
         Y = sentence[1]
         if "neg" in operator:
             return extended_falsify(state, Y, eval_world)
         if "not" in operator:
             return exclude(state, Y, eval_world)
@@ -280,16 +280,16 @@
 
     def extended_falsify(state, sentence, eval_world):
         """ext_sent is in prefix form. The state is the state that falsifies ext_sent. 
         returns a Z3 constraint"""
         if len(sentence) == 1:
             return falsify(state, sentence[0])
         operator = sentence[0]
-        hyper_ops = ["Box", "Diamond", "boxright", "circleright", "leq", "sqsubseteq", "equiv"]
-        for choice in hyper_ops:
+        non_ext_ops = ["Box", "Diamond", "boxright", "circleright", "leq", "sqsubseteq", "equiv", "preceq"]
+        for choice in non_ext_ops:
             if choice in operator:
                 return false_at(sentence, eval_world)
         Y = sentence[1]
         if "neg" in operator:
             return extended_verify(state, Y, eval_world)
         if "not" in operator:
             return exclude(state, Y, eval_world)
@@ -336,29 +336,29 @@
     def true_at(sentence, eval_world):
         """sentence is a sentence in prefix notation. Eval world is the world the sentence is
         to be evaluated at (changes for counterfactuals). 
         NOTE: the true_at/false-at definitions are bilateral to accommodate the fact
         that the exhaustivity constraint is not included in the definition of props
         this should avoid the need for specific clauses for (un)negated CFs. 
         returns a Z3 constraint"""
-        x = BitVec("t_x", N)
-        y = BitVec("t_y", N)
-        u = BitVec("t_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
             if 'top' not in str(sent)[0]: # top const alr in model, see find_model_constraints
+                x = BitVec("t_atom_x", N)
                 return Exists(x, And(is_part_of(x, eval_world), verify(x, sent)))
         if len(sentence) == 2:
             operator = sentence[0]
             Y = sentence[1]
             if "neg" in operator or "not" in operator or "pre" in operator:
                 return false_at(sentence[1], eval_world)
             if 'Box' in operator:
+                u = BitVec("t_nec_u", N)
                 return ForAll(u, Implies(is_world(u), true_at(sentence[1], u)))
             if 'Diamond' in operator:
+                u = BitVec("t_pos_u", N)
                 return Exists(u, And(is_world(u), true_at(sentence[1], u)))
         if len(sentence) == 3:
             operator = sentence[0]
             Y = sentence[1]
             Z = sentence[2]
             if "wedge" in operator:
                 return And(true_at(Y, eval_world), true_at(Z, eval_world))
@@ -368,102 +368,183 @@
                 return Or(
                     And(true_at(Y, eval_world), true_at(Z, eval_world)),
                     And(false_at(Y, eval_world), false_at(Z, eval_world)),
                 )
             if "rightarrow" in operator:
                 return Or(false_at(Y, eval_world), true_at(Z, eval_world))
             if "leq" in operator:
-                return ForAll(
-                    [x, y],
-                    And(
+                x = BitVec("t_leq_x", N)
+                y = BitVec("t_leq_y", N)
+                return And(
+                    ForAll(
+                        x,
                         Implies(
                             extended_verify(x, Y, eval_world),
                             extended_verify(x, Z, eval_world)
                         ),
+                    ),
+                    ForAll(
+                        [x, y],
                         Implies(
                             And(
                                 extended_falsify(x, Y, eval_world),
                                 extended_falsify(y, Z, eval_world)
                             ),
                             extended_falsify(fusion(x, y), Z, eval_world)
                         ),
+                    ),
+                    ForAll(
+                        x,
                         Implies(
-                            extended_falsify(y, Z, eval_world),
+                            extended_falsify(x, Z, eval_world),
                             Exists(
-                                u,
+                                y,
                                 And(
-                                    is_part_of(u, y),
-                                    extended_falsify(u, Y, eval_world)
+                                    extended_falsify(y, Y, eval_world),
+                                    is_part_of(y, x),
                                 )
                             )
                         )
                     )
                 )
             if "sqsubseteq" in operator:
-                return ForAll(
-                    [x, y],
-                    And(
+                x = BitVec("t_seq_x", N)
+                y = BitVec("t_seq_y", N)
+                return And(
+                    ForAll(
+                        [x, y],
                         Implies(
                             And(
                                 extended_verify(x, Y, eval_world),
                                 extended_verify(y, Z, eval_world)
                             ),
                             extended_verify(fusion(x, y), Z, eval_world)
                         ),
+                    ),
+                    ForAll(
+                        x,
                         Implies(
-                            extended_verify(y, Z, eval_world),
+                            extended_verify(x, Z, eval_world),
                             Exists(
-                                u,
+                                y,
                                 And(
-                                    is_part_of(u, y),
-                                    extended_verify(u, Y, eval_world)
+                                    extended_verify(y, Y, eval_world),
+                                    is_part_of(y, x),
                                 )
                             )
                         ),
+                    ),
+                    ForAll(
+                        x,
                         Implies(
                             extended_falsify(x, Y, eval_world),
                             extended_falsify(x, Z, eval_world)
                         )
                     )
                 )
+            if "preceq" in operator:
+                x = BitVec("t_peq_x", N)
+                y = BitVec("t_peq_y", N)
+                return And(
+                    ForAll(
+                        [x, y],
+                        Implies(
+                            And(
+                                extended_verify(x, Y, eval_world),
+                                extended_verify(y, Z, eval_world)
+                            ),
+                            extended_verify(fusion(x, y), Z, eval_world)
+                        ),
+                    ),
+                    ForAll(
+                        [x, y],
+                        Implies(
+                            And(
+                                extended_falsify(x, Y, eval_world),
+                                extended_falsify(y, Z, eval_world)
+                            ),
+                            extended_falsify(fusion(x, y), Z, eval_world)
+                        ),
+                    ),
+                    # ForAll(
+                    #     x,
+                    #     Implies(
+                    #         extended_verify(x, Z, eval_world),
+                    #         Exists(
+                    #             y,
+                    #             And(
+                    #                 is_part_of(y, x),
+                    #                 extended_verify(y, Y, eval_world)
+                    #             )
+                    #         )
+                    #     ),
+                    # ),
+                    # ForAll(
+                    #     x,
+                    #     Implies(
+                    #         extended_falsify(x, Z, eval_world),
+                    #         Exists(
+                    #             y,
+                    #             And(
+                    #                 is_part_of(y, x),
+                    #                 extended_falsify(y, Y, eval_world)
+                    #             )
+                    #         )
+                    #     ),
+                    # ),
+                )
             if "equiv" in operator:
-                return ForAll(
-                    x,
-                    And(
+                x = BitVec("t_id_x", N)
+                y = BitVec("t_id_y", N)
+                return And(
+                    ForAll(
+                        x,
                         Implies(
                             extended_verify(x, Y, eval_world),
                             extended_verify(x, Z, eval_world)
                         ),
+                    ),
+                    ForAll(
+                        x,
                         Implies(
                             extended_falsify(x, Y, eval_world),
                             extended_falsify(x, Z, eval_world)
                         ),
+                    ),
+                    ForAll(
+                        x,
                         Implies(
                             extended_verify(x, Z, eval_world),
                             extended_verify(x, Y, eval_world)
                         ),
+                    ),
+                    ForAll(
+                        x,
                         Implies(
                             extended_falsify(x, Z, eval_world),
                             extended_falsify(x, Y, eval_world)
                         ),
                     )
                 )
             if "boxright" in operator:
-                # print(f"TEST: cf operator = {op}, ant = {Y}, con = {Z}")
+                x = BitVec("t_ncf_x", N)
+                u = BitVec("t_ncf_u", N)
                 return ForAll(
                     [x, u],
                     Implies(
                         And(
                             extended_verify(x, Y, eval_world),
                             is_alternative(u, x, eval_world)
                         ),
                         true_at(Z, u),
                     ),
                 )
             if "circleright" in operator:
+                x = BitVec("t_pcf_x", N)
+                u = BitVec("t_pcf_u", N)
                 return Exists(
                     [x, u],
                     And(
                         extended_verify(x, Y, eval_world),
                         is_alternative(u, x, eval_world),
                         true_at(Z, u),
                     ),
@@ -472,29 +553,28 @@
             f'No if statements triggered— true_at for {sentence} at world {eval_world}'
         )
 
     def false_at(sentence, eval_world):
         """X is a sentence in prefix notation, eval world is the world the sentence is to be
         evaulated at. See true_at (above) for an important note on exhaustivity.
         returns a Z3 constraint"""
-        x = BitVec("f_x", N)
-        y = BitVec("f_y", N)
-        u = BitVec("f_u", N)
         if len(sentence) == 1:
             sent = sentence[0]
+            x = BitVec("f_atom_x", N)
             return Exists(x, And(is_part_of(x, eval_world), falsify(x, sent)))
         if len(sentence) == 2:
             operator = sentence[0]
             Y = sentence[1]
             if "neg" in operator or "not" in operator or "pre" in operator:
-                # print(f"TEST: neg operator = {op}")
                 return true_at(sentence[1], eval_world)
             if 'Box' in operator:
+                u = BitVec("f_nec_u", N)
                 return Exists(u, And(is_world(u), false_at(sentence[1], u)))
             if 'Diamond' in operator:
+                u = BitVec("f_pos_u", N)
                 return ForAll(u, Implies(is_world(u), false_at(sentence[1], u)))
         if len(sentence) == 3:
             operator = sentence[0]
             Y = sentence[1]
             Z = sentence[2]
             if "wedge" in operator:
                 return Or(false_at(Y, eval_world), false_at(Z, eval_world))
@@ -504,95 +584,172 @@
                 return Or(
                     And(true_at(Y, eval_world), false_at(Z, eval_world)),
                     And(false_at(Y, eval_world), true_at(Z, eval_world)),
                 )
             if "rightarrow" in operator:
                 return And(true_at(Y, eval_world), false_at(Z, eval_world))
             if "leq" in operator:
-                return Exists(
-                    [x, y],
-                    Or(
+                x = BitVec("f_leq_x", N)
+                y = BitVec("f_leq_y", N)
+                return Or(
+                    Exists(
+                        x,
                         And(
                             extended_verify(x, Y, eval_world),
                             Not(extended_verify(x, Z, eval_world))
                         ),
+                    ),
+                    Exists(
+                        [x, y],
                         And(
                             extended_falsify(x, Y, eval_world),
                             extended_falsify(y, Z, eval_world),
                             Not(extended_falsify(fusion(x, y), Z, eval_world))
                         ),
+                    ),
+                    Exists(
+                        x,
                         And(
-                            extended_falsify(y, Z, eval_world),
+                            extended_falsify(x, Z, eval_world),
                             ForAll(
-                                u,
+                                y,
                                 Implies(
-                                    is_part_of(u, y),
-                                    Not(extended_falsify(u, Y, eval_world))
+                                    extended_falsify(y, Y, eval_world),
+                                    Not(is_part_of(y, x)),
                                 )
                             )
                         )
                     )
                 )
             if "sqsubseteq" in operator:
-                return Exists(
-                    [x, y],
-                    Or(
+                x = BitVec("f_seq_x", N)
+                y = BitVec("f_seq_y", N)
+                return Or(
+                    Exists(
+                        [x, y],
                         And(
                             extended_verify(x, Y, eval_world),
                             extended_verify(y, Z, eval_world),
                             Not(extended_verify(fusion(x, y), Z, eval_world))
                         ),
+                    ),
+                    Exists(
+                        x,
                         And(
-                            extended_verify(y, Z, eval_world),
+                            extended_verify(x, Z, eval_world),
                             ForAll(
-                                u,
+                                y,
                                 Implies(
-                                    is_part_of(u, y),
-                                    Not(extended_verify(u, Y, eval_world))
+                                    extended_verify(y, Y, eval_world),
+                                    Not(is_part_of(y, x)),
                                 )
                             )
                         ),
+                    ),
+                    Exists(
+                        x,
                         And(
                             extended_falsify(x, Y, eval_world),
                             Not(extended_falsify(x, Z, eval_world))
                         )
                     )
                 )
+            if "preceq" in operator:
+                x = BitVec("f_peq_x", N)
+                y = BitVec("f_peq_y", N)
+                return Or(
+                    Exists(
+                        [x, y],
+                        And(
+                            extended_verify(x, Y, eval_world),
+                            extended_verify(y, Z, eval_world),
+                            Not(extended_verify(fusion(x, y), Z, eval_world))
+                        ),
+                    ),
+                    Exists(
+                        [x, y],
+                        And(
+                            extended_falsify(x, Y, eval_world),
+                            extended_falsify(y, Z, eval_world),
+                            Not(extended_falsify(fusion(x, y), Z, eval_world))
+                        ),
+                    )
+                    # Exists(
+                    #     x,
+                    #     And(
+                    #         extended_verify(x, Z, eval_world),
+                    #         ForAll(
+                    #             y,
+                    #             Implies(
+                    #                 is_part_of(y, x),
+                    #                 Not(extended_verify(y, Y, eval_world))
+                    #             )
+                    #         )
+                    #     ),
+                    # ),
+                    # Exists(
+                    #     x,
+                    #     And(
+                    #         extended_falsify(x, Z, eval_world),
+                    #         ForAll(
+                    #             y,
+                    #             Implies(
+                    #                 is_part_of(y, x),
+                    #                 Not(extended_falsify(y, Y, eval_world))
+                    #             )
+                    #         )
+                    #     ),
+                    # ),
+                )
             if "equiv" in operator:
-                return Exists(
-                    x,
-                    Or(
+                x = BitVec("f_id_x", N)
+                y = BitVec("f_id_y", N)
+                return Or(
+                    Exists(
+                        x,
                         And(
                             extended_verify(x, Y, eval_world),
                             Not(extended_verify(x, Z, eval_world))
                         ),
+                    ),
+                    Exists(
+                        x,
                         And(
                             extended_falsify(x, Y, eval_world),
                             Not(extended_falsify(x, Z, eval_world))
                         ),
+                    ),
+                    Exists(
+                        x,
                         And(
                             extended_verify(x, Z, eval_world),
                             Not(extended_verify(x, Y, eval_world))
                         ),
+                    ),
+                    Exists(
+                        x,
                         And(
                             extended_falsify(x, Z, eval_world),
                             Not(extended_falsify(x, Y, eval_world))
                         ),
                     )
                 )
             if "boxright" in operator:
-                # print(f"TEST: cf operator = {op}, ant = {Y}, con = {Z}")
+                x = BitVec("f_ncf_x", N)
+                u = BitVec("f_ncf_u", N)
                 return Exists(
                     [x, u],
                     And(
                         extended_verify(x, Y, eval_world),
                         is_alternative(u, x, eval_world),
                         false_at(Z, u)),
                 )
             if "circleright" in operator:
+                x = BitVec("f_pcf_x", N)
+                u = BitVec("f_pcf_u", N)
                 return ForAll(
                     [x, u],
                     Implies(
                         And(
                             extended_verify(x, Y, eval_world),
                             is_alternative(u, x, eval_world)
                         ),
@@ -641,27 +798,27 @@
                         Or(verify(y, atom), falsify(y, atom)),
                     ),
                 ),
             ),
         ]
         return sent_to_prop
 
-    def find_frame_constraints():
+    def find_frame_constraints(main_world):
         """returns constraints that govern how states act:
         1. for any two states x and y, if y is possible and x is a part of y, then x is possible
         2. for any two states x and y, there exists a state z that is the fusion of x and y
         3. there is a state which is a world state (we call it w)
         returns a list of Z3 constraints"""
         x = BitVec("frame_x", N)
         y = BitVec("frame_y", N)
         z = BitVec("frame_z", N)
         frame_constraints = [
             ForAll([x, y], Implies(And(possible(y), is_part_of(x, y)), possible(x))),
             ForAll([x, y], Exists(z, fusion(x, y) == z)),
-            is_world(w), # w is passed in from the big outer function define_N_semantics
+            is_world(main_world), # w is passed in from the big outer function define_N_semantics
         ]
         return frame_constraints
 
     def find_prop_constraints(sentence_letters):
         """Input: a list of all sentence letters in the premises and conclusions, as returned
         by the function all_sentence_letters (i.e., a list of AtomSorts).
         Returns the a list of the Z3 constraints that each atomic proposition gets, which is
@@ -682,34 +839,43 @@
                 )
                 prop_constraints.append(top_constraint)
                 continue # ie, make_atom_prop_constraint should never be called on '\\top'
             for constraint in make_atom_prop_constraint(sent_letter):
                 prop_constraints.append(constraint)
         return prop_constraints
 
-    def find_premise_const(prefix_premises):
+    def find_premise_const(prefix_premises, main_world):
         """find constraints corresponding to the input sentences
         takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
         returns a list of Z3 constraints
         used in find_all_constraints"""
         premise_constraints = []
         for premise in prefix_premises:
-            premise_constraint = true_at(premise, w)
+            premise_constraint = true_at(premise, main_world)
             premise_constraints.append(premise_constraint)
         return premise_constraints
 
-    def find_conclusion_const(prefix_conclusions):
+    def find_conclusion_const(prefix_conclusions, main_world):
         """find constraints corresponding to the input sentences
         takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
         returns a list of Z3 constraints
         used in find_all_constraints"""
         conclusion_constraints = []
         for conclusion in prefix_conclusions:
-            conclusion_constraint = false_at(conclusion, w) # M: is there a reason you chose to do it like this?
+            conclusion_constraint = false_at(conclusion, main_world)
+            # conclusion_constraint = Not(true_at(conclusion, main_world))
+            # M: is there a reason you chose to do it like this?
+            # B: the idea was to get it to try to find models where the premises are all true and
+            # the conclusions are all false. if there is no such model, we may conclude that any
+            # model where the premises are true is one where at least one conclusion is true.
+            # NOTE: it seems to find models where the premises are false, and similarly where the
+            # conclusions are true even though these shouldn't count as models. I suspect this is
+            # to do with a discrepancy between the z3 constraints and the found/printed propositions
             conclusion_constraints.append(conclusion_constraint)
+        # print(f"TEST CONST: {conclusion_constraints}")
         return conclusion_constraints
 
     # def find_sent_constraints(prefix_premises,prefix_conclusions):
     #     """find constraints corresponding to the input sentences
     #     takes in sentences in prefix form and the input sentence letters (a list of AtomSorts)
     #     returns a list of Z3 constraints
     #     used in find_all_constraints"""
@@ -720,27 +886,27 @@
     #         premise_constraints.append(premise_constraint)
     #     for conclusion in prefix_conclusions:
     #         conclusion_constraint = false_at(conclusion, w)
     #         conclusion_constraints.append(conclusion_constraint)
     #     model_constraints = premise_constraints + conclusion_constraints
     #     return model_constraints
 
-    def find_all_constraints(prefix_premises, prefix_conclusions):
+    def find_all_constraints(prefix_premises, prefix_conclusions, main_world):
         """find Z3 constraints for input sentences
         input_sents are a list of infix sentences
         returns a tuple with all Z3 constraints, for the model, the sentence letters
         (a list of AtomSorts), and the prefix_sentences (a list of lists, since prefix
         sentences are lists)
         function that is returned by the big outer function"""
         prefix_sentences = prefix_premises + prefix_conclusions
         sentence_letters = all_sentence_letters(prefix_sentences)
-        frame_constraints = find_frame_constraints()
+        frame_constraints = find_frame_constraints(main_world)
         prop_constraints = find_prop_constraints(sentence_letters)
-        premise_constraints = find_premise_const(prefix_premises)
-        conclusion_constraints = find_conclusion_const(prefix_conclusions)
+        premise_constraints = find_premise_const(prefix_premises, main_world)
+        conclusion_constraints = find_conclusion_const(prefix_conclusions, main_world)
         return frame_constraints, prop_constraints, premise_constraints, conclusion_constraints
 
     return find_all_constraints
 
 
 def solve_constraints(all_constraints): # all_constraints is a list of constraints
     """find model for the input constraints if there is any
```

### Comparing `model_checker-0.4.5/src/model_checker/syntax.py` & `model_checker-0.4.6/src/model_checker/syntax.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 capital_alphabet = {"A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M",
                     "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z",}
 unary_operators = {
     "\\neg", "neg",
     "\\not", "not",
     "\\pre", "pre",
     "Box", "\\Box",
-    "Diamond", "\\Diamond"
+    "Diamond", "\\Diamond",
 }
 binary_operators = {
     "\\wedge", "wedge",
     "\\vee", "vee",
     "\\rightarrow", "rightarrow",
     "\\leftrightarrow", "leftrightarrow",
     "\\boxright", "boxright",
     "\\circleright", "circleright",
     "\\leq", "leq",
     "\\sqsubseteq", "sqsubseteq",
-    "\\equiv", "equiv"
+    "\\equiv", "equiv",
+    "\\preceq", "preceq",
 }
 all_operators = unary_operators.union(binary_operators)
 
 
 def add_double_backslashes(tokens):
     """adds a double backslash to tokens in the output of tokenize that meet these 3 conditions:
     1. are not capital letters,
```

### Comparing `model_checker-0.4.5/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.4.6/src/model_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.5
+Version: 0.4.6
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -16,26 +16,27 @@
 
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 The language currently includes the following operators:
 
   - `neg` for _negation_
-  <!-- - `not` for _exclusion_ -->
   - `wedge` for _conjunction_
   - `vee` for _disjunction_
   - `rightarrow` for _material conditional_
   - `leftrightarrow` for _material biconditional_
   - `Box` for _necessity_
   - `Diamond` for _possibility_
   - `boxright` for the _must counterfactual conditional_
   - `circleright` for the _might counterfactual conditional_
   - `leq` for _ground_
   - `sqsubseteq` for _essence_
   - `equiv` for _propositional identity_
+  - `preceq` for _relevance_
+  <!-- - `not` for _exclusion_ -->
 
 Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
 To generate a test file run `model-checker` in the terminal without arguments.
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
@@ -99,19 +100,22 @@
 A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
 This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
 
 A _grounding sentence_ `A leq B` may be read '`A` is _sufficient for_ `B`' and an _essence sentence_ `A sqsubseteq B` may be read '`A` is _necessary for_ `B`'.
 A _propositional identity sentence_ `A equiv B` may be read '`A` _just is for_ `B`'.
+A _relevance sentence_ `A preceq B` may be read '`A` _is wholly relevant to_ `B`'.
 The semantics for ground requires every verifier for the antecedent to be a verifier for the consequent, any fusion of a falsifier for the antecedent and consequent to be a falsifier for the consequent, and any falsifier for the consequent to have a part that falsifies the antecedent.
 The semantics for essence requires every fusion of a verifier for the antecedent and consequent to be a verifier for the consequent, any verifier for the consequent must have a part that verifies the antecedent, and every falsifier for the antecedent to be a falsifier for the consequent.
 The semantics for propositional identity requires the two arguments to have the same verifiers and falsifiers.
-All three constitutive operators are interdefinable as indicated below: 
+The semantics for relevance requires any fusion of verifiers for the antecedent and consequent to be a verifier for the consequent and, similarly, any fusion of falsifiers for the antecedent and consequent to be a falsifier for the consequent.
+Whereas the first three constitutive operators are interdefinable, relevance is definable in terms of the other constitutive operators but not _vice versa_:
 
 - `A leq B  :=  neg A sqsubseteq neg B  :=  (A vee B) equiv B`.
 - `A sqsubseteq B  :=  neg A leq neg B  :=  (A wedge B) equiv B`.
 - `A equiv B  :=  (A leq B) wedge (B leq A)  :=  (A sqsubseteq B) wedge (B sqsubseteq A)`.
+- `A preceq B  :=  (A wedge B) leq B :=  (A vee B) sqsubseteq B`.
 
 Instead of a Boolean lattice as in extensional and intensional semantics theories, the space of hyperintensional propositions forms a non-interlaced bilattice as described in this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w), building on [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 
 More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.4.5/test/test_sat.py` & `model_checker-0.4.6/test/test_sat.py`

 * *Files identical despite different names*

