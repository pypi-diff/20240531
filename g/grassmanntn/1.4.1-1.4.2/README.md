# Comparing `tmp/grassmanntn-1.4.1.tar.gz` & `tmp/grassmanntn-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.4.1.tar", last modified: Wed May  8 09:05:33 2024, max compression
+gzip compressed data, was "grassmanntn-1.4.2.tar", last modified: Fri May 31 08:23:42 2024, max compression
```

## Comparing `grassmanntn-1.4.1.tar` & `grassmanntn-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2024-05-08 09:05:33.267320 grassmanntn-1.4.1/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.4.1/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2024-05-08 09:05:33.267320 grassmanntn-1.4.1/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.4.1/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2024-05-08 09:05:33.267320 grassmanntn-1.4.1/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   261943 2024-05-08 08:28:36.000000 grassmanntn-1.4.1/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    27565 2023-10-19 06:17:49.000000 grassmanntn-1.4.1/grassmanntn/arith.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     7833 2023-10-13 09:12:22.000000 grassmanntn-1.4.1/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     7895 2023-12-06 05:57:14.000000 grassmanntn-1.4.1/grassmanntn/example_block.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   147765 2023-12-06 09:40:38.000000 grassmanntn-1.4.1/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   147810 2023-12-06 09:39:57.000000 grassmanntn-1.4.1/grassmanntn/gauge2d_block.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.4.1/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2024-05-08 09:05:33.267320 grassmanntn-1.4.1/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2024-05-08 09:05:33.000000 grassmanntn-1.4.1/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      384 2024-05-08 09:05:33.000000 grassmanntn-1.4.1/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2024-05-08 09:05:33.000000 grassmanntn-1.4.1/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       30 2024-05-08 09:05:33.000000 grassmanntn-1.4.1/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2024-05-08 09:05:33.000000 grassmanntn-1.4.1/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2024-05-08 09:05:33.267320 grassmanntn-1.4.1/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1914 2024-05-08 08:31:56.000000 grassmanntn-1.4.1/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2024-05-31 08:23:42.605034 grassmanntn-1.4.2/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.4.2/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2024-05-31 08:23:42.605034 grassmanntn-1.4.2/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.4.2/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2024-05-31 08:23:42.605034 grassmanntn-1.4.2/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   217571 2024-05-29 06:00:27.000000 grassmanntn-1.4.2/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    27565 2023-10-19 06:17:49.000000 grassmanntn-1.4.2/grassmanntn/arith.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     7833 2023-10-13 09:12:22.000000 grassmanntn-1.4.2/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     7895 2023-12-06 05:57:14.000000 grassmanntn-1.4.2/grassmanntn/example_block.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   147765 2023-12-06 09:40:38.000000 grassmanntn-1.4.2/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   147810 2023-12-06 09:39:57.000000 grassmanntn-1.4.2/grassmanntn/gauge2d_block.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.4.2/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2024-05-31 08:23:42.605034 grassmanntn-1.4.2/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2024-05-31 08:23:42.000000 grassmanntn-1.4.2/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      384 2024-05-31 08:23:42.000000 grassmanntn-1.4.2/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2024-05-31 08:23:42.000000 grassmanntn-1.4.2/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       30 2024-05-31 08:23:42.000000 grassmanntn-1.4.2/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2024-05-31 08:23:42.000000 grassmanntn-1.4.2/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2024-05-31 08:23:42.605034 grassmanntn-1.4.2/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1914 2024-05-31 08:23:33.000000 grassmanntn-1.4.2/setup.py
```

### Comparing `grassmanntn-1.4.1/LICENSE.txt` & `grassmanntn-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/PKG-INFO` & `grassmanntn-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.4.1
+Version: 1.4.2
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_141.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_142.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.4.1/README.md` & `grassmanntn-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn/__init__.py` & `grassmanntn-1.4.2/grassmanntn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,15 +89,14 @@
             color="4"
         elif color=="purple":
             color="5"
         elif color=="cyan":
             color="6"
 
         if step > total:
-            #gtn.error("Error[show_progress]: <step> cannot be larger than <total>!")
             step = total
         print("\r",end="")
 
         if ratio :
             progress = str(step_inp)+"/"+str(total_inp)
         else :
             progress = '{:.4g} %'.format(step_inp/total_inp*100)
@@ -238,14 +237,17 @@
 
 ####################################################
 ##              Block Grassmann Array             ##
 ####################################################
 
 class block:
 
+    __array_priority__ = 1000000
+    
+
     def __init__(self, data=None):
         
         #import from dense only
         dat = data.copy()
         if type(data)==sparse:
             dat = dense(data)
         dat = dat.force_encoder('parity-preserving')
@@ -279,15 +281,15 @@
 
         # create a blank list
         sgn = []
         for p in [0,1]:
             sgn_p = []
             for d,stat in zip(dat.shape,dat.statistics):
                 if stat in fermi_type:
-                    dim = int(d/grading)
+                    dim = max(int(d/grading),1)
                 else:
                     dim = d
                 sgn_p+=[np.zeros([dim],dtype=int)]
             sgn += [sgn_p]
 
         for axis,(d,stat) in enumerate(zip(dat.shape,dat.statistics)):
             for i in range(d):
@@ -445,37 +447,36 @@
         for i in range(self.ndim):
             if self.statistics[i] in bose_type:
                 ret[i] = self.shape[i]
         return make_tuple(ret)
 
     @property
     def even_shape(self):
-        ret = [ len(v) for v in self.sgn[0] ]
+        ret = [ len(v) if v[0]!=0 else 0 for v in self.sgn[0] ]
         return make_tuple(ret)
 
     @property
     def odd_shape(self):
-        ret = [ len(v) for v in self.sgn[1] ]
+        ret = [ len(v) if v[0]!=0 else 0 for v in self.sgn[1] ]
         return make_tuple(ret)
-        return odd_shape
 
     @property
     def ndim(self):
         return len(self.shape)
     
     @property
     def dtype(self):
         it = np.nditer(self.data, flags=['multi_index','refs_ok'])
         for val in it:
             #total index
             return val.item().dtype
 
     def copy(self):
 
-        ret = block( gtn.random(shape=(2,2),statistics=(1,1)) )
+        ret = block( random(shape=(2,2),statistics=(1,1)) )
 
         ret.data = copy.deepcopy(self.data)
         ret.sgn  = copy.deepcopy(self.sgn)
         ret.statistics = self.statistics
         ret.format = self.format
         ret.shape = self.shape # not the actual shape, but the 'physical' shape
         ret.marked_as_joined = self.marked_as_joined
@@ -536,15 +537,14 @@
         return other+(-1)*self
         
     def __rmul__(self, other):
         return self*other
         
     def switch_format(self):
 
-
         def mult_along_axis(A, v, axis):
             # see [https://stackoverflow.com/questions/30031828/multiply-numpy-ndarray-with-1d-array-along-a-given-axis]
             # for explanation
             # ensure we're working with Numpy arrays
             A = np.array(A)
             v = np.array(v)
             shape = np.swapaxes(A, A.ndim-1, axis).shape
@@ -718,14 +718,24 @@
         shape_block = [ dim for dim,stat in zip(_.item().shape,obj.statistics) if stat in fermi_type]
         shape_sgn = make_tuple([ dim_sgn[p][i] for i,p in enumerate(block) ])
 
         shape_sgn = make_list(shape_sgn)
         shape_block = make_list(shape_block)
 
         if shape_sgn!=shape_block:
+
+            # no need to do anything if the inconsistent part is of dimension 1
+            is_ok = True
+            for s,b in zip(shape_sgn,shape_block):
+                if not (s==b or (s==1 and b==0)):
+                    is_ok = False
+                    break
+            if is_ok :
+                return False
+
             return True
 
     return False
 
 def correct_sign_size(InpObj):
     
     obj = InpObj.copy()
@@ -742,14 +752,23 @@
         shape_sgn = make_tuple([ dim_sgn[p][i] for i,p in enumerate(block) ])
 
         shape_sgn = make_list(shape_sgn)
         shape_block = make_list(shape_block)
 
         if shape_sgn!=shape_block:
 
+            # no need to do anything if the inconsistent part is of dimension 1
+            is_ok = True
+            for s,b in zip(shape_sgn,shape_block):
+                if not (s==b or (s==1 and b==0)):
+                    is_ok = False
+                    break
+            if is_ok :
+                return obj
+
             # get the block number but artifically add the bosonic one as well
             full_block = []
             fi = 0
             for i,stat in enumerate(obj.statistics):
                 if stat in fermi_type:
                     full_block += [block[fi]]
                     fi += 1
@@ -764,14 +783,17 @@
     return obj
 
 ####################################################
 ##             Densed Grassmann Array             ##
 ####################################################
 
 class dense:
+
+    __array_priority__ = 1000000
+    
     def __init__(self, data=None, encoder = "canonical", format = "standard", statistics=None):
     
         #copy dense properties
         self.data = None
         self.statistics = None
         self.format = format
         self.encoder = encoder
@@ -1092,14 +1114,17 @@
         return block(self)
 
 ####################################################
 ##            Sparse Grassmann arrays             ##
 ####################################################
 
 class sparse:
+
+    __array_priority__ = 1000000
+    
     def __init__(self, data=None, encoder = "canonical", format = "standard", statistics = None):
     
         #copy sparse properties
         self.data = None
         self.statistics = None
         self.format = format
         self.encoder = encoder
@@ -2190,686 +2215,14 @@
             if type(ret.data)==memoryview:
                 return ret
             else:
                 return ret.data[0]
         else:
             return np.array(ret).flatten()[0]
 
-def einsum_ds_v140(*args,format="standard",encoder="canonical",debug_mode=False):
-
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #                     Important variables and its meanings
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #
-    #               subscripts = the whole input text with spaces removed
-    #               has_output = True if the <input_string> has the output section
-    #             input_string = the left side of the arrow
-    #            output_string = the right side of the arrow
-    #                  summand = <input_string> without commas
-    #                     nobj = number of input objects
-    #           obj_index_list = list of individual index strings of input objects
-    #                 obj_list = list of input objects
-    #               stats_list = input object's stats joined into a single list
-    #               shape_list = input object's shape joined into a single list
-    #        summed_index_info = [ [char, conjugated_char], [index locations in <input_string>] ]
-
-
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 0: Input processing
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-
-    # remove spaces ---------------------------------------------------------------------------------
-    subscripts = args[0].replace(" ","")
-    subscripts = denumerate(subscripts)
-
-    has_output = subscripts.count("->") > 0
-    if subscripts.count("->") > 1 :
-        error("Error[einsum]: Only one arrow is allowed in the input string!")
-
-    if has_output:
-        input_string, output_string = subscripts.split("->")
-        if output_string.count(",") > 0 :
-            error("Error[einsum]: Output string must not contain commas (',') !")
-    else:
-        input_string = subscripts
-
-    summand = input_string.replace(",","")
-
-    obj_index_list = input_string.split(",")
-    nobj = len(obj_index_list)
-
-    obj_list = make_list(args[1:1+nobj])
-    stats_list = sum([ make_list(obj.statistics) for obj in obj_list ],[])
-    shape_list = sum([ make_list(obj.shape) for obj in obj_list ],[])
-
-    # force everything to be canonical and standard -------------------------------------------------
-    # also force everything to be of the same type
-
-    this_type = type(obj_list[0])
-    this_encoder = obj_list[0].encoder
-    this_format = obj_list[0].format
-    for i in range(len(obj_list)):
-        obj_list[i] = this_type(obj_list[i].force_encoder('canonical').force_format('standard')).data
-
-    # get some information about the summed indices -------------------------------------------------
-    # [ f=<char>, [index locations in lf], [statistics] ]
-    summed_index_info = []
-
-    for i,char in enumerate(summand):
-
-        # skip if bosonic
-        if stats_list[i] in bose_type:
-            continue
-
-        lf =  input_string.count(char)
-        if has_output :
-            rf = output_string.count(char)
-            if lf>2 or rf>1 or (lf+rf)%2==1 :
-                if lf>2 :
-                    reason = "lf>2"
-                elif rf>1 :
-                    reason = "rf>1"
-                else :
-                    reason = "(lf+rf)%2==1"
-                error("Error[einsum]: Inconsistent index statistics. (reason:"+reason+")")
-        else :
-            if lf>2:
-                reason = "lf>2"
-                error("Error[einsum]: Inconsistent index statistics. (reason:"+reason+")")
-
-        if lf==1:
-            continue
-
-        # add a new entry if it is a new character
-        if summand[:i].count(char)==0 :
-            summed_index_info += [ [ char, [i] , [stats_list[i]] ] ]
-        else:
-            for k in range(len(summed_index_info)):
-                if(summed_index_info[k][0]==char):
-                    summed_index_info[k][1] += [i]
-                    summed_index_info[k][2] += [stats_list[i]]
-
-    def is_statwise_inconsistent(stat1,stat2):
-        if [stat1,stat2] == [0,0]:
-            return False
-        elif [stat1,stat2] == [1,-1]:
-            return False
-        elif [stat1,stat2] == [-1,1]:
-            return False
-        elif [stat1,stat2] == [hybrid_symbol,hybrid_symbol]:
-            return False
-        else:
-            return True
-
-    for [char,location,stats] in summed_index_info:
-        if len(stats)==2 and is_statwise_inconsistent(stats[0],stats[1]):
-            error("Error[einsum]: The contracted indices have inconsistent statistics!")
-    
-    if debug_mode :
-        print()
-        print("input:",subscripts)
-        print("obj indices:")
-        for elem in obj_index_list:
-            print(" ",elem)
-    
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 1: replace the conjugated variable's index with a new character
-    #                      and remove bosonic string
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-
-    fsummand   = ""
-    fsummand_u = ""
-    fstats_list = []
-    fshape_list = []
-    charlist = summand
-    for i,char in enumerate(summand):
-        if stats_list[i] == 0:
-            continue
-
-        fsummand    += char
-        fstats_list += stats_list[i],
-        fshape_list += shape_list[i],
-
-        if stats_list[i] == -1 and summand.count(char)>1:
-            new_char = get_char(charlist)
-            charlist += new_char
-            fsummand_u += new_char
-
-            # edit the summed_index_info, with the position swapped a little bit as well
-            for j,[char2,location,stats] in enumerate(summed_index_info):
-                if char2==char :
-                    summed_index_info[j][0] = [char,new_char]
-                    if stats == [-1,1]:
-                        summed_index_info[j][1] = [ summed_index_info[j][1][1], summed_index_info[j][1][0] ]
-                        summed_index_info[j][2] = [ summed_index_info[j][2][1], summed_index_info[j][2][0] ]
-        else:
-            fsummand_u += char
-    fstats = fstats_list.copy()
-    fshape = fshape_list.copy()
-    fstats_u = fstats_list.copy()
-    fshape_u = fshape_list.copy()
-
-    # remove the stat entry as it is redundant
-    for i,elem in enumerate(summed_index_info):
-        summed_index_info[i] = elem[:2]
-
-    if debug_mode :
-        print()
-        print(" :::::::::: replace conjugated indices by unique characters :::::::::: ")
-        print(fsummand,"<--- fsummand = original indices")
-        print(fsummand_u,"<--- fsummand_u = replace conjugated indices by unique characters")
-        print(fstats_u,"<--- fstats_u")
-        print(fshape_u,"<--- fshape_u")
-        print("summed indices info:")
-        for elem in summed_index_info:
-            print(" "," = ".join(elem[0]),"( location =",elem[1],")")
-        
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 2: Arrange the indices (presum) and compute the sign factor
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-
-    # the summed indices are now next to each other with the conjugated one to the right
-
-    fsummand_ur = fsummand_u
-    for [ [c1,c2], loc ] in summed_index_info:
-        fsummand_ur = fsummand_ur.replace(c2,"")
-        fsummand_ur = fsummand_ur.replace(c1,c1+c2)
-
-    fstats_ur = reordering(fsummand_u,fsummand_ur,fstats_list)
-    fshape_ur = reordering(fsummand_u,fsummand_ur,fshape_list)
-
-    if debug_mode :
-        print()
-        print(" :::::::::::: move the conjugated to the right of its pair ::::::::::: ")
-        print(fsummand_u,"<--- fsummand_u")
-        print(fsummand_ur,"<--- fsummand_ur = move the conjugated to the right of its pair")
-        print(fstats_ur,"<--- fstats_ur")
-        print(fshape_ur,"<--- fshape_ur")
-        
-    # remove the leading and trailing chars that is the same as the pre-rearranged string
-
-    nall_u = len(fsummand_u)
-
-    nl = 0
-    for i in range(nall_u):
-        if fsummand_u[i] != fsummand_ur[i]:
-            break
-        nl+=1
-    nr = 0
-    for i in range(nall_u):
-        if fsummand_u[nall_u-1-i] != fsummand_ur[nall_u-1-i]:
-            break
-        nr+=1
-    nr = nall_u-nr
-
-    fsummand_ut  = fsummand_u[nl:nr]
-    fstats_ut   = fstats_u[nl:nr]
-    fshape_ut   = fshape_u[nl:nr]
-    fsummand_urt  = fsummand_ur[nl:nr]
-    fstats_urt   = fstats_ur[nl:nr]
-    fshape_urt   = fshape_ur[nl:nr]
-
-    if nl>nr :
-        skip_S1 = True
-    else:
-        skip_S1 = False
-
-    if debug_mode :
-        print()
-        print(" :::::::::::::::::::::::: trim left and right :::::::::::::::::::::::: ")
-        if skip_S1 :
-            print("fsummand_u and fsummand_ur are identical.")
-            print("S1 calculation is skipped.")
-        else :
-            print(fsummand_u,"<--- fsummand_u")
-            print(fsummand_ut,"<--- fsummand_ut = trim fsummand_u left and right")
-            print(fstats_ut,"<--- fstats_ut")
-            print(fshape_ut,"<--- fshape_ut")
-            print()
-            print(fsummand_ur,"<--- fsummand_ur")
-            print(fsummand_urt,"<--- fsummand_urt = trim fsummand_ur left and right")
-            print(fstats_urt,"<--- fstats_urt")
-            print(fshape_urt,"<--- fshape_urt")
-        
-    S1_sgn_computation_string = fsummand_ut+"->"+fsummand_urt
-    
-    if debug_mode and not skip_S1 :
-        print()
-        print(S1_sgn_computation_string,"<--- string used in S1 computation")
-    
-    # remove the conjugated character if both the nonnconjugated and conjugated are present
-    
-    # do the ut only
-    fsummand_utx = ""
-    fstats_utx   = []
-    fshape_utx   = []
-    nall_ut = len(fsummand_ut)
-    for i in range(nall_ut):
-        c = fsummand_ut[i]
-        to_skip = False
-        if fstats_ut[i]==-1 :
-            for [ [c1,c2], loc ] in summed_index_info:
-                if c==c2 and fsummand_ut.count(c1)>0:
-                    to_skip = True
-        if to_skip :
-            continue
-        fsummand_utx += fsummand_ut[i]
-        fstats_utx   += fstats_ut[i],
-        fshape_utx   += fshape_ut[i],
-    S1dim = len(fsummand_utx)
-
-    if debug_mode and not skip_S1 :
-        print()
-        print(" ::::::: remove the conjugated if both of the pair are present ::::::: ")
-        print(fsummand_ut,"<--- fsummand_ut")
-        print(fsummand_utx,"<--- fsummand_utx = remove on of the pair")
-        print(fstats_utx,"<--- fstats_utx")
-        print(fshape_utx,"<--- fshape_utx")
-    
-    # make the copy map
-    copy_map = []
-    fsummand_utx_r = list(fsummand_utx) #this is used in the mock reconstruction
-    for i_ut, c in enumerate(fsummand_ut):
-        if c not in fsummand_utx:
-            #find the location of its pair first
-            c_pair = "?"
-            for [[c1,c2],_] in summed_index_info:
-                if c==c2 :
-                    i_utx = fsummand_utx_r.index(c1)
-                    c_pair = c1
-                    break
-            copy_map += [i_ut,i_utx],
-            fsummand_utx_r.insert(i_ut,c)
-    
-    def use_copy_map(the_map,the_list,apply_negative=False):
-        new_list = list(the_list).copy()
-        for [i2,i1] in the_map :
-            if apply_negative :
-                new_list.insert(i2,-new_list[i1])
-            else :
-                new_list.insert(i2,new_list[i1])
-        return new_list
-    
-    if debug_mode and not skip_S1:
-        print()
-        print(" :::::::::::::::::::::::::: testing copy_map ::::::::::::::::::::::::: ")
-        fsummand_ut2 = ''.join(use_copy_map(copy_map,list(fsummand_utx)))
-        fstats_ut2 = use_copy_map(copy_map,fstats_utx,apply_negative=True)
-        fshape_ut2 = use_copy_map(copy_map,fshape_utx)
-        print(" ",fsummand_ut2,"vs",fsummand_ut)
-        print(" ",fstats_ut2,"vs",fstats_ut)
-        print(" ",fshape_ut2,"vs",fshape_ut)
-        
-    # fsummand_utx needs to be replaced with the original indices to obtain S1_index_string
-    S1_index_string  = ""
-    for c in fsummand_utx:
-        if c in summand:
-            S1_index_string += c
-        else:
-            for [ [c1,c2], loc ] in summed_index_info:
-                if c==c2 :
-                    S1_index_string += c1
-                    break
-    S1_shape = []
-    for c in S1_index_string:
-        ind = fsummand.index(c)
-        S1_shape += fshape[ind],
-    S1_shape = make_tuple(S1_shape)
-    
-    if debug_mode and not skip_S1 :
-        print()
-        print(" :::::::::::::::::::::::::::::: S1 stuff ::::::::::::::::::::::::::::: ")
-        print(S1_index_string,"<--- S1's index string")
-        print(S1_shape,"<--- S1's shape")
-        
-    # sign factor computation -------------------------------------------------------------------------
-    
-    if S1dim>0 and not skip_S1:
-
-        S1 = np.zeros(S1_shape,dtype=int)
-        iterator = np.nditer(S1, flags=['multi_index'])
-        parity_list = []
-        sgn_list = []
-
-        k=1
-        kmax = getsize(S1_shape)
-
-        s0 = time.time()
-        s00 = s0
-        progress_space() # << Don't remove this. This is for the show_progress!
-
-        for element in iterator:
-            coords = iterator.multi_index
-            dupped_coords = use_copy_map(copy_map,coords)
-            
-            parity = [ param.gparity(i)%2 for i in dupped_coords ]
-
-            if parity not in parity_list:
-                parity_list += parity,
-                sgn = relative_sign(S1_sgn_computation_string,parity)
-                sgn_list += sgn,
-            else:
-                index = parity_list.index(parity)
-                sgn = sgn_list[index]
-
-            S1[coords] = sgn
-
-            if time.time()-s0 > 2 :
-                show_progress(k,kmax+1,process_name = "einsum_sgn1",ratio = False,color="red",time=time.time()-s00)
-                s0 = time.time()
-            
-            k+=1
-
-        clear_progress()
-        tab_up()
-        
-    #  ::: Summary :::
-    #
-    #  S1 is the sign factor from the initial rearrangement
-    #  Its index string is S1_index_string
-
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 3: Sign factor from the summed pair
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-
-    S2_dimlist = []
-    S2_index_string = ""
-    summed_indices = fsummand_ur
-    for [ [c1,c2], loc ] in summed_index_info:
-        S2_dimlist += shape_list[ summand.index(c1) ],
-        S2_index_string += ","+c1
-        summed_indices = summed_indices.replace(c1+c2,"")
-    S2_index_string = S2_index_string[1:]
-    nS2 = len(S2_dimlist)
-    
-    
-    skip_S2 = nS2 == 0
-    
-    if debug_mode :
-        print()
-        print(" :::::::::::::::::::::::::::::: S2 stuff ::::::::::::::::::::::::::::: ")
-        if skip_S2 :
-            print("There is no summed indices.")
-            print("S2 calculation is skipped.")
-        else :
-            print(fsummand,"<--- fsummand")
-            print(S2_index_string,"<--- S2 index string")
-            print(S2_dimlist,"<--- S2's dim list")
-    
-    if not skip_S2 :
-
-        S2_list = []
-        for i in range(nS2):
-            S2i = [ param.sgn(j) for j in range(S2_dimlist[i]) ]
-            S2_list += np.array(S2i),
-
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 4: rearrange to the final form
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    
-    skip_S3 = True
-    if has_output :
-
-        foutput = ""
-        for c in output_string:
-            if stats_list[ summand.index(c) ] == 0 :
-                continue
-            else:
-                foutput+=c
-
-        S3_shape=[]
-        for c in summed_indices:
-            d = shape_list[ summand.index(c) ]
-            S3_shape += d,
-
-        # again... remove the leading and trailing duplicates
-
-        nall_ur = len(summed_indices)
-        nl = 0
-        for i in range(nall_ur):
-            if summed_indices[i] != foutput[i]:
-                break
-            nl+=1
-
-        nr = 0
-        for i in range(nall_ur):
-            if summed_indices[nall_ur-1-i] != foutput[nall_ur-1-i]:
-                break
-            nr+=1
-        nr = nall_ur-nr
-
-        final = foutput[nl:nr]
-        prefinal = summed_indices[nl:nr]
-        S3_shape   = S3_shape[nl:nr]
-
-        if nl>nr :
-            skip_S3 = True
-        else:
-            skip_S3 = False
-
-        S3_sgn_computation_string = prefinal+"->"+final
-        S3_index_string = prefinal
-
-        if not skip_S3 :
-
-            k=1
-            kmax = 1
-            for d in S3_shape:
-                kmax*=d
-
-            s0 = time.time()
-            s00 = s0
-            progress_space() # << Don't remove this. This is for the show_progress!
-
-            S3 = np.zeros(S3_shape,dtype=int)
-            iterator = np.nditer(S3, flags=['multi_index'])
-            parity_list = []
-            sgn_list = []
-            for element in iterator:
-                coords = iterator.multi_index
-
-                parity = [ param.gparity(i)%2 for i in coords ]
-
-                if parity not in parity_list:
-                    parity_list += parity,
-                    sgn = relative_sign(S3_sgn_computation_string,parity)
-                    sgn_list += sgn,
-                else:
-                    index = parity_list.index(parity)
-                    sgn = sgn_list[index]
-
-                S3[coords] = sgn
-
-                if time.time()-s0 > 0.5 :
-                    show_progress(k,kmax+1,process_name = "einsum_sgn3",ratio = False,color="red",time=time.time()-s00)
-                    s0 = time.time()
-
-                k+=1
-            clear_progress()
-            tab_up()
-
-            skip_S3 = len(S3_shape)==0
-
-    #  ::: Summary :::
-    #
-    #  S3 is the sign factor from the final rearrangement
-    #  Its index string is S3_index_string
-    
-    if debug_mode and not skip_S3:
-        print()
-        print(" :::::::::::::::::::::::::::::: S3 stuff ::::::::::::::::::::::::::::: ")
-        print(S3_sgn_computation_string,"<--- string used in the S3 computation")
-        print(S3_index_string,"<--- S3_index_string")
-        print(S3_shape,"<--- S3_shape")
-    
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 5: add the vertices
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    
-    einsum_input = input_string
-    einsum_obj_list = obj_list
-
-    if S1dim>0 and not skip_S1:
-        einsum_input += ","+S1_index_string
-        einsum_obj_list += S1,
-
-    if nS2>0 :
-        einsum_input += S2_index_string
-        einsum_obj_list += S2_list
-
-    if has_output :
-        if not skip_S3 :
-            einsum_input += ","+S3_index_string
-            einsum_obj_list += S3,
-
-    if this_type == sparse :
-        
-
-        instruction_all_indices = subscripts.replace(",","")
-        instruction_all_indices = instruction_all_indices.replace("->","")
-        instruction_all_indices = instruction_all_indices.replace(" ","")
-        if not skip_S1:
-            instruction_all_indices=instruction_all_indices+S1_index_string
-        if not skip_S2:
-            instruction_all_indices=instruction_all_indices+S2_index_string
-        if not skip_S3:
-            instruction_all_indices=instruction_all_indices+S3_index_string
-
-        # make a listing of duplicated indices
-        einsum_input_unique = ""
-        vertex_list = [] # [ indices , shape , number_of_legs ]
-        unique_char = ""
-        for i,c in enumerate(instruction_all_indices):
-            if c=="," :
-                continue
-            if instruction_all_indices[:i].count(c) == 0 :
-                vertex_list += [ c, shape_list[ summand.index(c) ] , instruction_all_indices.count(c) ],
-                unique_char += c
-
-        for i,[char,dim,nlegs] in enumerate(vertex_list) :
-            legchar = char
-            for leg in range(nlegs-1):
-                new_char = get_char(unique_char)
-                unique_char += new_char
-                legchar += new_char
-            vertex_list[i][0] = legchar
-
-        vertex_list_final = []
-        for elem in vertex_list :
-            if elem[2] > 2:
-                vertex_list_final += elem[:2],
-                
-        for i,elem in enumerate(vertex_list_final):
-            x = list(elem[0])
-            x.reverse()
-            vertex_list_final[i][0] = ''.join(x)
-        
-        if debug_mode :   
-            print()
-            print(" :::::::::::::::::::::::::::::: vertices ::::::::::::::::::::::::::::: ")
-            print(instruction_all_indices,"<-- the instruction strings with all char combined into one string")
-            print("vertex list:")
-            for vert in vertex_list_final:
-                print(" ",vert)
-    
-    
-    # now replace the einsum string with these new characters
-    
-    #get the correct einsum string first
-    einsum_string = input_string
-    if not skip_S1 :
-        einsum_string += ","+S1_index_string
-    if not skip_S2 :
-        einsum_string += ","+S2_index_string
-    if not skip_S3 :
-        einsum_string += ","+S3_index_string
-    if debug_mode :   
-        print()  
-        print(einsum_string,"<-- einsum_string = einsum string without vertices")
-    
-    if this_type == sparse :
-        einsum_string_replaced = einsum_string
-        for [vert,dim] in vertex_list_final:
-            c = vert[len(vert)-1]
-            nreplace = einsum_string_replaced.count(c)
-            for i in range(nreplace):
-                einsum_string_replaced = einsum_string_replaced.replace(c,vert[i],1)
-            einsum_string_replaced+=","+vert
-            
-        if debug_mode :   
-            print()
-            print(einsum_string_replaced,"<-- einsum_string with replacement")
-        
-        # construct the vertex tensors
-        vertex_obj_list = []
-        for [string,dim] in vertex_list_final :
-            shape=tuple([dim]*len(string))
-            coords = np.array([ [ i for i in range(dim) ] for j in range(len(string))])
-            data = np.array( [ 1 for i in range(dim) ] )
-            vertex = sp.COO( coords, data, shape=shape )
-            vertex_obj_list += vertex.copy(),
-
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 6: get the final statistics
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-
-    final_stats = []
-    if has_output :
-        for c in output_string :
-            final_stats += stats_list[ summand.index(c) ],
-
-    if debug_mode and has_output:
-        print()
-        print(" :::::::::::::::::::::::::: final statistics ::::::::::::::::::::::::: ")
-        print(final_stats,"<--- final stats")
-        
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-    #              Step 7: the actual sum
-    #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-
-    if this_type==sparse :
-        einsum_obj_list += vertex_obj_list
-        einsum_string = einsum_string_replaced
-    
-    if has_output :
-        einsum_string += "->"+output_string
-
-    # convert all object to this_type
-    if this_type == sparse :
-        for i, obj in enumerate(einsum_obj_list):
-            if type(obj) == np.ndarray:
-                einsum_obj_list[i] = sp.COO.from_numpy(obj)
-    if this_type == dense :
-        for i, obj in enumerate(einsum_obj_list):
-            if type(obj) != np.ndarray:
-                einsum_obj_list[i] = sp.COO.todense(obj)
-    
-    if debug_mode :
-        print(" ::::::::::::::::::::::::::: the actual sum :::::::::::::::::::::::::: ")
-        print(einsum_string,"<-- einsum string")
-        print("[shape,type]:")
-        for obj in einsum_obj_list:
-            print(" ",[obj.shape,type(obj)])
-
-    # [7-May-24] hot fix in case everything is bosonic
-    einsum_string = einsum_string.replace(",->","->")
-    
-    ret = oe.contract(*tuple([einsum_string]+einsum_obj_list))
-
-    if has_output :
-        return this_type(ret,statistics=final_stats).force_encoder(this_encoder).force_format(this_format)
-    else:
-        if this_type == sparse :
-            if type(ret.data)==memoryview:
-                return ret
-            else:
-                return ret.data[0]
-        else:
-            return np.array(ret).flatten()[0]
-
 def einsum(*args,ignore_anticommutation=False):
     subscripts = args[0].replace(" ","")
     subscripts = denumerate(subscripts)
 
     before=""
     after=""
     return_scalar = True
@@ -2942,16 +2295,14 @@
 
     rettype = int
     if has_float:
         rettype = float
     if has_complex:
         rettype = complex
 
-    #fstats_list = make_list( stat for i,stat in enumerate(stats_list) if stats_list[i] in fermi_type ) # not used
-    #fshape_list = make_list( shape for i,shape in enumerate(shape_list) if stats_list[i] in fermi_type )
     feshape_list = make_list( shape for i,shape in enumerate(eshape_list) if stats_list[i] in fermi_type )
     foshape_list = make_list( shape for i,shape in enumerate(oshape_list) if stats_list[i] in fermi_type )
 
     # the block version of before
     fbefore = ""
     for i,c in enumerate(summand):
         if stats_list[i] in fermi_type:
@@ -3268,631 +2619,27 @@
 
             # ======================================================================================================
             # get the specified block from each object
             # ======================================================================================================
             blocked_obj_list = [ obj.data[obj_block_list[i]] for i,obj in enumerate(obj_list) ]
 
             sigma_list = []
-            #print(summand)
-            #print(all_sgn[0])
-            #print(unique_fsummand)
-            #print(block)
-            
-            for ic, c in enumerate(unique_fsummand):
-                c_index_in_summand = summand.index(c)
-                sgn_c = all_sgn[block[ic]][c_index_in_summand]
-                if summand.count(c) > 1:
-                    err = 0
-                    for ic2, c2 in enumerate(summand):
-                        if c2==c :
-                            sgn_c2 = all_sgn[block[ic]][ic2]
-                            err += np.linalg.norm(sgn_c-sgn_c2)
-                    if err>numer_cutoff :
-                        error("Error[einsum_block]: some sign factors are not consistent.")
-                sigma_list += [ sgn_c if not ignore_anticommutation else 1 ]
-
-            # ======================================================================================================
-            # evaluate the block sign factor
-            # ======================================================================================================
-
-            # step1: from moving conjugated summed index to the non-conjugated counterpart
-            S1 = 1
-            #print("compute S1:", not skip_S1, end="; S1 = ")
-            if not skip_S1:
-                S1_com_before = S1_sgn_computation_string.split("->")[0]
-                # replaced the new index with the old index
-                for elem in summed_index_info:
-                    S1_com_before = S1_com_before.replace(elem[0][1],elem[0][0])
-                # get the parity list
-                parity_list = [ block[unique_fsummand.index(c)] for c in S1_com_before ]
-                S1 = relative_sign(S1_sgn_computation_string,parity_list)
-                #print("S1:",S1_sgn_computation_string,"=",S1)
-                #print(S1)
-
-            # step2: from moving the result after the summation to the specified output form
-            S3 = 1
-            #print("compute S3:", not skip_S3, end="; S3 = ")
-            if not skip_S3:
-                S3_com_before = S3_sgn_computation_string.split("->")[0]
-                parity_list = [ block[unique_fsummand.index(c)] for c in S3_com_before ]
-                S3 = relative_sign(S3_sgn_computation_string,parity_list)
-                #print("S3:",S3_sgn_computation_string,"=",S3)
-                #print(S3)
-
-            block_sign = S1*S3
-            #print("block sign = (",S1,")*(",S3,") =",block_sign)
-
-            # ======================================================================================================
-            # obtain the sign vectors
-            # ======================================================================================================
-            sigma_summed_list = []
-            for elem in summed_index_info:
-                c = elem[0][0]
-                sigma_summed_list += [ sigma_list[unique_fsummand.index(c)] ]
-            
-            # ======================================================================================================
-            # the summation
-            # ======================================================================================================
-            einsum_obj_list = blocked_obj_list + sigma_summed_list
-            for i,elem in enumerate(einsum_obj_list):
-                if elem.dtype == object :
-                    newelem = np.array(elem.tolist())
-                    einsum_obj_list[i] = newelem
-
-            sum_result = block_sign*np.einsum(*tuple([final_einsum_string]+einsum_obj_list))
-
-
-            # ======================================================================================================
-            # obtain the output block
-            # ======================================================================================================
-
-            out_block = tuple([ block[unique_fsummand.index(c)] for c in fafter ])
-            #print("output block:",fafter,";",out_block)
-            ret.data[out_block] += sum_result
-            ret.shape = newshape_final
-
-            skip_power_of_two_check = False
-            
-    else:
-        # if returns scalar
-        # count unique indices
-        unique_fsummand = "".join(sorted(list(set(fbefore))))
-        nsum = len(unique_fsummand)
-
-        # the comprehensive list of sign factors (fermion only)
-        all_sgn = [[],[]]
-        for obj in obj_list:
-            for ind_parity in [0,1]:
-                for s in obj.sgn[ind_parity]:
-                    all_sgn[ind_parity] += [s]
-
-        block_list = [[]] # this is the set of all blocks
-        for char in unique_fsummand:
-            block_list_E = [ config+[0] for config in block_list ]
-            block_list_O = [ config+[1] for config in block_list ]
-            block_list = block_list_E+block_list_O
-
-        block_list = [ tuple(block) for block in block_list ]
-
-        scalar_output=0
-        for block in block_list:
-            #print()
-            #print(unique_fsummand,"=",block)
-
-            # ======================================================================================================
-            # now you have the summand list and the block list, you can do whatever you want here
-            # unique_fsummand is the ordered list of summed indices
-            # block is the value of each index
-            # ======================================================================================================
-
-            # ======================================================================================================
-            # This part determines the block number of each object
-            # ======================================================================================================
-            obj_block_list = []
-            for i,findex in enumerate(obj_findex_list):
-                sub_block = []
-                for c in findex:
-                    if c not in unique_fsummand:
-                        error("Error[einsum_block]: the character c is not contained in unique_fsummand. Unexplanable error! Possibly a bug.")
-                    c_location = unique_fsummand.index(c)
-                    sub_block += [block[c_location]]
-                obj_block_list += [tuple(sub_block)]
-            
-            #print(obj_findex_list,"=",obj_block_list)
-
-            # ======================================================================================================
-            # get the specified block from each object
-            # ======================================================================================================
-            '''
-            blocked_obj_list = [ obj.data[obj_block_list[i]] for i,obj in enumerate(obj_list) ]
-            blocked_sgn_list = sum([ obj.sgn[obj_block_list[i]].tolist()  for i,obj in enumerate(obj_list) ],[])
-            blocked_sgn_list = [ np.array(elem) for elem in blocked_sgn_list ]
-            #
-            # /\
-            # ||
-            #
-            # dont use this one
-            #
-            # use this one instead
-            #
-            # |
-            # V
-            #
-            sigma_list = []
-            for c in unique_fsummand:
-                # check if there are multiples
-                sgn_c = blocked_sgn_list[summand.index(c)]
-                if summand.count(c) > 1:
-                    err = 0
-                    for c2 in summand:
-                        if c2==c :
-                            sgn_c2 = blocked_sgn_list[summand.index(c2)]
-                            err += np.linalg.norm(sgn_c-sgn_c2)
-                    if err>numer_cutoff :
-                        error("Error[einsum_block]: some sign factors are not consistent.")
-                sigma_list += [ sgn_c ]
-            '''
-            blocked_obj_list = [ obj.data[obj_block_list[i]] for i,obj in enumerate(obj_list) ]
-
-            sigma_list = []
-            #print(summand)
-            #print(all_sgn[0])
-            #print(unique_fsummand)
-            #print(block)
-            
-            for ic, c in enumerate(unique_fsummand):
-                c_index_in_summand = summand.index(c)
-                sgn_c = all_sgn[block[ic]][c_index_in_summand]
-                if summand.count(c) > 1:
-                    err = 0
-                    for ic2, c2 in enumerate(summand):
-                        if c2==c :
-                            sgn_c2 = all_sgn[block[ic]][ic2]
-                            err += np.linalg.norm(sgn_c-sgn_c2)
-                    if err>numer_cutoff :
-                        error("Error[einsum_block]: some sign factors are not consistent.")
-                sigma_list += [ sgn_c ]
-
-            # ======================================================================================================
-            # evaluate the block sign factor
-            # ======================================================================================================
-
-            # step1: from moving conjugated summed index to the non-conjugated counterpart
-            S1 = 1
-            #print("compute S1:", not skip_S1, end="; S1 = ")
-            if not skip_S1:
-                S1_com_before = S1_sgn_computation_string.split("->")[0]
-                # replaced the new index with the old index
-                for elem in summed_index_info:
-                    S1_com_before = S1_com_before.replace(elem[0][1],elem[0][0])
-                # get the parity list
-                parity_list = [ block[unique_fsummand.index(c)] for c in S1_com_before ]
-                S1 = relative_sign(S1_sgn_computation_string,parity_list)
-                #print("S1:",S1_sgn_computation_string,"=",S1)
-                #print(S1)
-
-            block_sign = S1
-            #print("block sign = (",S1,")*(",S3,") =",block_sign)
-
-            # ======================================================================================================
-            # obtain the sign vectors
-            # ======================================================================================================
-            sigma_summed_list = []
-            for elem in summed_index_info:
-                c = elem[0][0]
-                sigma_summed_list += [ sigma_list[unique_fsummand.index(c)] ]
-            
-            # ======================================================================================================
-            # the summation
-            # ======================================================================================================
-            einsum_obj_list = blocked_obj_list + sigma_summed_list
-            sum_result = block_sign*np.einsum(*tuple([final_einsum_string]+einsum_obj_list))
-
-            scalar_output+=sum_result
-
-            skip_power_of_two_check = False
-
-        return scalar_output
 
-    if incorrect_sign_size(ret):
-        ret = correct_sign_size(ret)
-        if incorrect_sign_size(ret):
-            error("Error[??]: Unsuccessful attempt at truncating the sgn vectors.")
-    
-    return ret.force_format(first_format)
-
-def einsum_block_v140(*args):
-
-    # =============================================================================================#
-    # Step I: Pre-generate the cells of the result                                                 #
-    # =============================================================================================#
-
-    global skip_power_of_two_check
-    skip_power_of_two_check = True
-    subscripts = args[0].replace(" ","")
-    subscripts = denumerate(subscripts)
-
-    before=""
-    after=""
-    return_scalar = True
-    if subscripts.count("->")==1 :
-        before,after = subscripts.split("->")
-        return_scalar = False
-    elif subscripts.count("->")>1 :
-        print(error("Error[einsum_block]: There should be no more than one '->' indicator in the subscript input."))
-    else:
-        before = subscripts
-    has_output = not return_scalar
-
-    summand = before.replace(",","")
-
-    obj_index_list = before.split(",")
-    nobj = len(obj_index_list)
-
-    obj_list = make_list(args[1:1+nobj])
-    stats_list = sum([ make_list(obj.statistics) for obj in obj_list ],[])
-    shape_list = sum([ make_list(obj.effective_shape) for obj in obj_list ],[])
-    eshape_list = sum([ make_list(obj.even_shape) for obj in obj_list ],[])
-    oshape_list = sum([ make_list(obj.odd_shape) for obj in obj_list ],[])
-    
-    has_int = False
-    has_float = False
-    has_complex = False
-    first_format = obj_list[0].format
-    for i,obj in enumerate(obj_list):
-        if type(obj)==dense or type(obj)==sparse:
-            error("Error[einsum_block]: This function only works with block data format.")
-        obj_list[i] = obj_list[i].force_format("standard")
-        has_int = has_int or obj_list[i].dtype==int
-        has_float = has_float or obj_list[i].dtype==float
-        has_complex = has_complex or obj_list[i].dtype==complex
-
-    rettype = int
-    if has_float:
-        rettype = float
-    if has_complex:
-        rettype = complex
-
-    #fstats_list = make_list( stat for i,stat in enumerate(stats_list) if stats_list[i] in fermi_type ) # not used
-    #fshape_list = make_list( shape for i,shape in enumerate(shape_list) if stats_list[i] in fermi_type )
-    feshape_list = make_list( shape for i,shape in enumerate(eshape_list) if stats_list[i] in fermi_type )
-    foshape_list = make_list( shape for i,shape in enumerate(oshape_list) if stats_list[i] in fermi_type )
-
-    # the block version of before
-    fbefore = ""
-    for i,c in enumerate(summand):
-        if stats_list[i] in fermi_type:
-            fbefore += c
-    obj_findex_list = obj_index_list.copy()
-    for i, findex in enumerate(obj_findex_list):
-        new_findex = ""
-        for c in findex:
-            if c in fbefore:
-                new_findex+=c
-        obj_findex_list[i] = new_findex
-    if has_output:
-        # the block version of after
-        fafter = ""
-        for c in after:
-            if c in fbefore:
-                fafter += c
-        fsubscripts = fbefore+"->"+fafter
-
-        # <fbefore> is <summand> without bose-type indices
-        # <fafter> is <after> without bose-type indices
-
-        newstats = reordering(summand,after,stats_list)   # tensor stats
-        newshape = reordering(summand,after,shape_list)   # tensor shape
-        neweshape = reordering(summand,after,eshape_list)   # tensor even shape
-        newoshape = reordering(summand,after,oshape_list)   # tensor odd shape
-        #newfshape = reordering(fbefore,fafter,fshape_list) # cell shape
-
-        newshape_final = make_tuple([
-                dim if stat in bose_type else 2**int(np.ceil(np.log2(dim)))
-                    for dim,stat in zip(newshape,newstats) ])
-        # correct ret's shape in the end
-        #ret = zero_block(effective_shape=newshape,statistics=newstats,format=first_format,dtype=rettype)
-        ret = zero_block_eo(neweshape,newoshape,statistics=newstats,format=first_format,dtype=rettype)
-
-        # copy the sign factors from here
-        ret_sgn_e = []
-        ret_sgn_o = []
-        for c in after:
-            found = False
-            obj_num = -1
-            ind_loc = -1
-            str_sample = ""
-            for obj_num_temp,obj_ind in enumerate(obj_index_list):
-                if c in obj_ind:
-                    obj_num = obj_num_temp
-                    ind_loc = obj_ind.index(c)
-                    str_sample = obj_ind
-                    break
-            if obj_num==-1 or ind_loc==-1:
-                error("Error[einsum_block]: cannot locate the final subscript in the original objects' subscripts")
-            ret_sgn_e += [obj_list[obj_num].sgn[0][ind_loc]]
-            ret_sgn_o += [obj_list[obj_num].sgn[1][ind_loc]]
-
-            #print("Found",c,"in "+str(ind_loc)+"-th index of "+str(obj_num)+"-th object;",str_sample)
-
-        ret.sgn = [ret_sgn_e,ret_sgn_o]
-
-    # =============================================================================================#
-    # Step II: Arrange the indices (presum) and generate the sign-factor computation string        #
-    #          Most of the stuff here are copied from einsum()                                     #
-    # =============================================================================================#
-
-    # get some information about the summed indices -------------------------------------------------
-    # [ f=<char>, [index locations in lf], [statistics] ]
-    summed_index_info = []
-
-    for i,char in enumerate(summand):
-
-        # skip if bosonic
-        if stats_list[i] in bose_type:
-            continue
-
-        lf =  before.count(char)
-        if has_output :
-            rf = after.count(char)
-            if lf>2 or rf>1 or (lf+rf)%2==1 :
-                if lf>2 :
-                    reason = "lf>2"
-                elif rf>1 :
-                    reason = "rf>1"
-                else :
-                    reason = "(lf+rf)%2==1"
-                error("Error[einsum]: Inconsistent index statistics. (reason:"+reason+")")
-        else :
-            if lf>2:
-                reason = "lf>2"
-                error("Error[einsum]: Inconsistent index statistics. (reason:"+reason+")")
-
-        if lf==1:
-            continue
-
-        # add a new entry if it is a new character
-        if summand[:i].count(char)==0 :
-            summed_index_info += [ [ char, [i] , [stats_list[i]] ] ]
-        else:
-            for k in range(len(summed_index_info)):
-                if(summed_index_info[k][0]==char):
-                    summed_index_info[k][1] += [i]
-                    summed_index_info[k][2] += [stats_list[i]]
-
-    def is_statwise_inconsistent(stat1,stat2):
-        if [stat1,stat2] == [0,0]:
-            return False
-        elif [stat1,stat2] == [1,-1]:
-            return False
-        elif [stat1,stat2] == [-1,1]:
-            return False
-        elif [stat1,stat2] == [hybrid_symbol,hybrid_symbol]:
-            return False
-        else:
-            return True
-
-    for [char,location,stats] in summed_index_info:
-        if len(stats)==2 and is_statwise_inconsistent(stats[0],stats[1]):
-            error("Error[einsum]: The contracted indices have inconsistent statistics!")
-    
-    fsummand   = ""
-    fsummand_u = ""
-    fstats_list = []
-    fshape_list = []
-    charlist = summand
-    for i,char in enumerate(summand):
-        if stats_list[i] == 0:
-            continue
-
-        fsummand    += char
-        fstats_list += stats_list[i],
-        fshape_list += shape_list[i],
-
-        if stats_list[i] == -1 and summand.count(char)>1:
-            new_char = get_char(charlist)
-            charlist += new_char
-            fsummand_u += new_char
-
-            # edit the summed_index_info, with the position swapped a little bit as well
-            for j,[char2,location,stats] in enumerate(summed_index_info):
-                if char2==char :
-                    summed_index_info[j][0] = [char,new_char]
-                    if stats == [-1,1]:
-                        summed_index_info[j][1] = [ summed_index_info[j][1][1], summed_index_info[j][1][0] ]
-                        summed_index_info[j][2] = [ summed_index_info[j][2][1], summed_index_info[j][2][0] ]
-        else:
-            fsummand_u += char
-    fstats = fstats_list.copy()
-    fshape = fshape_list.copy()
-    fstats_u = fstats_list.copy()
-    fshape_u = fshape_list.copy()
-
-    # remove the stat entry as it is redundant
-    for i,elem in enumerate(summed_index_info):
-        summed_index_info[i] = elem[:2]
-
-    # the summed indices are now next to each other with the conjugated one to the right
-
-    fsummand_ur = fsummand_u
-    for [ [c1,c2], loc ] in summed_index_info:
-        fsummand_ur = fsummand_ur.replace(c2,"")
-        fsummand_ur = fsummand_ur.replace(c1,c1+c2)
-
-    fstats_ur = reordering(fsummand_u,fsummand_ur,fstats_list)
-    fshape_ur = reordering(fsummand_u,fsummand_ur,fshape_list)
-
-    # remove the leading and trailing chars that is the same as the pre-rearranged string
-
-    nall_u = len(fsummand_u)
-
-    nl = 0
-    for i in range(nall_u):
-        if fsummand_u[i] != fsummand_ur[i]:
-            break
-        nl+=1
-    nr = 0
-    for i in range(nall_u):
-        if fsummand_u[nall_u-1-i] != fsummand_ur[nall_u-1-i]:
-            break
-        nr+=1
-    nr = nall_u-nr
-
-    fsummand_ut  = fsummand_u[nl:nr]
-    fstats_ut   = fstats_u[nl:nr]
-    fshape_ut   = fshape_u[nl:nr]
-    fsummand_urt  = fsummand_ur[nl:nr]
-    fstats_urt   = fstats_ur[nl:nr]
-    fshape_urt   = fshape_ur[nl:nr]
-
-    if nl>nr :
-        skip_S1 = True
-    else:
-        skip_S1 = False
-        
-    S1_sgn_computation_string = fsummand_ut+"->"+fsummand_urt
-    
-    # =============================================================================================#
-    # Step III: rearrange to the final form                                                        #
-    # =============================================================================================#
-
-    S2_dimlist = []
-    S2_index_string = ""
-    summed_indices = fsummand_ur
-    for [ [c1,c2], loc ] in summed_index_info:
-        S2_dimlist += shape_list[ summand.index(c1) ],
-        S2_index_string += ","+c1
-        summed_indices = summed_indices.replace(c1+c2,"")
-    S2_index_string = S2_index_string[1:]
-    nS2 = len(S2_dimlist)
-    
-    skip_S3 = True
-    if has_output :
-
-        foutput = ""
-        for c in after:
-            if stats_list[ summand.index(c) ] == 0 :
-                continue
-            else:
-                foutput+=c
-
-        S3_shape=[]
-        for c in summed_indices:
-            d = shape_list[ summand.index(c) ]
-            S3_shape += d,
-
-        # again... remove the leading and trailing duplicates
-
-        nall_ur = len(summed_indices)
-        nl = 0
-        for i in range(nall_ur):
-            if summed_indices[i] != foutput[i]:
-                break
-            nl+=1
-
-        nr = 0
-        for i in range(nall_ur):
-            if summed_indices[nall_ur-1-i] != foutput[nall_ur-1-i]:
-                break
-            nr+=1
-        nr = nall_ur-nr
-
-        final = foutput[nl:nr]
-        prefinal = summed_indices[nl:nr]
-        S3_shape   = S3_shape[nl:nr]
-
-        if nl>nr :
-            skip_S3 = True
-        else:
-            skip_S3 = False
-
-        S3_sgn_computation_string = prefinal+"->"+final
-
-    # =============================================================================================#
-    # Step IV: Determine the einsum string                                                         #
-    # =============================================================================================#
-
-    before_plus_sigma = before
-    for elem in summed_index_info:
-        before_plus_sigma+=(","+elem[0][0])
-    final_einsum_string = before_plus_sigma+"->"+after
-
-    # =============================================================================================#
-    # Step V: Iterate over all parity config                                                       #
-    #          For each parity config, the sign factor is computed                                 #
-    # =============================================================================================#
-
-    if has_output:
-        # count unique indices
-        unique_fsummand = "".join(sorted(list(set(fbefore))))
-        nsum = len(unique_fsummand)
-
-        # the comprehensive list of sign factors (fermion only)
-        all_sgn = [[],[]]
-        for obj in obj_list:
-            for ind_parity in [0,1]:
-                for s in obj.sgn[ind_parity]:
-                    all_sgn[ind_parity] += [s]
-
-        block_list = [[]] # this is the set of all blocks
-        for char in unique_fsummand:
-            block_list_E = [ config+[0] for config in block_list ]
-            block_list_O = [ config+[1] for config in block_list ]
-            block_list = block_list_E+block_list_O
-
-        block_list = [ tuple(block) for block in block_list ]
-
-        for block in block_list:
-            #print()
-            #print(unique_fsummand,"=",block)
-
-            # ======================================================================================================
-            # now you have the summand list and the block list, you can do whatever you want here
-            # unique_fsummand is the ordered list of summed indices
-            # block is the value of each index
-            # ======================================================================================================
-
-            # ======================================================================================================
-            # This part determines the block number of each object
-            # ======================================================================================================
-            obj_block_list = []
-            for i,findex in enumerate(obj_findex_list):
-                sub_block = []
-                for c in findex:
-                    if c not in unique_fsummand:
-                        error("Error[einsum_block]: the character c is not contained in unique_fsummand. Unexplanable error! Possibly a bug.")
-                    c_location = unique_fsummand.index(c)
-                    sub_block += [block[c_location]]
-                obj_block_list += [tuple(sub_block)]
-            
-            #print(obj_findex_list,"=",obj_block_list)
-
-            # ======================================================================================================
-            # get the specified block from each object
-            # ======================================================================================================
-            blocked_obj_list = [ obj.data[obj_block_list[i]] for i,obj in enumerate(obj_list) ]
-
-            sigma_list = []
-            #print(summand)
-            #print(all_sgn[0])
-            #print(unique_fsummand)
-            #print(block)
-            
             for ic, c in enumerate(unique_fsummand):
                 c_index_in_summand = summand.index(c)
                 sgn_c = all_sgn[block[ic]][c_index_in_summand]
                 if summand.count(c) > 1:
                     err = 0
                     for ic2, c2 in enumerate(summand):
                         if c2==c :
                             sgn_c2 = all_sgn[block[ic]][ic2]
                             err += np.linalg.norm(sgn_c-sgn_c2)
                     if err>numer_cutoff :
                         error("Error[einsum_block]: some sign factors are not consistent.")
-                sigma_list += [ sgn_c ]
+                sigma_list += [ sgn_c if not ignore_anticommutation else 1 ]
 
             # ======================================================================================================
             # evaluate the block sign factor
             # ======================================================================================================
 
             # step1: from moving conjugated summed index to the non-conjugated counterpart
             S1 = 1
@@ -4634,17 +3381,15 @@
             ret.sgn[1][axis] = ret.sgn[1][axis]*0
             fi += 1
         else:
             ndimaxis = len(ret.sgn[0][axis])
             ret.sgn[0][axis] = np.array(copy.deepcopy([1]*ndimaxis),dtype=int)
             ret.sgn[1][axis] = np.array(copy.deepcopy([1]*ndimaxis),dtype=int)
 
-    #print(ret.sgn[0][0].shape)
-    #print(ret.sgn[0][1].shape)
-    #print(ret.sgn[0][2].shape)
+
 
     group_block_info = []
     for elem in group_info:
         if 0 not in elem[1]:
             group_block_info += [elem]
 
     it = np.nditer(Obj.data, flags=['multi_index','refs_ok'])
@@ -4686,15 +3431,15 @@
             d0 = [ len(Obj.sgn[0][axis]) for axis in axis_loc ]
             d1 = [ len(Obj.sgn[1][axis]) for axis in axis_loc ]
 
             sgn_list = [ Obj.sgn[p][axis] for axis,p in zip(axis_loc,block_group[fielem]) ]
 
             x_list = zip(block_group[fielem],d0,d1,sgn_list)
 
-            _block,_shift,_size,_sgn = gtn.join_index(*x_list)
+            _block,_shift,_size,_sgn = join_index(*x_list)
             check_block += [_block]
             fblock_shift += [_shift]
             subblocksize += [_size]
             new_sgn_list += [_sgn]
             fielem += 1
 
         subblocksize = make_tuple(subblocksize)
@@ -5087,15 +3832,15 @@
 
 
     nnz = 0
     #if np.abs(Λ[0]) < numer_cutoff:
     #    error("Error[SortedSVD]: np.linalg.svd() returns zero singular value vector!")
 
     for i,s in enumerate(Λ):
-        if np.abs(s/Λ[0]) > numer_cutoff:
+        if np.abs(s/(np.abs(Λ[0])+numer_cutoff)) > numer_cutoff:
             nnz+=1
 
     if cutoff!=None and cutoff < nnz:
         nnz = cutoff
 
     Λ = Λ[:nnz]
     U = U[:,:nnz]
@@ -5249,14 +3994,15 @@
 
             if(i==len(separator_list)-1):
                 partition_string += " )"
 
         error("Error[svd]: The input string must contain one and only one partition "+partition_string+" in it.")
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #1
+
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 1 - JOIN LEGS BAESD ON THE GROUPINGS                                       :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
     # count the number of indices in the two groups
     n_left = 0
     n_right = 0
@@ -5276,14 +4022,56 @@
     join_legs_string_input = "("+join_legs_string_input+")"
 
     shape_left  = Obj.shape[:n_left]
     stats_left  = Obj.statistics[:n_left]
     shape_right = Obj.shape[n_left:]
     stats_right = Obj.statistics[n_left:]
 
+    # check if one of the legs (or both) are fermion with dimension 1
+
+    left_bond1  = list(stats_left)  in [[-1],[1]] and list(shape_left)  == [1]
+    right_bond1 = list(stats_right) in [[-1],[1]] and list(shape_right) == [1]
+
+    if left_bond1 or right_bond1:
+
+        Norm = Obj.norm
+        M = Obj.force_format("matrix")
+
+        if left_bond1 :
+            U = dense([[1]],statistics=(*stats_left,1),format='matrix')
+            Λ = dense([[Norm]],statistics=(-1,1),format='matrix')
+            V = M/Norm
+            Vstat = list(V.statistics)
+            Vstat[0] = -1
+            V.statistics = tuple(Vstat)
+        else :
+            U = M/Norm
+            Λ = dense([[Norm]],statistics=(-1,1),format='matrix')
+            V = dense([[1]],statistics=(-1,*stats_right),format='matrix')
+            Ustat = list(U.statistics)
+            Ustat[-1] = 1
+            U.statistics = tuple(Ustat)
+
+        if(this_format == 'standard'):
+            U = U.switch_format(save_memory=True)
+            Λ = Λ.switch_format(save_memory=True)
+            V = V.switch_format(save_memory=True)
+
+        if(this_encoder == 'parity-preserving'):
+            U = U.switch_encoder(save_memory=True)
+            Λ = Λ.switch_encoder(save_memory=True)
+            V = V.switch_encoder(save_memory=True)
+
+        if(this_type==sparse):
+            U = sparse(U)
+            Λ = sparse(Λ)
+            V = sparse(V)
+
+        return U,Λ,V
+
     def zero_or_else(vector,value):
         for elem in vector:
             if elem!=0:
                 return value
         return 0
     def get_stat(vector,prefer=None):
         boson_count = 0
@@ -5431,15 +4219,15 @@
     U, Λ, V = np.linalg.svd(M, full_matrices=False)
 
     nnz = 0
     #if np.abs(Λ[0]) < numer_cutoff:
     #    error("Error[SortedSVD]: np.linalg.svd() returns zero singular value vector!")
 
     for i,s in enumerate(Λ):
-        if np.abs(s/Λ[0]) > numer_cutoff:
+        if np.abs(s/(np.abs(Λ[0])+numer_cutoff)) > numer_cutoff:
             nnz+=1
 
     if cutoff!=None and cutoff < nnz:
         nnz = cutoff
 
     Λ = Λ[:nnz]
     U = U[:,:nnz]
@@ -5622,14 +4410,54 @@
     join_legs_string_input = "("+join_legs_string_input+")"
 
     shape_left  = Obj.shape[:n_left]
     stats_left  = Obj.statistics[:n_left]
     shape_right = Obj.shape[n_left:]
     stats_right = Obj.statistics[n_left:]
 
+    left_bond1  = list(stats_left)  in [[-1],[1]] and list(shape_left)  == [1]
+    right_bond1 = list(stats_right) in [[-1],[1]] and list(shape_right) == [1]
+
+    if left_bond1 or right_bond1:
+
+        Norm = Obj.norm
+        M = Obj.force_format("matrix")
+
+        if left_bond1 :
+            U = dense([[1]],statistics=(*stats_left,1),format='matrix')
+            Λ = dense([[Norm]],statistics=(-1,1),format='matrix')
+            V = M/Norm
+            Vstat = list(V.statistics)
+            Vstat[0] = -1
+            V.statistics = tuple(Vstat)
+        else :
+            U = M/Norm
+            Λ = dense([[Norm]],statistics=(-1,1),format='matrix')
+            V = dense([[1]],statistics=(-1,*stats_right),format='matrix')
+            Ustat = list(U.statistics)
+            Ustat[-1] = 1
+            U.statistics = tuple(Ustat)
+
+        if(this_format == 'standard'):
+            U = U.switch_format(save_memory=True)
+            Λ = Λ.switch_format(save_memory=True)
+            V = V.switch_format(save_memory=True)
+
+        if(this_encoder == 'parity-preserving'):
+            U = U.switch_encoder(save_memory=True)
+            Λ = Λ.switch_encoder(save_memory=True)
+            V = V.switch_encoder(save_memory=True)
+
+        if(this_type==sparse):
+            U = sparse(U)
+            Λ = sparse(Λ)
+            V = sparse(V)
+
+        return U,Λ,V
+
     def zero_or_else(vector,value):
         for elem in vector:
             if elem!=0:
                 return value
         return 0
     def get_stat(vector,prefer=None):
         boson_count = 0
@@ -5820,14 +4648,75 @@
 
     for separator in separator_list:
         if separator == "|":
             continue
         else:
             string = string.replace(separator,"|")
 
+
+    # ===========================================================================
+    # Patch 1.4.2 --- accomodate the case with bond dimension 1
+    # ===========================================================================
+
+    # count the number of indices in the two groups
+    n_left = 0
+    n_right = 0
+    partition_found = False
+    for char in string:
+        if char in separator_list :
+            partition_found = True
+            continue
+        if(partition_found):
+            n_right+=1
+        else:
+            n_left+=1
+
+    join_legs_string_input = string
+    for partition in separator_list:
+        join_legs_string_input = join_legs_string_input.replace(partition,")(")
+    join_legs_string_input = "("+join_legs_string_input+")"
+
+    shape_left  = Obj.shape[:n_left]
+    stats_left  = Obj.statistics[:n_left]
+    shape_right = Obj.shape[n_left:]
+    stats_right = Obj.statistics[n_left:]
+
+    # check if one of the legs (or both) are fermion with dimension 1
+
+    left_bond1  = list(stats_left)  in [[-1],[1]] and list(shape_left)  == [1]
+    right_bond1 = list(stats_right) in [[-1],[1]] and list(shape_right) == [1]
+
+    if left_bond1 or right_bond1:
+
+        Norm = Obj.norm
+        M = Obj.force_format("matrix")
+
+        if left_bond1 :
+            U = dense([[1]],statistics=(*stats_left,1),format='matrix').toblock()
+            Λ = dense([[Norm]],statistics=(-1,1),format='matrix').toblock()
+            V = M/Norm
+            Vstat = list(V.statistics)
+            Vstat[0] = -1
+            V.statistics = tuple(Vstat)
+        else :
+            U = M/Norm
+            Λ = dense([[Norm]],statistics=(-1,1),format='matrix').toblock()
+            V = dense([[1]],statistics=(-1,*stats_right),format='matrix').toblock()
+            Ustat = list(U.statistics)
+            Ustat[-1] = 1
+            U.statistics = tuple(Ustat)
+
+        if(this_format == 'standard'):
+            U = U.switch_format()
+            Λ = Λ.switch_format()
+            V = V.switch_format()
+
+        return U,Λ,V
+
+
     # ===========================================================================
     # These are the index info before the rearrangement
     # ===========================================================================
 
     index_num = 0
     subscripts1 = ["",""]
     stats1 = [[],[]]
@@ -6571,14 +5460,69 @@
     for separator in separator_list:
         if separator == "|":
             continue
         else:
             string = string.replace(separator,"|")
 
     # ===========================================================================
+    # Patch 1.4.2 --- accomodate the case with bond dimension 1
+    # ===========================================================================
+
+    # count the number of indices in the two groups
+    n_left = 0
+    n_right = 0
+    partition_found = False
+    for char in string:
+        if char in separator_list :
+            partition_found = True
+            continue
+        if(partition_found):
+            n_right+=1
+        else:
+            n_left+=1
+
+    join_legs_string_input = string
+    for partition in separator_list:
+        join_legs_string_input = join_legs_string_input.replace(partition,")(")
+    join_legs_string_input = "("+join_legs_string_input+")"
+
+    shape_left  = Obj.shape[:n_left]
+    stats_left  = Obj.statistics[:n_left]
+    shape_right = Obj.shape[n_left:]
+    stats_right = Obj.statistics[n_left:]
+
+    # check if one of the legs (or both) are fermion with dimension 1
+
+    left_bond1  = list(stats_left)  in [[-1],[1]] and list(shape_left)  == [1]
+    right_bond1 = list(stats_right) in [[-1],[1]] and list(shape_right) == [1]
+
+    if left_bond1 or right_bond1:
+        # forcefully make the dimension to 2
+
+        if right_bond1:
+            Obj.sgn[1][-1] = [1]
+            Obj.shape = tuple(list(Obj.shape[:-1])+[2])
+
+            ret = Obj.hconjugate(string)
+
+            ret.sgn[1][0] = [0]
+            ret.shape = tuple([1]+list(Obj.shape[:-1]))
+        else:
+            Obj.sgn[1][0] = [1]
+            Obj.shape = tuple([2]+list(Obj.shape[1:]))
+            
+            ret = Obj.hconjugate(string)
+
+            ret.sgn[1][-1] = [0]
+            ret.shape = tuple(list(Obj.shape[1:])+[1])
+
+        return ret
+
+
+    # ===========================================================================
     # These are the index info before the rearrangement
     # ===========================================================================
 
     index_num = 0
     subscripts1 = ["",""]
     stats1 = [[],[]]
     shape1 = [[],[]]
@@ -6903,14 +5847,17 @@
     if not skip_trimming:
         A = trim_grassmann_odd(A)
     if tensor_type==sparse:
         A = sparse(A)
         A = A.remove_zeros()
     return A
 
+def zeros(shape,statistics,tensor_type=dense,encoder="canonical",format="standard",dtype=float):
+    return 0.0*random(shape,statistics,tensor_type,encoder,format,dtype,True)
+
 def power(T,p):
     if type(T)==block:
         return power_block(T,p)
     else:
         return power_ds(T,p)
 
 def sqrt(T):
```

### Comparing `grassmanntn-1.4.1/grassmanntn/arith.py` & `grassmanntn-1.4.2/grassmanntn/arith.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn/example.py` & `grassmanntn-1.4.2/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn/example_block.py` & `grassmanntn-1.4.2/grassmanntn/example_block.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn/gauge2d.py` & `grassmanntn-1.4.2/grassmanntn/gauge2d.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn/gauge2d_block.py` & `grassmanntn-1.4.2/grassmanntn/gauge2d_block.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn/param.py` & `grassmanntn-1.4.2/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.4.1/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.4.2/grassmanntn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.4.1
+Version: 1.4.2
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_141.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_142.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.4.1/setup.py` & `grassmanntn-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.4.1',      # Start with a small number and increase it with every change you make
+  version = '1.4.2',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_141.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_142.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
           'sympy',
       ],
```

