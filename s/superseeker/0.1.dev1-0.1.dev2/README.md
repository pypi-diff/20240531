# Comparing `tmp/superseeker-0.1.dev1.tar.gz` & `tmp/superseeker-0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superseeker-0.1.dev1.tar", last modified: Thu May 30 22:37:19 2024, max compression
+gzip compressed data, was "superseeker-0.1.dev2.tar", last modified: Thu May 30 22:51:47 2024, max compression
```

## Comparing `superseeker-0.1.dev1.tar` & `superseeker-0.1.dev2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/
--rw-r--r--   0 u0829237 (1372016) marth     (2288)     1036 2024-05-16 18:51:10.000000 superseeker-0.1.dev1/LICENSE
--rw-r--r--   0 u0829237 (1372016) marth     (2288)     1933 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/PKG-INFO
--rw-r--r--   0 u0829237 (1372016) marth     (2288)     1427 2024-05-30 22:16:09.000000 superseeker-0.1.dev1/README.md
--rw-rw----   0 u0829237 (1372016) marth     (2288)       38 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/setup.cfg
--rw-r--r--   0 u0829237 (1372016) marth     (2288)      852 2024-05-30 22:33:19.000000 superseeker-0.1.dev1/setup.py
-drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker/
--rw-r--r--   0 u0829237 (1372016) marth     (2288)      186 2024-05-30 22:34:17.000000 superseeker-0.1.dev1/superseeker/__init__.py
--rw-r--r--   0 u0829237 (1372016) marth     (2288)    15740 2024-05-30 22:17:26.000000 superseeker-0.1.dev1/superseeker/data_manipulation.py
--rw-r--r--   0 u0829237 (1372016) marth     (2288)     2064 2024-05-30 22:16:12.000000 superseeker-0.1.dev1/superseeker/pipeline.py
-drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/
--rw-r--r--   0 u0829237 (1372016) marth     (2288)     1933 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/PKG-INFO
--rw-rw----   0 u0829237 (1372016) marth     (2288)      360 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/SOURCES.txt
--rw-rw----   0 u0829237 (1372016) marth     (2288)        1 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/dependency_links.txt
--rw-rw----   0 u0829237 (1372016) marth     (2288)       66 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/entry_points.txt
--rw-rw----   0 u0829237 (1372016) marth     (2288)       13 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/requires.txt
--rw-rw----   0 u0829237 (1372016) marth     (2288)       18 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/superseeker.egg-info/top_level.txt
-drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:37:19.000000 superseeker-0.1.dev1/tests/
--rw-r--r--   0 u0829237 (1372016) marth     (2288)       20 2024-05-16 18:39:26.000000 superseeker-0.1.dev1/tests/__init__.py
--rw-r--r--   0 u0829237 (1372016) marth     (2288)     2451 2024-05-16 18:44:20.000000 superseeker-0.1.dev1/tests/test_pipeline.py
+drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:51:47.000000 superseeker-0.1.dev2/
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)     1036 2024-05-16 18:51:10.000000 superseeker-0.1.dev2/LICENSE
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)     1933 2024-05-30 22:51:47.000000 superseeker-0.1.dev2/PKG-INFO
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)     1427 2024-05-30 22:16:09.000000 superseeker-0.1.dev2/README.md
+-rw-rw----   0 u0829237 (1372016) marth     (2288)       38 2024-05-30 22:51:47.000000 superseeker-0.1.dev2/setup.cfg
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)      852 2024-05-30 22:48:12.000000 superseeker-0.1.dev2/setup.py
+drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker/
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)      186 2024-05-30 22:34:17.000000 superseeker-0.1.dev2/superseeker/__init__.py
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)    16287 2024-05-30 22:50:17.000000 superseeker-0.1.dev2/superseeker/data_manipulation.py
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)     2064 2024-05-30 22:16:12.000000 superseeker-0.1.dev2/superseeker/pipeline.py
+drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:51:47.000000 superseeker-0.1.dev2/superseeker.egg-info/
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)     1933 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker.egg-info/PKG-INFO
+-rw-rw----   0 u0829237 (1372016) marth     (2288)      360 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker.egg-info/SOURCES.txt
+-rw-rw----   0 u0829237 (1372016) marth     (2288)        1 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker.egg-info/dependency_links.txt
+-rw-rw----   0 u0829237 (1372016) marth     (2288)       66 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker.egg-info/entry_points.txt
+-rw-rw----   0 u0829237 (1372016) marth     (2288)       13 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker.egg-info/requires.txt
+-rw-rw----   0 u0829237 (1372016) marth     (2288)       18 2024-05-30 22:51:46.000000 superseeker-0.1.dev2/superseeker.egg-info/top_level.txt
+drwxrws--x   0 u0829237 (1372016) marth     (2288)        0 2024-05-30 22:51:47.000000 superseeker-0.1.dev2/tests/
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)       20 2024-05-16 18:39:26.000000 superseeker-0.1.dev2/tests/__init__.py
+-rw-r--r--   0 u0829237 (1372016) marth     (2288)     2451 2024-05-16 18:44:20.000000 superseeker-0.1.dev2/tests/test_pipeline.py
```

### Comparing `superseeker-0.1.dev1/LICENSE` & `superseeker-0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `superseeker-0.1.dev1/PKG-INFO` & `superseeker-0.1.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superseeker
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: SuperSeeker_Pipeline is a Python library for identifying subclonal evolution in cancer.
 Home-page: https://github.com/gageblack/superseeker_pipeline
 Author: Gage Black
 Author-email: gage.black@utah.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `superseeker-0.1.dev1/README.md` & `superseeker-0.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `superseeker-0.1.dev1/setup.py` & `superseeker-0.1.dev2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='superseeker',
-    version='0.1.dev1',
+    version='0.1.dev2',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `superseeker-0.1.dev1/superseeker/data_manipulation.py` & `superseeker-0.1.dev2/superseeker/data_manipulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     # 1. Read in VCF file, and get the sample names that are included in VCF
     # 2. Read in the facets cncf files for each sample one at at time
     # 3. For each sample, store the CNV info for each region. Include the start and end, and the major/minor info.
     # 4. For each variant in the VCF file, iterate through each of the sample read count values. Add one line
     #    to the output per sample, indicating which sample it came from and inputting the needed info
     # 5. Once each sample value for that variant has a line in the output, move on to the next variant
     # 6. Make sure that Y chromosomes are getting a Normal CN of 1. Everything else is 2.
-    
+  
     HIGH_IMPACT = False #I think all variants are needed for clustering.
     ## Step 1. ##
     if vcf_file_name[-7:] == ".vcf.gz": ## This is not working yet. For some reason it adds b' ' to every line.
         #vcf_file = gzip.open(vcf_file_name, "rb")
         print("VCF file is compressed. Please decompress and try again.")
     elif vcf_file_name[-4:] == ".vcf":
         vcf_file = open(vcf_file_name, "r")
@@ -167,22 +167,16 @@
     if germfilter == "TRUE":
         germline_sample = columns[9]
         samples = columns[10:] # I think this way of getting sample IDs will only work for the CLL workflow. It will need to be more robust in future. Starts at 10 to skip germline sample.
     else: 
         samples = columns[9:]
     print(samples)
 
-    if facets_dir == "":
-        cn_override = "TRUE"
-
     samples_cn_lists = []
-    if patient_sex == "M":
-        X_normal_cn = 1
-    else:
-        X_normal_cn = 2
+    X_normal_cn = 2
     ## Step 3 ##
     if cn_override != "TRUE":
         samples_cn_lists, X_normal_cn = get_CN_info(samples)
 
     ## print to ouput file.
     output_file.write("mutation_id\tsample_id\tref_counts\talt_counts\tmajor_cn\tminor_cn\tnormal_cn\n")
     for line in variant_lines:
@@ -351,21 +345,42 @@
             replacement_list.append(ID)
         
     if replacement:
         print("Replacement")
         output_file.write("Replacement\n")
     elif emergence:
         print("Positive Selection")
-        output_file.write("New Clone Emergence\n")
+        output_file.write("Positive Selection\n")
     elif selection:
         print("Negative Selection")
-        output_file.write("Selection\n")
+        output_file.write("Negative Selection\n")
     else:
         print("No Evolution")
         output_file.write("No Evolution\n")
 
-    output_file.write("Subclones with selection: "+",".join(selection_list)+"\n")
-    output_file.write("Subclones with new clone emergence: "+",".join(emergence_list)+"\n")
-    output_file.write("Subclones with replacement: "+",".join(replacement_list)+"\n")
+    output_file.write("Subclones with Negative Selection: "+",".join(selection_list)+"\n")
+    output_file.write("Subclones with Postive Selection: "+",".join(emergence_list)+"\n")
+    output_file.write("Subclones with Replacement: "+",".join(replacement_list)+"\n")
 
     input_file.close()
     output_file.close()
+
+def make_dot_files(subclones_vcf, tmp_graph_files):
+    vcf_file_name = subclones_vcf
+    tmp_dir = tmp_graph_files
+
+    infile = open(vcf_file_name, "r")
+    i = 0
+    for line in infile:
+        if line[0] != "#":
+            break
+        if line[0:10] == "##subclone":
+            i=i+1
+            edges = line.split("\"")[1]
+            outfile = open(tmp_dir+"/solution"+str(i)+".gv", "w")
+            outfile.write("digraph D{\n")
+            for edge in edges.split(", "):
+                outfile.write(edge+"\n")
+            outfile.write("label=\"Solution "+str(i)+"\"\nlabelloc=\"t\"\n}"+"\n")
+            outfile.close()
+
+    infile.close()
```

### Comparing `superseeker-0.1.dev1/superseeker/pipeline.py` & `superseeker-0.1.dev2/superseeker/pipeline.py`

 * *Files identical despite different names*

### Comparing `superseeker-0.1.dev1/superseeker.egg-info/PKG-INFO` & `superseeker-0.1.dev2/superseeker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superseeker
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: SuperSeeker_Pipeline is a Python library for identifying subclonal evolution in cancer.
 Home-page: https://github.com/gageblack/superseeker_pipeline
 Author: Gage Black
 Author-email: gage.black@utah.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `superseeker-0.1.dev1/tests/test_pipeline.py` & `superseeker-0.1.dev2/tests/test_pipeline.py`

 * *Files identical despite different names*

