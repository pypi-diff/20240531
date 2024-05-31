# Comparing `tmp/cyclicpeptide-1.0.1.tar.gz` & `tmp/cyclicpeptide-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclicpeptide-1.0.1.tar", last modified: Fri May 31 06:49:29 2024, max compression
+gzip compressed data, was "cyclicpeptide-1.0.2.tar", last modified: Fri May 31 06:52:50 2024, max compression
```

## Comparing `cyclicpeptide-1.0.1.tar` & `cyclicpeptide-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:49:29.175430 cyclicpeptide-1.0.1/
--rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.1/LICENSE.md
--rw-r--r--   0 willow     (501) staff       (20)     2547 2024-05-31 06:49:29.175354 cyclicpeptide-1.0.1/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.1/README.md
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:49:29.174118 cyclicpeptide-1.0.1/cyclicpeptide/
--rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.1/cyclicpeptide/AminoAcids.txt
--rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.1/cyclicpeptide/Chemical_P.csv
--rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.1/cyclicpeptide/GraphAlignment.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.1/cyclicpeptide/IOManager.py
--rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.1/cyclicpeptide/PropertyAnalysis.py
--rwxr-xr-x   0 willow     (501) staff       (20)     9971 2024-05-31 06:47:23.000000 cyclicpeptide-1.0.1/cyclicpeptide/Sequence2Structure.py
--rw-r--r--   0 willow     (501) staff       (20)    11017 2024-05-13 03:22:59.000000 cyclicpeptide-1.0.1/cyclicpeptide/SequenceTransformer.py
--rwxr-xr-x   0 willow     (501) staff       (20)    39454 2024-05-31 06:48:50.000000 cyclicpeptide-1.0.1/cyclicpeptide/Structure2Sequence.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.1/cyclicpeptide/StructureTransformer.py
--rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.1/cyclicpeptide/__init__.py
--rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.1/cyclicpeptide/aa_smiles.txt
--rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.1/cyclicpeptide/aas.txt
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:49:29.175041 cyclicpeptide-1.0.1/cyclicpeptide.egg-info/
--rw-r--r--   0 willow     (501) staff       (20)     2547 2024-05-31 06:49:29.000000 cyclicpeptide-1.0.1/cyclicpeptide.egg-info/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)      597 2024-05-31 06:49:29.000000 cyclicpeptide-1.0.1/cyclicpeptide.egg-info/SOURCES.txt
--rw-r--r--   0 willow     (501) staff       (20)        1 2024-05-31 06:49:29.000000 cyclicpeptide-1.0.1/cyclicpeptide.egg-info/dependency_links.txt
--rw-r--r--   0 willow     (501) staff       (20)       92 2024-05-31 06:49:29.000000 cyclicpeptide-1.0.1/cyclicpeptide.egg-info/requires.txt
--rw-r--r--   0 willow     (501) staff       (20)       14 2024-05-31 06:49:29.000000 cyclicpeptide-1.0.1/cyclicpeptide.egg-info/top_level.txt
--rw-r--r--   0 willow     (501) staff       (20)       78 2024-05-31 06:49:29.175667 cyclicpeptide-1.0.1/setup.cfg
--rw-r--r--   0 willow     (501) staff       (20)     1099 2024-05-31 06:49:08.000000 cyclicpeptide-1.0.1/setup.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:52:50.223370 cyclicpeptide-1.0.2/
+-rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.2/LICENSE.md
+-rw-r--r--   0 willow     (501) staff       (20)     2547 2024-05-31 06:52:50.223304 cyclicpeptide-1.0.2/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.2/README.md
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:52:50.222036 cyclicpeptide-1.0.2/cyclicpeptide/
+-rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.2/cyclicpeptide/AminoAcids.txt
+-rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.2/cyclicpeptide/Chemical_P.csv
+-rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.2/cyclicpeptide/GraphAlignment.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.2/cyclicpeptide/IOManager.py
+-rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.2/cyclicpeptide/PropertyAnalysis.py
+-rwxr-xr-x   0 willow     (501) staff       (20)     9972 2024-05-31 06:52:09.000000 cyclicpeptide-1.0.2/cyclicpeptide/Sequence2Structure.py
+-rw-r--r--   0 willow     (501) staff       (20)    11017 2024-05-13 03:22:59.000000 cyclicpeptide-1.0.2/cyclicpeptide/SequenceTransformer.py
+-rwxr-xr-x   0 willow     (501) staff       (20)    39456 2024-05-31 06:52:29.000000 cyclicpeptide-1.0.2/cyclicpeptide/Structure2Sequence.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.2/cyclicpeptide/StructureTransformer.py
+-rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.2/cyclicpeptide/__init__.py
+-rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.2/cyclicpeptide/aa_smiles.txt
+-rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.2/cyclicpeptide/aas.txt
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:52:50.223029 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/
+-rw-r--r--   0 willow     (501) staff       (20)     2547 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)      597 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/SOURCES.txt
+-rw-r--r--   0 willow     (501) staff       (20)        1 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/dependency_links.txt
+-rw-r--r--   0 willow     (501) staff       (20)       92 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/requires.txt
+-rw-r--r--   0 willow     (501) staff       (20)       14 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/top_level.txt
+-rw-r--r--   0 willow     (501) staff       (20)       78 2024-05-31 06:52:50.223606 cyclicpeptide-1.0.2/setup.cfg
+-rw-r--r--   0 willow     (501) staff       (20)     1099 2024-05-31 06:52:45.000000 cyclicpeptide-1.0.2/setup.py
```

### Comparing `cyclicpeptide-1.0.1/LICENSE.md` & `cyclicpeptide-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/PKG-INFO` & `cyclicpeptide-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple example package
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cyclicpeptide-1.0.1/README.md` & `cyclicpeptide-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/AminoAcids.txt` & `cyclicpeptide-1.0.2/cyclicpeptide/AminoAcids.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/Chemical_P.csv` & `cyclicpeptide-1.0.2/cyclicpeptide/Chemical_P.csv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/GraphAlignment.py` & `cyclicpeptide-1.0.2/cyclicpeptide/GraphAlignment.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/IOManager.py` & `cyclicpeptide-1.0.2/cyclicpeptide/IOManager.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/PropertyAnalysis.py` & `cyclicpeptide-1.0.2/cyclicpeptide/PropertyAnalysis.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/Sequence2Structure.py` & `cyclicpeptide-1.0.2/cyclicpeptide/Sequence2Structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         backbone, backbone_idx = detect_backbone(mol)
         c_index = backbone[0]
         n_index = backbone[-1]
         mol = link_aa_by_peptide_bond(mol, c_index, n_index)
     return mol
 
 
-def reference_aa_monomer(monomers_path='cyclicpeptide/monomer.tsv'): #未修改
+def reference_aa_monomer(monomers_path=r'cyclicpeptide/monomer.tsv'): #未修改
     """
 
     :param monomers_path: sequence of essential AA.
     :type sequence: One letter code
     :param cyclic: Optional "cyclic".
     :type cyclic: True or False
     :return: mol
```

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/SequenceTransformer.py` & `cyclicpeptide-1.0.2/cyclicpeptide/SequenceTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/Structure2Sequence.py` & `cyclicpeptide-1.0.2/cyclicpeptide/Structure2Sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
                     # new_mol.AddBond(atom_mapping[inner_idx], new_idx, bond.GetBondType())
         new_mol = new_mol.GetMol()
         Chem.SanitizeMol(new_mol)
         aas.append(new_mol)
     return aas, atom_mappings
 
 
-def reference_aa_monomer(monomers_path='cyclicpeptide/monomer.tsv'):
+def reference_aa_monomer(monomers_path=r'cyclicpeptide/monomer.tsv'):
     """
     Identify amino acids based on the monomer reference library
 
     * Identify the type of each amino acid unit;
     * If it can be directly recognized by 20 essential amino acids, then the amino acid can be directly determined;
     * If it cannot be directly recognized by essential amino acids, use library to find the maximum matching reference unit;
     * For cross amino acid units, select the two reference units with the most matching atoms and no cross;
@@ -577,15 +577,15 @@
             display(SVG(svg_data))
         return svg_data
     else:
         print('Image failed to draw!')
         return ''
 
 
-def transform(smiles, monomers_path='cyclicpeptide/monomer.tsv'):
+def transform(smiles, monomers_path=r'cyclicpeptide/monomer.tsv'):
     """
     Transform and report generation through an integrated function.
     
     Example::
 
         from IPython.display import HTML
```

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide/StructureTransformer.py` & `cyclicpeptide-1.0.2/cyclicpeptide/StructureTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide.egg-info/PKG-INFO` & `cyclicpeptide-1.0.2/cyclicpeptide.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple example package
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `cyclicpeptide-1.0.1/cyclicpeptide.egg-info/SOURCES.txt` & `cyclicpeptide-1.0.2/cyclicpeptide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.1/setup.py` & `cyclicpeptide-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name='cyclicpeptide',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     description='A simple example package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Willow0316/cyclicpeptide/tree/master',
     author='Willow',
     author_email='willow.yang.b@gmail.com',
```

