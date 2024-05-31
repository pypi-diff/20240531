# Comparing `tmp/kfre-0.1.5.tar.gz` & `tmp/kfre-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfre-0.1.5.tar", last modified: Sat May  4 20:35:35 2024, max compression
+gzip compressed data, was "kfre-0.1.5a0.tar", last modified: Fri May 31 15:21:13 2024, max compression
```

## Comparing `kfre-0.1.5.tar` & `kfre-0.1.5a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:35:35.044159 kfre-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 20:35:26.000000 kfre-0.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-04 20:35:35.044159 kfre-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-05-04 20:35:26.000000 kfre-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:35:35.044159 kfre-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-04 20:35:26.000000 kfre-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:35:35.040159 kfre-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:35:35.040159 kfre-0.1.5/src/kfre/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-04 20:35:26.000000 kfre-0.1.5/src/kfre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-04 20:35:26.000000 kfre-0.1.5/src/kfre/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:35:35.040159 kfre-0.1.5/src/kfre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-04 20:35:35.000000 kfre-0.1.5/src/kfre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 20:35:35.000000 kfre-0.1.5/src/kfre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:35:35.000000 kfre-0.1.5/src/kfre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-04 20:35:35.000000 kfre-0.1.5/src/kfre.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 20:35:35.000000 kfre-0.1.5/src/kfre.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:21:13.973806 kfre-0.1.5a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-31 15:21:06.000000 kfre-0.1.5a0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-31 15:21:13.973806 kfre-0.1.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-05-31 15:21:06.000000 kfre-0.1.5a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:21:13.973806 kfre-0.1.5a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-31 15:21:06.000000 kfre-0.1.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:21:13.969806 kfre-0.1.5a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:21:13.969806 kfre-0.1.5a0/src/kfre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-31 15:21:06.000000 kfre-0.1.5a0/src/kfre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-05-31 15:21:06.000000 kfre-0.1.5a0/src/kfre/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:21:13.973806 kfre-0.1.5a0/src/kfre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-31 15:21:13.000000 kfre-0.1.5a0/src/kfre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 15:21:13.000000 kfre-0.1.5a0/src/kfre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:21:13.000000 kfre-0.1.5a0/src/kfre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 15:21:13.000000 kfre-0.1.5a0/src/kfre.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 15:21:13.000000 kfre-0.1.5a0/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.5/LICENSE.md` & `kfre-0.1.5a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.5/PKG-INFO` & `kfre-0.1.5a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: A Python library for estimating kidney failure risk using the KFRE model developed by Tangri et al.
 Author: Leonid Shpaner
 Author-email: lshpaner@ucla.edu
 Project-URL: Author Website, https://www.leonshpaner.com
 Project-URL: Documentation, https://lshpaner.github.io/kfre_docs/
 Project-URL: Zenodo Archive, https://zenodo.org/records/11100222
 Project-URL: Source Code, https://github.com/lshpaner/kfre
@@ -81,14 +81,16 @@
 If you have any questions or issues with `kfre`, please open an issue on this GitHub repository.
 
 ## Acknowledgements
 The KFRE model developed by Tangri et al. has made significant contributions to kidney disease research.
 
 The `kfre` library is based on the risk prediction models developed in the studies referenced below. Please refer to these studies for an in-depth understanding of the kidney failure risk prediction models used within this library.
 
+I would like to extend my gratitude to Panayiotis Petousis, PhD, Obidiugwu Duru, MD, MS, Kenn B. Daratha, PhD, Keith C. Norris, MD, PhD, Katherine R. Tuttle MD, FASN, FACP, FNKF, Susanne B. Nicholas, MD, MPH, PhD, and Alex Bui, PhD. Their exceptional work on end-stage kidney disease has greatly inspired the creation of this library.
+
 ## References 
 
 Sumida, K., Nadkarni, G. N., Grams, M. E., Sang, Y., Ballew, S. H., Coresh, J., Matsushita, K., Surapaneni, A., Brunskill, N., Chadban, S. J., Chang, A. R., Cirillo, M., Daratha, K. B., Gansevoort, R. T., Garg, A. X., Iacoviello, L., Kayama, T., Konta, T., Kovesdy, C. P., Lash, J., Lee, B. J., Major, R. W., Metzger, M., Miura, K., Naimark, D. M. J., Nelson, R. G., Sawhney, S., Stempniewicz, N., Tang, M., Townsend, R. R., Traynor, J. P., Valdivielso, J. M., Wetzels, J., Polkinghorne, K. R., & Heerspink, H. J. L. (2020). Conversion of urine protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine ratio for use in chronic kidney disease screening and prognosis. *Annals of Internal Medicine*, *173*(6), 426-435. https://doi.org/10.7326/M20-0529
 
 Tangri, N., Grams, M. E., Levey, A. S., Coresh, J., Appel, L. J., Astor, B. C., Chodick, G., Collins, A. J., Djurdjev, O., Elley, C. R., Evans, M., Garg, A. X., Hallan, S. I., Inker, L. A., Ito, S., Jee, S. H., Kovesdy, C. P., Kronenberg, F., Heerspink, H. J. L., Marks, A., Nadkarni, G. N., Navaneethan, S. D., Nelson, R. G., Titze, S., Sarnak, M. J., Stengel, B., Woodward, M., Iseki, K., & for the CKD Prognosis Consortium. (2016). Multinational assessment of accuracy of equations for predicting risk of kidney failure: A meta-analysis. *JAMA, 315*(2), 164–174. https://doi.org/10.1001/jama.2015.18202
 
 Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O., Naimark, D., Levin, A., & Levey, A. S. (2011). A predictive model for progression of chronic kidney disease to kidney failure. *JAMA*, *305*(15), 1553-1559. https://doi.org/10.1001/jama.2011.451
```

### Comparing `kfre-0.1.5/README.md` & `kfre-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `kfre-0.1.5/setup.py` & `kfre-0.1.5a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.5",
+    version="0.1.5a",
     author="Leonid Shpaner",
     author_email="lshpaner@ucla.edu",
     description="A Python library for estimating kidney failure risk using the KFRE model developed by Tangri et al.",
     long_description=open("min_readme.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
     package_dir={"": "src"},  # Directory where your package files are located
     # Automatically find packages in the specified directory
```

### Comparing `kfre-0.1.5/src/kfre/__init__.py` & `kfre-0.1.5a0/src/kfre/__init__.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.5/src/kfre/main.py` & `kfre-0.1.5a0/src/kfre/main.py`

 * *Files identical despite different names*

### Comparing `kfre-0.1.5/src/kfre.egg-info/PKG-INFO` & `kfre-0.1.5a0/src/kfre.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfre
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: A Python library for estimating kidney failure risk using the KFRE model developed by Tangri et al.
 Author: Leonid Shpaner
 Author-email: lshpaner@ucla.edu
 Project-URL: Author Website, https://www.leonshpaner.com
 Project-URL: Documentation, https://lshpaner.github.io/kfre_docs/
 Project-URL: Zenodo Archive, https://zenodo.org/records/11100222
 Project-URL: Source Code, https://github.com/lshpaner/kfre
@@ -81,14 +81,16 @@
 If you have any questions or issues with `kfre`, please open an issue on this GitHub repository.
 
 ## Acknowledgements
 The KFRE model developed by Tangri et al. has made significant contributions to kidney disease research.
 
 The `kfre` library is based on the risk prediction models developed in the studies referenced below. Please refer to these studies for an in-depth understanding of the kidney failure risk prediction models used within this library.
 
+I would like to extend my gratitude to Panayiotis Petousis, PhD, Obidiugwu Duru, MD, MS, Kenn B. Daratha, PhD, Keith C. Norris, MD, PhD, Katherine R. Tuttle MD, FASN, FACP, FNKF, Susanne B. Nicholas, MD, MPH, PhD, and Alex Bui, PhD. Their exceptional work on end-stage kidney disease has greatly inspired the creation of this library.
+
 ## References 
 
 Sumida, K., Nadkarni, G. N., Grams, M. E., Sang, Y., Ballew, S. H., Coresh, J., Matsushita, K., Surapaneni, A., Brunskill, N., Chadban, S. J., Chang, A. R., Cirillo, M., Daratha, K. B., Gansevoort, R. T., Garg, A. X., Iacoviello, L., Kayama, T., Konta, T., Kovesdy, C. P., Lash, J., Lee, B. J., Major, R. W., Metzger, M., Miura, K., Naimark, D. M. J., Nelson, R. G., Sawhney, S., Stempniewicz, N., Tang, M., Townsend, R. R., Traynor, J. P., Valdivielso, J. M., Wetzels, J., Polkinghorne, K. R., & Heerspink, H. J. L. (2020). Conversion of urine protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine ratio for use in chronic kidney disease screening and prognosis. *Annals of Internal Medicine*, *173*(6), 426-435. https://doi.org/10.7326/M20-0529
 
 Tangri, N., Grams, M. E., Levey, A. S., Coresh, J., Appel, L. J., Astor, B. C., Chodick, G., Collins, A. J., Djurdjev, O., Elley, C. R., Evans, M., Garg, A. X., Hallan, S. I., Inker, L. A., Ito, S., Jee, S. H., Kovesdy, C. P., Kronenberg, F., Heerspink, H. J. L., Marks, A., Nadkarni, G. N., Navaneethan, S. D., Nelson, R. G., Titze, S., Sarnak, M. J., Stengel, B., Woodward, M., Iseki, K., & for the CKD Prognosis Consortium. (2016). Multinational assessment of accuracy of equations for predicting risk of kidney failure: A meta-analysis. *JAMA, 315*(2), 164–174. https://doi.org/10.1001/jama.2015.18202
 
 Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O., Naimark, D., Levin, A., & Levey, A. S. (2011). A predictive model for progression of chronic kidney disease to kidney failure. *JAMA*, *305*(15), 1553-1559. https://doi.org/10.1001/jama.2011.451
```

