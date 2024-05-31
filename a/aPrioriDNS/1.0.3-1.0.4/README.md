# Comparing `tmp/aprioridns-1.0.3.tar.gz` & `tmp/aprioridns-1.0.4.tar.gz`

## Comparing `aprioridns-1.0.3.tar` & `aprioridns-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0   138671 2020-02-02 00:00:00.000000 aprioridns-1.0.3/src/aPrioriDNS/DNS.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aprioridns-1.0.3/src/aPrioriDNS/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aprioridns-1.0.3/src/aPrioriDNS/_data_struct.py
--rw-r--r--   0        0        0    10684 2020-02-02 00:00:00.000000 aprioridns-1.0.3/src/aPrioriDNS/_utils.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aprioridns-1.0.3/src/aPrioriDNS/_variables.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 aprioridns-1.0.3/LICENSE
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aprioridns-1.0.3/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 aprioridns-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 aprioridns-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aprioridns-1.0.4/README.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 aprioridns-1.0.4/Updates.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 aprioridns-1.0.4/test_unreleased_version.py
+-rw-r--r--   0        0        0   139275 2020-02-02 00:00:00.000000 aprioridns-1.0.4/src/aPrioriDNS/DNS.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aprioridns-1.0.4/src/aPrioriDNS/__init__.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aprioridns-1.0.4/src/aPrioriDNS/_data_struct.py
+-rw-r--r--   0        0        0    10684 2020-02-02 00:00:00.000000 aprioridns-1.0.4/src/aPrioriDNS/_utils.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aprioridns-1.0.4/src/aPrioriDNS/_variables.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 aprioridns-1.0.4/tutorials/01-cut_a_scalar.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 aprioridns-1.0.4/tutorials/02-filter_scalar.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aprioridns-1.0.4/tutorials/05-initialize_DNS_field.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aprioridns-1.0.4/tutorials/06-cut_DNS_field.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aprioridns-1.0.4/tutorials/07-filter_DNS_field.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 aprioridns-1.0.4/LICENSE
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 aprioridns-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aprioridns-1.0.4/PKG-INFO
```

### Comparing `aprioridns-1.0.3/src/aPrioriDNS/DNS.py` & `aprioridns-1.0.4/src/aPrioriDNS/DNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 from tabulate import tabulate
 import shutil
 from scipy.ndimage import convolve
 from scipy.ndimage import gaussian_filter
 import matplotlib.pyplot as plt
 import numpy as np
 import cantera as ct
-from scipy.fftpack import fftn, ifftn, fftshift, ifftshift
-from scipy.signal import tukey
-from scipy.ndimage import gaussian_filter1d
 
 from ._variables import variables_list
 from ._variables import mesh_list
 from ._utils import (
     check_data_files,
     check_folder_structure,
     extract_species,
@@ -988,15 +985,15 @@
                         print("Operation aborted.")
                         sys.exit()
                     else:
                         count += 1
                         delete_file(path)
                 else:
                     delete_file(path)
-        delete_file(self.find_path('Mu'))
+
         delete_file(self.find_path(f'HRR_{mode}'))
         
         # Step 5: Compute reaction rates
         chunk_size = self.shape[0] * self.shape [1] * self.shape[2] // n_chunks
         gas = ct.Solution(self.kinetic_mechanism)
         
         # Open output files in writing mode
@@ -1028,30 +1025,30 @@
             
             # iterate through the chunks and compute the Reaction Rates
             for j in range(len(T_chunk)):
                 gas.TPY  = T_chunk[j], P_chunk[j], Y_chunk[:, j]
                 tau_star = np.minimum(Tau_c_chunk[j], Tau_m_chunk[j])
                 
                 Y0       = gas.Y
-                h0       = gas.enthalpy_mass # Specific enthalpy [J/kg].
+                h0       = gas.partial_molar_enthalpies/gas.molecular_weights # partial mass enthalpy [J/kg].
                 
                 reactor  = ct.IdealGasReactor(gas)
                 sim      = ct.ReactorNet([reactor])
                 t_start  = 0
                 t_end    = tau_star
                 
                 # integrate the batch reactor in time
                 while t_start < t_end:
                     t_start = sim.step()
                 
                 Ystar    = gas.Y
                 hstar    = gas.enthalpy_mass # Specific enthalpy [J/kg].
                 
                 R_chunk[:, j] = RHO_chunk[j] / tau_star * (Ystar - Y0)
-                HRR_chunk[j]  = RHO_chunk[j] / tau_star * (hstar - h0)
+                HRR_chunk[j]  = -np.sum (h0 * R_chunk[:, j])
                 
             # Save files
             save_file(HRR_chunk, output_file_HRR)
             R_chunk = R_chunk.tolist()
             for k in range(len(self.species)):
                 save_file(np.array(R_chunk[k]), output_files_R[k])
             
@@ -1595,14 +1592,17 @@
         if not os.path.exists(filt_data_path):
             os.makedirs(filt_data_path)
         if not os.path.exists(filt_grid_path):
             shutil.copytree(self.grid_path, filt_grid_path)
         if not os.path.exists(filt_chem_path):
             shutil.copytree(self.chem_path, filt_chem_path)
         if not os.path.exists(os.path.join(filt_folder_path, 'info.json')):
+            # TODO: it's wrong handling this like that, because if the folder already existed with a different
+            # size of the field, the file info.json is not updated. In summary, you have to delete the 
+            # entire folder before starting cause it's better
             shutil.copy(os.path.join(self.folder_path, 'info.json'), os.path.join(filt_folder_path, 'info.json'))
         
         if filter_type.lower() == 'gauss':
             RHO_filt = filter_gauss(self.RHO._3d, filter_size)
         elif filter_type.lower() == 'box':
             RHO_filt = filter_box(self.RHO._3d, filter_size)
         else:
@@ -2275,30 +2275,39 @@
         >>> print("Cut field with equal mode:")
         >>> print(cut_field_equal)
         >>> # Cut the field with specified number of samples removed for each dimension
         >>> cut_field_xyz = field.cut(n_cut=(1, 2, 3), mode='xyz')
         >>> print("\nCut field with xyz mode:")
         >>> print(cut_field_xyz)
         """
+        valid_modes = ['equal', 'xyz']
+        check_input_string(mode, valid_modes, 'mode')
+        
         if not self.is_light_mode():
             # TODO: update this function to handle the xyz mode also in this branch
             self.reshape_3d()
             if mode=='equal':
                 self.value = self.value[n_cut:self.Nx-n_cut,n_cut:self.Ny-n_cut,n_cut:self.Nz-n_cut]
             self.shape = self.value.shape #update the shape of the field
         else:
-            field_cut = self.reshape_3d()
+            field_cut = self._3d
             if mode=='equal':
                 field_cut = field_cut[n_cut:self.Nx-n_cut,n_cut:self.Ny-n_cut,n_cut:self.Nz-n_cut]
-            elif mode=='xyz':
+                return field_cut
+            elif mode=='xyz' and len(n_cut)==3: # Light mode
                 n_cut_x = n_cut[0]
                 n_cut_y = n_cut[1]
                 n_cut_z = n_cut[2]
                 field_cut = field_cut[n_cut_x:self.Nx-n_cut_x,n_cut_y:self.Ny-n_cut_y,n_cut_z:self.Nz-n_cut_z]
                 return field_cut
+            elif mode=='xyz' and len(n_cut)==6:
+                field_cut = field_cut[n_cut[0]:self.Nx-n_cut[1],n_cut[2]:self.Ny-n_cut[3],n_cut[4]:self.Nz-n_cut[5]]
+                return field_cut
+            else:
+                raise ValueError("The lenght of the cutting vector must be 3 or 6 for the mode xyz.")
     
     def filter_gauss(self, delta,n_cut=0,mute=False):
         """
         Filters the scalar field with a Gaussian function.
         The variance sigma is considered equal to:
             sigma = sqrt(1/12*delta**2) 
         where delta is the filter size (in this case specified as
```

### Comparing `aprioridns-1.0.3/src/aPrioriDNS/_utils.py` & `aprioridns-1.0.4/src/aPrioriDNS/_utils.py`

 * *Files identical despite different names*

### Comparing `aprioridns-1.0.3/src/aPrioriDNS/_variables.py` & `aprioridns-1.0.4/src/aPrioriDNS/_variables.py`

 * *Files identical despite different names*

### Comparing `aprioridns-1.0.3/LICENSE` & `aprioridns-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aprioridns-1.0.3/pyproject.toml` & `aprioridns-1.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aPrioriDNS"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Lorenzo Piu", email="lorenzo.piu@ulb.be" },
 ]
 description = "A package to process Direct Numerical Simulations of reacting and non reacting flows"
-readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

