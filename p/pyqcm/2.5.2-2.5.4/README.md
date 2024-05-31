# Comparing `tmp/pyqcm-2.5.2.tar.gz` & `tmp/pyqcm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqcm-2.5.2.tar", last modified: Wed Apr  3 21:30:03 2024, max compression
+gzip compressed data, was "pyqcm-2.5.4.tar", last modified: Fri May 31 15:43:58 2024, max compression
```

## Comparing `pyqcm-2.5.2.tar` & `pyqcm-2.5.4.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.641532 pyqcm-2.5.2/
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-03 21:29:54.000000 pyqcm-2.5.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-03 21:29:54.000000 pyqcm-2.5.2/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11718 2024-04-03 21:29:54.000000 pyqcm-2.5.2/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     5088 2024-04-03 21:29:54.000000 pyqcm-2.5.2/INSTALL.md
--rw-rw-rw-   0 root         (0) root         (0)    35216 2024-04-03 21:29:54.000000 pyqcm-2.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     2773 2024-04-03 21:30:03.641532 pyqcm-2.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2467 2024-04-03 21:29:54.000000 pyqcm-2.5.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/ED/
--rw-rw-rw-   0 root         (0) root         (0)      693 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_ED.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_ED2.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_ED2_laptop.txt
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_GS.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_GS2.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_GS_loop.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/model_1D.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/model_2D.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/plot_bench_ED.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/integrals/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/plot_concurrent.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/plot_integrals.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/integrals/small/
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/integrals_small.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/integrals_small_concurrent.txt
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/integrals_small_results.txt
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/model_small.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/vca/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/vca/bench_vca.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/vca/bench_vca2.py
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.621531 pyqcm-2.5.2/docs/
--rwxrwxrwx   0 root         (0) root         (0)      623 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/Makefile
--rwxrwxrwx   0 root         (0) root         (0)      134 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/makedoc
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.621531 pyqcm-2.5.2/docs/source/
--rwxrwxrwx   0 root         (0) root         (0)     7924 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/2x2.png
--rwxrwxrwx   0 root         (0) root         (0)    65032 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/T6.png
--rwxrwxrwx   0 root         (0) root         (0)      917 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/cdmft.rst
--rwxrwxrwx   0 root         (0) root         (0)     5631 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/defining_cluster_models.rst
--rwxrwxrwx   0 root         (0) root         (0)     9560 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/defining_models.rst
--rwxrwxrwx   0 root         (0) root         (0)    37228 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/h4-6b.png
--rwxrwxrwx   0 root         (0) root         (0)     1265 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/h8.asy
--rw-rw-rw-   0 root         (0) root         (0)    57104 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/h8.png
--rw-rw-rw-   0 root         (0) root         (0)     1935 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/hartree.rst
--rwxrwxrwx   0 root         (0) root         (0)    66076 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/hexa6.png
--rwxrwxrwx   0 root         (0) root         (0)      579 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/index.rst
--rwxrwxrwx   0 root         (0) root         (0)     5217 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/intro.rst
--rwxrwxrwx   0 root         (0) root         (0)    18237 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/models.rst
--rw-rw-rw-   0 root         (0) root         (0)     6033 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/options.rst
--rwxrwxrwx   0 root         (0) root         (0)      782 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/options_intro.txt
--rwxrwxrwx   0 root         (0) root         (0)      236 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/other_functions.rst
--rwxrwxrwx   0 root         (0) root         (0)     6231 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel.rst
--rw-rw-rw-   0 root         (0) root         (0)    23261 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel_performance_concurrent.png
--rw-rw-rw-   0 root         (0) root         (0)    23202 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel_performance_ed.png
--rw-rw-rw-   0 root         (0) root         (0)    34896 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel_performance_integrals.png
--rwxrwxrwx   0 root         (0) root         (0)     8130 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parameters.rst
--rw-rw-rw-   0 root         (0) root         (0)    43029 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/t15.png
--rwxrwxrwx   0 root         (0) root         (0)      535 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/vca.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/examples/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.621531 pyqcm-2.5.2/examples/1D_2_4b/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/QCM_params.def
--rw-rw-rw-   0 root         (0) root         (0)   116475 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/averages.tsv
--rw-rw-rw-   0 root         (0) root         (0)    37866 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft.tsv
--rw-rw-rw-   0 root         (0) root         (0)     2620 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft_distance.tsv
--rw-rw-rw-   0 root         (0) root         (0)   114242 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft_grid.tsv
--rw-rw-rw-   0 root         (0) root         (0)   548325 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft_iter.tsv
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug_complex.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug_dvmc.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug_variable_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)    20439 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/dos.tsv
--rw-rw-rw-   0 root         (0) root         (0)    17095 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/h1.pdf
--rw-rw-rw-   0 root         (0) root         (0)    35032 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/h2.pdf
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/hop.npy
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/hopping.def
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/interaction.def
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/interaction.npy
--rwxrwxrwx   0 root         (0) root         (0)     2491 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/model_1D_2_4b.py
--rw-rw-rw-   0 root         (0) root         (0)    10812 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/out
--rw-rw-rw-   0 root         (0) root         (0)    20251 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/s1.pdf
--rw-rw-rw-   0 root         (0) root         (0)    21433 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/s2.pdf
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.625532 pyqcm-2.5.2/examples/1D_4/
--rw-rw-rw-   0 root         (0) root         (0)     3185 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/GS.tsv
--rw-rw-rw-   0 root         (0) root         (0)    18259 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/ave.tsv
--rw-rw-rw-   0 root         (0) root         (0)    18259 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/averages.tsv
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug_cdw.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug_dvmc.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug_rhoAB.py
--rw-rw-rw-   0 root         (0) root         (0)    11556 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/hartree.tsv
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/model_1D_4.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/model_1D_4_C2.py
--rw-rw-rw-   0 root         (0) root         (0)     3315 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/record.py
--rw-rw-rw-   0 root         (0) root         (0)  1077770 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/sef.tsv
--rw-rw-rw-   0 root         (0) root         (0)    29277 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/vca.tsv
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.625532 pyqcm-2.5.2/external/
--rw-rw-rw-   0 root         (0) root         (0)     1639 2024-04-03 21:29:54.000000 pyqcm-2.5.2/external/FindAVX2.cmake
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.625532 pyqcm-2.5.2/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)    21298 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/AF_VCA_vs_L.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/AF_VCA_vs_L.py
--rw-rw-rw-   0 root         (0) root         (0)   188540 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/CDW_1D.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4051 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/CDW_1D.py
--rw-rw-rw-   0 root         (0) root         (0)     9942 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_Weyl.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4186 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_Weyl.py
--rw-rw-rw-   0 root         (0) root         (0)     8976 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4928 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.py
--rw-rw-rw-   0 root         (0) root         (0)     6067 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Rashba_coupling.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Rashba_coupling.py
--rw-rw-rw-   0 root         (0) root         (0)     9414 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     6699 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.py
--rw-rw-rw-   0 root         (0) root         (0)   216639 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/dimerization_1D.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/dimerization_1D.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro1.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro1.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro2.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1834 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro2.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro3.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro3.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/periodic_cluster.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/periodic_cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     6472 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/superconductivity_VCA.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2237 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/superconductivity_VCA.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-03 21:29:54.000000 pyqcm-2.5.2/print_version.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyproject.toml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.629531 pyqcm-2.5.2/pyqcm/
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/Kolmogorov_Smirnov.py
--rwxrwxrwx   0 root         (0) root         (0)    90393 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16492 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/_draw.py
--rw-rw-rw-   0 root         (0) root         (0)    18556 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/_loop.py
--rwxrwxrwx   0 root         (0) root         (0)    73917 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/_spectral.py
--rw-rw-rw-   0 root         (0) root         (0)    56083 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/cdmft.py
--rw-rw-rw-   0 root         (0) root         (0)    19152 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/cdw.py
--rw-rw-rw-   0 root         (0) root         (0)     8979 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/dca.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/external.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm/qcm_git_hash.py
--rw-rw-rw-   0 root         (0) root         (0)     4314 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/slab.py
--rw-rw-rw-   0 root         (0) root         (0)     5806 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/variable_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)    39560 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/vca.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.629531 pyqcm-2.5.2/pyqcm.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2773 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8580 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-03 21:29:54.000000 pyqcm-2.5.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-03 21:30:03.641532 pyqcm-2.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-03 21:29:54.000000 pyqcm-2.5.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.629531 pyqcm-2.5.2/src_ed/
--rw-rw-rw-   0 root         (0) root         (0)     1288 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/.clang-format
--rw-rw-rw-   0 root         (0) root         (0)   108593 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    12658 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/ED_basis.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3338 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/ED_basis.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1134 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Green_function_set.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.633531 pyqcm-2.5.2/src_ed/Hamiltonian/
--rw-rw-rw-   0 root         (0) root         (0)     2473 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/CSR_hermitian.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6351 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Davidson.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3925 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_CSR.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5826 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Dense.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3826 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2558 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8025 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_base.hpp
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_ops.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1654 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12662 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.hpp
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/PRIMME_solver.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5263 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/PRIMME_solver.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.633531 pyqcm-2.5.2/src_ed/Operators/
--rw-rw-rw-   0 root         (0) root         (0)     4737 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_Heisenberg_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_Hermitian_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2230 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_Hund_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2073 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_anomalous_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4076 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_factorized_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2452 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_general_interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2640 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_half_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3816 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_nondiagonal_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2107 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_one_body_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1598 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2592 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3757 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Hermitian_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2485 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Hund_operator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Hund_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)    13374 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/anomalous_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/destruction_operator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1963 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/destruction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4497 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/general_interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)    16552 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/one_body_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8220 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Q_matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4798 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Q_matrix_set.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/binary_state.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2305 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/binary_state.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1854 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction.cpp
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5328 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction_set.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction_set.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/flex_array.hpp
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/fraction.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2034 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/index.hpp
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/index_pair.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1296 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/matrix_element.hpp
--rw-rw-rw-   0 root         (0) root         (0)     9564 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2667 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8222 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance.cpp
--rw-rw-rw-   0 root         (0) root         (0)    43555 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5566 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance_base.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3655 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance_base.hpp
--rw-rw-rw-   0 root         (0) root         (0)    13893 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/qcm_ED.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10059 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/qcm_ED.hpp
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/sector.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3979 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/sector.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/sparse_matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3017 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/state.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/symmetric_orbital.hpp
--rw-rw-rw-   0 root         (0) root         (0)    18543 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/symmetry_group.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5610 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/symmetry_group.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.633531 pyqcm-2.5.2/src_python/
--rw-rw-rw-   0 root         (0) root         (0)    12457 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/common_Py.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1395 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/common_Py.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5230 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_ED_lib.cpp
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_ED_only.hpp
--rw-rw-rw-   0 root         (0) root         (0)    37936 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_ED_wrap.hpp
--rw-rw-rw-   0 root         (0) root         (0)    11030 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_lib.cpp
--rwxrwxrwx   0 root         (0) root         (0)    79768 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_wrap.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/src_qcm/
--rwxrwxrwx   0 root         (0) root         (0)    12342 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/CPT.cpp
--rwxrwxrwx   0 root         (0) root         (0)    12499 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/Chern.cpp
--rwxrwxrwx   0 root         (0) root         (0)   108585 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/Doxyfile
--rwxrwxrwx   0 root         (0) root         (0)     1556 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/Green_function.hpp
--rwxrwxrwx   0 root         (0) root         (0)    32998 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/QCM.cpp
--rwxrwxrwx   0 root         (0) root         (0)     6294 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/QCM.hpp
--rwxrwxrwx   0 root         (0) root         (0)    16971 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/average.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3401 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/basis3D.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1033 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/basis3D.hpp
--rwxrwxrwx   0 root         (0) root         (0)     5745 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice3D.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1212 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice3D.hpp
--rwxrwxrwx   0 root         (0) root         (0)     2892 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_matrix_element.hpp
--rwxrwxrwx   0 root         (0) root         (0)    39191 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model.cpp
--rwxrwxrwx   0 root         (0) root         (0)     9353 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model.hpp
--rwxrwxrwx   0 root         (0) root         (0)    22767 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model_instance.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5941 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model_instance.hpp
--rwxrwxrwx   0 root         (0) root         (0)     8228 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_operator.cpp
--rwxrwxrwx   0 root         (0) root         (0)     2751 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)    16126 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/omp.h
--rwxrwxrwx   0 root         (0) root         (0)     6655 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/parameter_set.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1611 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/parameter_set.hpp
--rwxrwxrwx   0 root         (0) root         (0)    12256 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/print.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5341 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/profile.cpp
--rwxrwxrwx   0 root         (0) root         (0)     7224 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/vector3D.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/src_util/
--rw-rw-rw-   0 root         (0) root         (0)     9275 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/ED_global_parameter.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10036 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/VDVH_kernel.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1469 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/VDVH_kernel.hpp
--rw-rw-rw-   0 root         (0) root         (0)     7156 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/block_matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)    47325 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/cblas.h
--rw-rw-rw-   0 root         (0) root         (0)   263401 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/clapack.h
--rw-rw-rw-   0 root         (0) root         (0)    13424 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/f2c.h
--rwxrwxrwx   0 root         (0) root         (0)     6941 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/global_parameter.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2650 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/global_parameter.hpp
--rwxrwxrwx   0 root         (0) root         (0)    24433 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/integrate.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5770 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/integrate.hpp
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/lapack-blas.h
--rw-rw-rw-   0 root         (0) root         (0)     7187 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/matrix.cpp
--rw-rw-rw-   0 root         (0) root         (0)    20538 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/parser.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/parser.hpp
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/types.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4354 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/vector_num.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5978 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/vector_num.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_all.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/tests/test_diagonalization/
--rw-rw-rw-   0 root         (0) root         (0)    27349 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/S_format.ref
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/S_format_complex.ref
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/common.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/model_1D_8.py
--rw-rw-rw-   0 root         (0) root         (0)     1608 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution_complex.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.641532 pyqcm-2.5.2/tests/test_files/
--rw-rw-rw-   0 root         (0) root         (0)     1290 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2712 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_2_4b.py
--rwxrwxrwx   0 root         (0) root         (0)     1297 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_4.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_4_C2.py
--rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_2x2_C2.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_2x2_C2_vca.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_G4_6b_2C.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_WSM.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_graphene_bath.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_hartree.py
--rw-rw-rw-   0 root         (0) root         (0)     4846 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_2x2.py
--rw-rw-rw-   0 root         (0) root         (0)     8484 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_2x2_8b.py
--rw-rw-rw-   0 root         (0) root         (0)   108854 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_2x2_anom.py
--rw-rw-rw-   0 root         (0) root         (0)    19410 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_WSM.py
--rw-rw-rw-   0 root         (0) root         (0)   208082 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_WSM2.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_spin.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_2clusters.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_CF.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_averages.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_averages_bath.py
--rw-rw-rw-   0 root         (0) root         (0)     1995 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_berry.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_cdmft.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_cdmft_hartree.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_cluster_average.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_controlled_loop.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_fidelity.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_fixed_density_loop.py
--rw-rw-rw-   0 root         (0) root         (0)     1845 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_hartree.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_hybridization.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_instances.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_mixing.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_mixing2.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_mixing_cf.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_reset.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_spectral.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_varia.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_vca.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_vca_MPI.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_write.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.618808 pyqcm-2.5.4/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-31 15:43:41.000000 pyqcm-2.5.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-05-31 15:43:41.000000 pyqcm-2.5.4/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11765 2024-05-31 15:43:41.000000 pyqcm-2.5.4/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5088 2024-05-31 15:43:41.000000 pyqcm-2.5.4/INSTALL.md
+-rw-rw-rw-   0 root         (0) root         (0)    35216 2024-05-31 15:43:41.000000 pyqcm-2.5.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2024-05-31 15:43:58.618808 pyqcm-2.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2024-05-31 15:43:41.000000 pyqcm-2.5.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.582808 pyqcm-2.5.4/bench/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.586808 pyqcm-2.5.4/bench/ED/
+-rw-rw-rw-   0 root         (0) root         (0)      693 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/bench_ED.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/bench_ED2.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/bench_ED2_laptop.txt
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/bench_GS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/bench_GS2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/bench_GS_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/model_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/model_2D.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/ED/plot_bench_ED.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.586808 pyqcm-2.5.4/bench/integrals/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/integrals/plot_concurrent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/integrals/plot_integrals.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.586808 pyqcm-2.5.4/bench/integrals/small/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/integrals/small/integrals_small.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/integrals/small/integrals_small_concurrent.txt
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/integrals/small/integrals_small_results.txt
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/integrals/small/model_small.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.586808 pyqcm-2.5.4/bench/vca/
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/vca/bench_vca.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bench/vca/bench_vca2.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-31 15:43:41.000000 pyqcm-2.5.4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.586808 pyqcm-2.5.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      623 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)      134 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/makedoc
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.586808 pyqcm-2.5.4/docs/source/
+-rwxrwxrwx   0 root         (0) root         (0)     7924 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/2x2.png
+-rwxrwxrwx   0 root         (0) root         (0)    65032 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/T6.png
+-rwxrwxrwx   0 root         (0) root         (0)      917 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/cdmft.rst
+-rwxrwxrwx   0 root         (0) root         (0)     5631 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/defining_cluster_models.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9560 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/defining_models.rst
+-rwxrwxrwx   0 root         (0) root         (0)    37228 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/h4-6b.png
+-rwxrwxrwx   0 root         (0) root         (0)     1265 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/h8.asy
+-rw-rw-rw-   0 root         (0) root         (0)    57104 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/h8.png
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/hartree.rst
+-rwxrwxrwx   0 root         (0) root         (0)    66076 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/hexa6.png
+-rwxrwxrwx   0 root         (0) root         (0)      579 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/index.rst
+-rwxrwxrwx   0 root         (0) root         (0)     5217 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/intro.rst
+-rwxrwxrwx   0 root         (0) root         (0)    18237 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/models.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6033 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/options.rst
+-rwxrwxrwx   0 root         (0) root         (0)      782 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/options_intro.txt
+-rwxrwxrwx   0 root         (0) root         (0)      236 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/other_functions.rst
+-rwxrwxrwx   0 root         (0) root         (0)     6231 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/parallel.rst
+-rw-rw-rw-   0 root         (0) root         (0)    23261 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/parallel_performance_concurrent.png
+-rw-rw-rw-   0 root         (0) root         (0)    23202 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/parallel_performance_ed.png
+-rw-rw-rw-   0 root         (0) root         (0)    34896 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/parallel_performance_integrals.png
+-rwxrwxrwx   0 root         (0) root         (0)     8130 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/parameters.rst
+-rw-rw-rw-   0 root         (0) root         (0)    43029 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/t15.png
+-rwxrwxrwx   0 root         (0) root         (0)      535 2024-05-31 15:43:41.000000 pyqcm-2.5.4/docs/source/vca.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.582808 pyqcm-2.5.4/examples/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.590808 pyqcm-2.5.4/examples/1D_2_4b/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/QCM_params.def
+-rw-rw-rw-   0 root         (0) root         (0)   116475 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/averages.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    37866 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/cdmft.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/cdmft_distance.tsv
+-rw-rw-rw-   0 root         (0) root         (0)   114242 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/cdmft_grid.tsv
+-rw-rw-rw-   0 root         (0) root         (0)   548325 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/cdmft_iter.tsv
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/debug_complex.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/debug_dvmc.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/debug_variable_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)    20439 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/dos.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    17095 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/h1.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    35032 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/h2.pdf
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/hop.npy
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/hopping.def
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/interaction.def
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/interaction.npy
+-rwxrwxrwx   0 root         (0) root         (0)     2491 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/model_1D_2_4b.py
+-rw-rw-rw-   0 root         (0) root         (0)    10812 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/out
+-rw-rw-rw-   0 root         (0) root         (0)    20251 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/s1.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    21433 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_2_4b/s2.pdf
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.594808 pyqcm-2.5.4/examples/1D_4/
+-rw-rw-rw-   0 root         (0) root         (0)     3185 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/GS.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    18259 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/ave.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    18259 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/averages.tsv
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/debug_cdw.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/debug_dvmc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/debug_rhoAB.py
+-rw-rw-rw-   0 root         (0) root         (0)    11556 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/hartree.tsv
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/model_1D_4.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/model_1D_4_C2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/record.py
+-rw-rw-rw-   0 root         (0) root         (0)  1077770 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/sef.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    29277 2024-05-31 15:43:41.000000 pyqcm-2.5.4/examples/1D_4/vca.tsv
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.594808 pyqcm-2.5.4/external/
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2024-05-31 15:43:41.000000 pyqcm-2.5.4/external/FindAVX2.cmake
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.594808 pyqcm-2.5.4/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)    21298 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/AF_VCA_vs_L.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/AF_VCA_vs_L.py
+-rw-rw-rw-   0 root         (0) root         (0)   188540 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/CDW_1D.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4051 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/CDW_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     9942 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/Mott_Weyl.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4186 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/Mott_Weyl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8976 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/Mott_transition_graphene_CDMFT.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4928 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/Mott_transition_graphene_CDMFT.py
+-rw-rw-rw-   0 root         (0) root         (0)     6067 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/Rashba_coupling.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/Rashba_coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)     9414 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/antiferromagnetism_VCA.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6699 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/antiferromagnetism_VCA.py
+-rw-rw-rw-   0 root         (0) root         (0)   216639 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/dimerization_1D.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/dimerization_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/intro1.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/intro1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/intro2.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/intro2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/intro3.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/intro3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/periodic_cluster.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/periodic_cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     6472 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/superconductivity_VCA.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2237 2024-05-31 15:43:41.000000 pyqcm-2.5.4/notebooks/superconductivity_VCA.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-05-31 15:43:41.000000 pyqcm-2.5.4/print_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyproject.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.598808 pyqcm-2.5.4/pyqcm/
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/Kolmogorov_Smirnov.py
+-rwxrwxrwx   0 root         (0) root         (0)    90393 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16492 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/_draw.py
+-rw-rw-rw-   0 root         (0) root         (0)    18556 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/_loop.py
+-rwxrwxrwx   0 root         (0) root         (0)    73989 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/_spectral.py
+-rw-rw-rw-   0 root         (0) root         (0)    56399 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/cdmft.py
+-rw-rw-rw-   0 root         (0) root         (0)    19152 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/cdw.py
+-rw-rw-rw-   0 root         (0) root         (0)     8979 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/dca.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/external.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-31 15:43:58.000000 pyqcm-2.5.4/pyqcm/qcm_git_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     4314 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/slab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5806 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/variable_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)    39560 2024-05-31 15:43:41.000000 pyqcm-2.5.4/pyqcm/vca.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.598808 pyqcm-2.5.4/pyqcm.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2024-05-31 15:43:58.000000 pyqcm-2.5.4/pyqcm.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2024-05-31 15:43:58.000000 pyqcm-2.5.4/pyqcm.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-31 15:43:58.000000 pyqcm-2.5.4/pyqcm.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-31 15:43:58.000000 pyqcm-2.5.4/pyqcm.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-31 15:43:58.000000 pyqcm-2.5.4/pyqcm.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-31 15:43:41.000000 pyqcm-2.5.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-31 15:43:58.618808 pyqcm-2.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-05-31 15:43:41.000000 pyqcm-2.5.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.602808 pyqcm-2.5.4/src_ed/
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/.clang-format
+-rw-rw-rw-   0 root         (0) root         (0)   108593 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    12658 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/ED_basis.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/ED_basis.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Green_function_set.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.602808 pyqcm-2.5.4/src_ed/Hamiltonian/
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/CSR_hermitian.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Davidson.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_CSR.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Dense.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     8025 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_base.hpp
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_ops.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Lanczos.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    12662 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/Lanczos.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/PRIMME_solver.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Hamiltonian/PRIMME_solver.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.606808 pyqcm-2.5.4/src_ed/Operators/
+-rw-rw-rw-   0 root         (0) root         (0)     4737 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_Heisenberg_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_Hermitian_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_Hund_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_anomalous_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_factorized_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_general_interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_half_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3816 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_nondiagonal_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_one_body_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/HS_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2592 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/Heisenberg_operator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/Heisenberg_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/Hermitian_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/Hund_operator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/Hund_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    13374 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/anomalous_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/destruction_operator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/destruction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4497 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/general_interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    16552 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Operators/one_body_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     8220 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Q_matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/Q_matrix_set.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/binary_state.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/binary_state.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/continued_fraction.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/continued_fraction.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5328 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/continued_fraction_set.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/continued_fraction_set.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/flex_array.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/fraction.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/index.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/index_pair.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/matrix_element.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     9564 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/model.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/model.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     8222 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/model_instance.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    43555 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/model_instance.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/model_instance_base.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/model_instance_base.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    13893 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/qcm_ED.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/qcm_ED.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/sector.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/sector.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/sparse_matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/state.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/symmetric_orbital.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    18543 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/symmetry_group.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5610 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_ed/symmetry_group.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.606808 pyqcm-2.5.4/src_python/
+-rw-rw-rw-   0 root         (0) root         (0)    12457 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/common_Py.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/common_Py.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5230 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/qcm_ED_lib.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/qcm_ED_only.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    37936 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/qcm_ED_wrap.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    11030 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/qcm_lib.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    79768 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_python/qcm_wrap.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.610808 pyqcm-2.5.4/src_qcm/
+-rwxrwxrwx   0 root         (0) root         (0)    12342 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/CPT.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    12499 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/Chern.cpp
+-rwxrwxrwx   0 root         (0) root         (0)   108585 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/Doxyfile
+-rwxrwxrwx   0 root         (0) root         (0)     1556 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/Green_function.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    32998 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/QCM.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     6294 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/QCM.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    16971 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/average.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3401 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/basis3D.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1033 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/basis3D.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     5745 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice3D.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1212 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice3D.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     2892 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_matrix_element.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    39191 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_model.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     9353 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_model.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    22767 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_model_instance.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     5941 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_model_instance.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     8228 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_operator.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     2751 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/lattice_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    16126 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/omp.h
+-rwxrwxrwx   0 root         (0) root         (0)     6655 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/parameter_set.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1611 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/parameter_set.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    12256 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/print.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     5341 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/profile.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_qcm/vector3D.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.610808 pyqcm-2.5.4/src_util/
+-rw-rw-rw-   0 root         (0) root         (0)     9275 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/ED_global_parameter.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    10036 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/VDVH_kernel.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/VDVH_kernel.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     7156 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/block_matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/cblas.h
+-rw-rw-rw-   0 root         (0) root         (0)   263401 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/clapack.h
+-rw-rw-rw-   0 root         (0) root         (0)    13424 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/f2c.h
+-rwxrwxrwx   0 root         (0) root         (0)     6941 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/global_parameter.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/global_parameter.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    24433 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/integrate.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     5770 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/integrate.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/lapack-blas.h
+-rw-rw-rw-   0 root         (0) root         (0)     7401 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/matrix.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    20538 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6696 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/parser.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/parser.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/types.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/vector_num.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5978 2024-05-31 15:43:41.000000 pyqcm-2.5.4/src_util/vector_num.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.610808 pyqcm-2.5.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_all.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.614808 pyqcm-2.5.4/tests/test_diagonalization/
+-rw-rw-rw-   0 root         (0) root         (0)    27349 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/S_format.ref
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/S_format_complex.ref
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/model_1D_8.py
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/test_pole_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_diagonalization/test_pole_distribution_complex.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-31 15:43:58.618808 pyqcm-2.5.4/tests/test_files/
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_1D_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_1D_2_4b.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_1D_4.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_1D_4_C2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_2x2_C2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_2x2_C2_vca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_G4_6b_2C.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_WSM.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_graphene_bath.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/model_hartree.py
+-rw-rw-rw-   0 root         (0) root         (0)     4846 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/record_2x2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/record_2x2_8b.py
+-rw-rw-rw-   0 root         (0) root         (0)   108854 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/record_2x2_anom.py
+-rw-rw-rw-   0 root         (0) root         (0)    19410 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/record_WSM.py
+-rw-rw-rw-   0 root         (0) root         (0)   208082 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/record_WSM2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/record_spin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_2clusters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_CF.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_averages.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_averages_bath.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_berry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_cdmft.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_cdmft_hartree.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_cluster_average.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_controlled_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_fidelity.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_fixed_density_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1845 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_hartree.py
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_hybridization.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_instances.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_mixing.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_mixing2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_mixing_cf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_reset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_spectral.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_varia.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_vca.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_vca_MPI.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-31 15:43:41.000000 pyqcm-2.5.4/tests/test_files/test_write.py
```

### Comparing `pyqcm-2.5.2/CMakeLists.txt` & `pyqcm-2.5.4/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -247,21 +247,24 @@
 # Optimized kernel for Green function evaluation
 #-----------------------------------------------
 if (GENERIC_BUILD)
   set( WITH_GF_OPT_KERNEL OFF)
   message(WARNING "Generic build cannot use AVX2 optimized kernel for Green function evaluation. Setting WITH_GF_OPT_KERNEL to false")
 endif()
 if (WITH_GF_OPT_KERNEL)
-  set( CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/external" ${CMAKE_MODULE_PATH} )
-  include(FindAVX2)
-  if (AVX2_FOUND)
-    add_compile_definitions(HAVE_AVX2)
+  if(APPLE)
   else()
-    message(WARNING "WITH_GF_KERNEL specified but the host processor does not have AVX2 capability: optimized kernel will not be used.")
-    set(AVX2_FOUND false)
+    set( CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/external" ${CMAKE_MODULE_PATH} )
+    include(FindAVX2)
+    if (AVX2_FOUND)
+      add_compile_definitions(HAVE_AVX2)
+    else()
+      message(WARNING "WITH_GF_KERNEL specified but the host processor does not have AVX2 capability: optimized kernel will not be used.")
+      set(AVX2_FOUND false)
+    endif()
   endif()
   message(STATUS "Using AVX2 optimized kernel for Green function evaluation: ${AVX2_FOUND}")
 endif()
 
 
 #------------------
 # Parallelization using OpenMP
```

### Comparing `pyqcm-2.5.2/INSTALL.md` & `pyqcm-2.5.4/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/LICENSE` & `pyqcm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/PKG-INFO` & `pyqcm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqcm
-Version: 2.5.2
+Version: 2.5.4
 Summary: Quantum cluster methods for the physics of strongly correlated systems
 Home-page: https://bitbucket.org/dsenechQCM/qcm_wed/
 Author: David Sénéchal
 License: GPL
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyqcm-2.5.2/README.md` & `pyqcm-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/bench_ED.py` & `pyqcm-2.5.4/bench/ED/bench_ED.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/bench_ED2.py` & `pyqcm-2.5.4/bench/ED/bench_ED2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/bench_GS.py` & `pyqcm-2.5.4/bench/ED/bench_GS.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/bench_GS2.py` & `pyqcm-2.5.4/bench/ED/bench_GS2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/bench_GS_loop.py` & `pyqcm-2.5.4/bench/ED/bench_GS_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/model_1D.py` & `pyqcm-2.5.4/bench/ED/model_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/model_2D.py` & `pyqcm-2.5.4/bench/ED/model_2D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/ED/plot_bench_ED.py` & `pyqcm-2.5.4/bench/ED/plot_bench_ED.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/integrals/plot_concurrent.py` & `pyqcm-2.5.4/bench/integrals/plot_concurrent.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/integrals/plot_integrals.py` & `pyqcm-2.5.4/bench/integrals/plot_integrals.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/integrals/small/model_small.py` & `pyqcm-2.5.4/bench/integrals/small/model_small.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/vca/bench_vca.py` & `pyqcm-2.5.4/bench/vca/bench_vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/bench/vca/bench_vca2.py` & `pyqcm-2.5.4/bench/vca/bench_vca2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/Makefile` & `pyqcm-2.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/2x2.png` & `pyqcm-2.5.4/docs/source/2x2.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/T6.png` & `pyqcm-2.5.4/docs/source/T6.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/cdmft.rst` & `pyqcm-2.5.4/docs/source/cdmft.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/conf.py` & `pyqcm-2.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/defining_cluster_models.rst` & `pyqcm-2.5.4/docs/source/defining_cluster_models.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/defining_models.rst` & `pyqcm-2.5.4/docs/source/defining_models.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/h4-6b.png` & `pyqcm-2.5.4/docs/source/h4-6b.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/h8.asy` & `pyqcm-2.5.4/docs/source/h8.asy`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/h8.png` & `pyqcm-2.5.4/docs/source/h8.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/hartree.rst` & `pyqcm-2.5.4/docs/source/hartree.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/hexa6.png` & `pyqcm-2.5.4/docs/source/hexa6.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/index.rst` & `pyqcm-2.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/intro.rst` & `pyqcm-2.5.4/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/models.rst` & `pyqcm-2.5.4/docs/source/models.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/options.rst` & `pyqcm-2.5.4/docs/source/options.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/options_intro.txt` & `pyqcm-2.5.4/docs/source/options_intro.txt`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/parallel.rst` & `pyqcm-2.5.4/docs/source/parallel.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/parallel_performance_concurrent.png` & `pyqcm-2.5.4/docs/source/parallel_performance_concurrent.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/parallel_performance_ed.png` & `pyqcm-2.5.4/docs/source/parallel_performance_ed.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/parallel_performance_integrals.png` & `pyqcm-2.5.4/docs/source/parallel_performance_integrals.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/parameters.rst` & `pyqcm-2.5.4/docs/source/parameters.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/t15.png` & `pyqcm-2.5.4/docs/source/t15.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/docs/source/vca.rst` & `pyqcm-2.5.4/docs/source/vca.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/averages.tsv` & `pyqcm-2.5.4/examples/1D_2_4b/averages.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/cdmft.tsv` & `pyqcm-2.5.4/examples/1D_2_4b/cdmft.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/cdmft_distance.tsv` & `pyqcm-2.5.4/examples/1D_2_4b/cdmft_distance.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/cdmft_grid.tsv` & `pyqcm-2.5.4/examples/1D_2_4b/cdmft_grid.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/cdmft_iter.tsv` & `pyqcm-2.5.4/examples/1D_2_4b/cdmft_iter.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/debug.py` & `pyqcm-2.5.4/examples/1D_2_4b/debug.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/debug_complex.py` & `pyqcm-2.5.4/examples/1D_2_4b/debug_complex.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/debug_dvmc.py` & `pyqcm-2.5.4/examples/1D_2_4b/debug_dvmc.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/debug_variable_parameter.py` & `pyqcm-2.5.4/examples/1D_2_4b/debug_variable_parameter.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/dos.tsv` & `pyqcm-2.5.4/examples/1D_2_4b/dos.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/h1.pdf` & `pyqcm-2.5.4/examples/1D_2_4b/h1.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/h2.pdf` & `pyqcm-2.5.4/examples/1D_2_4b/h2.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/hop.npy` & `pyqcm-2.5.4/examples/1D_2_4b/hop.npy`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/model_1D_2_4b.py` & `pyqcm-2.5.4/examples/1D_2_4b/model_1D_2_4b.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/out` & `pyqcm-2.5.4/examples/1D_2_4b/out`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/s1.pdf` & `pyqcm-2.5.4/examples/1D_2_4b/s1.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_2_4b/s2.pdf` & `pyqcm-2.5.4/examples/1D_2_4b/s2.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/GS.tsv` & `pyqcm-2.5.4/examples/1D_4/GS.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/ave.tsv` & `pyqcm-2.5.4/examples/1D_4/ave.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/averages.tsv` & `pyqcm-2.5.4/examples/1D_4/averages.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/debug_cdw.py` & `pyqcm-2.5.4/examples/1D_4/debug_cdw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/debug_rhoAB.py` & `pyqcm-2.5.4/examples/1D_4/debug_rhoAB.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/hartree.tsv` & `pyqcm-2.5.4/examples/1D_4/hartree.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/model_1D_4.py` & `pyqcm-2.5.4/examples/1D_4/model_1D_4.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/record.py` & `pyqcm-2.5.4/examples/1D_4/record.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/sef.tsv` & `pyqcm-2.5.4/examples/1D_4/sef.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/examples/1D_4/vca.tsv` & `pyqcm-2.5.4/examples/1D_4/vca.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/external/FindAVX2.cmake` & `pyqcm-2.5.4/external/FindAVX2.cmake`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/AF_VCA_vs_L.ipynb` & `pyqcm-2.5.4/notebooks/AF_VCA_vs_L.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/AF_VCA_vs_L.py` & `pyqcm-2.5.4/notebooks/AF_VCA_vs_L.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/CDW_1D.ipynb` & `pyqcm-2.5.4/notebooks/CDW_1D.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/CDW_1D.py` & `pyqcm-2.5.4/notebooks/CDW_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/Mott_Weyl.ipynb` & `pyqcm-2.5.4/notebooks/Mott_Weyl.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/Mott_Weyl.py` & `pyqcm-2.5.4/notebooks/Mott_Weyl.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.ipynb` & `pyqcm-2.5.4/notebooks/Mott_transition_graphene_CDMFT.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.py` & `pyqcm-2.5.4/notebooks/Mott_transition_graphene_CDMFT.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/Rashba_coupling.ipynb` & `pyqcm-2.5.4/notebooks/Rashba_coupling.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/Rashba_coupling.py` & `pyqcm-2.5.4/notebooks/Rashba_coupling.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.ipynb` & `pyqcm-2.5.4/notebooks/antiferromagnetism_VCA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.py` & `pyqcm-2.5.4/notebooks/antiferromagnetism_VCA.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/dimerization_1D.ipynb` & `pyqcm-2.5.4/notebooks/dimerization_1D.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/dimerization_1D.py` & `pyqcm-2.5.4/notebooks/dimerization_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/intro1.ipynb` & `pyqcm-2.5.4/notebooks/intro1.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/intro1.py` & `pyqcm-2.5.4/notebooks/intro1.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/intro2.ipynb` & `pyqcm-2.5.4/notebooks/intro2.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/intro2.py` & `pyqcm-2.5.4/notebooks/intro2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/intro3.ipynb` & `pyqcm-2.5.4/notebooks/intro3.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/intro3.py` & `pyqcm-2.5.4/notebooks/intro3.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/periodic_cluster.ipynb` & `pyqcm-2.5.4/notebooks/periodic_cluster.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/periodic_cluster.py` & `pyqcm-2.5.4/notebooks/periodic_cluster.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/superconductivity_VCA.ipynb` & `pyqcm-2.5.4/notebooks/superconductivity_VCA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/notebooks/superconductivity_VCA.py` & `pyqcm-2.5.4/notebooks/superconductivity_VCA.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/Kolmogorov_Smirnov.py` & `pyqcm-2.5.4/pyqcm/Kolmogorov_Smirnov.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/__init__.py` & `pyqcm-2.5.4/pyqcm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/_draw.py` & `pyqcm-2.5.4/pyqcm/_draw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/_loop.py` & `pyqcm-2.5.4/pyqcm/_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/_spectral.py` & `pyqcm-2.5.4/pyqcm/_spectral.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         if threeD:
             ax.plot(np.real(w), A[:, j], 'k-', lw=0.5, zdir='y', zs = offset * j, **kwargs)
         else:
             if plot_down:
                 ax.plot(np.real(w), A_down[:, j] + offset * j, 'r-', lw=0.5, **kwargs)
             ax.plot(np.real(w), A[:, j] + offset * j, 'b-', lw=0.5, **kwargs)
     if title is None and plt_ax is None:
-        ax.set_title(r'$A(\mathbf{k},\omega)$: '+self.model.parameter_string(), fontsize=6)
+        ax.set_title(r'$A(\mathbf{k},\omega)$: '+self.model.parameter_string(clus=0), fontsize=6)
     else:
         ax.set_title(title, fontsize=6)
     if threeD:
         ax.set_ylim(0, (1+len(k))* offset)
         ax.set_zlim(0, 2*np.max(A))
         ax.xaxis.pane.fill = False
         ax.yaxis.pane.fill = False
@@ -268,15 +268,15 @@
         ax.set_xlim(np.real(w[0]), np.real(w[-1]))
         for j in range(d*d):
             ax.plot(np.real(w), A[:, j] + offset * j, 'b-', lw=0.5, **kwargs)
     ax.axvline(0, c='r', ls='solid', lw=0.5)
     if plt_ax is None:
         plt.xlabel(r'$\omega$')
         plt.ylabel(r'$\Gamma(\omega)$')
-        plt.title(r'$\Gamma(\omega)$: '+self.model.parameter_string())
+        plt.title(r'$\Gamma(\omega)$: '+self.model.parameter_string(clus=0))
 
     if file is not None:
         plt.savefig(file)
         plt.close()
     elif plt_ax is None:
         plt.show()
 
@@ -354,15 +354,15 @@
     else:
         ax.set_xlim(np.real(w[0]), np.real(w[-1]))
         for j in range(dd):
             plt.plot(np.real(w), A[:, j] + offset * j, '-', lw=0.5, color=color, **kwargs)
 
     plt.xlabel(r'$\omega$')
     plt.axvline(0, ls='solid', lw=0.5)
-    plt.title(self.model.parameter_string(), fontsize=6)
+    plt.title(self.model.parameter_string(clus=0), fontsize=6)
 
     if file is not None:
         plt.savefig(file)
         plt.close()
     elif plt_ax is None:
         plt.show()
 
@@ -396,15 +396,15 @@
 
     k, tick_pos, tick_str = pyqcm.wavevector_path(nk, path)  # defines the array of wavevectors
 
     assert (orb <= self.model.nband and orb > 0), 'The orbital index in spectral_function_Lehmann() must vary from 1 to {:d}'.format(self.model.nband)
 
     if lims is not None:
         plt.xlim(lims[0], lims[1])
-    plt.title(self.model.parameter_string(), fontsize=6)
+    plt.title(self.model.parameter_string(clus=0), fontsize=6)
     plt.yticks(offset * tick_pos, tick_str)
     G = self.Lehmann_Green_function(k, orb)
     for i in range(len(k)):
         plt.vlines(G[i][0], i*offset, G[i][1]+i*offset, lw=0.8, color='b')
         plt.axhline(i*offset, lw=0.25, color='grey')
 
     plt.xlabel(r'$\omega$')
@@ -820,15 +820,15 @@
     :return: None
     
     """
     if plt_ax is None:
         plt.figure()
         plt.gcf().set_size_inches(14/2.54, 14/2.54)
         ax = plt.gca()
-        plt.title('anomalous mdc: '+self.model.parameter_string(), fontsize=6)
+        plt.title('anomalous mdc: '+self.model.parameter_string(clus=0), fontsize=6)
     else:
         ax = plt_ax
     ax.set_aspect(1)
 
     mix = self.model.mixing
     assert (mix == 1 or mix == 3), 'The system is not anomalous! Abort mdc_anomalous().'
 
@@ -936,15 +936,15 @@
     else:
         x, y = np.meshgrid(x, x)
         for j in orbs:
             ax.plot_surface(x, y, e[:, :, j], rstride=1,cstride=1, linewidth=0.2, antialiased=False, **kwargs)
             
     if plt_ax is None:
         axis = _set_legend_mdc(plane, k_perp)
-        plt.title(axis+' '+self.model.parameter_string(), fontsize=6)
+        plt.title(axis+' '+self.model.parameter_string(clus=0), fontsize=6)
 
     if file is not None:
         plt.savefig(file)
         plt.close()
     elif plt_ax is None:
         plt.show()
 
@@ -962,15 +962,15 @@
 
     """
     
     if plt_ax is None:
         plt.figure()
         plt.gcf().set_size_inches(14/2.54, 14/2.54)
         ax = plt.gca()
-        plt.title(self.model.parameter_string(), fontsize=6)
+        plt.title(self.model.parameter_string(clus=0), fontsize=6)
     else:
         ax = plt_ax
 
     k, tick_pos, tick_str = pyqcm.wavevector_path(nk, path)  # defines the array of wavevectors
     d = self.model.dimGF_red
     e = self.dispersion(k)
 
@@ -1033,15 +1033,15 @@
     e.shape = (nk, nk, d)
 
     for j in orbs:
         plt.contour(x, x, e[:, :, j], levels=[0.0], **kwargs)
 
     if plt_ax is None:
         axis = _set_legend_mdc('xy', 0.0)
-        plt.title('Fermi surface: '+axis+' '+self.model.parameter_string(), fontsize=6)
+        plt.title('Fermi surface: '+axis+' '+self.model.parameter_string(clus=0), fontsize=6)
     
     if file is not None:
         plt.savefig(file)
         plt.close()
     elif plt_ax is None:
         plt.show()
 
@@ -1071,15 +1071,15 @@
         plt.figure()
         plt.gcf().set_size_inches(14/2.54, 14/2.54)
         if contour:
             ax = plt.gca()
             plt.gca().set_aspect(1)
         else:
             ax = plt.axes(projection='3d')
-        plt.title('G dispersion: '+self.model.parameter_string(), fontsize=6)
+        plt.title('G dispersion: '+self.model.parameter_string(clus=0), fontsize=6)
     else:
         ax = plt_ax
 
     freq = 0.1j
 
     k, x = __kgrid(ax, nk, quadrant=quadrant, k_perp=k_perp, plane=plane)
 
@@ -1149,15 +1149,15 @@
 
     """
 
     if plt_ax is None:
         plt.figure()
         plt.gcf().set_size_inches(14/2.54, 14/2.54)
         ax = plt.gca()
-        plt.title('Luttinger surface : '+self.model.parameter_string(), fontsize=6)
+        plt.title('Luttinger surface : '+self.model.parameter_string(clus=0), fontsize=6)
     else:
         ax = plt_ax
     ax.set_aspect(1)
 
     k, x = __kgrid(ax, nk, quadrant=quadrant, k_perp=k_perp, plane=plane)
     
     g = self.periodized_Green_function(0.0, k)
@@ -1191,15 +1191,15 @@
     
     """
 
     if plt_ax is None:
         plt.figure()
         plt.gcf().set_size_inches(14/2.54, 14/2.54)
         ax = plt.gca()
-        plt.title('profile of '+op+' : '+self.model.parameter_string(), fontsize=6)
+        plt.title('profile of '+op+' : '+self.model.parameter_string(clus=0), fontsize=6)
     else:
         ax = plt_ax
     ax.set_aspect(1)
 
     k, x = __kgrid(ax, nk, quadrant=quadrant, k_perp=k_perp, plane=plane)
 
     # reserves space for the average
@@ -1825,14 +1825,14 @@
         if np.sqrt(sx*sx+sz*sz) > 0.01 :
             ax.add_patch(patches.Arrow(x-0.5*sx, y-0.5*sz, sx, sz, width=0.2, fc = 'blue', ec = 'black', lw = 0.5, zorder=100))
         sx = spinI[0]
         sz = spinI[1]
         if np.sqrt(sx*sx+sz*sz) > 0.01 :
             ax.add_patch(patches.Arrow(x-0.5*sx, y-0.5*sz, sx, sz, width=0.2, fc = 'red', ec = 'black', lw = 0.5, zorder=100))
 
-    plt.gcf().suptitle(self.model.parameter_string()+', layer '+str(layer), y=1.0, fontsize=6)
+    plt.gcf().suptitle(self.model.parameter_string(clus=0)+', layer '+str(layer), y=1.0, fontsize=6)
     plt.tight_layout()
 
     if file is None:
         plt.show()
     else:
         plt.savefig(file)
```

### Comparing `pyqcm-2.5.2/pyqcm/cdmft.py` & `pyqcm-2.5.4/pyqcm/cdmft.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     :param boolean check_ground_state: if True, checks the ground state consistency and raises exception if inconsistent
     :param int max_function_eval: maximum number of distance function evaluations when minimizing distance
     :param boolean compute_potential_energy: If True, computes Tr(Sigma*G) along with the averages
     :param ndarray host_function: if not None, function that computes the host array and passes it to qcm
     :param function pre_host: function to be executed before computing the host. Takes a model instance as argument
     :param float max_value: maximum absolute value of variational parameters
     :param boolean fallback: if True, falls back to the other iteration method (Broyden or fixed_point) if the current one fails
+    :param boolean cap: if True, caps variational parameters to the maximum to a magnitude of max_value
     :ivar lattice_model model: (unique) model on which the computation is based
     :ivar ndarray Hyb: host function
     :ivar ndarray Hyb_down: host function for the spin down component in the case of mixing=4
     :ivar I: current model instance (changes in the course of the computation)
     
     """
 
@@ -172,15 +173,16 @@
         SEF=False,
         check_ground_state = False,
         max_function_eval = 500000,
         compute_potential_energy = False,
         host_function = None,
         pre_host = None,
         max_value = 100,
-        fallback=False
+        fallback=False,
+        cap = False
     ):
 
         self.model =model
         self.Hyb = None # internal : hybridization function
         self.Hyb_down = None # internal : hybridization function (spin downs, when mixing=4)
         self.sigma = None # internal : self-energy
         self.sigma_down = None # internal : self-energy (spin downs, when mixing=4)
@@ -193,14 +195,15 @@
         self.method = method
         self.initial_step = initial_step
         self.accur_bath = accur_bath
         self.accur_dist = accur_dist
         self.max_function_eval = max_function_eval
         self.max_value = max_value
         self.alpha = alpha
+        self.cap = cap
 
         if pyqcm.is_sequence(accur) == False:
             accur = (accur,)
 
         if pyqcm.is_sequence(hartree) == False and hartree is not None:
             hartree = (hartree,)
         else: hartree = hartree
@@ -428,14 +431,18 @@
             print(sol)
             pyqcm.banner('NaN found in optimization of bath parameters', '!')
             raise pyqcm.MinimizationError('NaN found in optimization of bath parameters')
 
         # push back into array
         x_new[0:self.nvar] = np.copy(sol.x)
         
+        if self.cap :
+            for i in range(self.nvar):
+                if np.abs(x_new[i]) > self.max_value: x_new[i] = np.sign(x_new[i])*self.max_value*0.99999
+
         try:
             check_bounds(x_new[0:self.nvar], self.max_value, v=self.var)
         except pyqcm.OutOfBoundsError as error:
             raise error
         except:
             raise ValueError
```

### Comparing `pyqcm-2.5.2/pyqcm/cdw.py` & `pyqcm-2.5.4/pyqcm/cdw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/dca.py` & `pyqcm-2.5.4/pyqcm/dca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/external.py` & `pyqcm-2.5.4/pyqcm/external.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/slab.py` & `pyqcm-2.5.4/pyqcm/slab.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/variable_parameter.py` & `pyqcm-2.5.4/pyqcm/variable_parameter.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm/vca.py` & `pyqcm-2.5.4/pyqcm/vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/pyqcm.egg-info/PKG-INFO` & `pyqcm-2.5.4/pyqcm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqcm
-Version: 2.5.2
+Version: 2.5.4
 Summary: Quantum cluster methods for the physics of strongly correlated systems
 Home-page: https://bitbucket.org/dsenechQCM/qcm_wed/
 Author: David Sénéchal
 License: GPL
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyqcm-2.5.2/pyqcm.egg-info/SOURCES.txt` & `pyqcm-2.5.4/pyqcm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/setup.py` & `pyqcm-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/.clang-format` & `pyqcm-2.5.4/src_ed/.clang-format`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Doxyfile` & `pyqcm-2.5.4/src_ed/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/ED_basis.cpp` & `pyqcm-2.5.4/src_ed/ED_basis.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/ED_basis.hpp` & `pyqcm-2.5.4/src_ed/ED_basis.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Green_function_set.hpp` & `pyqcm-2.5.4/src_ed/Green_function_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/CSR_hermitian.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/CSR_hermitian.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Davidson.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Davidson.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_CSR.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_CSR.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Dense.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Dense.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Operator.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_Operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_base.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Hamiltonian_base.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.cpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Lanczos.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/Lanczos.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Hamiltonian/PRIMME_solver.hpp` & `pyqcm-2.5.4/src_ed/Hamiltonian/PRIMME_solver.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_Heisenberg_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_Heisenberg_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_Hermitian_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_Hermitian_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_Hund_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_Hund_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_anomalous_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_anomalous_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_factorized_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_factorized_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_general_interaction_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_general_interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_half_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_half_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_interaction_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_nondiagonal_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_nondiagonal_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_one_body_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_one_body_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/HS_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/HS_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.cpp` & `pyqcm-2.5.4/src_ed/Operators/Heisenberg_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/Heisenberg_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/Hermitian_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/Hermitian_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/Hund_operator.cpp` & `pyqcm-2.5.4/src_ed/Operators/Hund_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/Hund_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/Hund_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/anomalous_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/anomalous_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/destruction_operator.cpp` & `pyqcm-2.5.4/src_ed/Operators/destruction_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/destruction_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/destruction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/general_interaction_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/general_interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/interaction_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Operators/one_body_operator.hpp` & `pyqcm-2.5.4/src_ed/Operators/one_body_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Q_matrix.hpp` & `pyqcm-2.5.4/src_ed/Q_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/Q_matrix_set.hpp` & `pyqcm-2.5.4/src_ed/Q_matrix_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/binary_state.cpp` & `pyqcm-2.5.4/src_ed/binary_state.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/binary_state.hpp` & `pyqcm-2.5.4/src_ed/binary_state.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/continued_fraction.cpp` & `pyqcm-2.5.4/src_ed/continued_fraction.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/continued_fraction.hpp` & `pyqcm-2.5.4/src_ed/continued_fraction.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/continued_fraction_set.cpp` & `pyqcm-2.5.4/src_ed/continued_fraction_set.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/continued_fraction_set.hpp` & `pyqcm-2.5.4/src_ed/continued_fraction_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/flex_array.hpp` & `pyqcm-2.5.4/src_ed/flex_array.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/fraction.hpp` & `pyqcm-2.5.4/src_ed/fraction.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/index.hpp` & `pyqcm-2.5.4/src_ed/index.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/index_pair.hpp` & `pyqcm-2.5.4/src_ed/index_pair.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/matrix_element.hpp` & `pyqcm-2.5.4/src_ed/matrix_element.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/model.cpp` & `pyqcm-2.5.4/src_ed/model.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/model.hpp` & `pyqcm-2.5.4/src_ed/model.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/model_instance.cpp` & `pyqcm-2.5.4/src_ed/model_instance.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/model_instance.hpp` & `pyqcm-2.5.4/src_ed/model_instance.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/model_instance_base.cpp` & `pyqcm-2.5.4/src_ed/model_instance_base.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/model_instance_base.hpp` & `pyqcm-2.5.4/src_ed/model_instance_base.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/qcm_ED.cpp` & `pyqcm-2.5.4/src_ed/qcm_ED.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/qcm_ED.hpp` & `pyqcm-2.5.4/src_ed/qcm_ED.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/sector.cpp` & `pyqcm-2.5.4/src_ed/sector.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/sector.hpp` & `pyqcm-2.5.4/src_ed/sector.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/sparse_matrix.hpp` & `pyqcm-2.5.4/src_ed/sparse_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/state.hpp` & `pyqcm-2.5.4/src_ed/state.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/symmetric_orbital.hpp` & `pyqcm-2.5.4/src_ed/symmetric_orbital.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/symmetry_group.cpp` & `pyqcm-2.5.4/src_ed/symmetry_group.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_ed/symmetry_group.hpp` & `pyqcm-2.5.4/src_ed/symmetry_group.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/common_Py.cpp` & `pyqcm-2.5.4/src_python/common_Py.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/common_Py.hpp` & `pyqcm-2.5.4/src_python/common_Py.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/qcm_ED_lib.cpp` & `pyqcm-2.5.4/src_python/qcm_ED_lib.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/qcm_ED_only.hpp` & `pyqcm-2.5.4/src_python/qcm_ED_only.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/qcm_ED_wrap.hpp` & `pyqcm-2.5.4/src_python/qcm_ED_wrap.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/qcm_lib.cpp` & `pyqcm-2.5.4/src_python/qcm_lib.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_python/qcm_wrap.hpp` & `pyqcm-2.5.4/src_python/qcm_wrap.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/CPT.cpp` & `pyqcm-2.5.4/src_qcm/CPT.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
 
 //==============================================================================
 /** 
  Computes the CDMFT host
  @param freqs [in] frequency array (along the imaginary axis)
  @param weights [in] weights of the different frequencies in the distance function
  */
-void lattice_model_instance::CDMFT_Host(const vector<double>& freqs, const vector<double>& weights)
+void lattice_model_instance::CDMFT_host(const vector<double>& freqs, const vector<double>& weights)
 {
 	CDMFT_weights = weights;
 	CDMFT_freqs = freqs;
 
 	if(G_host.size()==0){
 		G_host.assign(freqs.size(), vector<matrix<Complex>>(n_clus));
 		for(int i=0; i<freqs.size(); i++){
```

### Comparing `pyqcm-2.5.2/src_qcm/Chern.cpp` & `pyqcm-2.5.4/src_qcm/Chern.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/Doxyfile` & `pyqcm-2.5.4/src_qcm/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/Green_function.hpp` & `pyqcm-2.5.4/src_qcm/Green_function.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/QCM.cpp` & `pyqcm-2.5.4/src_qcm/QCM.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -922,15 +922,15 @@
   }
 
   void CDMFT_host(const vector<double>& freqs, const vector<double>& weights, int label)
   {
     #ifdef QCM_DEBUG
     check_instance(label);
     #endif
-    lattice_model_instances.at(label)->CDMFT_Host(freqs, weights); 
+    lattice_model_instances.at(label)->CDMFT_host(freqs, weights); 
   }
 
   void set_CDMFT_host(int label, const vector<double>& freqs, const int clus, const vector<matrix<Complex>>& H, const bool spin_down)
   {
     #ifdef QCM_DEBUG
     check_instance(label);
     #endif
```

### Comparing `pyqcm-2.5.2/src_qcm/QCM.hpp` & `pyqcm-2.5.4/src_qcm/QCM.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/average.cpp` & `pyqcm-2.5.4/src_qcm/average.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/basis3D.cpp` & `pyqcm-2.5.4/src_qcm/basis3D.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/basis3D.hpp` & `pyqcm-2.5.4/src_qcm/basis3D.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice3D.cpp` & `pyqcm-2.5.4/src_qcm/lattice3D.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice3D.hpp` & `pyqcm-2.5.4/src_qcm/lattice3D.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice_matrix_element.hpp` & `pyqcm-2.5.4/src_qcm/lattice_matrix_element.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice_model.cpp` & `pyqcm-2.5.4/src_qcm/lattice_model.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice_model.hpp` & `pyqcm-2.5.4/src_qcm/lattice_model.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice_model_instance.cpp` & `pyqcm-2.5.4/src_qcm/lattice_model_instance.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice_model_instance.hpp` & `pyqcm-2.5.4/src_qcm/lattice_model_instance.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 	vector<pair<vector<double>, vector<double>>> Lehmann_Green_function(vector<vector3D<double>> &k, int orb, bool spin_down);
 	vector<vector<matrix<Complex>>> get_CDMFT_host(bool spin_down);
 	void set_CDMFT_host(const vector<double>& freqs, const int clus, const vector<matrix<Complex>>& H, const bool spin_down);
 	void average_integrand_per(Complex w, vector3D<double> &k, const int *nv, double *I);
 	void average_integrand(Complex w, vector3D<double> &k, const int *nv, double *I);
 	void build_cluster_H();
 	void build_H();
-	void CDMFT_Host(const vector<double>& freqs, const vector<double>& weights);
+	void CDMFT_host(const vector<double>& freqs, const vector<double>& weights);
 	void cluster_self_energy(Green_function& G);
 	void Green_eigensystem(Green_function &G, const vector3D<double> &k, vector<double> &e, matrix<Complex> &U, int opt);
 	void Green_function_solve(); //!< calls the Green_function solver for all clusters
 	void inverse_Gcpt(const block_matrix<Complex> &Ginv, Green_function_k &M);
 	void periodized_Green_function(Green_function_k &M);
 	void potential_energy_integrand(Complex w, vector3D<double> &k, const int *nv, double *I);
 	void print_parameters(ostream& out, print_format format);
```

### Comparing `pyqcm-2.5.2/src_qcm/lattice_operator.cpp` & `pyqcm-2.5.4/src_qcm/lattice_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/lattice_operator.hpp` & `pyqcm-2.5.4/src_qcm/lattice_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/omp.h` & `pyqcm-2.5.4/src_qcm/omp.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/parameter_set.cpp` & `pyqcm-2.5.4/src_qcm/parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/parameter_set.hpp` & `pyqcm-2.5.4/src_qcm/parameter_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/print.cpp` & `pyqcm-2.5.4/src_qcm/print.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/profile.cpp` & `pyqcm-2.5.4/src_qcm/profile.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_qcm/vector3D.hpp` & `pyqcm-2.5.4/src_qcm/vector3D.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/ED_global_parameter.cpp` & `pyqcm-2.5.4/src_util/ED_global_parameter.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/VDVH_kernel.cpp` & `pyqcm-2.5.4/src_util/VDVH_kernel.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/VDVH_kernel.hpp` & `pyqcm-2.5.4/src_util/VDVH_kernel.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/block_matrix.hpp` & `pyqcm-2.5.4/src_util/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/cblas.h` & `pyqcm-2.5.4/src_util/cblas.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/clapack.h` & `pyqcm-2.5.4/src_util/clapack.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/f2c.h` & `pyqcm-2.5.4/src_util/f2c.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/global_parameter.cpp` & `pyqcm-2.5.4/src_util/global_parameter.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     new_global_int(0,"seed","seed of the random number generator");
     new_global_int(1024,"cuba2D_mineval","minimum number of integrand evaluations in CUBA (2D)");
     new_global_int(16000,"cuba3D_mineval","minimum number of integrand evaluations in CUBA (3D)");
     new_global_int(32,"kgrid_side","number of wavevectors on the side in a fixed wavevector grid");
     new_global_int(60,"max_iter_QN","maximum number of iterations in the quasi-Newton method");
     new_global_int(64,"max_dim_print","Maximum dimension for printing vectors and matrices");
     new_global_int(8, "GK_min_regions","minimum number of regions in the Gauss-Kronrod method");
-    new_global_int(8,"print_precision","precision of printed output");
+    new_global_int(9,"print_precision","precision of printed output");
 
     new_global_char('G', "periodization", "periodization scheme: G, S, M, C or N (None)");
 
     // ED global parameters
 
     new_global_bool(false,"check_lanczos_residual","checks the Lanczos residual at the end of the eigenvector computation");
     new_global_bool(false,"no_degenerate_BL","forbids band lanczos to proceed when the eigenstates have degenerate energies");
```

### Comparing `pyqcm-2.5.2/src_util/global_parameter.hpp` & `pyqcm-2.5.4/src_util/global_parameter.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/integrate.cpp` & `pyqcm-2.5.4/src_util/integrate.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/integrate.hpp` & `pyqcm-2.5.4/src_util/integrate.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/matrix.cpp` & `pyqcm-2.5.4/src_util/matrix.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -137,19 +137,20 @@
 	
 	vector<integer> IPIV(r);
 	vector<doublecomplex> WORK(r);
 	
 	N = r;
 	M = r;
 	LDA = r;
-	
-	zgetrf_(&M, &N,(doublecomplex*)&v[0], &LDA, IPIV.data(),&INFO);
-	assert((int)INFO==0);
-	zgetri_(&N,(doublecomplex*)&v[0],&LDA,IPIV.data(),WORK.data(),&N,&INFO);
-	assert((int)INFO==0);
+	try{
+		zgetrf_(&M, &N,(doublecomplex*)&v[0], &LDA, IPIV.data(),&INFO);
+		if((int)INFO) qcm_throw("Error in matrix inversion:  zgetrf_() produces INFO = "+to_string<int>(INFO));
+		zgetri_(&N,(doublecomplex*)&v[0],&LDA,IPIV.data(),WORK.data(),&N,&INFO);
+		if((int)INFO) qcm_throw("Error in matrix inversion:  zgetri_() produces INFO = "+to_string<int>(INFO));
+	} catch(const string& s) {qcm_catch(s);}
 }
```

### Comparing `pyqcm-2.5.2/src_util/matrix.hpp` & `pyqcm-2.5.4/src_util/matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/parser.cpp` & `pyqcm-2.5.4/src_util/parser.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -300,23 +300,23 @@
   }
 }
 
 
 
 void qcm_throw(const std::string& s)
 {
-    // banner('*', s, std::cerr);
+    banner('*', s, std::cerr);
     throw(s);
 }
 
 
 
 void qcm_ED_throw(const std::string& s)
 {
-    // banner('*', s, std::cerr);
+    banner('*', s, std::cerr);
     throw(s);
 }
 
 
 void qcm_warning(const std::string& s)
 {
     if(global_bool("verb_warning")) cout << "QCM WARNING : " << s << endl;
```

### Comparing `pyqcm-2.5.2/src_util/parser.hpp` & `pyqcm-2.5.4/src_util/parser.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/types.hpp` & `pyqcm-2.5.4/src_util/types.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/vector_num.cpp` & `pyqcm-2.5.4/src_util/vector_num.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/src_util/vector_num.hpp` & `pyqcm-2.5.4/src_util/vector_num.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_all.py` & `pyqcm-2.5.4/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/S_format.ref` & `pyqcm-2.5.4/tests/test_diagonalization/S_format.ref`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/S_format_complex.ref` & `pyqcm-2.5.4/tests/test_diagonalization/S_format_complex.ref`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py` & `pyqcm-2.5.4/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/common.py` & `pyqcm-2.5.4/tests/test_diagonalization/common.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/model_1D_8.py` & `pyqcm-2.5.4/tests/test_diagonalization/model_1D_8.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py` & `pyqcm-2.5.4/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution.py` & `pyqcm-2.5.4/tests/test_diagonalization/test_pole_distribution.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution_complex.py` & `pyqcm-2.5.4/tests/test_diagonalization/test_pole_distribution_complex.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_1D.py` & `pyqcm-2.5.4/tests/test_files/model_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_1D_2.py` & `pyqcm-2.5.4/tests/test_files/model_1D_2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_1D_2_4b.py` & `pyqcm-2.5.4/tests/test_files/model_1D_2_4b.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_1D_4.py` & `pyqcm-2.5.4/tests/test_files/model_1D_4.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_1D_4_C2.py` & `pyqcm-2.5.4/tests/test_files/model_1D_4_C2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_2x2_C2.py` & `pyqcm-2.5.4/tests/test_files/model_2x2_C2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_2x2_C2_vca.py` & `pyqcm-2.5.4/tests/test_files/model_2x2_C2_vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_G4_6b_2C.py` & `pyqcm-2.5.4/tests/test_files/model_G4_6b_2C.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_WSM.py` & `pyqcm-2.5.4/tests/test_files/model_WSM.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_graphene_bath.py` & `pyqcm-2.5.4/tests/test_files/model_graphene_bath.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/model_hartree.py` & `pyqcm-2.5.4/tests/test_files/model_hartree.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/record_2x2.py` & `pyqcm-2.5.4/tests/test_files/record_2x2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/record_2x2_8b.py` & `pyqcm-2.5.4/tests/test_files/record_2x2_8b.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/record_2x2_anom.py` & `pyqcm-2.5.4/tests/test_files/record_2x2_anom.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/record_WSM.py` & `pyqcm-2.5.4/tests/test_files/record_WSM.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/record_WSM2.py` & `pyqcm-2.5.4/tests/test_files/record_WSM2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/record_spin.py` & `pyqcm-2.5.4/tests/test_files/record_spin.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_2clusters.py` & `pyqcm-2.5.4/tests/test_files/test_2clusters.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_CF.py` & `pyqcm-2.5.4/tests/test_files/test_CF.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_averages.py` & `pyqcm-2.5.4/tests/test_files/test_averages.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_berry.py` & `pyqcm-2.5.4/tests/test_files/test_berry.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_cdmft.py` & `pyqcm-2.5.4/tests/test_files/test_cdmft.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_cdmft_hartree.py` & `pyqcm-2.5.4/tests/test_files/test_cdmft_hartree.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_cluster_average.py` & `pyqcm-2.5.4/tests/test_files/test_cluster_average.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_controlled_loop.py` & `pyqcm-2.5.4/tests/test_files/test_controlled_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_draw.py` & `pyqcm-2.5.4/tests/test_files/test_draw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_fidelity.py` & `pyqcm-2.5.4/tests/test_files/test_fidelity.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_fixed_density_loop.py` & `pyqcm-2.5.4/tests/test_files/test_fixed_density_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_hartree.py` & `pyqcm-2.5.4/tests/test_files/test_hartree.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_mixing.py` & `pyqcm-2.5.4/tests/test_files/test_mixing.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_mixing2.py` & `pyqcm-2.5.4/tests/test_files/test_mixing2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_mixing_cf.py` & `pyqcm-2.5.4/tests/test_files/test_mixing_cf.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_reset.py` & `pyqcm-2.5.4/tests/test_files/test_reset.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_spectral.py` & `pyqcm-2.5.4/tests/test_files/test_spectral.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_vca.py` & `pyqcm-2.5.4/tests/test_files/test_vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_vca_MPI.py` & `pyqcm-2.5.4/tests/test_files/test_vca_MPI.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.2/tests/test_files/test_write.py` & `pyqcm-2.5.4/tests/test_files/test_write.py`

 * *Files identical despite different names*

