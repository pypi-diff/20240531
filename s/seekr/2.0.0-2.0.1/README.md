# Comparing `tmp/seekr-2.0.0.tar.gz` & `tmp/seekr-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seekr-2.0.0.tar", last modified: Sun Mar 10 20:03:58 2024, max compression
+gzip compressed data, was "seekr-2.0.1.tar", last modified: Fri May 31 17:45:04 2024, max compression
```

## Comparing `seekr-2.0.0.tar` & `seekr-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-03-10 20:03:58.705279 seekr-2.0.0/
--rw-r--r--   0 sl         (501) staff       (20)     1079 2024-03-10 13:45:41.000000 seekr-2.0.0/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)    43477 2024-03-10 20:03:58.704980 seekr-2.0.0/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)    42949 2024-03-10 13:45:41.000000 seekr-2.0.0/README.md
--rw-r--r--   0 sl         (501) staff       (20)       30 2024-03-10 13:45:41.000000 seekr-2.0.0/pyproject.toml
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-03-10 20:03:58.680893 seekr-2.0.0/seekr/
--rw-r--r--   0 sl         (501) staff       (20)      141 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)      277 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/__version__.py
--rw-r--r--   0 sl         (501) staff       (20)     8191 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/adj_pval.py
--rw-r--r--   0 sl         (501) staff       (20)    64713 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/console_scripts.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-03-10 20:03:58.683724 seekr-2.0.0/seekr/data/
--rw-r--r--   0 sl         (501) staff       (20)   275572 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/data/arial.ttf
--rw-r--r--   0 sl         (501) staff       (20) 20731727 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/data/gencode.vM25.lncRNA_transcripts.unique.genesequence_withfullairn.fa
--rw-r--r--   0 sl         (501) staff       (20)     6129 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/fasta.py
--rw-r--r--   0 sl         (501) staff       (20)     3229 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/fasta_reader.py
--rw-r--r--   0 sl         (501) staff       (20)    12114 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/filter_gencode.py
--rw-r--r--   0 sl         (501) staff       (20)    18350 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/find_dist.py
--rw-r--r--   0 sl         (501) staff       (20)     9861 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/find_pval.py
--rw-r--r--   0 sl         (501) staff       (20)    10251 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_comp_textplot.py
--rw-r--r--   0 sl         (501) staff       (20)     7950 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_count_barplot.py
--rw-r--r--   0 sl         (501) staff       (20)     8717 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_counts.py
--rw-r--r--   0 sl         (501) staff       (20)     7632 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_dendrogram.py
--rw-r--r--   0 sl         (501) staff       (20)    18554 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_heatmap.py
--rw-r--r--   0 sl         (501) staff       (20)     9989 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_indi_textplot.py
--rw-r--r--   0 sl         (501) staff       (20)    17329 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_leiden.py
--rw-r--r--   0 sl         (501) staff       (20)     8403 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/kmer_msd_barplot.py
--rwxr-xr-x   0 sl         (501) staff       (20)      709 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/my_tqdm.py
--rw-r--r--   0 sl         (501) staff       (20)     1083 2024-03-10 13:45:41.000000 seekr-2.0.0/seekr/pearson.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2024-03-10 20:03:58.682822 seekr-2.0.0/seekr.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)    43477 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)      759 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)     1055 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/entry_points.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)      129 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)        6 2024-03-10 20:03:58.000000 seekr-2.0.0/seekr.egg-info/top_level.txt
--rw-r--r--   0 sl         (501) staff       (20)       38 2024-03-10 20:03:58.705356 seekr-2.0.0/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     2869 2024-03-10 13:45:41.000000 seekr-2.0.0/setup.py
+drwxr-xr-x   0 shuang     (501) staff       (20)        0 2024-05-31 17:45:04.865535 seekr-2.0.1/
+-rw-r--r--   0 shuang     (501) staff       (20)     1079 2024-05-31 17:38:23.000000 seekr-2.0.1/LICENSE
+-rw-r--r--   0 shuang     (501) staff       (20)    43787 2024-05-31 17:45:04.865245 seekr-2.0.1/PKG-INFO
+-rw-r--r--   0 shuang     (501) staff       (20)    42950 2024-05-31 17:38:23.000000 seekr-2.0.1/README.md
+-rw-r--r--   0 shuang     (501) staff       (20)       30 2024-05-31 17:38:23.000000 seekr-2.0.1/pyproject.toml
+drwxr-xr-x   0 shuang     (501) staff       (20)        0 2024-05-31 17:45:04.850706 seekr-2.0.1/seekr/
+-rw-r--r--   0 shuang     (501) staff       (20)      141 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/__init__.py
+-rw-r--r--   0 shuang     (501) staff       (20)      277 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/__version__.py
+-rw-r--r--   0 shuang     (501) staff       (20)     8191 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/adj_pval.py
+-rw-r--r--   0 shuang     (501) staff       (20)    64715 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/console_scripts.py
+drwxr-xr-x   0 shuang     (501) staff       (20)        0 2024-05-31 17:45:04.851964 seekr-2.0.1/seekr/data/
+-rw-r--r--   0 shuang     (501) staff       (20)   275572 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/data/arial.ttf
+-rw-r--r--   0 shuang     (501) staff       (20) 20731727 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/data/gencode.vM25.lncRNA_transcripts.unique.genesequence_withfullairn.fa
+-rw-r--r--   0 shuang     (501) staff       (20)     6129 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/fasta.py
+-rw-r--r--   0 shuang     (501) staff       (20)     3229 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/fasta_reader.py
+-rw-r--r--   0 shuang     (501) staff       (20)    12114 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/filter_gencode.py
+-rw-r--r--   0 shuang     (501) staff       (20)    18338 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/find_dist.py
+-rw-r--r--   0 shuang     (501) staff       (20)     9861 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/find_pval.py
+-rw-r--r--   0 shuang     (501) staff       (20)    10251 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_comp_textplot.py
+-rw-r--r--   0 shuang     (501) staff       (20)     7950 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_count_barplot.py
+-rw-r--r--   0 shuang     (501) staff       (20)     8717 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_counts.py
+-rw-r--r--   0 shuang     (501) staff       (20)     7632 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_dendrogram.py
+-rw-r--r--   0 shuang     (501) staff       (20)    18554 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_heatmap.py
+-rw-r--r--   0 shuang     (501) staff       (20)     9989 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_indi_textplot.py
+-rw-r--r--   0 shuang     (501) staff       (20)    17329 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_leiden.py
+-rw-r--r--   0 shuang     (501) staff       (20)     8403 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/kmer_msd_barplot.py
+-rwxr-xr-x   0 shuang     (501) staff       (20)      709 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/my_tqdm.py
+-rw-r--r--   0 shuang     (501) staff       (20)     1083 2024-05-31 17:38:23.000000 seekr-2.0.1/seekr/pearson.py
+drwxr-xr-x   0 shuang     (501) staff       (20)        0 2024-05-31 17:45:04.864964 seekr-2.0.1/seekr.egg-info/
+-rw-r--r--   0 shuang     (501) staff       (20)    43787 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/PKG-INFO
+-rw-r--r--   0 shuang     (501) staff       (20)      759 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/SOURCES.txt
+-rw-r--r--   0 shuang     (501) staff       (20)        1 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/dependency_links.txt
+-rw-r--r--   0 shuang     (501) staff       (20)     1055 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/entry_points.txt
+-rw-r--r--   0 shuang     (501) staff       (20)        1 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/not-zip-safe
+-rw-r--r--   0 shuang     (501) staff       (20)      129 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/requires.txt
+-rw-r--r--   0 shuang     (501) staff       (20)        6 2024-05-31 17:45:04.000000 seekr-2.0.1/seekr.egg-info/top_level.txt
+-rw-r--r--   0 shuang     (501) staff       (20)       38 2024-05-31 17:45:04.866611 seekr-2.0.1/setup.cfg
+-rw-r--r--   0 shuang     (501) staff       (20)     2869 2024-05-31 17:38:23.000000 seekr-2.0.1/setup.py
```

### Comparing `seekr-2.0.0/LICENSE` & `seekr-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/PKG-INFO` & `seekr-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: seekr
-Version: 2.0.0
-Summary: Count small kmer frequencies in nucleotide sequences.
-Home-page: https://github.com/CalabreseLab/seekr
-Author: Jessime Kirk, Shuang Li, Luke Ni
-Author-email: shuang9@email.unc.edu
-License: MIT
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SEEKR
 
 [![Build Status](https://travis-ci.com/CalabreseLab/seekr.svg?branch=master)](https://travis-ci.com/CalabreseLab/seekr)
 [![Build Status](https://img.shields.io/pypi/v/seekr.svg)](https://pypi.python.org/pypi/seekr)
 
 Find communities of nucleotide sequences based on *k*-mer frequencies.
 
@@ -45,15 +29,15 @@
 
 First you need to install Docker on your local computer. Then pull the Docker Image:
 
 ```
 $ docker pull calabreselab/seekr:latest
 ```
 
-This will install the Docker container which enables running seekr from the command line or Jupyter Notebook. See below the Seekr Docker Image secion for more details.
+This will install the Docker container which enables running seekr from the command line or Jupyter Notebook. See below the Seekr Docker Image section for more details.
 
 ### CentOS
 
 Users have been successful in installing `seekr` from source on CentOS:
 
 ```
 conda create --name seekr_source python=3.9
```

### Comparing `seekr-2.0.0/README.md` & `seekr-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: seekr
+Version: 2.0.1
+Summary: Count small kmer frequencies in nucleotide sequences.
+Home-page: https://github.com/CalabreseLab/seekr
+Author: Jessime Kirk, Shuang Li, Luke Ni
+Author-email: shuang9@email.unc.edu
+License: MIT
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cython
+Requires-Dist: tqdm
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: networkx>=3.1
+Requires-Dist: python-igraph==0.10.4
+Requires-Dist: leidenalg==0.9.1
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: seaborn
+Requires-Dist: scipy
+Requires-Dist: statsmodels
+
 # SEEKR
 
 [![Build Status](https://travis-ci.com/CalabreseLab/seekr.svg?branch=master)](https://travis-ci.com/CalabreseLab/seekr)
 [![Build Status](https://img.shields.io/pypi/v/seekr.svg)](https://pypi.python.org/pypi/seekr)
 
 Find communities of nucleotide sequences based on *k*-mer frequencies.
 
@@ -29,15 +57,15 @@
 
 First you need to install Docker on your local computer. Then pull the Docker Image:
 
 ```
 $ docker pull calabreselab/seekr:latest
 ```
 
-This will install the Docker container which enables running seekr from the command line or Jupyter Notebook. See below the Seekr Docker Image secion for more details.
+This will install the Docker container which enables running seekr from the command line or Jupyter Notebook. See below the Seekr Docker Image section for more details.
 
 ### CentOS
 
 Users have been successful in installing `seekr` from source on CentOS:
 
 ```
 conda create --name seekr_source python=3.9
```

### Comparing `seekr-2.0.0/seekr/adj_pval.py` & `seekr-2.0.1/seekr/adj_pval.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/console_scripts.py` & `seekr-2.0.1/seekr/console_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,29 +220,29 @@
 For more details of the inputs and outputs, please refer to the manual listed under https://github.com/CalabreseLab/seekr/
 Any issues can be reported to https://github.com/CalabreseLab/seekr/issues
 
 """
 
 FIND_PVAL_DOC = """
 Description: 
-calculte p values of the seekr.pearson correlation values for input sequence 1 vs input sequence 2 
+calculate p values of the seekr.pearson correlation values for input sequence 1 vs input sequence 2 
 p value is based on the output of find_dist, which is either a list of distributions or a npy array
 
 Details:
 this function connects the output of find_dist and the input sequnces of interests (2 input sequences)
-given the background sequencs, find_dist calculate all possible pairwise seekr.pearson values
+given the background sequences, find_dist calculate all possible pairwise seekr.pearson values
 and then outputs either a list of fitted distributions or the npy array of the actual data 
 find_pval firstly calculates the seekr.pearson of the two input sequences, which produces a correlation matrix 
 find_pval then calculate the p value for each r value in the pearson correlation matrix based on the output of find_dist
 the output of find_pval is a dataframe of p values, with the row names (input 1) and column names (input 2) as the headers of the input sequences
 
 Example:
 calculate p values for the seekr.pearson correlation between input sequences 1 and input sequences 2
 with kmer size of 4, log2 transform of 'Log2.post', and corresponding normalization vectors saved as mean_4mer.npy and std_4mer.npy
-with the bakcground distribution saved as a list of fitted distributions fitres.csv, among which the best fitted distribution is the first one
+with the background distribution saved as a list of fitted distributions fitres.csv, among which the best fitted distribution is the first one
 show progress bar for the p value calculation step and save the output to test_pval.csv under current directory
     
     $ seekr_find_pval seqs1.fa seqs2.fa mean_4mer.npy std_4mer.npy 4 fitres.csv -ft distribution -bf 1 -o test_pval -pb
 
 to save under other location change to -o /Users/username/Desktop/test_pval
 to not save the result, leave out -o and its argument
```

### Comparing `seekr-2.0.0/seekr/data/arial.ttf` & `seekr-2.0.1/seekr/data/arial.ttf`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/data/gencode.vM25.lncRNA_transcripts.unique.genesequence_withfullairn.fa` & `seekr-2.0.1/seekr/data/gencode.vM25.lncRNA_transcripts.unique.genesequence_withfullairn.fa`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/fasta.py` & `seekr-2.0.1/seekr/fasta.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/fasta_reader.py` & `seekr-2.0.1/seekr/fasta_reader.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/filter_gencode.py` & `seekr-2.0.1/seekr/filter_gencode.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/find_dist.py` & `seekr-2.0.1/seekr/find_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # k_mer: k-mer size, by default k_mer=4
 # log2: whether to do log2 transform, possible options are: 'Log2.post','Log2.pre' and 'Log2.none', default is 'Log2.post'
 # Log2.post -- Log2 transformation post-standardization: self.counts += np.abs(np.min(self.counts)) self.counts += 1 self.counts = np.log2(self.counts)
 # Log2.pre -- Log2 transformation pre-standardization: self.counts += np.abs(np.min(self.counts)) self.counts += 1
 # Log2.none -- no log2 transformation
 # models: groups of candidate models for fitting, options are: 'all','common10' (default), or a list of distributions by user input for example ['norm','expon','pareto']
 # 'all' - fit all available distributions from scipy stats, both rv_continuous and rv_discrete: https://docs.scipy.org/doc/scipy/reference/stats.html#continuous-distributions
-# 'common10' - fit 10 common distributions ('cauchy', 'chi2', 'expon', 'exponpow', 'gamma', 'lognorm', 'norm', 'pareto', 'rayleigh', 'uniform')
+# 'common10' - fit 10 common distributions ('cauchy', 'chi2', 'expon', 'exponpow', 'gamma', 'lognorm', 'norm', 'pareto', 'rayleigh', 't')
 # common10 distributions are deteremined from get_common_distributions() from the Fitter library with 'powerlaw' replaced by 'pareto' as pareto belongs to powerlaw family and bears a biology relation 
 # user can also choose to input their own list of distributions in a list format, but be sure all distributions are available in scipy.stats
 # subsetting: True (default) or False. whether or not to use a subset of the data for fitting or output. For large datasets, subsetting is recommended to save time
 # here subsetting is performed after getting all possible pairwise seekr pearson correlation values for the background sequences
 # subsetting is not performed on the input background sequences
 # subset_size: the size of the subset to use for fitting or output. Default is 100000. only be used when subsetting=True
 # if subset_size is larger than the actual data size, the actual data size will be used instead
@@ -91,15 +91,15 @@
         
         # Construct the path to the .fa file
         inputseq = os.path.join(current_dir, 'data', 'gencode.vM25.lncRNA_transcripts.unique.genesequence_withfullairn.fa')
     
     #preprare the list of distributions to be used
     if models == 'common10':
         distributions = ['cauchy', 'chi2', 'expon', 'exponpow', 'gamma', 
-                         'lognorm', 'norm', 'pareto', 'rayleigh', 'uniform']
+                         'lognorm', 'norm', 'pareto', 'rayleigh', 't']
         
     else: 
         #Create all distributions (continous and discrete) that would be used
         continuous_distributions = [d for d in dir(stats) if
                         isinstance(getattr(stats, d), stats.rv_continuous)]
 
         discrete_distributions = [d for d in dir(stats) if
```

### Comparing `seekr-2.0.0/seekr/find_pval.py` & `seekr-2.0.1/seekr/find_pval.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_comp_textplot.py` & `seekr-2.0.1/seekr/kmer_comp_textplot.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_count_barplot.py` & `seekr-2.0.1/seekr/kmer_count_barplot.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_counts.py` & `seekr-2.0.1/seekr/kmer_counts.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_dendrogram.py` & `seekr-2.0.1/seekr/kmer_dendrogram.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_heatmap.py` & `seekr-2.0.1/seekr/kmer_heatmap.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_indi_textplot.py` & `seekr-2.0.1/seekr/kmer_indi_textplot.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_leiden.py` & `seekr-2.0.1/seekr/kmer_leiden.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/kmer_msd_barplot.py` & `seekr-2.0.1/seekr/kmer_msd_barplot.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/my_tqdm.py` & `seekr-2.0.1/seekr/my_tqdm.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr/pearson.py` & `seekr-2.0.1/seekr/pearson.py`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr.egg-info/PKG-INFO` & `seekr-2.0.1/seekr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Metadata-Version: 2.1
 Name: seekr
-Version: 2.0.0
+Version: 2.0.1
 Summary: Count small kmer frequencies in nucleotide sequences.
 Home-page: https://github.com/CalabreseLab/seekr
 Author: Jessime Kirk, Shuang Li, Luke Ni
 Author-email: shuang9@email.unc.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cython
+Requires-Dist: tqdm
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: networkx>=3.1
+Requires-Dist: python-igraph==0.10.4
+Requires-Dist: leidenalg==0.9.1
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: seaborn
+Requires-Dist: scipy
+Requires-Dist: statsmodels
 
 # SEEKR
 
 [![Build Status](https://travis-ci.com/CalabreseLab/seekr.svg?branch=master)](https://travis-ci.com/CalabreseLab/seekr)
 [![Build Status](https://img.shields.io/pypi/v/seekr.svg)](https://pypi.python.org/pypi/seekr)
 
 Find communities of nucleotide sequences based on *k*-mer frequencies.
@@ -45,15 +57,15 @@
 
 First you need to install Docker on your local computer. Then pull the Docker Image:
 
 ```
 $ docker pull calabreselab/seekr:latest
 ```
 
-This will install the Docker container which enables running seekr from the command line or Jupyter Notebook. See below the Seekr Docker Image secion for more details.
+This will install the Docker container which enables running seekr from the command line or Jupyter Notebook. See below the Seekr Docker Image section for more details.
 
 ### CentOS
 
 Users have been successful in installing `seekr` from source on CentOS:
 
 ```
 conda create --name seekr_source python=3.9
```

### Comparing `seekr-2.0.0/seekr.egg-info/SOURCES.txt` & `seekr-2.0.1/seekr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/seekr.egg-info/entry_points.txt` & `seekr-2.0.1/seekr.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `seekr-2.0.0/setup.py` & `seekr-2.0.1/setup.py`

 * *Files identical despite different names*

