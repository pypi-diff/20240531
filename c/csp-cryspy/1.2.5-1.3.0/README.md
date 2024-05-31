# Comparing `tmp/csp_cryspy-1.2.5.tar.gz` & `tmp/csp_cryspy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp_cryspy-1.2.5.tar", last modified: Fri May 10 04:58:33 2024, max compression
+gzip compressed data, was "csp_cryspy-1.3.0.tar", last modified: Fri May 31 06:45:25 2024, max compression
```

## Comparing `csp_cryspy-1.2.5.tar` & `csp_cryspy-1.3.0.tar`

### file list

```diff
@@ -1,130 +1,132 @@
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.923330 csp_cryspy-1.2.5/
--rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp_cryspy-1.2.5/LICENSE
--rw-r--r--   0 yamashita06   (501) staff       (20)     6311 2024-05-10 04:58:33.923096 csp_cryspy-1.2.5/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     4376 2024-05-10 04:52:57.000000 csp_cryspy-1.2.5/README.md
--rw-------   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp_cryspy-1.2.5/pyproject.toml
--rw-r--r--   0 yamashita06   (501) staff       (20)       38 2024-05-10 04:58:33.923373 csp_cryspy-1.2.5/setup.cfg
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.894028 csp_cryspy-1.2.5/src/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.894792 csp_cryspy-1.2.5/src/cryspy/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.896642 csp_cryspy-1.2.5/src/cryspy/BO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/BO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2651 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/bo_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7087 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/bo_next_select.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/BO/bo_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4907 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/combo_cryspy.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      757 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/select_descriptor.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.898662 csp_cryspy-1.2.5/src/cryspy/EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/EA/__init__.py
--rw-------   0 yamashita06   (501) staff       (20)      823 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/calc_ef.py
--rw-------   0 yamashita06   (501) staff       (20)     4834 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/calc_hull.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4042 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_append.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8211 2024-05-06 04:10:37.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_child.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4107 2024-05-07 01:16:55.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7725 2024-05-07 04:29:17.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_next_gen.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.902115 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/__init__.py
--rw-------   0 yamashita06   (501) staff       (20)     1963 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/addition.py
--rw-------   0 yamashita06   (501) staff       (20)    14110 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/adj_comp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    30058 2024-05-07 01:18:49.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/crossover.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    14404 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/ea_generation.py
--rw-------   0 yamashita06   (501) staff       (20)     1299 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/elimination.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8444 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/permutation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2849 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/rotation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9549 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/select_parents.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6428 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/strain.py
--rw-------   0 yamashita06   (501) staff       (20)     2688 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/substitution.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.903709 csp_cryspy-1.2.5/src/cryspy/IO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/IO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/IO/change_input.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1794 2023-11-17 03:52:02.000000 csp_cryspy-1.2.5/src/cryspy/IO/io_stat.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6223 2024-05-10 04:42:44.000000 csp_cryspy-1.2.5/src/cryspy/IO/out_results.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5079 2024-04-30 07:56:08.000000 csp_cryspy-1.2.5/src/cryspy/IO/pkl_data.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    78090 2024-05-02 13:30:51.000000 csp_cryspy-1.2.5/src/cryspy/IO/read_input.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.905768 csp_cryspy-1.2.5/src/cryspy/LAQA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/calc_score.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1475 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1929 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_next_selection.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1116 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_restart.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.906721 csp_cryspy-1.2.5/src/cryspy/RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.907603 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    25584 2024-05-10 04:40:12.000000 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    19080 2023-11-11 11:29:31.000000 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/random_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/rs_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/rs_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.908072 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.908918 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/
--rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2821 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/calc_FP.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.910492 csp_cryspy-1.2.5/src/cryspy/interactive/
--rw-------   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp_cryspy-1.2.5/src/cryspy/interactive/__init__.py
--rw-------   0 yamashita06   (501) staff       (20)     1026 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interactive/action.py
--rw-------   0 yamashita06   (501) staff       (20)     1839 2023-10-18 03:35:51.000000 csp_cryspy-1.2.5/src/cryspy/interactive/energy_plot.py
--rw-------   0 yamashita06   (501) staff       (20)     6479 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interactive/restart_intract.py
--rw-------   0 yamashita06   (501) staff       (20)      505 2023-10-18 03:35:51.000000 csp_cryspy-1.2.5/src/cryspy/interactive/rslt_energy.py
--rw-------   0 yamashita06   (501) staff       (20)      452 2023-10-18 03:35:51.000000 csp_cryspy-1.2.5/src/cryspy/interactive/view_atom.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.911077 csp_cryspy-1.2.5/src/cryspy/interface/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.912036 csp_cryspy-1.2.5/src/cryspy/interface/ASE/
--rw-------   0 yamashita06   (501) staff       (20)      818 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/ASE/calc_files_ase.py
--rw-------   0 yamashita06   (501) staff       (20)     1156 2023-12-24 01:43:02.000000 csp_cryspy-1.2.5/src/cryspy/interface/ASE/collect_ase.py
--rw-------   0 yamashita06   (501) staff       (20)     1838 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/ASE/ctrl_job_ase.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.913103 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      988 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/calc_files_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1621 2023-11-17 03:46:18.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/collect_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2281 2023-11-17 03:46:25.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2955 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.914182 csp_cryspy-1.2.5/src/cryspy/interface/OMX/
--rw-r--r--   0 yamashita06   (501) staff       (20)      886 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/calc_files_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2851 2023-11-17 03:46:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/collect_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4616 2024-04-24 09:10:55.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/ctrl_job_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3205 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.915461 csp_cryspy-1.2.5/src/cryspy/interface/QE/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      836 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/calc_files_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    11391 2023-11-17 03:47:37.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/collect_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4484 2024-04-24 08:59:19.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/ctrl_job_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2945 2024-04-24 09:06:06.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.916551 csp_cryspy-1.2.5/src/cryspy/interface/VASP/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      795 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/calc_files_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9130 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/collect_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3606 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/ctrl_job_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.917192 csp_cryspy-1.2.5/src/cryspy/interface/ext/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/ext/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      513 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/ext/collect_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8681 2023-11-17 03:44:32.000000 csp_cryspy-1.2.5/src/cryspy/interface/select_code.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.918354 csp_cryspy-1.2.5/src/cryspy/interface/soiap/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      839 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/calc_files_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7519 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/collect_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2358 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/ctrl_job_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2416 2023-11-15 04:16:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.919006 csp_cryspy-1.2.5/src/cryspy/job/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/job/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    13495 2024-05-10 04:40:12.000000 csp_cryspy-1.2.5/src/cryspy/job/ctrl_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    33247 2024-05-10 04:40:12.000000 csp_cryspy-1.2.5/src/cryspy/job/ctrl_job.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.920026 csp_cryspy-1.2.5/src/cryspy/scripts/
--rw-------   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/scripts/__init__.py
--rwx------   0 yamashita06   (501) staff       (20)     4416 2023-11-10 02:37:20.000000 csp_cryspy-1.2.5/src/cryspy/scripts/cryspy.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.921019 csp_cryspy-1.2.5/src/cryspy/start/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/start/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5544 2024-04-27 15:01:58.000000 csp_cryspy-1.2.5/src/cryspy/start/cryspy_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4701 2024-04-27 20:49:23.000000 csp_cryspy-1.2.5/src/cryspy/start/cryspy_restart.py
--rw-------   0 yamashita06   (501) staff       (20)     7376 2023-11-11 09:28:31.000000 csp_cryspy-1.2.5/src/cryspy/start/gen_init_struc.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.921861 csp_cryspy-1.2.5/src/cryspy/util/
--rw-------   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/util/constants.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    15905 2023-11-11 04:14:25.000000 csp_cryspy-1.2.5/src/cryspy/util/struc_util.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3825 2024-05-10 04:48:14.000000 csp_cryspy-1.2.5/src/cryspy/util/utility.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.922833 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/
--rw-r--r--   0 yamashita06   (501) staff       (20)     6311 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/PKG-INFO
--rw-------   0 yamashita06   (501) staff       (20)     3543 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/SOURCES.txt
--rw-------   0 yamashita06   (501) staff       (20)        1 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/dependency_links.txt
--rw-------   0 yamashita06   (501) staff       (20)       54 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/entry_points.txt
--rw-------   0 yamashita06   (501) staff       (20)       14 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/requires.txt
--rw-------   0 yamashita06   (501) staff       (20)        7 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/top_level.txt
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.688634 csp_cryspy-1.3.0/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp_cryspy-1.3.0/LICENSE
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6432 2024-05-31 06:45:25.688441 csp_cryspy-1.3.0/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4497 2024-05-31 06:42:45.000000 csp_cryspy-1.3.0/README.md
+-rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp_cryspy-1.3.0/pyproject.toml
+-rw-r--r--   0 yamashita06   (501) staff       (20)       38 2024-05-31 06:45:25.688681 csp_cryspy-1.3.0/setup.cfg
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.673656 csp_cryspy-1.3.0/src/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.674210 csp_cryspy-1.3.0/src/cryspy/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.674883 csp_cryspy-1.3.0/src/cryspy/BO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/BO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2906 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/BO/bo_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8560 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/BO/bo_next_select.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      635 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/BO/bo_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      544 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/BO/select_descriptor.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.676028 csp_cryspy-1.3.0/src/cryspy/EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      823 2024-05-07 06:33:41.000000 csp_cryspy-1.3.0/src/cryspy/EA/calc_ef.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4815 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/calc_hull.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5423 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/ea_append.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    10092 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/ea_child.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5582 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/ea_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9039 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/ea_next_gen.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.677599 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4683 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/addition.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    14085 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/adj_comp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    14574 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/crossover.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3743 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/elimination.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5446 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/permutation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4388 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/rotation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3771 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/select_parents.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5106 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/strain.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6332 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/substitution.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2923 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/EA/survival.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.678790 csp_cryspy-1.3.0/src/cryspy/IO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/IO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      354 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/change_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1098 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/diff_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      921 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/io_stat.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5605 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/out_results.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8603 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/pkl_data.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    43627 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/read_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1632 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/IO/write_input.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.679619 csp_cryspy-1.3.0/src/cryspy/LAQA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/LAQA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp_cryspy-1.3.0/src/cryspy/LAQA/calc_score.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1582 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/LAQA/laqa_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2035 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/LAQA/laqa_next_selection.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1159 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/LAQA/laqa_restart.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.680312 csp_cryspy-1.3.0/src/cryspy/RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/RS/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.680706 csp_cryspy-1.3.0/src/cryspy/RS/gen_struc_RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/RS/gen_struc_RS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    28356 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    18583 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/RS/gen_struc_RS/random_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    10123 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/RS/rs_gen.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      403 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/RS/rs_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      591 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/RS/rs_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.680851 csp_cryspy-1.3.0/src/cryspy/calc_dscrpt/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.681100 csp_cryspy-1.3.0/src/cryspy/calc_dscrpt/FP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/calc_dscrpt/FP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1065 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/calc_dscrpt/FP/calc_FP.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/calc_dscrpt/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.681944 csp_cryspy-1.3.0/src/cryspy/interactive/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp_cryspy-1.3.0/src/cryspy/interactive/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1458 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interactive/action.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1839 2023-10-18 03:35:51.000000 csp_cryspy-1.3.0/src/cryspy/interactive/energy_plot.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3706 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interactive/restart_interact.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3706 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interactive/restart_interact_subprocess.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      505 2023-10-18 03:35:51.000000 csp_cryspy-1.3.0/src/cryspy/interactive/rslt_energy.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-10-18 03:35:51.000000 csp_cryspy-1.3.0/src/cryspy/interactive/view_atom.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.682187 csp_cryspy-1.3.0/src/cryspy/interface/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.682590 csp_cryspy-1.3.0/src/cryspy/interface/ASE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      743 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/ASE/calc_files_ase.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1111 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/ASE/collect_ase.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1760 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/ASE/ctrl_job_ase.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.683200 csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      910 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1534 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/collect_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2287 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2927 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.683712 csp_cryspy-1.3.0/src/cryspy/interface/OMX/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      845 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/OMX/calc_files_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2779 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/OMX/collect_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4584 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/OMX/ctrl_job_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3180 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/OMX/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.684324 csp_cryspy-1.3.0/src/cryspy/interface/QE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/interface/QE/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      747 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/QE/calc_files_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    11254 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/QE/collect_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4441 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/QE/ctrl_job_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2945 2024-05-07 06:33:41.000000 csp_cryspy-1.3.0/src/cryspy/interface/QE/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.684863 csp_cryspy-1.3.0/src/cryspy/interface/VASP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/interface/VASP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      719 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/VASP/calc_files_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9028 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/VASP/collect_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3540 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/VASP/ctrl_job_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/interface/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.685122 csp_cryspy-1.3.0/src/cryspy/interface/ext/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/interface/ext/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      483 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/ext/collect_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    10415 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/select_code.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.685915 csp_cryspy-1.3.0/src/cryspy/interface/soiap/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/interface/soiap/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      762 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/soiap/calc_files_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7430 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/soiap/collect_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2324 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/soiap/ctrl_job_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2380 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/interface/soiap/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.686348 csp_cryspy-1.3.0/src/cryspy/job/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/job/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    14934 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/job/ctrl_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    35131 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/job/ctrl_job.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.686592 csp_cryspy-1.3.0/src/cryspy/scripts/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/scripts/__init__.py
+-rwxr-xr-x   0 yamashita06   (501) staff       (20)     4507 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/scripts/cryspy.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.686953 csp_cryspy-1.3.0/src/cryspy/start/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/start/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5407 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/start/cryspy_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4924 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/start/cryspy_restart.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.687339 csp_cryspy-1.3.0/src/cryspy/util/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp_cryspy-1.3.0/src/cryspy/util/constants.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    17028 2024-05-31 06:26:37.000000 csp_cryspy-1.3.0/src/cryspy/util/struc_util.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3505 2024-05-31 06:43:22.000000 csp_cryspy-1.3.0/src/cryspy/util/utility.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-31 06:45:25.688211 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6432 2024-05-31 06:45:25.000000 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3596 2024-05-31 06:45:25.000000 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/SOURCES.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2024-05-31 06:45:25.000000 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/dependency_links.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)       54 2024-05-31 06:45:25.000000 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/entry_points.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)       14 2024-05-31 06:45:25.000000 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/requires.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)        7 2024-05-31 06:45:25.000000 csp_cryspy-1.3.0/src/csp_cryspy.egg-info/top_level.txt
```

### Comparing `csp_cryspy-1.2.5/LICENSE` & `csp_cryspy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.5/PKG-INFO` & `csp_cryspy-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.2.5
+Version: 1.3.0
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -43,17 +43,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.2.5 (2024 May 10)
+version 1.3.0 (2024 May 31)
 
 ## News
+- [2024 May 31] CrySPY 1.3.0 released.
+    + There are important changes. See [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info)
 - [2024 May 10] CrySPY 1.2.5 released.
     + bug fix for order_ef in out_results.py
 - [2024 May 7] CrySPY 1.2.4 released.
     + bug fix
 - [2023 October 21] CrySPY 1.2.3 released.
     + bug fix for MPI
 - [2023 October 18] CrySPY 1.2.2 released.
@@ -77,33 +79,31 @@
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
 
 (optional)
-- [COMBO](https://github.com/Tomoki-YAMASHITA/combo3 "COMBO") (required if algo is BO)
-- mpi4py
+- [PHYSBO](https://www.pasums.issp.u-tokyo.ac.jp/physbo/en/about "PHYSBO") (required if algo is BO)
+- [DScribe](https://singroup.github.io/dscribe/latest/ "DScribe") (required if algo is BO)
+- [mpi4py](https://mpi4py.readthedocs.io/en/stable "mpi4py")
 
 
 See [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc/installation/requirements/ "CrySPY document") in detail.
 
 ### Structure optimizer
 At least one optimizer is required.
 
 - [VASP](https://www.vasp.at "VASP") (tested with version 5.4.4)
 - [QUANTUM ESPRESSO](http://www.quantum-espresso.org "Quantum ESPRESSO") (tested with version 6.x, version 5.x does not work)
 - [OpenMX](http://www.openmx-square.org "OpenMX")
 - [soiap](https://github.com/nbsato/soiap "soiap") (tested with version 0.2.2)
 - [LAMMPS](http://lammps.sandia.gov "LAMMPS")
+- [ASE](https://wiki.fysik.dtu.dk/ase "ASE")
 
-### Others
-(optional)
-- cal-fingerprint: (required if algo is BO)
-- [find_wy](https://github.com/nim-hrkn/find_wy "find_wy"): find_wy can randomly select a combination of Wyckoff positions for a given chemical composition and space group. 
 
 ## Document (English/Japanese)
 [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc "CrySPY documment")
 
 ## CrySPY Utility
 [CrySPY Utility](https://github.com/Tomoki-YAMASHITA/CrySPY_utility "CrySPY Utility")
```

### Comparing `csp_cryspy-1.2.5/README.md` & `csp_cryspy-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.2.5 (2024 May 10)
+version 1.3.0 (2024 May 31)
 
 ## News
+- [2024 May 31] CrySPY 1.3.0 released.
+    + There are important changes. See [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info)
 - [2024 May 10] CrySPY 1.2.5 released.
     + bug fix for order_ef in out_results.py
 - [2024 May 7] CrySPY 1.2.4 released.
     + bug fix
 - [2023 October 21] CrySPY 1.2.3 released.
     + bug fix for MPI
 - [2023 October 18] CrySPY 1.2.2 released.
@@ -39,33 +41,31 @@
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
 
 (optional)
-- [COMBO](https://github.com/Tomoki-YAMASHITA/combo3 "COMBO") (required if algo is BO)
-- mpi4py
+- [PHYSBO](https://www.pasums.issp.u-tokyo.ac.jp/physbo/en/about "PHYSBO") (required if algo is BO)
+- [DScribe](https://singroup.github.io/dscribe/latest/ "DScribe") (required if algo is BO)
+- [mpi4py](https://mpi4py.readthedocs.io/en/stable "mpi4py")
 
 
 See [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc/installation/requirements/ "CrySPY document") in detail.
 
 ### Structure optimizer
 At least one optimizer is required.
 
 - [VASP](https://www.vasp.at "VASP") (tested with version 5.4.4)
 - [QUANTUM ESPRESSO](http://www.quantum-espresso.org "Quantum ESPRESSO") (tested with version 6.x, version 5.x does not work)
 - [OpenMX](http://www.openmx-square.org "OpenMX")
 - [soiap](https://github.com/nbsato/soiap "soiap") (tested with version 0.2.2)
 - [LAMMPS](http://lammps.sandia.gov "LAMMPS")
+- [ASE](https://wiki.fysik.dtu.dk/ase "ASE")
 
-### Others
-(optional)
-- cal-fingerprint: (required if algo is BO)
-- [find_wy](https://github.com/nim-hrkn/find_wy "find_wy"): find_wy can randomly select a combination of Wyckoff positions for a given chemical composition and space group. 
 
 ## Document (English/Japanese)
 [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc "CrySPY documment")
 
 ## CrySPY Utility
 [CrySPY Utility](https://github.com/Tomoki-YAMASHITA/CrySPY_utility "CrySPY Utility")
```

### Comparing `csp_cryspy-1.2.5/pyproject.toml` & `csp_cryspy-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.5/src/cryspy/BO/bo_init.py` & `csp_cryspy-1.3.0/src/cryspy/BO/bo_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-'''
-Initialize Bayesian optimization
-'''
-
 import configparser
 from logging import getLogger
 import random
 
 import pandas as pd
 
 from .select_descriptor import select_descriptor
 from ..IO import io_stat, pkl_data
-from ..IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def initialize(stat, init_struc_data, rslt_data):
+
+def initialize(rin, init_struc_data, rslt_data):
     # ---------- log
     logger.info('# ---------- Selection: 1')
 
     # ---------- check init_struc_data
     if None in init_struc_data.values():
         raise ValueError('init_struc_data includes None')
 
@@ -29,27 +25,34 @@
     id_select_hist = []
     bo_mean = {}
     bo_var = {}
     bo_score = {}
 
     # ---------- rslt_data, add and sort
     rslt_data['Select'] = pd.Series(dtype=int)
-    rslt_data = rslt_data[['Select', 'Spg_num',
-                           'Spg_sym', 'Spg_num_opt',
-                           'Spg_sym_opt', 'E_eV_atom', 'Magmom', 'Opt']]
+    rslt_data = rslt_data[[
+                    'Select',
+                    'Spg_num',
+                    'Spg_sym',
+                    'Spg_num_opt',
+                    'Spg_sym_opt',
+                    'E_eV_atom',
+                    'Magmom',
+                    'Opt',
+                ]]
     pkl_data.save_rslt(rslt_data)
 
     # ---------- random select
     all_id = [i for i in range(len(init_struc_data))]
     if rin.manual_select_bo:
         # ------ manual select bo
         x = ' '.join(str(i) for i in rin.manual_select_bo)
         logger.info(f'Manual select: {x}')
         nselect = rin.nselect_bo - len(rin.manual_select_bo)
-        id_queueing = rin.manual_select_bo[:]    # shallow copy
+        id_queueing = list(rin.manual_select_bo[:])    # shallow copy
         if 0 < nselect:
             diff_id = list(set(all_id) - set(id_queueing))
             id_queueing.extend(random.sample(diff_id, nselect))
         # ------ delete the value for manual_select_bo in cryspy.in
         config = configparser.ConfigParser()
         config.read('cryspy.in')
         config.set('BO', 'manual_select_bo', '')
@@ -58,24 +61,30 @@
     else:
         id_queueing = random.sample(all_id, rin.nselect_bo)
 
     # ---------- id_select_hist
     id_select_hist.append(id_queueing[:])    # append shallow copy
 
     # ---------- calc descriptor
-    init_dscrpt_data = select_descriptor(init_struc_data)
+    init_dscrpt_data = select_descriptor(rin, init_struc_data)
     opt_dscrpt_data = {}  # initialize in dict
 
     # ---------- save for BO
-    bo_id_data = (n_selection, id_queueing, id_running, id_select_hist)
-    pkl_data.save_bo_id(bo_id_data)
-    bo_data = (init_dscrpt_data, opt_dscrpt_data, bo_mean, bo_var, bo_score)
-    pkl_data.save_bo_data(bo_data)
+    pkl_data.save_id_queueing(id_queueing)
+    pkl_data.save_id_running(id_running)
+    pkl_data.save_n_selection(n_selection)
+    pkl_data.save_id_select_hist(id_select_hist)
+    pkl_data.save_init_dscrpt_data(init_dscrpt_data)
+    pkl_data.save_opt_dscrpt_data(opt_dscrpt_data)
+    pkl_data.save_bo_mean(bo_mean)
+    pkl_data.save_bo_var(bo_var)
+    pkl_data.save_bo_score(bo_score)
 
     # ---------- status
+    stat = io_stat.stat_read()
     io_stat.set_common(stat, 'selection', n_selection)
     io_stat.set_id(stat, 'selected_id', id_queueing)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- out and log
     x = ' '.join(str(a) for a in id_queueing)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/BO/bo_next_select.py` & `csp_cryspy-1.3.0/src/cryspy/BO/bo_next_select.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,49 @@
-'''
-Selection in Bayesian optimization
-'''
-
 import configparser
 from contextlib import redirect_stdout
 from logging import getLogger
 import os
 
 import numpy as np
+import physbo
 
-from .combo_cryspy import Policy_cryspy
 from ..IO import io_stat, out_results, pkl_data
-from ..IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def next_select(stat, rslt_data, bo_id_data, bo_data, noprint=False):
+
+def next_select(rin, rslt_data, bo_id_data, bo_data, noprint=False):
     # ---------- log
     logger.info('# ------ Bayesian optimization')
 
     # ---------- bo_id_data and bo_data
     n_selection, id_running, id_queueing, id_select_hist = bo_id_data
     init_dscrpt_data, opt_dscrpt_data, bo_mean, bo_var, bo_score = bo_data
 
     # ---------- n_selection
     n_selection += 1
 
     # ---------- manual select
-    if rin.manual_select_bo:
-        x = ' '.join(str(i) for i in rin.manual_select_bo)
+    if rin.manual_select_bo is not None:
+        manual_list = list(rin.manual_select_bo)
+        x = ' '.join(str(i) for i in manual_list)
         logger.info(f'Manual select: {x}')
         # ------ check already selected
-        tmp_list = [i for i in rin.manual_select_bo if i in opt_dscrpt_data]
+        tmp_list = [i for i in manual_list if i in opt_dscrpt_data]
         for j in tmp_list:
-            rin.manual_select_bo.remove(j)
+            manual_list.remove(j)
             logger.info(f'ID {j} was already selected. Remove it')
         # ------ number of structure to be selected
-        nselect = rin.nselect_bo - len(rin.manual_select_bo)
-        id_queueing = rin.manual_select_bo
+        nselect = rin.nselect_bo - len(manual_list)
+        id_queueing = manual_list
         # ------ delete the value for manual_select_bo in cryspy.in
         config = configparser.ConfigParser()
         config.read('cryspy.in')
-        config.set('BO', 'manual_select_bo', '')
+        config.set('BO', 'manual_select_bo', '')    # clear
         with open('cryspy.in', 'w') as f:
             config.write(f)
     else:
         nselect = rin.nselect_bo
     # ------ if number of remaining structures < nselect
     if len(init_dscrpt_data) - len(opt_dscrpt_data) < nselect:
         nselect = len(init_dscrpt_data) - len(opt_dscrpt_data)
@@ -76,60 +73,76 @@
                         logger.info(f'Eliminate ID {i}: {x} < emin_bo')
                         continue
                 s_act.append(len(descriptors))
                 done_id.append(i)
                 descriptors.append(opt_dscrpt_data[i])
             else:
                 # -- not yet
-                if i in rin.manual_select_bo:
-                    # remove manualy selected IDs not to select them
-                    non_error_id.remove(i)
+                if rin.manual_select_bo is not None:
+                    if i in rin.manual_select_bo:
+                        # remove manualy selected IDs not to select them
+                        non_error_id.remove(i)
+                    else:
+                        descriptors.append(init_dscrpt_data[i])
                 else:
                     descriptors.append(init_dscrpt_data[i])
         # ------ targets
         targets = [rslt_data.loc[cid]['E_eV_atom'] for cid in done_id]
         # ------ list --> numpy
         s_act = np.array(s_act, dtype=int)
         descriptors = np.array(descriptors)
         targets = np.array(targets, dtype=float)
         # ------ Bayesian optimization
-        actions, cryspy_mean, cryspy_var, cryspy_score = bayes_opt(
-            s_act, descriptors, targets, nselect, noprint)
+        actions, cryspy_mean, cryspy_var, cryspy_score = _bayes_opt(
+            s_act, descriptors, targets, nselect,
+            rin.score, rin.cdev, rin.num_rand_basis, noprint)
+        # t_act, t_mean, t_var, t_score = _bayes_opt2(
+        #     s_act, descriptors, targets, nselect,
+        #     rin.score, rin.cdev, rin.num_rand_basis, noprint)
+        # logger.debug(f't_act: {t_act}')
+        # logger.debug(f't_mean: {t_mean}')
+        # logger.debug(f't_var: {t_var}')
+        # logger.debug(f't_score: {t_score}')
         # ------ actions --> id_queueing
         for i in actions:
             id_queueing.append(non_error_id[i])
         # ------ bo_mean, bo_var, bo_score
         remaining_id = list(set(non_error_id) - set(done_id))
         bo_mean[n_selection] = dict(zip(remaining_id, cryspy_mean))
         bo_var[n_selection] = dict(zip(remaining_id, cryspy_var))
         if rin.score == 'TS':
             # -- in TS, nested list [[score1, socre2, ...]] is used
             bo_score[n_selection] = dict(zip(remaining_id, cryspy_score[0]))
         else:
             bo_score[n_selection] = dict(zip(remaining_id, cryspy_score))
         # ------ out
-        out_results.out_bo_common('BO_mean', bo_mean, rin.tot_struc)
-        out_results.out_bo_common('BO_var', bo_var, rin.tot_struc)
-        out_results.out_bo_common('BO_score', bo_score, rin.tot_struc)
+        out_results.out_bo_common('bo_mean', bo_mean, rin.tot_struc)
+        out_results.out_bo_common('bo_var', bo_var, rin.tot_struc)
+        out_results.out_bo_common('bo_score', bo_score, rin.tot_struc)
         out_results.out_bo_status(bo_mean, bo_var, bo_score,
                                   n_selection)
         # ------ save bo_data
-        bo_data = (init_dscrpt_data, opt_dscrpt_data,
-                   bo_mean, bo_var, bo_score)
-        pkl_data.save_bo_data(bo_data)
+        pkl_data.save_init_dscrpt_data(init_dscrpt_data)
+        pkl_data.save_opt_dscrpt_data(opt_dscrpt_data)
+        pkl_data.save_bo_mean(bo_mean)
+        pkl_data.save_bo_var(bo_var)
+        pkl_data.save_bo_score(bo_score)
 
     # ---------- id_select_hist
     id_select_hist.append(id_queueing[:])    # append shallow copy
     out_results.out_bo_id_hist(id_select_hist)
 
     # ---------- save
-    bo_id_data = (n_selection, id_queueing, id_running, id_select_hist)
-    pkl_data.save_bo_id(bo_id_data)
+    pkl_data.save_id_queueing(id_queueing)
+    # pkl_data.save_id_running(id_running)    # not used here
+    pkl_data.save_n_selection(n_selection)
+    pkl_data.save_id_select_hist(id_select_hist)
 
     # ---------- status
+    stat = io_stat.stat_read()
     io_stat.set_common(stat, 'selection', n_selection)
     io_stat.set_id(stat, 'selected_id', id_queueing)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- out and log
     logger.info(f'# ---------- Selection: {n_selection}')
@@ -138,53 +151,72 @@
 
     # ---------- ext
     if rin.calc_code == 'ext':
         with open('ext/stat_job', 'w') as fstat:
             fstat.write('out\n')
 
 
-def bayes_opt(s_act, descriptors, targets, nselect, noprint=False):
-    # ---------- start COMBO part
-    # ------ standardization
-    # X = combo.misc.centering(descriptors)
+def _bayes_opt(
+    s_act,
+    descriptors,
+    targets,
+    nselect,
+    score,
+    cdev=0.001,
+    num_rand_basis=0,
+    noprint=False,
+):
+    '''
+    # ---------- args
+    s_act (ndarray): indexes of already calculated structures. NOT structure ID.
+    descriptors (ndarray): descriptors of all structures, without error
+    targets (ndarray): energies of already calculated structures
+    nselect (int): number of structures to be selected
+    score (str): 'PI', EI' or 'TS'
+    cdev (float): cutoff value for standard deviation
+    num_rand_basis (int): number of basis functions. if 0, gaussian process
+    noprint (bool): if True, suppress print
+
+    # ---------- return
+    actions (ndarray): indexes of selected structures
+    p_mean (ndarray): mean of predicted energies
+    p_var (ndarray): variance of predicted energies
+    p_score (ndarray): value of acquisition function
+    '''
+
+    # ---------- standardization
     dev = np.std(descriptors, axis=0)
-    nonzero_indx = np.where(dev > rin.cdev)[0]
+    nonzero_indx = np.where(dev > cdev)[0]
     X = (descriptors[:, nonzero_indx] - np.mean(
         descriptors[:, nonzero_indx], axis=0)) / dev[nonzero_indx]
 
-    # ------ Declaring the policy by
-    pc = Policy_cryspy(test_X=X)
-
-    # ------ pick up data, already optimized
-    actions = pc.specified_search(specified_actions=s_act, max_num_probes=1)
+    # ---------- Declaring the policy by
+    policy = physbo.search.discrete.policy(test_X=X, initial_data=[s_act, -targets])
 
-    # ------ write
-    pc.write(actions, -targets)    # minus for minimum search
-
-    # ------ log
-    out_log(pc.history)
-
-    # ------ Bayes_search
+    # ---------- Bayes search
     if noprint:
         with redirect_stdout(open(os.devnull, 'w')):
-            actions, cryspy_mean, cryspy_var, cryspy_score = pc.bayes_search_cryspy(
-                max_num_probes=1,
-                num_search_each_probe=nselect,
-                score=rin.score,
-                num_rand_basis=rin.num_rand_basis)
+            actions = policy.bayes_search(
+                                max_num_probes=1,
+                                num_search_each_probe=nselect,
+                                simulator=None,
+                                score=score,
+                                interval=0,
+                                num_rand_basis = num_rand_basis,
+                            )
     else:
-        actions, cryspy_mean, cryspy_var, cryspy_score = pc.bayes_search_cryspy(
-            max_num_probes=1,
-            num_search_each_probe=nselect,
-            score=rin.score,
-            num_rand_basis=rin.num_rand_basis)
+        actions = policy.bayes_search(
+                            max_num_probes=1,
+                            num_search_each_probe=nselect,
+                            simulator=None,
+                            score=score,
+                            interval=0,
+                            num_rand_basis = num_rand_basis,
+                        )
+
+    # ---------- mean, var, score
+    p_mean = policy.get_post_fmean(X)
+    p_var = policy.get_post_fcov(X)
+    p_score = policy.get_score(mode=score, xs=X)
 
     # ------ return
-    return actions, cryspy_mean, cryspy_var, cryspy_score
-
-
-# ---------- just for log
-def out_log(history):
-    n = history.total_num_search
-    index = np.argmax(history.fx[0:n])
-
-    logger.info(f'current best E = {-history.fx[index]}')
+    return actions, p_mean, p_var, p_score
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/EA/calc_ef.py` & `csp_cryspy-1.3.0/src/cryspy/EA/calc_ef.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.5/src/cryspy/EA/calc_hull.py` & `csp_cryspy-1.3.0/src/cryspy/EA/calc_hull.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from logging import getLogger
 
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
 from scipy.spatial import ConvexHull
 
-from ..IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
 
-def calc_convex_hull_2d(ratio_data, ef_all, c_ids, gen):
+def calc_convex_hull_2d(rin, ratio_data, ef_all, c_ids, gen):
     '''
     Input:
         ratio_data [dict]: ratio of all structures, {ID: [ratio list], ...}
         ef_all [dict]: formation energy of all structures, {ID: Ef, ...}
         c_ids [array]: ID array of current generation structures
         gen [int]: current generation
 
@@ -32,15 +30,15 @@
             ef_chull.append(ef_all[cid])
 
     # ---------- no negative Ef
     #            in this case, hull distance is equivalent to Ef
     if len(ef_chull) == 2:    # only end points
         # np.nan --> np.inf in hdist
         hdist = {cid: np.inf if np.isnan(ef_all[cid]) else ef_all[cid] for cid in ef_all}
-        draw_convex_hull_2d(None, ratio_data, ef_all, c_ids, gen)
+        draw_convex_hull_2d(rin, None, ratio_data, ef_all, c_ids, gen)
         return hdist
 
     # ---------- calc convex hull
     points = list(zip(ratio_chull, ef_chull))
     hull = ConvexHull(points)
     vpoints = hull.points[hull.vertices]    # hull.vertices: index of vertices in hull.points
     vpoints = np.vstack((vpoints, vpoints[0]))    # just for plot. vpoints[0] should be [1, 0] by ConvexHull()
@@ -49,15 +47,15 @@
     hdist = {
         cid: np.inf if np.isnan(ef_all[cid])
         else hull_distance_2d(ratio_data[cid][0], ef_all[cid], hull.equations)
         for cid in ef_all
     }
 
     # ---------- draw convex hull
-    draw_convex_hull_2d(vpoints, ratio_data, ef_all, c_ids, gen)
+    draw_convex_hull_2d(rin, vpoints, ratio_data, ef_all, c_ids, gen)
 
     # ---------- return
     return hdist
 
 
 def hull_distance_2d(x, y, equations):
     '''
@@ -72,15 +70,15 @@
             if dist < 0.0:
                 logger.warning('hdist <= 0.0, check hull distance.')
             hdists.append(dist)
 
     return min(hdists)
 
 
-def draw_convex_hull_2d(vpoints, ratio_data, ef_all, c_ids, gen):
+def draw_convex_hull_2d(rin, vpoints, ratio_data, ef_all, c_ids, gen):
     # ---------- setting
     plt.rcParams.update(_set_params())
 
     # ---------- fig
     fig, ax = plt.subplots(1, 1)
 
     # ---------- hline
@@ -88,15 +86,15 @@
 
     # ---------- label
     ax.set_xlabel('$x$ in '+f'{rin.atype[0]}'+'$_{x}$'+f'{rin.atype[1]}'+'$_{1-x}$')
     ax.set_ylabel('Formation energy (eV/atom)')
 
     # ---------- lim
     min_ef = min(ef_all.values())
-    ymin = min_ef * 1.1 if min_ef < -0.01 else -0.01
+    ymin = min_ef - 0.01 if min_ef < 0 else -0.01
     ax.set_ylim(ymin, 0.05)
 
     # ---------- plot ef_all
     for cid in ef_all:
         if np.isnan(ef_all[cid]):
             continue
         if cid in c_ids:
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/EA/ea_append.py` & `csp_cryspy-1.3.0/src/cryspy/interface/VASP/ctrl_job_vasp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,104 @@
-'''
-Append structures by evolutionary algorithm
-'''
-
 from logging import getLogger
 import os
+import shutil
 
-import pandas as pd
+from pymatgen.core import Structure
+from pymatgen.io.vasp import Kpoints
 
-from .ea_child import child_gen
-from .gen_struc_EA.select_parents import Select_parents
-from ..IO import change_input, io_stat, out_results, pkl_data
-from ..IO import read_input as rin
+from ...IO.out_results import out_kpts
+from ...IO import pkl_data
 
 
 logger = getLogger('cryspy')
 
-def append_struc(stat, init_struc_data):
-    # ---------- append structures by EA
-    logger.info('# ---------- Append structures by EA')
-
-    # ---------- load data
-    opt_struc_data = pkl_data.load_opt_struc()
-    rslt_data = pkl_data.load_rslt()
-
-    # ---------- fitness
-    fitness = rslt_data['E_eV_atom'].to_dict()    # {ID: energy, ..,}
-
-    # ---------- instantiate Seclect_parents class
-    logger.info('# ------ select parents')
-    sp = Select_parents(opt_struc_data, fitness, None, None, rin.n_fittest)
-    if rin.slct_func == 'TNM':
-        sp.set_tournament()
-    else:
-        sp.set_roulette()
-
-    # ---------- generate offspring by EA
-    logger.info('# ------ Generate structures')
-    init_struc_data, eagen = child_gen(sp, init_struc_data)
-
-    # ----------  ea_info
-    if os.path.isfile('./data/pkl_data/EA_data.pkl'):
-        _, _, ea_info, ea_origin = pkl_data.load_ea_data()
-    else:
-        # ------ initialize
-        # -- ea_info
-        ea_info = pd.DataFrame(columns=['Gen', 'Population',
-                                        'Crossover', 'Permutation', 'Strain',
-                                        'Random', 'Elite',
-                                        'crs_lat', 'slct_func'])
-        ea_info.iloc[:, 0:7] = ea_info.iloc[:, 0:7].astype(int)
-        # -- ea_origin
-        ea_origin = pd.DataFrame(columns=['Gen', 'Struc_ID',
-                                          'Operation', 'Parent'])
-        ea_origin.iloc[:, 0:2] = ea_origin.iloc[:, 0:2].astype(int)
-    # ------ register ea_info
-    tmp_info = pd.DataFrame([[rin.tot_struc, rin.n_pop, rin.n_crsov,
-                              rin.n_perm, rin.n_strain, rin.n_rand, 0,
-                              rin.crs_lat, rin.slct_func]],
-                            columns=ea_info.columns)
-    ea_info = pd.concat([ea_info, tmp_info], axis=0, ignore_index=True)
-    # ------ out ea_info
-    out_results.out_ea_info(ea_info)
-
-    # ---------- ea_origin
-    # ------ EA operation part
-    for cid in range(rin.tot_struc, rin.tot_struc + rin.n_pop - rin.n_rand):
-        tmp_origin = pd.DataFrame([[rin.tot_struc, cid, eagen.operation[cid],
-                                    eagen.parents[cid]]], columns=ea_origin.columns)
-        ea_origin = pd.concat([ea_origin, tmp_origin], axis=0, ignore_index=True)
-    # ------ random part
-    for cid in range(rin.tot_struc + rin.n_pop - rin.n_rand,
-                     rin.tot_struc + rin.n_pop):
-        tmp_origin = pd.DataFrame([[rin.tot_struc, cid, 'random', None]],
-                                  columns=ea_origin.columns)
-        ea_origin = pd.concat([ea_origin, tmp_origin], axis=0, ignore_index=True)
-    # ------  out ea_origin
-    out_results.out_ea_origin(ea_origin)
-
-    # ---------- save ea_data
-    ea_data = (None, None, ea_info, ea_origin)
-    pkl_data.save_ea_data(ea_data)
-
-    # ---------- change variables in cryspy.in
-    config = change_input.config_read()
-    logger.info('# -- Changed cryspy.in')
-    # ------ tot_struc
-    change_input.change_basic(config, 'tot_struc', rin.tot_struc + rin.n_pop)
-    logger.info(f'Changed tot_struc in cryspy.in from {rin.tot_struc} to {rin.tot_struc + rin.n_pop}')
-    rin.tot_struc = rin.tot_struc + rin.n_pop
-    # ------ append_struc_ea: True --> False
-    change_input.change_option(config, 'append_struc_ea', False)
-    logger.info('Changed append_struc_ea in cryspy.in from True to Flase')
-    # ------ write
-    change_input.write_config(config)
-
-    # ---------- status
-    io_stat.set_input_common(stat, 'basic', 'tot_struc', rin.tot_struc)
-    io_stat.set_input_common(stat, 'option', 'append_struc_ea', False)
-    io_stat.write_stat(stat)
+
+def next_stage_vasp(rin, stage, work_path, kpt_data, cid):
+    # ---------- skip_flag
+    skip_flag = False
+
+    # ---------- rename VASP files at the current stage
+    vasp_files = ['POSCAR', 'KPOINTS', 'CONTCAR',
+                  'OUTCAR', 'OSZICAR', 'vasprun.xml']
+    for file in vasp_files:
+        if not os.path.isfile(work_path + file):
+            logger.error('Not found ' + work_path + file)
+            raise SystemExit(1)
+        os.rename(work_path + file, work_path + f'stage{stage}_' + file)
+
+    # ---------- cp CONTCAR POSCAR
+    shutil.copyfile(work_path + f'stage{stage}_CONTCAR',
+                    work_path + 'POSCAR')
+
+    # ---------- remove STOPCAR
+    if os.path.isfile(work_path+'STOPCAR'):
+        os.remove(work_path+'STOPCAR')
+
+    # ---------- KPOINTS for the next stage using pymatgen
+    try:
+        structure = Structure.from_file(work_path+'POSCAR')
+    except ValueError:
+        skip_flag = True
+        kpt_data[cid].append(['skip'])
+        pkl_data.save_kpt(kpt_data)
+        out_kpts(kpt_data)
+        logger.info(f'    error in VASP,  skip structure {cid}')
+        return skip_flag, kpt_data
+    # kppvol[0]: <--> stage 1, kppvol[1] <--> stage2, ...
+    #   so (stage - 1): current stage, stage: next stage in kppvol
+    kpoints = Kpoints.automatic_density_by_vol(structure=structure,
+                                               kppvol=rin.kppvol[stage],
+                                               force_gamma=rin.force_gamma)
+    kpoints.write_file(work_path+'KPOINTS')
+
+    # ---------- kpt_data
+    kpt_data[cid].append(kpoints.kpts[0])
+    pkl_data.save_kpt(kpt_data)
+    out_kpts(kpt_data)
+
+    # ---------- cp INCAR_? from ./calc_in for the next stage: (stage + 1)
+    fincar = f'./calc_in/INCAR_{stage + 1}'
+    shutil.copyfile(fincar, work_path+'INCAR')
+
+    # ---------- return
+    return skip_flag, kpt_data
+
+
+def next_struc_vasp(rin, structure, cid, work_path, kpt_data):
+    # ---------- copy files
+    calc_inputs = ['POTCAR', 'INCAR']
+    for f in calc_inputs:
+        ff = f+'_1' if f == 'INCAR' else f
+        if not os.path.isfile('./calc_in/' + ff):
+            logger.error('Could not find ./calc_in/' + ff)
+            raise SystemExit(1)
+        # ------ e.g. cp ./calc_in/INCAR_1 work/1/INCAR
+        shutil.copyfile('./calc_in/'+ff, work_path+f)
+
+    # ---------- generate POSCAR
+    structure.to(fmt='poscar', filename=work_path+'POSCAR')
+    if not os.path.isfile(work_path+'POSCAR'):
+        logger.error(f'Could not find {work_path}POSCAR')
+        raise SystemExit(1)
+
+    # ---------- Change the title of POSCAR
+    with open(work_path+'POSCAR', 'r') as f:
+        lines = f.readlines()
+    lines[0] = f'ID_{cid}\n'
+    with open(work_path+'POSCAR', 'w') as f:
+        for line in lines:
+            f.write(line)
+
+    # ---------- generate KPOINTS using pymatgen
+    kpoints = Kpoints.automatic_density_by_vol(structure=structure,
+                                               kppvol=rin.kppvol[0],
+                                               force_gamma=rin.force_gamma)
+    kpoints.write_file(work_path+'KPOINTS')
+
+    # ---------- kpt_data
+    kpt_data[cid] = []    # initialize
+    kpt_data[cid].append(kpoints.kpts[0])
+    pkl_data.save_kpt(kpt_data)
+    out_kpts(kpt_data)
 
     # ---------- return
-    return init_struc_data
+    return kpt_data
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/EA/ea_child.py` & `csp_cryspy-1.3.0/src/cryspy/EA/ea_child.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,296 @@
 from logging import getLogger
 
-from .gen_struc_EA.crossover import Crossover
-from .gen_struc_EA.ea_generation import EA_generation
-from .gen_struc_EA.permutation import Permutation
-from .gen_struc_EA.rotation import Rotation
-from .gen_struc_EA.strain import Strain
-from .gen_struc_EA.addition import Addition
-from .gen_struc_EA.elimination import Elimination
-from .gen_struc_EA.substitution import Substitution
+from .gen_struc_EA.select_parents import SelectParents
+from .gen_struc_EA.crossover import gen_crossover
+from .gen_struc_EA.permutation import gen_permutation
+from .gen_struc_EA.strain import gen_strain
+from .gen_struc_EA.addition import gen_addition
+from .gen_struc_EA.elimination import gen_elimination
+from .gen_struc_EA.substitution import gen_substitution
+#from .gen_struc_EA.rotation import gen_rotation
 from ..IO import pkl_data
-from ..IO import read_input as rin
 from ..IO.out_results import out_nat_data
+from ..RS.rs_gen import gen_random
 from ..util.utility import check_fwpath
-from ..util.struc_util import set_mindist, out_poscar, get_nat
+from ..util.struc_util import set_mindist, get_mol_data, out_poscar, get_nat
 
 # ---------- import later
-#from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
-#from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
+#from ..RS.gen_struc_RS import gen_pyxtal
+#from ..RS.gen_struc_RS import random_generation
 
 
 logger = getLogger('cryspy')
 
-def child_gen(sp, init_struc_data, struc_mol_id=None, ea_vc_data=None):
-    # ---------- instantiate EA_generation class
-    eagen = EA_generation(sp=sp, id_start=rin.tot_struc,
-                          init_pos_path='./data/init_POSCARS')
+
+def child_gen(rin, ranking, fittest, struc_data, init_struc_data,
+              struc_mol_id=None, ea_vc_data=None):
+
+    # ---------- instantiate SelectParents class
+    sp = SelectParents(ranking)    # after set_xxx, we can use sp.get_parents(n_parent)
+    if rin.slct_func == 'TNM':
+        sp.set_tournament(rin.t_size)
+    else:
+        sp.set_roulette(fittest, rin.a_rlt, rin.b_rlt, rin.fit_reverse)
+        logger.debug(f'cumulative fitness in roulette: {sp.cum_fit}')
 
     # ---------- set mindist
-    logger.info('# mindist')
-    mindist = set_mindist(rin.mindist, rin.mindist_factor)
+    logger.info('# -- mindist')
+    mindist = set_mindist(rin.atype, rin.mindist, rin.mindist_factor, rin.struc_mode)
     if rin.struc_mode == 'mol_bs':
-        mindist_dummy = set_mindist(rin.mindist_mol_bs, rin.mindist_mol_bs_factor)
+        mindist_dummy = set_mindist(rin.atype,
+                                    rin.mindist_mol_bs,
+                                    rin.mindist_mol_bs_factor,
+                                    rin.struc_mode,
+                                    dummy=True,
+                                    mol_file=rin.mol_file,
+                                    mpi_rank=0)
+    # ---------- initialize
+    children = {}
+    #children_mol_id = {}
+    parents = {}
+    operation = {}
+    id_start = rin.tot_struc
+    vc = True if rin.algo == 'EA-vc' else False
 
-    # ------ Crossover
+    # ---------- Crossover
     if rin.n_crsov > 0:
         if rin.struc_mode not in ['mol', 'mol_bs']:
-            co = Crossover(mindist)
-            eagen.gen_crossover(co, None, molecular=False)
+            co_children, co_parents, co_operation = gen_crossover(
+                rin.atype,
+                rin.nat,
+                mindist,
+                struc_data,
+                sp,
+                rin.n_crsov,
+                id_start,
+                rin.symprec,
+                rin.crs_lat,
+                rin.nat_diff_tole,
+                rin.maxcnt_ea,
+                vc,
+                rin.ll_nat,
+                rin.ul_nat,
+                struc_mol_id=None,
+                molecular=False,
+            )
         else:
-            co = Crossover(mindist)
-            eagen.gen_crossover(co, struc_mol_id, molecular=True)
+            logger.error('Crossover is not implemented for mol or mol_bs')
+            # co = Crossover(rin, mindist)
+            # eagen.gen_crossover(rin, co, struc_mol_id, molecular=True)
+        # ------ update
+        children.update(co_children)
+        parents.update(co_parents)
+        operation.update(co_operation)
+        id_start += rin.n_crsov
 
-    # ------ Permutation
+    # ---------- Permutation
     if rin.n_perm > 0:
         if rin.struc_mode not in ['mol', 'mol_bs']:
-            pm = Permutation(mindist)
-            eagen.gen_permutation(pm, None, molecular=False)
+            pm_children, pm_parents, pm_operation = gen_permutation(
+                rin.atype,
+                mindist,
+                struc_data,
+                sp,
+                rin.n_perm,
+                id_start,
+                rin.symprec,
+                rin.ntimes,
+                rin.maxcnt_ea,
+                struc_mol_id=None,
+                molecular=False,
+            )
         else:
-            pm = Permutation(mindist)
-            eagen.gen_permutation(pm, struc_mol_id, molecular=True)
+            logger.error('Permutation is not implemented for mol or mol_bs')
+            # pm = Permutation(mindist)
+            # eagen.gen_permutation(rin, pm, struc_mol_id, molecular=True)
+        # ------ update
+        children.update(pm_children)
+        parents.update(pm_parents)
+        operation.update(pm_operation)
+        id_start += rin.n_perm
 
-    # ------ Strain
+    # ---------- Strain
     if rin.n_strain > 0:
         if rin.struc_mode not in ['mol', 'mol_bs']:
-            st = Strain(mindist)
-            eagen.gen_strain(st, None)
+            st_children, st_parents, st_operation = gen_strain(
+                rin.atype,
+                mindist,
+                struc_data,
+                sp,
+                rin.n_strain,
+                id_start,
+                rin.symprec,
+                rin.sigma_st,
+                rin.maxcnt_ea,
+                struc_mol_id=None,
+                molecular=False,
+                protect_mol_struc=True,
+            )
         else:
-            st = Strain(mindist)
-            eagen.gen_strain(st, struc_mol_id, protect_mol_struc=True)
+            logger.error('Strain is not implemented for mol or mol_bs')
+            # st = Strain(mindist)
+            # eagen.gen_strain(rin, st, struc_mol_id, protect_mol_struc=True)
+        # ------ update
+        children.update(st_children)
+        parents.update(st_parents)
+        operation.update(st_operation)
+        id_start += rin.n_strain
 
-    # ------ EA-vc
+    # ---------- EA-vc
     if rin.algo == 'EA-vc':
-        nat_data, _, _ = ea_vc_data
+        nat_data, ratio_data, _ = ea_vc_data
 
-        # -- Addition
+        # ------ Addition
         if rin.n_add > 0:
             if rin.struc_mode not in ['mol', 'mol_bs']:
-                ad = Addition(mindist, rin.target)
-                eagen.gen_addition(ad, nat_data)
+                ad_children, ad_parents, ad_operation = gen_addition(
+                    rin.atype,
+                    mindist,
+                    struc_data,
+                    sp,
+                    rin.n_add,
+                    nat_data,
+                    rin.ul_nat,
+                    id_start,
+                    rin.symprec,
+                    rin.maxcnt_ea,
+                    rin.target,
+                )
             else:
+                logger.error('Addition is not implemented for mol or mol_bs')
                 raise SystemExit(1)
+            # ------ update
+            children.update(ad_children)
+            parents.update(ad_parents)
+            operation.update(ad_operation)
+            id_start += rin.n_add
 
-        # -- Elimination
+        # ------ Elimination
         if rin.n_elim > 0:
             if rin.struc_mode not in ['mol', 'mol_bs']:
-                el = Elimination(mindist, rin.target)
-                eagen.gen_elimination(el, nat_data)
+                el_children, el_parents, el_operation = gen_elimination(
+                    rin.atype,
+                    struc_data,
+                    sp,
+                    rin.n_elim,
+                    nat_data,
+                    rin.ll_nat,
+                    id_start,
+                    rin.symprec,
+                    rin.target,
+                )
             else:
+                logger.error('Elimination is not implemented for mol or mol_bs')
                 raise SystemExit(1)
+            # ------ update
+            children.update(el_children)
+            parents.update(el_parents)
+            operation.update(el_operation)
+            id_start += rin.n_elim
 
-        # -- Substitution
+        # ------ Substitution
         if rin.n_subs > 0:
             if rin.struc_mode not in ['mol', 'mol_bs']:
-                su = Substitution(mindist, rin.target)
-                eagen.gen_substitution(su, nat_data)
+                sb_children, sb_parents, sb_operation = gen_substitution(
+                    rin.atype,
+                    mindist,
+                    struc_data,
+                    sp,
+                    rin.n_subs,
+                    nat_data,
+                    rin.ll_nat,
+                    rin.ul_nat,
+                    id_start,
+                    rin.symprec,
+                    rin.maxcnt_ea,
+                    rin.target,
+                )
             else:
+                logger.error('Substitution is not implemented for mol or mol_bs')
                 raise SystemExit(1)
+            # ------ update
+            children.update(sb_children)
+            parents.update(sb_parents)
+            operation.update(sb_operation)
+            id_start += rin.n_subs
+
+    # ---------- Rotation
+    # if rin.struc_mode in ['mol', 'mol_bs']:
+    #     if rin.n_rotation > 0:
+    #         rot = Rotation(mindist)
+    #         eagen.gen_rotation(rin, struc_mol_id, rot=rot)
+
+    # ---------- write init_POSCARS
+    out_poscar(children, './data/init_POSCARS')
+
+    # ---------- update init_struc_data
+    init_struc_data.update(children)
+    # if rin.struc_mode in ['mol', 'mol_bs']:
+    #     struc_mol_id.update(children_mol_id)
 
-    # ------ Rotation
-    if rin.struc_mode in ['mol', 'mol_bs']:
-        if rin.n_rotation > 0:
-            rot = Rotation(mindist)
-            eagen.gen_rotation(struc_mol_id, rot=rot)
-
-    # ------ update init_struc_data
-    init_struc_data.update(eagen.offspring)
-    if rin.struc_mode in ['mol', 'mol_bs']:
-        struc_mol_id.update(eagen.offspring_mol_id)
-
-    # ------ save EA-vc_data.pkl
+    # ---------- save EA-vc_data.pkl
     if rin.algo == 'EA-vc':
-        nat_data, ratio_data, hdist_data = ea_vc_data
-        for cid, struc in eagen.offspring.items():
+        # ea_vc_data is already loaded above
+        for cid, struc in children.items():
             nat_data[cid], ratio_data[cid] = get_nat(struc, rin.atype)
-        ea_vc_data = (nat_data, ratio_data, hdist_data)
-        pkl_data.save_ea_vc_data(ea_vc_data)
+        pkl_data.save_nat_data(nat_data)
+        pkl_data.save_ratio_data(ratio_data)
 
     # ---------- random generation
     if rin.n_rand > 0:
-        # ------ pyxtal
-        if not (rin.spgnum == 0 or rin.use_find_wy):
-            from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
-            rsgx = Rnd_struc_gen_pyxtal(mindist=mindist)
-            # -- crystal
-            if rin.struc_mode == 'crystal':
-                if not rin.algo == 'EA-vc':
-                    rsgx.gen_struc(nstruc=rin.n_rand, id_offset=eagen.cid)
-                else:    # vc
-                    rsgx.gen_struc(nstruc=rin.n_rand, id_offset=eagen.cid, vc=True)
-            # -- molecular crystal
-            elif rin.struc_mode == 'mol':
-                rsgx.set_mol()
-                rsgx.gen_struc_mol(nstruc=rin.n_rand, id_offset=eagen.cid)
-            # ------ molecular crystal breaking symmetry
-            elif rin.struc_mode == 'mol_bs':
-                logger.info('# -- mindist_mol_bs')
-                mindist_dummy = set_mindist(rin.mindist_mol_bs, rin.mindist_mol_bs_factor, dummy=True)
-                rsgx.set_mol()
-                rsgx.gen_struc_mol_break_sym(nstruc=rin.n_rand,
-                                             mindist_dummy=mindist_dummy,
-                                             id_offset=eagen.cid)
-            # -- update
-            init_struc_data.update(rsgx.init_struc_data)
-            if rin.struc_mode in ['mol', 'mol_bs']:
-                struc_mol_id.update(rsgx.struc_mol_id)
-            # -- save EA-vc_data.pkl
-            if rin.algo == 'EA-vc':
-                # ea_vc_data is already loaded above
-                for cid, struc in rsgx.init_struc_data.items():
-                    nat_data[cid], ratio_data[cid] = get_nat(struc, rin.atype)
-                ea_vc_data = (nat_data, ratio_data, hdist_data)
-                pkl_data.save_ea_vc_data(ea_vc_data)
-            # -- init_POSCARS
-            for cid, struc in rsgx.init_struc_data.items():
-                out_poscar(struc, cid, './data/init_POSCARS')
-        # ------ Rnd_struc_gen
-        else:
-            from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
-            rsg = Rnd_struc_gen(mindist=mindist)
-            if rin.spgnum == 0:
-                if not rin.algo == 'EA-vc':
-                    rsg.gen_wo_spg(nstruc=rin.n_rand, id_offset=eagen.cid)
-                else:    # vc
-                    rsg.gen_wo_spg(nstruc=rin.n_rand, id_offset=eagen.cid, vc=True)
-            else:
-                fwpath = check_fwpath(rin.fwpath)
-                if not rin.algo == 'EA-vc':
-                    rsg.gen_with_find_wy(nstruc=rin.n_rand,
-                                         id_offset=eagen.cid,
-                                         fwpath=fwpath)
-                else:
-                    rsg.gen_with_find_wy(nstruc=rin.n_rand,
-                                         id_offset=eagen.cid,
-                                         fwpath=fwpath, vc=True)
-            # -- update
-            init_struc_data.update(rsg.init_struc_data)
-            # -- save EA-vc_data.pkl
-            if rin.algo == 'EA-vc':
-                # ea_vc_data is already loaded above
-                for cid, struc in rsg.init_struc_data.items():
-                    nat_data[cid], ratio_data[cid] = get_nat(struc, rin.atype)
-                ea_vc_data = (nat_data, ratio_data, hdist_data)
-                pkl_data.save_ea_vc_data(ea_vc_data)
-            # -- init_POSCARS
-            for cid, struc in rsg.init_struc_data.items():
-                out_poscar(struc, cid, './data/init_POSCARS')
+        tmp_struc_data, tmp_mol_id = gen_random(
+            rin,
+            rin.n_rand,
+            id_start,
+            comm=None,
+            mpi_rank=0,
+            mpi_size=1,
+        )
+        # ------ update
+        init_struc_data.update(tmp_struc_data)
+        # if rin.struc_mode in ['mol', 'mol_bs']:
+        #     struc_mol_id.update(tmp_mol_id)
+        # ------ save EA-vc_data.pkl
+        if rin.algo == 'EA-vc':
+            # ea_vc_data is already loaded above
+            for cid, struc in tmp_struc_data.items():
+                nat_data[cid], ratio_data[cid] = get_nat(struc, rin.atype)
+            pkl_data.save_nat_data(nat_data)
+            pkl_data.save_ratio_data(ratio_data)
+        # ------ write init_POSCARS
+        out_poscar(tmp_struc_data, './data/init_POSCARS')
 
     # ---------- save init_struc_data
     pkl_data.save_init_struc(init_struc_data)
-    if rin.struc_mode in ['mol', 'mol_bs']:
-        pkl_data.save_struc_mol_id(struc_mol_id)
+    # if rin.struc_mode in ['mol', 'mol_bs']:
+    #     pkl_data.save_struc_mol_id(struc_mol_id)
 
     # ---------- out nat_data
     if rin.algo == 'EA-vc':
         out_nat_data(nat_data, rin.atype)
 
     # ----------return
-    return init_struc_data, eagen, struc_mol_id
+    return init_struc_data, parents, operation
+    #return init_struc_data, parents, operation, struc_mol_id
 
 
 # not used in this version
 # this is used in adj_comp.py
-def check_vcnat(child):
-    from ..util.struc_util import get_nat
-    nat, ratio = get_nat(child,rin.atype)
-
-    if len(rin.atype) == 2:
-        for i in range(len(rin.atype)):
-            if (nat[i] >= rin.ll_nat[i]) and (nat[i]<= rin.ul_nat[i]):
-                check_nat = True
-            else:
-                #check_nat = False
-                return False
+# def check_vcnat(rin, child):
+#     from ..util.struc_util import get_nat
+#     nat, ratio = get_nat(child, rin.atype)
+
+#     if len(rin.atype) == 2:
+#         for i in range(len(rin.atype)):
+#             if (nat[i] >= rin.ll_nat[i]) and (nat[i]<= rin.ul_nat[i]):
+#                 check_nat = True
+#             else:
+#                 #check_nat = False
+#                 return False
 
-        return True
+#         return True
         
-    elif len(rin.atype) == 3:
-        SystemExit(1) #temporary
-    else:
-        SystemExit(1) #temporary
+#     elif len(rin.atype) == 3:
+#         SystemExit(1) #temporary
+#     else:
+#         SystemExit(1) #temporary
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/adj_comp.py` & `csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/adj_comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from logging import getLogger
 import random
 import numpy as np
 from pymatgen.transformations.site_transformations import ReplaceSiteSpeciesTransformation
 from ...IO import pkl_data
-from ...IO import read_input as rin
 from ...util.struc_util import get_nat
 
 
 logger = getLogger('cryspy')
 
 
-def convex_hull_check():
+def convex_hull_check(rin):
     '''
     convex hullのどの区間にどれくらいの構造があるかをカウントする
     とりあえずconvex hullを5分割して考える
     ''' 
     # どの区間にどれだけの構造があるかをカウントする
     nat_data, ratio_data = pkl_data.load_ea_vc_data()
     section = [0,0,0,0,0]
@@ -72,28 +71,28 @@
         else:
             rslt = tmp_arr[0]
         logger.info(f'tmp_arr: {tmp_arr}')
         logger.info(f'select_section: {rslt}')
 
     return rslt
 
-def operation_atoms(method,child, section):
+def operation_atoms(rin, method,child, section):
     """
     構造が少ないところをターゲットにして子構造生成を行う
     methondにはaddition, elimination, substitutionのいずれかを指定する
 
     section = 0 : 0<=x<0.2
     section = 1 : 0.2<=x<0.4
     section = 2 : 0.4<=x<0.6
     section = 3 : 0.6<=x<0.8
     section = 4 : 0.8<=x<=1.0
     """
     # どの区間に対して子構造を生成するかを決める
     # 候補が多い場合はランダムで一つ決める
-    #section = convex_hull_check()
+    #section = convex_hull_check(rin)
     
     nat,ratio = get_nat(child,rin.atype)
     ratio = ratio[0]
     # ---------- addition
     if method == 'addition':
         logger.info(' ---------- addition')
         cnt = 0
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/strain.py` & `csp_cryspy-1.3.0/src/cryspy/EA/gen_struc_EA/strain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,150 @@
-'''
-Strain class
-'''
 from logging import getLogger
-import sys
 
 import numpy as np
 from pymatgen.core import Structure
 from pymatgen.core.periodic_table import DummySpecie
 
-from ...IO import read_input as rin
 from ...util.struc_util import sort_by_atype, sort_by_atype_mol, check_distance, cal_g, find_site
 
 
 logger = getLogger('cryspy')
 
-class Strain:
+
+def gen_strain(
+        atype,
+        mindist,
+        struc_data,
+        sp,
+        n_strain,
+        id_start=None,
+        symprec=0.01,
+        sigma_st=0.5,
+        maxcnt_ea=50,
+        struc_mol_id=None,
+        molecular=False,
+        protect_mol_struc=True,
+    ):
+    '''
+
+        tuple may be replaced by list
+
+    atype (tuple): e.g. ('Na', 'Cl')
+    mindist (tuple): minimum interatomic distance, e.g. ((1.5, 1.5), (1.5, 1.5))
+    struc_data (dict): {id: structure data}
+    sp (instance): instance of SelectParents class
+    n_strain (int): number of structures to generate by strain
+    id_start (int): start ID for new structures
+    symprec (float): tolerance for symmetry
+    sigma_st (float): standard deviation for strain matrix
+    maxcnt_ea (int): maximum number of trial in permutation
+
+    # ---------- return
+    children (dict): {id: structure data}
+    parents (dict): {id: (id of parent_A, )}
+    operation (dict): {id: 'strain'}
     '''
-    strain
+    # ---------- initialize
+    struc_cnt = 0
+    children = {}
+    #children_mol_id = {}
+    parents = {}
+    operation = {}
+
+    # ---------- id_offset
+    if id_start is None:
+        cid = max(struc_data.keys()) + 1
+    else:
+        if id_start < (max(struc_data.keys()) + 1):
+            logger.error('id_start is already included in structure ID of the data')
+        else:
+            cid = id_start
+
+    # ---------- generate structures by strain
+    while struc_cnt < n_strain:
+        # ------ select parents
+        pid_A, = sp.get_parents(n_parent=1)    # comma for list[0]
+        parent_A = struc_data[pid_A]
+        # ------ generate child
+        if molecular:
+            logger.error('protect_mol_struc is not implemented yet.')
+            # if protect_mol_struc:
+                # child, mol_id = gen_child_mol(rin,
+                #                                     struc_data[pid],
+                #                                     struc_mol_id[pid])
+            #else:
+            #    child = gen_child(atype, mindist, parent_struc, sigma_st, maxcnt_ea)
+        else:
+            child = gen_child(atype, mindist, parent_A, sigma_st, maxcnt_ea)
+        # ------ success
+        if child is not None:
+            children[cid] = child
+            # if molecular:
+            #     children_mol_id[cid] = mol_id
+            parents[cid] = (pid_A, )    # tuple
+            operation[cid] = 'strain'
+            try:
+                spg_sym, spg_num = child.get_space_group_info(symprec=symprec)
+            except TypeError:
+                spg_num = 0
+                spg_sym = None
+            logger.info(f'Structure ID {cid:>6} was generated'
+                    f' from {pid_A:>6} by strain.'
+                    f' Space group: {spg_num:>3} {spg_sym}')
+            cid += 1
+            struc_cnt += 1
 
-    # ---------- instance methods
-    gen_child(self, struc)
+    # ---------- return
+    return children, parents, operation
+
+
+def gen_child(atype, mindist, parent_A, sigma_st=0.5, maxcnt_ea=50):
     '''
 
-    def __init__(self, mindist):
-        self.mindist = mindist
+        tuple may be replaced by list
+
+    atype (tuple): e.g. ('Na', 'Cl')
+    mindist (tuple): minimum interatomic distance, e.g. ((1.5, 1.5), (1.5, 1.5))
+    parent_A (Structure): pymatgen Structure object
+    sigma_st (float): standard deviation for strain matrix
+    maxcnt_ea (int): maximum number of trial in crossover
+
+    # ---------- return
+    (if success) child (Structure): pymatgen Structure object
+    (if fail) None
+    '''
+    # ---------- initialize
+    child = parent_A.copy()    # keep original structure
+    lat_mat = child.lattice.matrix.T    # lattice vector as matrix
+    cnt = 0
+
+    # ---------- generate strained structure
+    while True:
+        # ------ strain matrix
+        strain_matrix = np.empty([3, 3])
+        for i in range(3):
+            for j in range(3):
+                if i <= j:
+                    if i == j:
+                        strain_matrix[i][j] = 1.0 + np.random.normal(loc=0.0, scale=sigma_st)
+                    else:
+                        strain_matrix[i][j] = np.random.normal(loc=0.0, scale=sigma_st)/2.0
+                        strain_matrix[j][i] = strain_matrix[i][j]
+        # ------ strained lattice
+        strained_lattice = np.dot(strain_matrix, lat_mat).T
+        # ------ child
+        child = Structure(strained_lattice, child.species, child.frac_coords)
+        # ------ scale lattice
+        child.scale_lattice(parent_A.volume)
+        # ------ check distance
+        success, mindist_ij, dist = check_distance(child, atype, mindist)
+        if success:
+            child = sort_by_atype(child, atype)
+            return child
+        else:
+            type0 = atype[mindist_ij[0]]
+            type1 = atype[mindist_ij[1]]
+            logger.warning(f'mindist in strain: {type0} - {type1}, {dist}. retry.')
+            cnt += 1
+            if cnt >= maxcnt_ea:
+                return None    # change parent
 
-    def gen_child(self, struc):
-        '''
-        generate child struture
-
-        # ---------- return
-        (if success) self.child:
-        (if fail) None:
-        '''
-        # ---------- init
-        cnt = 0
-        lat_mat = struc.lattice.matrix.T    # lattice vector as matrix
-        # ---------- generate strained structure
-        while True:
-            # ------ strain matrix
-            strain_matrix = np.empty([3, 3])
-            for i in range(3):
-                for j in range(3):
-                    if i <= j:
-                        if i == j:
-                            strain_matrix[i][j] = 1.0 + np.random.normal(
-                                loc=0.0, scale=rin.sigma_st)
-                        else:
-                            strain_matrix[i][j] = np.random.normal(
-                                loc=0.0, scale=rin.sigma_st)/2.0
-                            strain_matrix[j][i] = strain_matrix[i][j]
-            # ------ strained lattice
-            strained_lattice = np.dot(strain_matrix, lat_mat).T
-            # ------ child
-            self.child = Structure(strained_lattice, struc.species,
-                                   struc.frac_coords)
-            # ------ scale lattice
-            self.child.scale_lattice(struc.volume)
-            # ------ check distance
-            success, mindist_ij, dist = check_distance(self.child,
-                                                       rin.atype,
-                                                       self.mindist)
-            if success:
-                self.child = sort_by_atype(self.child, rin.atype)
-                return self.child
-            else:
-                type0 = rin.atype[mindist_ij[0]]
-                type1 = rin.atype[mindist_ij[1]]
-                logger.warning(f'mindist in strain: {type0} - {type1}, {dist}. retry.')
-                cnt += 1
-                if cnt >= rin.maxcnt_ea:
-                    self.child = None
-                    return None    # change parent
-
-    def gen_child_mol(self, struc, mol_id):
-        '''
-        generate child structures for mol
-
-        # ---------- return
-        (if success) self.child:
-        (if fail) None:
-        '''
-        # ---------- init
-        cnt = 0
-        lat_mat = struc.lattice.matrix.T    # lattice vector as matrix
-        # ---------- generate strained structure
-        while True:
-            # ------ strain matrix
-            strain_matrix = np.empty([3, 3])
-            for i in range(3):
-                for j in range(3):
-                    if i <= j:
-                        if i == j:
-                            strain_matrix[i][j] = 1.0 + np.random.normal(
-                                loc=0.0, scale=rin.sigma_st)
-                        else:
-                            strain_matrix[i][j] = np.random.normal(
-                                loc=0.0, scale=rin.sigma_st)/2.0
-                            strain_matrix[j][i] = strain_matrix[i][j]
-            # ------ strained lattice
-            strained_lattice = np.dot(strain_matrix, lat_mat).T
-            # -- generate dummy structure
-            dum_coords = cal_g(struc, mol_id[0], mol_id[1], mol_id[2])
-            dum_species = []
-            for i in range(len(dum_coords)):
-                dum_species.append(DummySpecie("X{}".format(i)))
-            dum_struc = Structure(strained_lattice, dum_species, dum_coords)
-            # ------ scale lattice
-            dum_struc.scale_lattice(struc.volume)
-            # --calcurate atom coords to replace molecure
-            fix_frac_coords, fix_group_id, fix_species, fix_mol_id = find_site(struc,
-                                                                               mol_id[0],
-                                                                               mol_id[1],
-                                                                               mol_id[2])
-            rm_spe = []
-            strained_mol_id = []
-            strained_group_id = []
-            append_spe_co = []
-            append_mol_gr = []
-            for i, dum in enumerate(dum_struc):
-                for j, mid in enumerate(fix_group_id):
-                    if mid == i:
-                        coord = (struc.lattice.get_cartesian_coords(fix_frac_coords[j])
-                                 - struc.lattice.get_cartesian_coords(dum_coords[i])
-                                 + dum_struc.cart_coords[i])
-                        append_spe_co.append([fix_species[j], coord])
-                        append_mol_gr.append([fix_mol_id[j], fix_group_id[j]])
-                rm_spe.append(dum.specie)
-            # replace mol
-            for spe_co, mol_gr in zip(append_spe_co, append_mol_gr):
-                dum_struc.append(spe_co[0], spe_co[1], coords_are_cartesian=True)
-                strained_mol_id.append(mol_gr[0])
-                strained_group_id.append(mol_gr[1])
-            # remove dummy
-            dum_struc.remove_species(rm_spe)
-            # ------ child
-            self.child = dum_struc
-            # ------ check distance
-            success, mindist_ij, dist = check_distance(self.child,
-                                                       rin.atype,
-                                                       self.mindist)
-            if success:
-                self.child, self.mol_id, self.group_id = sort_by_atype_mol(self.child, rin.atype,
-                                                                           strained_mol_id, strained_group_id)
-                return self.child, [self.mol_id, self.group_id, mol_id[2]]
-            else:
-                type0 = rin.atype[mindist_ij[0]]
-                type1 = rin.atype[mindist_ij[1]]
-                logger.warning(f'mindist in permutation: {type0} - {type1}, {dist}. retry.')
-                cnt += 1
-                if cnt >= rin.maxcnt_ea:
-                    self.child = None
-                    return None    # change parent
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/LAQA/calc_score.py` & `csp_cryspy-1.3.0/src/cryspy/LAQA/calc_score.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_init.py` & `csp_cryspy-1.3.0/src/cryspy/LAQA/laqa_init.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-'''
-Initialize LAQA
-'''
-
 from logging import getLogger
 
 from ..IO import io_stat, pkl_data
-from ..IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def initialize(stat):
+def initialize(rin):
     logger.info('# ---------- Initialize LAQA')
 
     # ---------- initialize
     tot_step_select = [0]
     laqa_step = {}
     laqa_struc = {}
     laqa_energy = {}
@@ -27,21 +22,26 @@
         laqa_bias[i] = []
         laqa_score[i] = [float('inf')]
     id_queueing = [i for i in range(rin.tot_struc)]
     id_select_hist = []
     id_running = []
 
     # ---------- save for LAQA
-    laqa_id_data = (id_queueing, id_running, id_select_hist)
-    pkl_data.save_laqa_id(laqa_id_data)
-    laqa_data = (tot_step_select, laqa_step, laqa_struc,
-                 laqa_energy, laqa_bias, laqa_score)
-    pkl_data.save_laqa_data(laqa_data)
+    pkl_data.save_id_queueing(id_queueing)
+    pkl_data.save_id_running(id_running)
+    pkl_data.save_id_select_hist(id_select_hist)
+    pkl_data.save_tot_step_select(tot_step_select)
+    pkl_data.save_laqa_step(laqa_step)
+    pkl_data.save_laqa_struc(laqa_struc)
+    pkl_data.save_laqa_energy(laqa_energy)
+    pkl_data.save_laqa_bias(laqa_bias)
+    pkl_data.save_laqa_score(laqa_score)
 
     # ---------- status
+    stat = io_stat.stat_read()
     io_stat.set_common(stat, 'selection', 0)
     io_stat.set_common(stat, 'total_step', 0)
     io_stat.set_id(stat, 'selected_id', id_queueing)    # all IDs
     io_stat.set_id(stat, 'id_queueing', id_queueing)    # all IDs
     io_stat.write_stat(stat)
 
     # ---------- log
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_next_selection.py` & `csp_cryspy-1.3.0/src/cryspy/LAQA/laqa_next_selection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-'''
-Selection in LAQA
-'''
-
 from logging import getLogger
 import os
 
 from ..IO import io_stat, pkl_data
-from ..IO import read_input as rin
 from ..IO.out_results import out_laqa_id_hist
 
 
 logger = getLogger('cryspy')
 
-def next_selection(stat, laqa_id_data, laqa_data):
+
+def next_selection(rin, laqa_id_data, laqa_data):
     # ---------- laqa_id_data and laqa_data
     (id_queueing, id_running, id_select_hist) = laqa_id_data
     (tot_step_select, laqa_step, laqa_struc,
      laqa_energy, laqa_bias, laqa_score) = laqa_data
 
     # ---------- LAQA selection
     for k, v in sorted(laqa_score.items(), key=lambda x: -x[1][-1]):
@@ -37,21 +33,26 @@
     id_select_hist.append(id_queueing[:])    # append shallow copy
     out_laqa_id_hist(id_select_hist)
 
     # ---------- tot_step_select for next selection
     tot_step_select.append(0)
 
     # ---------- save
-    laqa_id_data = (id_queueing, id_running, id_select_hist)
-    pkl_data.save_laqa_id(laqa_id_data)
-    laqa_data = (tot_step_select, laqa_step, laqa_struc,
-                 laqa_energy, laqa_bias, laqa_score)
-    pkl_data.save_laqa_data(laqa_data)
+    pkl_data.save_id_queueing(id_queueing)
+    pkl_data.save_id_running(id_running)
+    pkl_data.save_id_select_hist(id_select_hist)
+    pkl_data.save_tot_step_select(tot_step_select)
+    pkl_data.save_laqa_step(laqa_step)
+    pkl_data.save_laqa_struc(laqa_struc)
+    pkl_data.save_laqa_energy(laqa_energy)
+    pkl_data.save_laqa_bias(laqa_bias)
+    pkl_data.save_laqa_score(laqa_score)
 
     # ---------- status
+    stat = io_stat.stat_read()
     io_stat.set_common(stat, 'selection', len(id_select_hist))
     io_stat.set_id(stat, 'selected_id', id_queueing)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- out and log
     logger.info(f'# ---------- Selection {len(id_select_hist)}')
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py` & `csp_cryspy-1.3.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,533 +1,651 @@
 '''
 Random structure generation using PyXtal (https://github.com/qzhu2017/PyXtal)
 '''
-
 import collections
 from contextlib import redirect_stdout, redirect_stderr
 from io import StringIO
 from logging import getLogger
 from multiprocessing import Process, Queue
-import os
 import random
 import sys
 
 import numpy as np
-from pymatgen.core import Structure, Molecule
+from pymatgen.core import Structure
 from pymatgen.core.periodic_table import DummySpecie
 from pyxtal import pyxtal
-from pyxtal.database.collection import Collection
 from pyxtal.tolerance import Tol_matrix
 
 from ...util.struc_util import check_distance, sort_by_atype, get_nat
 from ...util.struc_util import get_atype_dummy, scale_cell_mol, rot_mat
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-class Rnd_struc_gen_pyxtal:
+
+def gen_struc(
+        nstruc,
+        atype,
+        nat,
+        mindist,
+        spgnum,
+        symprec=0.01,
+        id_offset=0,
+        vol_factor=1.1,
+        vol_mu=None,
+        vol_sigma=None,
+        vc=False,
+        ll_nat=None,
+        ul_nat=None
+    ):
     '''
-    Random structure generation using pyxtal
+    Generate random structures for given space groups
+
+        tuple may be replaced by list
+
+    # ---------- args
+    nstruc (int): number of structures to be generated
+    atype (tuple): atom type (e.g. ('Na', 'Cl'))
+    nat (tuple): number of atoms (e.g. (4, 4)), None if vc=True
+    mindist (): minimum interatomic distance (e.g. ((2.0, 1.5), (1.5, 2.0)))
+    spgnum (str, int, or tuple): space group number 'all', 0, or tuple of space group numbers
+    symprec (float): symmetry tolerance
+    id_offset (int): structure ID starts from id_offset
+                        e.g. nstruc = 3, id_offset = 10
+                             you obtain ID 10, ID 11, ID 12
+    vol_factor (float): volume factor for structure generation
+    vol_mu (float): mean for volume scaling
+    vol_sigma (float): standard deviation for volume scaling
+    vc (bool): variable composition. it needs ll_nat and ul_nat
+    ll_nat (tuple): lower limit of number of atoms (e.g. (1, 1))
+    ul_nat (tuple): upper limit of number of atoms (e.g. (8, 8))
+
+    # ---------- return
+    init_struc_data (dict): {ID: pymatgen Structure, ...}
     '''
 
-    def __init__(self, mindist):
-        self.mindist = mindist
+    # ---------- initialize
+    init_struc_data = {}
 
-    def set_mol(self):
-        '''
-        set molecule files and number of molecules
-        '''
-        # ----------
-        mol_data = []
-        pyxtal_mol_data = Collection('molecules')
-        pyxtal_mol_names = list(Collection('molecules'))
-        for i, mf in enumerate(rin.mol_file):
-            if os.path.isfile(mf):
-                mol = Molecule.from_file(mf)
-            elif mf in pyxtal_mol_names:
-                mol = pyxtal_mol_data[mf]
-            else:
-                logger.error('no molecular files')
-                raise SystemExit(1)
-            mol_data.append(mol)
-        # ---------- self.xxx
-        self.mol_data = mol_data
-
-    def gen_struc(self, nstruc, id_offset=0, vc=False):
-        '''
-        Generate random structures for given space groups
-
-        # ---------- args
-        nstruc (int): number of generated structures
-
-        id_offset (int): default: 0
-                         structure ID starts from id_offset
-                         e.g. nstruc = 3, id_offset = 10
-                              you obtain ID 10, ID 11, ID 12
-
-        vc (bool): variable composition. it needs ll_nat and ul_nat
-
-        # ---------- comment
-        generated structure data are saved in self.init_struc_data
-        '''
-        # ---------- initialize
-        self.init_struc_data = {}
-        # ---------- Tol_matrix
-        tolmat = self._set_tol_mat(rin.atype, self.mindist)
-        # ---------- loop for structure generattion
-        while len(self.init_struc_data) < nstruc:
-            # ------ spgnum --> spg
-            if rin.spgnum == 'all':
-                spg = random.randint(1, 230)
-            else:
-                spg = random.choice(rin.spgnum)
-            # ------ vol_factor
-            rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
-            # ------ generate structure
-            tmp_crystal = pyxtal()
-            if not vc:
-                numIons = rin.nat
-            else:    # variable composition
-                numIons = [random.randint(l, u) for l, u in zip(rin.ll_nat, rin.ul_nat)]
+    # ---------- Tol_matrix
+    tolmat = _set_tol_mat(atype, mindist)
+
+    # ---------- loop for structure generation
+    while len(init_struc_data) < nstruc:
+        # ------ spgnum --> spg
+        if spgnum == 'all':
+            spg = random.randint(1, 230)
+        else:
+            spg = random.choice(spgnum)
+        # ------ generate structure
+        tmp_crystal = pyxtal()
+        if not vc:
+            numIons = nat
+        else:    # variable composition
+            numIons = [random.randint(l, u) for l, u in zip(ll_nat, ul_nat)]
+            numIons = tuple(numIons)
+        try:
+            f = StringIO()    # to get output from pyxtal
+            with redirect_stdout(f):
+                tmp_crystal.from_random(dim=3, group=spg, species=atype,
+                                        numIons=numIons, factor=vol_factor,
+                                        conventional=False, tm=tolmat)
+            s = f.getvalue().rstrip()    # to delete \n
+            if s:
+                logger.warning(s)
+        except Exception as e:
+            logger.warning(f'{e}:     spg = {spg} retry.')
+            continue
+        if tmp_crystal.valid:
+            tmp_struc = tmp_crystal.to_pymatgen(resort=False)
+            tmp_nat, _ = get_nat(tmp_struc, atype)
+            # -- check the number of atoms
+            if tmp_nat != numIons:
+                # (pyxtal 0.1.4) cryspy adopts "conventional=False",
+                #     which is better for DFT calculation
+                # pyxtal returns conventional cell, that is, too many atoms
+                tmp_struc = tmp_struc.get_primitive_structure()
+                # recheck nat
+                if tmp_nat != numIons:    # failure
+                    continue
+            # -- sort, just in case
+            tmp_struc = sort_by_atype(tmp_struc, atype)
+            # -- scale volume
+            if vol_mu is not None:
+                vol = random.gauss(mu=vol_mu, sigma=vol_sigma)
+                tmp_struc.scale_lattice(volume=vol)
+            # -- check actual space group
             try:
-                f = StringIO()
+                spg_sym, spg_num = tmp_struc.get_space_group_info(
+                    symprec=symprec)
+            except TypeError:
+                spg_num = 0
+                spg_sym = None
+            # -- tmp_struc --> init_struc_data
+            cid = len(init_struc_data) + id_offset
+            init_struc_data[cid] = tmp_struc
+            logger.info(f'Structure ID {cid:>6}: {numIons}'
+                    f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
+
+    # ---------- return
+    return init_struc_data
+
+
+def gen_struc_mol(
+        nstruc,
+        atype,
+        nat,
+        mindist,
+        spgnum,
+        mol_data,
+        nmol,
+        symprec=0.01,
+        id_offset=0,
+        vol_factor=1.1,
+        vol_mu=None,
+        vol_sigma=None,
+        timeout_mol=None,
+    ):
+    '''
+    Generate random molecular crystal structures for given space groups
+
+    # ---------- args
+    nstruc (int): number of structures to be generated
+    atype (tuple): atom type (e.g. ('Na', 'Cl'))
+    nat (tuple): number of atoms (e.g. (4, 4))
+    mindist (): minimum interatomic distance (e.g. ((2.0, 1.5), (1.5, 2.0)))
+    spgnum (str, int, or tuple): space group number 'all', 0, or tuple of space group numbers
+    mol_data (tuple or list): pymatgen Molecule data
+    nmol (tuple): number of molecules (e.g. (4, 4))
+    symprec (float): symmetry tolerance
+    id_offset (int): structure ID starts from id_offset
+                        e.g. nstruc = 3, id_offset = 10
+                            you obtain ID 10, ID 11, ID 12
+    vol_factor (float): volume factor for structure generation
+    vol_mu (float): mean for volume scaling
+    vol_sigma (float): standard deviation for volume scaling
+    timeout_mol (None or float): if float, timeout for molecular structure generation
+
+    # ---------- return
+    init_struc_data (dict): {ID: pymatgen Structure, ...}
+    struc_mol_id (dict):    not implemented yet, just return vacant dict for now
+    '''
+
+    # ---------- initialize
+    init_struc_data = {}
+    struc_mol_id = {}    # for EA and mol, not implemented yet
+
+    # ---------- Tol_matrix
+    tolmat = _set_tol_mat(atype, mindist)
+
+    # ---------- loop for structure generattion
+    while len(init_struc_data) < nstruc:
+        # ------ spgnum --> spg
+        if spgnum == 'all':
+            spg = random.randint(1, 230)
+        else:
+            spg = random.choice(spgnum)
+        # ------ generate structure
+        if timeout_mol is None:
+            tmp_crystal = pyxtal(molecular=True)
+            try:
+                f = StringIO()    # to get output from pyxtal
                 with redirect_stdout(f):
-                    tmp_crystal.from_random(dim=3, group=spg, species=rin.atype,
-                                            numIons=numIons, factor=rand_vol,
-                                            conventional=False, tm=tolmat)
+                    tmp_crystal.from_random(
+                        dim=3,
+                        group=spg,
+                        species=mol_data,
+                        numIons=nmol,
+                        factor=vol_factor,
+                        conventional=False,
+                        tm=tolmat
+                    )
                 s = f.getvalue().rstrip()    # to delete \n
                 if s:
                     logger.warning(s)
+                tmp_valid = tmp_crystal.valid
+                if tmp_valid:
+                    tmp_struc = tmp_crystal.to_pymatgen(resort=False)
             except Exception as e:
-                logger.warning(str(e.args[0]) + f': spg = {spg} retry.')
+                logger.warning(f'{e}:     spg = {spg} retry.')
                 continue
-            if tmp_crystal.valid:
-                tmp_struc = tmp_crystal.to_pymatgen(resort=False)    # pymatgen Structure format
-                tmp_nat, _ = get_nat(tmp_struc, rin.atype)
-                # -- check the number of atoms
-                if tmp_nat != numIons:
-                    # (pyxtal 0.1.4) cryspy adopts "conventional=False",
-                    #     which is better for DFT calculation
-                    # pyxtal returns conventional cell, that is, too many atoms
-                    tmp_struc = tmp_struc.get_primitive_structure()
-                    # recheck nat
-                    if tmp_nat != numIons:    # failure
-                        continue
-                # -- sort, just in case
-                tmp_struc = sort_by_atype(tmp_struc, rin.atype)
-                # -- scale volume
-                if rin.vol_mu is not None:
-                    vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
-                    tmp_struc.scale_lattice(volume=vol)
-                # -- check actual space group
-                try:
-                    spg_sym, spg_num = tmp_struc.get_space_group_info(
-                        symprec=rin.symprec)
-                except TypeError:
-                    spg_num = 0
-                    spg_sym = None
-                # -- register the structure in pymatgen format
-                cid = len(self.init_struc_data) + id_offset
-                self.init_struc_data[cid] = tmp_struc
-                logger.info(f'Structure ID {cid:>6}: {numIons}'
-                      f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
-
-    def gen_struc_mol(self, nstruc, id_offset=0):
-        '''
-        Generate random molecular crystal structures for given space groups
-        one have to run self.set_mol() in advance
-        # ---------- args
-        nstruc (int): number of generated structures
-
-        id_offset (int): default: 0
-                         structure ID starts from id_offset
-                         e.g. nstruc = 3, id_offset = 10
-                              you obtain ID 10, ID 11, ID 12
-
-        # ---------- comment
-        generated structure data are saved in self.init_struc_data
-        '''
-        # ---------- initialize
-        self.init_struc_data = {}
-        if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
-            self.struc_mol_id = {}
-        # ---------- Tol_matrix
-        tolmat = self._set_tol_mat(rin.atype, self.mindist)
-        # ---------- loop for structure generattion
-        while len(self.init_struc_data) < nstruc:
-            # ------ spgnum --> spg
-            if rin.spgnum == 'all':
-                spg = random.randint(1, 230)
-            else:
-                spg = random.choice(rin.spgnum)
-            rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
-            # ------ generate structure
-            # -- multiprocess for measures against hangup
+            # if algo in ['EA', 'EA-vc']:
+            #     tmp_struc = tmp_crystal.to_pymatgen(resort=False)
+            #     tmp_lattice = tmp_struc.lattice
+            #     dums = []        # dummy atoms
+            #     dum_pos = []     # internal position of dummy
+            #     in_dists = []
+            #     mol_dists = []
+            #     for i, site in enumerate(tmp_crystal.mol_sites):
+            #         for j, mol in enumerate(mol_data):
+            #             if mol.species == site.mol.species:
+            #                 dum = DummySpecie(f"X{j}{i}")
+            #                 dums.append(dum)
+            #                 dum_pos.append(site.position)
+            #                 # -- calculate atom distance by pyxtal
+            #                 in_dists.append(np.linalg.norm(site.position.dot(tmp_crystal.lattice.get_matrix()) -
+            #                                                 site.get_coords_and_species(absolute=True)[0]
+            #                                                 [0:len(site.mol.species)], axis=1))
+            #     # -- calculate atom distance from self.mol_data
+            #     for j, mol in enumerate(mol_data):
+            #         tmp_dists = []
+            #         for n, m in enumerate(mol):
+            #             tmp_dists.append(mol.get_distance(0, n))
+            #         mol_dists.append(tmp_dists)
+            #     dum_struc = Structure.from_spacegroup(spg, tmp_lattice, dums, dum_pos)
+            #     for ds, dc in zip(dum_struc.species, dum_struc.cart_coords):
+            #         tmp_struc.append(ds, dc, coords_are_cartesian=True)
+        else:
+            # -- multiprocess for hangup prevention
             q = Queue()
-            p = Process(target=self._mp_mc, args=(tolmat, spg, rin.nmol, rand_vol, q, rin.algo))
+            p = Process(target=_mp_mc, args=(tolmat, spg, mol_data, nmol,
+                                            vol_factor, q))
             p.start()
-            p.join(timeout=rin.timeout_mol)
+            p.join(timeout=timeout_mol)
             if p.is_alive():
                 p.terminate()
                 p.join()
             if sys.version_info.minor >= 7:
                 # Process.close() available from python 3.7
                 p.close()
             if q.empty():
                 logger.warning('timeout for molecular structure generation. retry.')
                 continue
             else:
                 # -- get struc data from _mp_mc
-                if rin.algo in ['EA', 'EA-vc']:
-                    tmp_q = q.get()
-                    tmp_struc = tmp_q[0]    # structure data
-                    dums = tmp_q[1]         # dummy element
-                    in_dists = tmp_q[2]     # interatomic distance in a molecule
-                    mol_dists = tmp_q[3]    # distance between molecules
-                else:
-                    tmp_struc = q.get()
+                # if rin.algo in ['EA', 'EA-vc']:
+                #     tmp_q = q.get()
+                #     tmp_struc = tmp_q[0]    # structure data
+                #     dums = tmp_q[1]         # dummy element
+                #     in_dists = tmp_q[2]     # interatomic distance in a molecule
+                #     mol_dists = tmp_q[3]    # distance between molecules
+                # else:
+                #     tmp_struc = q.get()
+                tmp_struc = q.get()
                 tmp_valid = q.get()
                 if tmp_struc == 'error':
                     # in case of 'error', tmp_valid <-- error message (Exception)
                     logger.warning(tmp_valid.args[0] + f': spg = {spg} retry.')
                     continue
-            if tmp_valid:
-                # -- scale volume
-                if rin.vol_mu is not None:
-                    vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
-                    vol = vol * tmp_struc.num_sites / rin.natot    # for conv. cell
-                    tmp_struc = scale_cell_mol(tmp_struc, self.mol_data, vol)
-                    if not tmp_struc:    # case: scale_cell_mol returns False
-                        logger.warning('failed scale cell. retry.')
-                        continue
+        if tmp_valid:
+            # -- scale volume
+            if vol_mu is not None:
+                vol = random.gauss(mu=vol_mu, sigma=vol_sigma)
+                vol = vol * tmp_struc.num_sites / sum(nat)    # for conv. cell
+                tmp_struc = scale_cell_mol(tmp_struc, mol_data, vol)
+                if not tmp_struc:    # case: scale_cell_mol returns False
+                    logger.warning('failed scale cell. retry.')
+                    continue
+            # -- check nat
+            tmp_nat, _ = get_nat(tmp_struc, atype)
+            if tmp_nat != nat:
+                # cryspy adopts conventional=True
+                # pyxtal returns conventional cell,
+                # too many atoms if centering
+                tmp_struc = tmp_struc.get_primitive_structure()
+                # recheck nat
+                if tmp_nat != nat:    # failure
+                    logger.warning(f'different num. of atoms. {tmp_nat}, {nat} retry.')
+                    continue
+            # -- grouping atoms for molecule using interatomic distance
+            # if rin.algo in ['EA', 'EA-vc']:
+            #     loopcnt = 0
+            #     while loopcnt < 10:
+            #         loopcnt += 1
+            #         mol_group = []
+            #         group_id = 0
+            #         # check atom distance from dummy atom
+            #         for i, ts in enumerate(tmp_struc.species):
+            #             for dn, dummyatom in enumerate(dums):
+            #                 if ts == dummyatom:
+            #                     mol_indx = int(ts.symbol[1:2])
+            #                     for j, tc_fc in enumerate(tmp_struc.frac_coords):
+            #                         if i == j:
+            #                             continue
+            #                         dist = tmp_struc.get_distance(i, j)
+            #                         for dist_indx, true_dist in enumerate(in_dists[dn]):
+            #                             if round(true_dist, 2) == round(dist, 2):
+            #                                 mol_group.append([tc_fc, group_id, mol_indx, dist_indx])
+            #                                 break
+            #                     group_id += 1
+            #         success_cnt = 0
+            #         # check number of atom per group
+            #         # if failed, shuffle struc data, and continue(max 10times)
+            #         mol_cnt = collections.Counter([x[2] for x in mol_group])
+            #         for mc_key, mc_value in mol_cnt.items():
+            #             if mc_value % len(mol_data[mc_key]) == 0:
+            #                 success_cnt += 1
+            #         if success_cnt == len(mol_data):
+            #             break
+            #         random.shuffle(tmp_struc)
+            #     if loopcnt == 10:
+            #         continue
+            #     tmp_struc.remove_species(dums)
+            # -- sort, necessary in molecular crystal
+            tmp_struc = sort_by_atype(tmp_struc, atype)
+            # -- record group_id, mol_id, and dist_index
+            # if rin.algo in ['EA', 'EA-vc']:
+            #     tmp_id = []
+            #     tmp_mol_indx = []
+            #     tmp_dist_indx = []
+            #     for atom_fc in tmp_struc.frac_coords:
+            #         for gatom in mol_group:
+            #             if np.array_equal(atom_fc, gatom[0]):
+            #                 tmp_id.append(gatom[1])
+            #                 tmp_mol_indx.append(gatom[2])
+            #                 tmp_dist_indx.append(gatom[3])
+            # -- check minimum distance
+            #    from CrySPY 0.10.4
+            #    Tol_matrix is used for mindist
+            #
+            #if self.mindist is not None:
+            #    success, mindist_ij, dist = check_distance(tmp_struc,
+            #                                               self.atype,
+            #                                               self.mindist)
+            #    if not success:
+            #        print('mindist in gen_struc_mol: {} - {}, {}. retry.'.format(
+            #            self.atype[mindist_ij[0]],
+            #            self.atype[mindist_ij[1]],
+            #            dist), file=sys.stderr)
+            #        continue    # failure
+            # -- check actual space group
+            try:
+                spg_sym, spg_num = tmp_struc.get_space_group_info(
+                    symprec=symprec)
+            except TypeError:
+                spg_num = 0
+                spg_sym = None
+            # -- register the structure in pymatgen format
+            cid = len(init_struc_data) + id_offset
+            init_struc_data[cid] = tmp_struc
+            # if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
+            #     struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
+            logger.info(f'Structure ID {cid:>6} was generated.'
+                    f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
+
+    # ---------- return
+    #            struc_mol_id is not implemented yet, just return vacant dict for now
+    return init_struc_data, struc_mol_id
+
+
+def gen_struc_mol_break_sym(
+        nstruc,
+        atype,
+        nat,
+        mindist,
+        mindist_dummy,
+        spgnum,
+        mol_data,
+        nmol,
+        symprec=0.01,
+        id_offset=0,
+        vol_factor=1.1,
+        vol_mu=None,
+        vol_sigma=None,
+        rot_mol='random_wyckoff',
+        nrot=20,
+    ):
+    '''
+    Generate random molecular crystal structures
+    molecules are put at a Wyckoff position without consideration of symmetry
+
+    # ---------- args
+    nstruc (int): number of structures to be generated
+    atype (tuple): atom type (e.g. ('Na', 'Cl'))
+    nat (tuple): number of atoms (e.g. (4, 4))
+    mindist (): minimum interatomic distance (e.g. ((2.0, 1.5), (1.5, 2.0)))
+    mindist_dummy: mindist for dummy atoms (= intermolecular distance)
+    spgnum (str, int, or tuple): space group number 'all', 0, or tuple of space group numbers
+    mol_data (tuple or list): pymatgen Molecule data
+    nmol (tuple): number of molecules (e.g. (4, 4))
+    symprec (float): symmetry tolerance
+    id_offset (int): structure ID starts from id_offset
+                        e.g. nstruc = 3, id_offset = 10
+                            you obtain ID 10, ID 11, ID 12
+    vol_factor (float): volume factor for structure generation
+    vol_mu (float): mean for volume scaling
+    vol_sigma (float): standard deviation for volume scaling
+    rot_mol (str): rotation option. 'random', 'random_mol', or 'random_wyckoff'
+    nrot (int): maximum number of trials to rotate molecules
+
+    # ---------- return
+    init_struc_data (dict): {ID: pymatgen Structure, ...}
+    struc_mol_id (dict):   not implemented yet, just return vacant dict for now
+    '''
+
+    # ---------- initialize
+    init_struc_data = {}
+    struc_mol_id = {}    # for EA and mol, not implemented yet
+
+    # ------ dummy atom type
+    atype_dummy = get_atype_dummy(len(mol_data))
+
+    # ---------- Tol_matrix for dummy atoms
+    tolmat = _set_tol_mat(atype_dummy, mindist_dummy)
+
+    # ---------- loop for structure generattion
+    while len(init_struc_data) < nstruc:
+        # ------ spgnum --> spg
+        if spgnum == 'all':
+            spg = random.randint(1, 230)
+        else:
+            spg = random.choice(spgnum)
+        # ------ generate structure
+        tmp_crystal = pyxtal()
+        try:
+            f = StringIO()
+            with redirect_stdout(f):
+                tmp_crystal.from_random(
+                    dim=3,
+                    group=spg,
+                    species=atype_dummy,
+                    numIons=nmol,
+                    factor=vol_factor,
+                    conventional=False,
+                    tm=tolmat
+                )
+            s = f.getvalue().rstrip()    # to delete \n
+            if s:
+                logger.warning(s)
+        except Exception as e:
+            logger.warning(f'{e}:    spg = {spg} retry.')
+            continue
+        if tmp_crystal.valid:
+            # -- each wyckoff position --> dummy atom
+            dums = []        # dummy atoms
+            dum_pos = []     # internal position of dummy
+            dum_type = {}    # type of dummy
+                                #  e.g. {DummySpecie X00+: 'Rn',
+                                #        DummySpecie X10+: 'Rn',
+                                #        DummySpecie X20+: 'Xe',
+                                #        DummySpecie X30+: 'Xe'}
+            for i, site in enumerate(tmp_crystal.atom_sites):
+                dum = DummySpecie(f"X{i}")
+                dums.append(dum)
+                dum_pos.append(site.position)
+                dum_type[dum] = site.specie
+            # -- tmp_struc with dummy atoms
+            lattice = tmp_crystal.lattice.get_matrix()
+            tmp_struc = Structure.from_spacegroup(spg, lattice, dums, dum_pos)
+            tmp_struc = tmp_struc.get_primitive_structure()
+            # -- scale volume
+            if vol_mu is not None:
+                vol = random.gauss(mu=vol_mu, sigma=vol_sigma)
+                tmp_struc.scale_lattice(volume=vol)
+            # -- save dummy coords
+            dum_species = tmp_struc.species
+            dum_coords = tmp_struc.cart_coords
+            # if rin.algo in ['EA', 'EA-vc']:
+            #     tmp_mol_indx = []
+            #     tmp_id = []
+            #     tmp_id_cnt = 0
+            # -- remove dummy
+            tmp_struc.remove_sites(range(0, len(dum_species)))
+            tmp_struc_ori = tmp_struc.copy()
+            rot_success = False
+            # -- rotate molecules
+            for nrel in range(nrot):
+                tmp_struc = tmp_struc_ori.copy()
+                for (dum_specie, dum_coord) in zip(dum_species, dum_coords):
+                    mol_index = atype_dummy.index(dum_type[dum_specie])
+                    mol = mol_data[mol_index]
+                    # rotation option
+                    if rot_mol is None:
+                        rot_mol_coord = mol.cart_coords
+                    if rot_mol == 'random':
+                        angle = 2 * np.pi * np.random.rand(3)
+                        R = rot_mat(angle)
+                        rot_mol_coord = np.matmul(mol.cart_coords, R)
+                    if rot_mol == 'random_mol':
+                        # each mol_data
+                        mol_angles = []    # [angles of mol 1, angles of mol 2, ...]
+                        for i in range(len(mol_data)):
+                            mol_angles.append(2 * np.pi * np.random.rand(3))
+                        angle = mol_angles[mol_index]
+                        R = rot_mat(angle)
+                        rot_mol_coord = np.matmul(mol.cart_coords, R)
+                    if rot_mol == 'random_wyckoff':
+                        # each Wyckoff
+                        dum_angles = {}    # e.g.
+                                            # {DummySpecie X00+: array([ , , ]),
+                                            #  DummySpecie X10+: array([ , , ]),
+                                            #  DummySpecie X20+: array([ , , ]),
+                                            #  DummySpecie X30+: array([ , , ])}
+                        angles = 2 * np.pi * np.random.rand(len(dums), 3)
+                        for (dum, angle) in zip(dums, angles):
+                            dum_angles[dum] = angle
+                        angle = dum_angles[dum_specie]
+                        R = rot_mat(angle)
+                        rot_mol_coord = np.matmul(mol.cart_coords, R)
+                    # rotate coord
+                    coord = rot_mol_coord + dum_coord
+                    # append mol
+                    for i, ms in enumerate(mol.species):
+                        tmp_struc.append(ms, coord[i], coords_are_cartesian=True)
+                        # if rin.algo in ['EA', 'EA-vc']:
+                        #     tmp_id.append(tmp_id_cnt)
+                        #     tmp_mol_indx.append(mol_index)
+                    # if rin.algo in ['EA', 'EA-vc']:
+                    #     tmp_id_cnt += 1
                 # -- check nat
-                tmp_nat, _ = get_nat(tmp_struc, rin.atype)
-                if tmp_nat != rin.nat:
-                    # cryspy adopts conventional=True
+                tmp_nat, _ = get_nat(tmp_struc, atype)
+                if tmp_nat != nat:
                     # pyxtal returns conventional cell,
                     # too many atoms if centering
                     tmp_struc = tmp_struc.get_primitive_structure()
                     # recheck nat
-                    if tmp_nat != rin.nat:    # failure
-                        logger.warning('different num. of atoms. retry.')
+                    if tmp_nat != nat:    # failure
+                        if rot_mol is None:
+                            break    # go back to the while loop
                         continue
-                # -- grouping atoms for molecule using interatomic distance
-                if rin.algo in ['EA', 'EA-vc']:
-                    loopcnt = 0
-                    while loopcnt < 10:
-                        loopcnt += 1
-                        mol_group = []
-                        group_id = 0
-                        # check atom distance from dummy atom
-                        for i, ts in enumerate(tmp_struc.species):
-                            for dn, dummyatom in enumerate(dums):
-                                if ts == dummyatom:
-                                    mol_indx = int(ts.symbol[1:2])
-                                    for j, tc_fc in enumerate(tmp_struc.frac_coords):
-                                        if i == j:
-                                            continue
-                                        dist = tmp_struc.get_distance(i, j)
-                                        for dist_indx, true_dist in enumerate(in_dists[dn]):
-                                            if round(true_dist, 2) == round(dist, 2):
-                                                mol_group.append([tc_fc, group_id, mol_indx, dist_indx])
-                                                break
-                                    group_id += 1
-                        success_cnt = 0
-                        # check number of atom per group
-                        # if failed, shuffle struc data, and continue(max 10times)
-                        mol_cnt = collections.Counter([x[2] for x in mol_group])
-                        for mc_key, mc_value in mol_cnt.items():
-                            if mc_value % len(self.mol_data[mc_key]) == 0:
-                                success_cnt += 1
-                        if success_cnt == len(self.mol_data):
-                            break
-                        random.shuffle(tmp_struc)
-                    if loopcnt == 10:
-                        continue
-                    tmp_struc.remove_species(dums)
                 # -- sort, necessary in molecular crystal
-                tmp_struc = sort_by_atype(tmp_struc, rin.atype)
-                # -- record group_id, mol_id, and dist_index
-                if rin.algo in ['EA', 'EA-vc']:
-                    tmp_id = []
-                    tmp_mol_indx = []
-                    tmp_dist_indx = []
-                    for atom_fc in tmp_struc.frac_coords:
-                        for gatom in mol_group:
-                            if np.array_equal(atom_fc, gatom[0]):
-                                tmp_id.append(gatom[1])
-                                tmp_mol_indx.append(gatom[2])
-                                tmp_dist_indx.append(gatom[3])
+                tmp_struc = sort_by_atype(tmp_struc, atype)
                 # -- check minimum distance
-                #    from CrySPY 0.10.4
-                #    Tol_matrix is used for mindist
-                #
-                #if self.mindist is not None:
-                #    success, mindist_ij, dist = check_distance(tmp_struc,
-                #                                               self.atype,
-                #                                               self.mindist)
-                #    if not success:
-                #        print('mindist in gen_struc_mol: {} - {}, {}. retry.'.format(
-                #            self.atype[mindist_ij[0]],
-                #            self.atype[mindist_ij[1]],
-                #            dist), file=sys.stderr)
-                #        continue    # failure
-                # -- check actual space group
+                if mindist is not None:
+                    success, mindist_ij, dist = check_distance(tmp_struc,
+                                                               atype,
+                                                               mindist)
+                    if not success:
+                        type0 = atype[mindist_ij[0]]
+                        type1 = atype[mindist_ij[1]]
+                        logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
+                        if rot_mol is None:
+                            break    # go back to the while loop
+                        continue    # failure
+                # -- check actual space group (success)
                 try:
                     spg_sym, spg_num = tmp_struc.get_space_group_info(
-                        symprec=rin.symprec)
+                        symprec=symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
-                # -- register the structure in pymatgen format
-                cid = len(self.init_struc_data) + id_offset
-                self.init_struc_data[cid] = tmp_struc
-                if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
-                    self.struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
-                logger.info(f'Structure ID {cid:>6} was generated.'
-                      f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
-
-    def gen_struc_mol_break_sym(self, nstruc, mindist_dummy,
-                                id_offset=0):
-        '''
-        Generate random molecular crystal structures
-        one have to run self.set_mol() in advance
-        molecules are put a Wyckoff position without consideration of symmetry
-
-        # ---------- args
-        nstruc (int): number of generated structures
-
-        mindist_dummy: mindist for dummy atoms
-
-        id_offset (int): default: 0
-                         structure ID starts from id_offset
-                         e.g. nstruc = 3, id_offset = 10
-                              you obtain ID 10, ID 11, ID 12
-
-        # ---------- comment
-        generated structure data are saved in self.init_struc_data
-        '''
-        # ---------- initialize
-        self.init_struc_data = {}
-        if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
-            self.struc_mol_id = {}
-        # ------ dummy atom type
-        atype_dummy = get_atype_dummy()
-        # ---------- Tol_matrix for dummy atoms
-        tolmat = self._set_tol_mat(atype_dummy, mindist_dummy)
-        # ---------- loop for structure generattion
-        while len(self.init_struc_data) < nstruc:
-            # ------ spgnum --> spg
-            if rin.spgnum == 'all':
-                spg = random.randint(1, 230)
-            else:
-                spg = random.choice(rin.spgnum)
-            # ------ vol_factor
-            rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
-            # ------ generate structure
-            tmp_crystal = pyxtal()
-            try:
-                f = StringIO()
-                with redirect_stdout(f):
-                    tmp_crystal.from_random(dim=3, group=spg, species=atype_dummy,
-                                            numIons=rin.nmol, factor=rand_vol,
-                                            conventional=False, tm=tolmat)
-                s = f.getvalue().rstrip()    # to delete \n
-                if s:
-                    logger.warning(s)
-            except Exception as e:
-                logger.warning(str(e.args[0]) + f': spg = {spg} retry.')
-                continue
-            if tmp_crystal.valid:
-                # -- each wyckoff position --> dummy atom
-                dums = []        # dummy atoms
-                dum_pos = []     # internal position of dummy
-                dum_type = {}    # type of dummy
-                                 #  e.g. {DummySpecie X00+: 'Rn',
-                                 #        DummySpecie X10+: 'Rn',
-                                 #        DummySpecie X20+: 'Xe',
-                                 #        DummySpecie X30+: 'Xe'}
-                for i, site in enumerate(tmp_crystal.atom_sites):
-                    dum = DummySpecie("X{}".format(i))
-                    dums.append(dum)
-                    dum_pos.append(site.position)
-                    dum_type[dum] = site.specie
-                # -- tmp_struc with dummy atoms
-                lattice = tmp_crystal.lattice.get_matrix()
-                tmp_struc = Structure.from_spacegroup(spg, lattice, dums, dum_pos)
-                tmp_struc = tmp_struc.get_primitive_structure()
-                # -- scale volume
-                if rin.vol_mu is not None:
-                    vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
-                    tmp_struc.scale_lattice(volume=vol)
-                # -- save dummy coords
-                dum_species = tmp_struc.species
-                dum_coords = tmp_struc.cart_coords
-                if rin.algo in ['EA', 'EA-vc']:
-                    tmp_mol_indx = []
-                    tmp_id = []
-                    tmp_id_cnt = 0
-                # -- remove dummy
-                tmp_struc.remove_sites(range(0, len(dum_species)))
-                tmp_struc_ori = tmp_struc.copy()
-                rot_success = False
-                # -- rotate molecules
-                for nrel in range(rin.nrot):
-                    tmp_struc = tmp_struc_ori.copy()
-                    for (dum_specie, dum_coord) in zip(dum_species, dum_coords):
-                        mol_index = atype_dummy.index(dum_type[dum_specie])
-                        mol = self.mol_data[mol_index]
-                        # rotation option
-                        if rin.rot_mol is None:
-                            rot_mol_coord = mol.cart_coords
-                        if rin.rot_mol == 'random':
-                            angle = 2 * np.pi * np.random.rand(3)
-                            R = rot_mat(angle)
-                            rot_mol_coord = np.matmul(mol.cart_coords, R)
-                        if rin.rot_mol == 'random_mol':
-                            # each mol_data
-                            mol_angles = []    # [angles of mol 1, angles of mol 2, ...]
-                            for i in range(len(self.mol_data)):
-                                mol_angles.append(2 * np.pi * np.random.rand(3))
-                            angle = mol_angles[mol_index]
-                            R = rot_mat(angle)
-                            rot_mol_coord = np.matmul(mol.cart_coords, R)
-                        if rin.rot_mol == 'random_wyckoff':
-                            # each Wyckoff
-                            dum_angles = {}    # e.g.
-                                               # {DummySpecie X00+: array([ , , ]),
-                                               #  DummySpecie X10+: array([ , , ]),
-                                               #  DummySpecie X20+: array([ , , ]),
-                                               #  DummySpecie X30+: array([ , , ])}
-                            angles = 2 * np.pi * np.random.rand(len(dums), 3)
-                            for (dum, angle) in zip(dums, angles):
-                                dum_angles[dum] = angle
-                            angle = dum_angles[dum_specie]
-                            R = rot_mat(angle)
-                            rot_mol_coord = np.matmul(mol.cart_coords, R)
-                        # rotate coord
-                        coord = rot_mol_coord + dum_coord
-                        # append mol
-                        for i, ms in enumerate(mol.species):
-                            tmp_struc.append(ms, coord[i], coords_are_cartesian=True)
-                            if rin.algo in ['EA', 'EA-vc']:
-                                tmp_id.append(tmp_id_cnt)
-                                tmp_mol_indx.append(mol_index)
-                        if rin.algo in ['EA', 'EA-vc']:
-                            tmp_id_cnt += 1
-                    # -- check nat
-                    tmp_nat, _ = get_nat(tmp_struc, rin.atype)
-                    if tmp_nat != rin.nat:
-                        # pyxtal returns conventional cell,
-                        # too many atoms if centering
-                        tmp_struc = tmp_struc.get_primitive_structure()
-                        # recheck nat
-                        if tmp_nat != rin.nat:    # failure
-                            if rin.rot_mol is None:
-                                break    # go back to the while loop
-                            continue
-                    # -- sort, necessary in molecular crystal
-                    tmp_struc = sort_by_atype(tmp_struc, rin.atype)
-                    # -- check minimum distance
-                    if self.mindist is not None:
-                        success, mindist_ij, dist = check_distance(tmp_struc,
-                                                                   rin.atype,
-                                                                   self.mindist)
-                        if not success:
-                            type0 = rin.atype[mindist_ij[0]]
-                            type1 = rin.atype[mindist_ij[1]]
-                            logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
-                            if rin.rot_mol is None:
-                                break    # go back to the while loop
-                            continue    # failure
-                    # -- check actual space group (success)
-                    try:
-                        spg_sym, spg_num = tmp_struc.get_space_group_info(
-                            symprec=rin.symprec)
-                    except TypeError:
-                        spg_num = 0
-                        spg_sym = None
-                    rot_success = True
-                    break
-                # -- reach maximum times to rotate (failure)
-                if not rot_success:
-                    continue    # go back to the while loop
-                # -- register the structure in pymatgen format
-                cid = len(self.init_struc_data) + id_offset
-                self.init_struc_data[cid] = tmp_struc
-                if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
-                    # calculate interatomic distance of mol_data
-                    mol_dists = []
-                    for j, mol in enumerate(self.mol_data):
-                        tmp_dists = []
-                        for n, m in enumerate(mol):
-                            tmp_dists.append(mol.get_distance(0, n))
-                        mol_dists.append(tmp_dists)
-                    self.struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
-                logger.info(f'Structure ID {cid:>6} was generated.'
-                      f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
-
-    def _set_tol_mat(self, atype, mindist):
-        tolmat = Tol_matrix()
-        for i, itype in enumerate(atype):
-            for j, jtype in enumerate(atype):
-                if i <= j:
-                    tolmat.set_tol(itype, jtype, mindist[i][j])
-        return tolmat
-
-    def _mp_mc(self, tolmat, spg, nmol, rand_vol, q, algo):
-        '''
-        multiprocess part
-        here cannot use rin.xxx and logging
-        '''
-        try:
-            np.random.seed(random.randint(0, 100000000))
-            tmp_crystal = pyxtal(molecular=True)
-            f = StringIO()
-            with redirect_stdout(f):
-                with redirect_stderr(f):
-                    tmp_crystal.from_random(dim=3, group=spg,
-                                            species=self.mol_data, numIons=nmol,
-                                            factor=rand_vol, conventional=False, tm=tolmat)
-            s = f.getvalue().rstrip()    # to delete \n
-            if s:
-                logger.warning(s)
-            if algo in ['EA', 'EA-vc']:
-                tmp_struc = tmp_crystal.to_pymatgen(resort=False)
-                tmp_lattice = tmp_struc.lattice
-                dums = []        # dummy atoms
-                dum_pos = []     # internal position of dummy
-                in_dists = []
-                mol_dists = []
-                for i, site in enumerate(tmp_crystal.mol_sites):
-                    for j, mol in enumerate(self.mol_data):
-                        if mol.species == site.mol.species:
-                            dum = DummySpecie("X{}{}".format(j, i))
-                            dums.append(dum)
-                            dum_pos.append(site.position)
-                            # -- calculate atom distance by pyxtal
-                            in_dists.append(np.linalg.norm(site.position.dot(tmp_crystal.lattice.get_matrix()) -
-                                                           site.get_coords_and_species(absolute=True)[0]
-                                                           [0:len(site.mol.species)], axis=1))
-                # -- calculate atom distance from self.mol_data
-                for j, mol in enumerate(self.mol_data):
-                    tmp_dists = []
-                    for n, m in enumerate(mol):
-                        tmp_dists.append(mol.get_distance(0, n))
-                    mol_dists.append(tmp_dists)
-                dum_struc = Structure.from_spacegroup(spg, tmp_lattice, dums, dum_pos)
-                for ds, dc in zip(dum_struc.species, dum_struc.cart_coords):
-                    tmp_struc.append(ds, dc, coords_are_cartesian=True)
-            # ---------- queue
-            if tmp_crystal.valid:
-                if algo in ['EA', 'EA-vc']:
-                    q.put([tmp_struc, dums, in_dists, mol_dists])
-                else:
-                    q.put(tmp_crystal.to_pymatgen(resort=False))
-                q.put(tmp_crystal.valid)
-            else:
-                q.put(None)
-                q.put(tmp_crystal.valid)
-        except Exception as e:
-            q.put('error')
-            q.put(e)
+                rot_success = True
+                break
+            # -- reach maximum times to rotate (failure)
+            if not rot_success:
+                continue    # go back to the while loop
+            # -- tmp_struc --> init_struc_data
+            cid = len(init_struc_data) + id_offset
+            init_struc_data[cid] = tmp_struc
+            # if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
+            #     # calculate interatomic distance of mol_data
+            #     mol_dists = []
+            #     for j, mol in enumerate(mol_data):
+            #         tmp_dists = []
+            #         for n, m in enumerate(mol):
+            #             tmp_dists.append(mol.get_distance(0, n))
+            #         mol_dists.append(tmp_dists)
+            #     struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
+            logger.info(f'Structure ID {cid:>6} was generated.'
+                    f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
+
+    # ---------- return
+    #            struc_mol_id is not implemented yet, just return vacant dict for now
+    return init_struc_data, struc_mol_id
+
+
+def _set_tol_mat(atype, mindist):
+    tolmat = Tol_matrix()
+    for i, itype in enumerate(atype):
+        for j, jtype in enumerate(atype):
+            if i <= j:
+                tolmat.set_tol(itype, jtype, mindist[i][j])
+    return tolmat
+
+
+def _mp_mc(tolmat, spg, mol_data, nmol, vol_factor, q):
+    '''
+    multiprocess part
+    here cannot use rin.xxx and logging
+    '''
+    try:
+        np.random.seed(random.randint(0, 100000000))
+        tmp_crystal = pyxtal(molecular=True)
+        f = StringIO()
+        with redirect_stdout(f):
+            with redirect_stderr(f):
+                tmp_crystal.from_random(dim=3, group=spg,
+                                        species=mol_data, numIons=nmol,
+                                        factor=vol_factor, conventional=False, tm=tolmat)
+        s = f.getvalue().rstrip()    # to delete \n
+        if s:
+            logger.warning(s)
+        # if algo in ['EA', 'EA-vc']:
+        #     tmp_struc = tmp_crystal.to_pymatgen(resort=False)
+        #     tmp_lattice = tmp_struc.lattice
+        #     dums = []        # dummy atoms
+        #     dum_pos = []     # internal position of dummy
+        #     in_dists = []
+        #     mol_dists = []
+        #     for i, site in enumerate(tmp_crystal.mol_sites):
+        #         for j, mol in enumerate(mol_data):
+        #             if mol.species == site.mol.species:
+        #                 dum = DummySpecie(f"X{j}{i}")
+        #                 dums.append(dum)
+        #                 dum_pos.append(site.position)
+        #                 # -- calculate atom distance by pyxtal
+        #                 in_dists.append(np.linalg.norm(site.position.dot(tmp_crystal.lattice.get_matrix()) -
+        #                                                 site.get_coords_and_species(absolute=True)[0]
+        #                                                 [0:len(site.mol.species)], axis=1))
+        #     # -- calculate atom distance from self.mol_data
+        #     for j, mol in enumerate(mol_data):
+        #         tmp_dists = []
+        #         for n, m in enumerate(mol):
+        #             tmp_dists.append(mol.get_distance(0, n))
+        #         mol_dists.append(tmp_dists)
+        #     dum_struc = Structure.from_spacegroup(spg, tmp_lattice, dums, dum_pos)
+        #     for ds, dc in zip(dum_struc.species, dum_struc.cart_coords):
+        #         tmp_struc.append(ds, dc, coords_are_cartesian=True)
+        # ---------- queue
+        if tmp_crystal.valid:
+            # if algo in ['EA', 'EA-vc']:
+            #     q.put([tmp_struc, dums, in_dists, mol_dists])
+            # else:
+            #     q.put(tmp_crystal.to_pymatgen(resort=False))
+            q.put(tmp_crystal.to_pymatgen(resort=False))
+            q.put(tmp_crystal.valid)
+        else:
+            q.put(None)
+            q.put(tmp_crystal.valid)
+    except Exception as e:
+        q.put('error')
+        q.put(e)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/random_generation.py` & `csp_cryspy-1.3.0/src/cryspy/RS/gen_struc_RS/random_generation.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,468 +8,524 @@
 import os
 import random
 import subprocess
 
 import numpy as np
 from pymatgen.core import Structure
 
-from ...IO import read_input as rin
 from ...util.struc_util import check_distance
 
 
 logger = getLogger('cryspy')
 
-class Rnd_struc_gen:
+
+def gen_wo_spg(
+        nstruc,
+        atype,
+        nat,
+        mindist,
+        spgnum,
+        minlen,
+        maxlen,
+        dangle,
+        symprec=0.01,
+        maxcnt=50,
+        id_offset=0,
+        vol_mu=None,
+        vol_sigma=None,
+        vc=False,
+        ll_nat=None,
+        ul_nat=None,
+    ):
     '''
-    Random structure generation w/o pyxtal
+    Generate random structures without space group information
+
+    # ---------- args
+    nstruc (int): number of structures to be generated
+    atype (tuple): atom types, e.g. ('Na', 'Cl')
+    nat (tuple): number of atoms, e.g. (8, 8)
+    mindist (): minumum interatomic distance, e.g. ((2.0, 1.5), (1.5, 2.0))
+    spgnum (str, int, or tuple): space group number 'all', 0, or tuple of space group numbers
+    minlen (float): minimum length of lattice vector
+    maxlen (float): maximum length of lattice vector
+    dangle (float): maximum deviation of lattice angle
+    symprec (float): tolerance to find space group
+    maxcnt (int): maximum trial to generate a structure
+    id_offset (int): structure ID starts from id_offset
+                        e.g. nstruc = 3, id_offset = 10
+                            you obtain ID 10, ID 11, ID 12
+    vol_mu (float): mean of volume scaling
+    vol_sigma (float): standard deviation of volume scaling
+    vc (bool): variable composition. it needs ll_nat and ul_nat
+    ll_nat (tuple): lower limit of number of atoms, e.g. (1, 1)
+    ul_nat (tuple): upper limit of number of atoms, e.g. (8, 8)
+
+    # ---------- return
+    init_struc_data (dict): {ID: pymatgen structure data}
     '''
 
-    def __init__(self, mindist):
-        self.mindist = mindist
+    # ---------- initialize
+    init_struc_data = {}
 
-    def gen_wo_spg(self, nstruc, id_offset=0, vc=False):
-        '''
-        Generate random structures without space group information
-
-        # ---------- args
-        nstruc (int): number of generated structures
-
-        id_offset (int): structure ID starts from id_offset
-                         e.g. nstruc = 3, id_offset = 10
-                              you obtain ID 10, ID 11, ID 12
-
-        vc (bool): variable composition. it needs ll_nat and ul_nat
-
-        # ---------- comment
-        generated init_struc_data is saved in self.init_struc_data
-        '''
-        # ---------- initialize
-        init_struc_data = {}
-        # ---------- generate structures
-        while len(init_struc_data) < nstruc:
-            # ------ vc
-            if not vc:
-                numIons = rin.nat
-            else:    # variable composition
-                numIons = [random.randint(l, u) for l, u in zip(rin.ll_nat, rin.ul_nat)]
-            self._get_atomlist(numIons)    # get self.atomlist
-            # ------ get spg, a, b, c, alpha, beta, gamma in self.*
-            self._gen_lattice()
-            # ------ get va, vb, and vc in self.*
-            self._calc_latvec()
-            # ------ get structure
-            tmp_struc = self._gen_struc_wo_spg(numIons)
-            if tmp_struc is not None:    # success of generation
-                # ------ scale volume
-                if rin.vol_mu is not None:
-                    vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
-                    tmp_struc.scale_lattice(volume=vol)
-                    success, mindist_ij, dist = check_distance(tmp_struc,
-                                                               rin.atype,
-                                                               self.mindist)
-                    if not success:
-                        type0 = rin.atype[mindist_ij[0]]
-                        type1 = rin.atype[mindist_ij[1]]
-                        logger.warning(f'mindist in gen_wo_spg: {type0} - {type1}, {dist}. retry.')
-                        continue    # failure
-                # ------ check actual space group using pymatgen
-                try:
-                    spg_sym, spg_num = tmp_struc.get_space_group_info(
-                        symprec=rin.symprec)
-                except TypeError:
-                    spg_num = 0
-                    spg_sym = None
-                # ------ register the structure in pymatgen format
-                cid = len(init_struc_data) + id_offset
-                init_struc_data[cid] = tmp_struc
-                logger.info(f'Structure ID {cid:>6}: {numIons}'
-                      f' Space group: {spg_num:>3} {spg_sym}')
-        # ---------- to self
-        self.init_struc_data = init_struc_data
-
-    def gen_with_find_wy(self, nstruc, id_offset=0,
-                         fwpath='find_wy', mpi_rank=0, vc=False):
-        '''
-        Generate random structures with space gruop information
-        using find_wy program
-
-        # ---------- args
-        nstruc (int): number of generated structures
-
-        id_offset (int): structure ID starts from id_offset
-                         e.g. nstruc = 3, id_offset = 10
-                              you obtain ID 10, ID 11, ID 12
-
-        fwpath (str): specify a path for a executable file of find_wy program
-
-        vc (bool): variable composition. it needs ll_nat and ul_nat
-
-        # ---------- comment
-        generated init_struc_data is saved in self.init_struc_data
-        '''
-        # ---------- initialize
-        init_struc_data = {}
-        # ---------- cd tmp_gen_struc
-        os.makedirs(f'tmp_gen_struc/rank_{mpi_rank}', exist_ok=True)
-        os.chdir(f'tmp_gen_struc/rank_{mpi_rank}')
-
-        # ---------- generate structures
-        while len(init_struc_data) < nstruc:
-            # ------ vc
-            if not vc:
-                numIons = rin.nat
-            else:    # variable composition
-                numIons = [random.randint(l, u) for l, u in zip(rin.ll_nat, rin.ul_nat)]
-            # ------ get spg, a, b, c, alpha, beta, gamma in self.*
-            self._gen_lattice()
-            # ------ get cosa, cosb, and cosg in self.*
-            self._calc_cos()
-            # ------ write an input file for find_wy
-            self._fw_input(numIons)
-            # ------ loop for same fw_input
-            cnt = 0
-            while cnt <= rin.maxcnt:
-                # -- run find_wy
-                with open('log_find_wy', 'w') as f:
-                    subprocess.call([fwpath, 'input'], stdout=f, stderr=f)
-                # -- generate a structure using POS_WY_SKEL_ALL.json
-                if not os.path.isfile('POS_WY_SKEL_ALL.json'):
-                    wyflag = False
-                    break
-                wyflag, tmp_struc = self._gen_struc_with_spg()
-                if wyflag is False:    # Failure
-                    os.remove('POS_WY_SKEL_ALL.json')
-                    cnt += 1
-                    continue
-                else:    # Success
-                    self._rm_files()    # rm input POS_WY_SKEL_ALL.json
-                    break         # break fw_input loop
-            if wyflag is False:
-                # -- maximum trial or no POS_WY_SKEL_ALL.json file
-                self._rm_files()    # clean
-                continue      # to new fw_input
+    # ---------- generate structures
+    while len(init_struc_data) < nstruc:
+        # ------ vc
+        if not vc:
+            numIons = nat
+        else:    # variable composition
+            numIons = [random.randint(l, u) for l, u in zip(ll_nat, ul_nat)]
+            numIons = tuple(numIons)
+        atomlist = _get_atomlist(atype, numIons)
+        # ------ get spg, a, b, c, alpha, beta, gamma
+        spg, a, b, c, alpha, beta, gamma = _gen_lattice(spgnum, minlen, maxlen, dangle)
+        # ------ get a1, a2, a3
+        a1, a2, a3 = _calc_latvec(a, b, c, alpha, beta, gamma)
+        # ------ get structure
+        tmp_struc = _gen_struc_wo_spg(atype, numIons, atomlist, a1, a2, a3, mindist, maxcnt)
+        if tmp_struc is not None:    # success of generation
             # ------ scale volume
-            if rin.vol_mu is not None:
-                vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
+            if vol_mu is not None:
+                vol = random.gauss(mu=vol_mu, sigma=vol_sigma)
                 tmp_struc.scale_lattice(volume=vol)
-                success, mindist_ij, dist = check_distance(tmp_struc,
-                                                           rin.atype,
-                                                           self.mindist)
+                success, mindist_ij, dist = check_distance(tmp_struc, atype, mindist)
                 if not success:
-                    type0 = rin.atype[mindist_ij[0]]
-                    type1 = rin.atype[mindist_ij[1]]
-                    logger.warning(f'mindist in gen_with_find_wy: {type0} - {type1}, {dist}. retry.')
+                    type0 = atype[mindist_ij[0]]
+                    type1 = atype[mindist_ij[1]]
+                    logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
                     continue    # failure
             # ------ check actual space group using pymatgen
             try:
-                spg_sym, spg_num = tmp_struc.get_space_group_info(
-                    symprec=rin.symprec)
+                spg_sym, spg_num = tmp_struc.get_space_group_info(symprec=symprec)
             except TypeError:
                 spg_num = 0
                 spg_sym = None
             # ------ register the structure in pymatgen format
             cid = len(init_struc_data) + id_offset
             init_struc_data[cid] = tmp_struc
             logger.info(f'Structure ID {cid:>6}: {numIons}'
-                  f' Space group: {self.spg:>3} --> {spg_num:>3} {spg_sym}')
-            # ------ clean
-            self._rm_files()
-        # ---------- go back to ..
-        os.chdir('../../')
-        # ---------- init_struc_data
-        self.init_struc_data = init_struc_data
-
-    def _get_atomlist(self, numIons):
-        '''
-        e.g. Na2Cl2
-            atomlist = ['Na', 'Na', 'Cl', 'Cl']
-        '''
-        atomlist = []
-        for i in range(len(rin.atype)):
-            atomlist += [rin.atype[i]]*numIons[i]
-        self.atomlist = atomlist
-
-    def _gen_lattice(self):
-        # ---------- for spgnum = 0: no space group
-        if rin.spgnum == 0:
-            crystal_systems = ['Triclinic',
-                               'Monoclinic',
-                               'Orthorhombic',
-                               'Tetragonal',
-                               'Rhombohedral',
-                               'Hexagonal',
-                               'Cubic']
-            spg = 0
-            csys = random.choice(crystal_systems)
-        # ---------- for spgnum 1--230
+                    f' Space group: {spg_num:>3} {spg_sym}')
+
+    # ---------- return
+    return init_struc_data
+
+
+def gen_with_find_wy(
+        nstruc,
+        atype,
+        nat,
+        mindist,
+        spgnum,
+        minlen,
+        maxlen,
+        dangle,
+        symprec=0.01,
+        maxcnt=50,
+        id_offset=0,
+        vol_mu=None,
+        vol_sigma=None,
+        fwpath='find_wy',
+        mpi_rank=0,
+        vc=False,
+        ll_nat=None,
+        ul_nat=None,
+    ):
+    '''
+    Generate random structures with space gruop information
+    using find_wy program
+
+    # ---------- args
+    nstruc (int): number of generated structures
+    atype (tuple): atom types, e.g. ('Na', 'Cl')
+    nat (tuple): number of atoms, e.g. (8, 8)
+    mindist (): minimum interatomic distance e.g. ((2.0, 1.5), (1.5, 2.0))
+    spgnum (str, int, or tuple): space group number 'all', 0, or tuple of space group numbers
+    minlen (float): minimum length of lattice vector
+    maxlen (float): maximum length of lattice vector
+    dangle (float): maximum deviation of lattice angle
+    symprec (float): tolerance to find space group
+    maxcnt (int): maximum trial to generate a structure
+    id_offset (int): structure ID starts from id_offset
+                        e.g. nstruc = 3, id_offset = 10
+                            you obtain ID 10, ID 11, ID 12
+    vol_mu (float): mean of volume scaling
+    vol_sigma (float): standard deviation of volume scaling
+    fwpath (str): specify a path for a executable file of find_wy program
+    mpi_rank (int): rank of MPI process
+    vc (bool): variable composition. it needs ll_nat and ul_nat
+    ll_nat (tuple): lower limit of number of atoms, e.g. (1, 1)
+    ul_nat (tuple): upper limit of number of atoms, e.g. (8, 8)
+
+    # ---------- return
+    init_struc_data (dict): {ID: pymatgen Structre}
+    '''
+
+    # ---------- initialize
+    init_struc_data = {}
+
+    # ---------- cd tmp_gen_struc
+    os.makedirs(f'tmp_gen_struc/rank_{mpi_rank}', exist_ok=True)
+    os.chdir(f'tmp_gen_struc/rank_{mpi_rank}')
+
+    # ---------- generate structures
+    while len(init_struc_data) < nstruc:
+        # ------ vc
+        if not vc:
+            numIons = nat
+        else:    # variable composition
+            numIons = [random.randint(l, u) for l, u in zip(ll_nat, ul_nat)]
+            numIons = tuple(numIons)
+        # ------ get spg, a, b, c, alpha, beta, gamma
+        spg, a, b, c, alpha, beta, gamma = _gen_lattice(spgnum, minlen, maxlen, dangle)
+        # ------ get cosa, cosb, and cosc
+        cosa, cosb, cosg = _calc_cos(alpha, beta, gamma)
+        # ------ write an input file for find_wy
+        _fw_input(atype, numIons, spg, a, b, c, cosa, cosb, cosg)
+        # ------ loop for same fw_input
+        cnt = 0
+        while cnt <= maxcnt:
+            # -- run find_wy
+            with open('log_find_wy', 'w') as f:
+                subprocess.call([fwpath, 'input'], stdout=f, stderr=f)
+            # -- generate a structure using POS_WY_SKEL_ALL.json
+            if not os.path.isfile('POS_WY_SKEL_ALL.json'):
+                wyflag = False
+                break
+            wyflag, tmp_struc = _gen_struc_with_spg(atype, mindist, maxcnt)
+            if wyflag is False:    # Failure
+                os.remove('POS_WY_SKEL_ALL.json')
+                cnt += 1
+                continue
+            else:    # Success
+                _rm_files()    # rm input POS_WY_SKEL_ALL.json
+                break          # break fw_input loop
+        if wyflag is False:
+            # -- maximum trial or no POS_WY_SKEL_ALL.json file
+            _rm_files()    # clean
+            continue       # to new fw_input
+        # ------ scale volume
+        if vol_mu is not None:
+            vol = random.gauss(mu=vol_mu, sigma=vol_sigma)
+            tmp_struc.scale_lattice(volume=vol)
+            success, mindist_ij, dist = check_distance(tmp_struc, atype, mindist)
+            if not success:
+                type0 = atype[mindist_ij[0]]
+                type1 = atype[mindist_ij[1]]
+                logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
+                continue    # failure
+        # ------ check actual space group using pymatgen
+        try:
+            spg_sym, spg_num = tmp_struc.get_space_group_info(
+                symprec=symprec)
+        except TypeError:
+            spg_num = 0
+            spg_sym = None
+        # ------ tmp_struc --> init_struc_data
+        cid = len(init_struc_data) + id_offset
+        init_struc_data[cid] = tmp_struc
+        logger.info(f'Structure ID {cid:>6}: {numIons}'
+                f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
+        # ------ clean
+        _rm_files()
+
+    # ---------- go back to ..
+    os.chdir('../../')
+
+    # ---------- return
+    return init_struc_data
+
+
+def _get_atomlist(atype, numIons):
+    '''
+    e.g. Na2Cl2
+        atomlist = ['Na', 'Na', 'Cl', 'Cl']
+    '''
+    atomlist = []
+    for i in range(len(atype)):
+        atomlist += [atype[i]]*numIons[i]
+    return atomlist
+
+def _gen_lattice(spgnum, minlen, maxlen, dangle):
+    # ---------- for spgnum = 0: no space group
+    if spgnum == 0:
+        crystal_systems = ['Triclinic',
+                            'Monoclinic',
+                            'Orthorhombic',
+                            'Tetragonal',
+                            'Rhombohedral',
+                            'Hexagonal',
+                            'Cubic']
+        spg = 0
+        csys = random.choice(crystal_systems)
+    # ---------- for spgnum 1--230
+    else:
+        # ------ spgnum --> spg
+        if spgnum == 'all':
+            spg = random.randint(1, 230)
+        else:
+            spg = random.choice(spgnum)
+        if 1 <= spg <= 2:
+            csys = 'Triclinic'
+        elif 3 <= spg <= 15:
+            csys = 'Monoclinic'
+        elif 16 <= spg <= 74:
+            csys = 'Orthorhombic'
+        elif 75 <= spg <= 142:
+            csys = 'Tetragonal'
+        elif 143 <= spg <= 167:
+            # trigonal includes rhombohedral in find_wy
+            csys = 'Trigonal'
+        elif 168 <= spg <= 194:
+            csys = 'Hexagonal'
+        elif 195 <= spg <= 230:
+            csys = 'Cubic'
         else:
-            # ------ spgnum --> spg
-            if rin.spgnum == 'all':
-                spg = random.randint(1, 230)
+            logger.error('spg is wrong')
+            raise SystemExit(1)
+    # ---------- generate lattice constants a, b, c, alpha, beta, gamma
+    if csys == 'Triclinic':
+        t1 = random.uniform(minlen, maxlen)
+        t2 = random.uniform(minlen, maxlen)
+        t3 = random.uniform(minlen, maxlen)
+        t = [t1, t2, t3]
+        t.sort()
+        a, b, c = t
+        r = random.random()
+        if r < 0.5:    # Type I
+            alpha = 90.0 - random.uniform(0, dangle)
+            beta  = 90.0 - random.uniform(0, dangle)
+            gamma = 90.0 - random.uniform(0, dangle)
+        else:    # Type II
+            alpha = 90.0 + random.uniform(0, dangle)
+            beta  = 90.0 + random.uniform(0, dangle)
+            gamma = 90.0 + random.uniform(0, dangle)
+    elif csys == 'Monoclinic':
+        a = random.uniform(minlen, maxlen)
+        b = random.uniform(minlen, maxlen)
+        c = random.uniform(minlen, maxlen)
+        if a > c:
+            a, c = c, a
+        alpha = gamma = 90.0
+        beta = 90.0 + random.uniform(0, dangle)
+    elif csys == 'Orthorhombic':
+        t1 = random.uniform(minlen, maxlen)
+        t2 = random.uniform(minlen, maxlen)
+        t3 = random.uniform(minlen, maxlen)
+        t = [t1, t2, t3]
+        t.sort()
+        a, b, c = t
+        alpha = beta = gamma = 90.0
+    elif csys == 'Tetragonal':
+        a = b = random.uniform(minlen, maxlen)
+        c = random.uniform(minlen, maxlen)
+        alpha = beta = gamma = 90.0
+    elif csys == 'Trigonal':
+        a = b = random.uniform(minlen, maxlen)
+        c = random.uniform(minlen, maxlen)
+        alpha = beta = 90.0
+        gamma = 120.0
+    elif csys == 'Rhombohedral':
+        a = b = c = random.uniform(minlen, maxlen)
+        alpha = beta = gamma = 90 + random.uniform(-dangle,
+                                                    dangle)
+    elif csys == 'Hexagonal':
+        a = b = random.uniform(minlen, maxlen)
+        c = random.uniform(minlen, maxlen)
+        alpha = beta = 90.0
+        gamma = 120.0
+    elif csys == 'Cubic':
+        a = b = c = random.uniform(minlen, maxlen)
+        alpha = beta = gamma = 90.0
+
+    # ---------- return
+    return spg, a, b, c, alpha, beta, gamma
+
+
+def _calc_latvec(a, b, c, alpha, beta, gamma):
+    # ---------- degree to radian
+    alpha_rad = math.radians(alpha)
+    beta_rad = math.radians(beta)
+    gamma_rad = math.radians(gamma)
+    # ---------- calculate components
+    bx = b*math.cos(gamma_rad)
+    by = b*math.sin(gamma_rad)
+    cx = c*math.cos(beta_rad)
+    cy = (c*math.cos(alpha_rad)
+            - cx*math.cos(gamma_rad))/math.sin(gamma_rad)
+    cz = math.sqrt(c*c - cx*cx - cy*cy)
+    # ---------- lattice vector as list
+    a1 = [a, 0.0, 0.0]
+    a2 = [bx, by, 0.0]
+    a3 = [cx, cy, cz]
+    # ---------- return
+    return a1, a2, a3
+
+
+def _calc_cos(alpha, beta, gamma):
+    # ---------- degree to radian
+    a_rad = math.radians(alpha)
+    b_rad = math.radians(beta)
+    g_rad = math.radians(gamma)
+    cosa = math.cos(a_rad)
+    cosb = math.cos(b_rad)
+    cosg = math.cos(g_rad)
+    # ---------- return
+    return cosa, cosb, cosg
+
+
+def _gen_struc_wo_spg(atype, numIons, atomlist, a1, a2, a3, mindist, maxcnt=50):
+    '''
+    Success --> return structure data in pymatgen format
+    Failure --> return None
+    '''
+    # ---------- initialize
+    cnt = 0
+    incoord = []
+    natot = sum(numIons)    # do not use rin.natot because of vc
+    # ---------- generate internal coordinates
+    while len(incoord) < natot:
+        tmp_coord = np.random.rand(3)
+        incoord.append(tmp_coord)
+        tmp_struc = Structure([a1, a2, a3],
+                                atomlist[:len(incoord)],
+                                incoord)
+        success, mindist_ij, dist = check_distance(tmp_struc, atype, mindist)
+        if not success:
+            type0 = atype[mindist_ij[0]]
+            type1 = atype[mindist_ij[1]]
+            logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
+            incoord.pop(-1)    # cancel
+            cnt += 1
+            if maxcnt < cnt:
+                return None
+    return tmp_struc
+
+
+def _fw_input(atype, numIons, spg, a, b, c, cosa, cosb, cosg):
+    with open('input', 'w') as f:
+        f.write(f'nspecies {len(atype)}\n')
+        f.write('species_name')
+        for aa in atype:
+            f.write(f'  {aa}')
+        f.write('\n')
+        f.write('species_num')
+        for i in numIons:
+            f.write(f'  {i}')
+        f.write('\n')
+        f.write(f'spacegroup  {spg}\n')
+        f.write('originchoice  1\n')
+        f.write('\n')
+        f.write(f'a  {a}\n')
+        f.write(f'b  {b}\n')
+        f.write(f'c  {c}\n')
+        f.write(f'cosa  {cosa}\n')
+        f.write(f'cosb  {cosb}\n')
+        f.write(f'cosc  {cosg}\n')
+        f.write('\n')
+        # f.write('selectone true\n')
+        f.write('randomseed auto\n')
+
+
+def _gen_struc_with_spg(atype, mindist, maxcnt):
+    '''
+    Success --> return True, structure data
+    Failure --> return False, _
+    '''
+    # ---------- load POS_WY_SKEL_ALL.json
+    with open('POS_WY_SKEL_ALL.json', 'r') as f:
+        wydata = json.load(f)
+    # ---------- generate structure
+    plat = wydata['primitivevector']
+    clat = wydata['conventionalvector']
+    n_uniq, wydata_eq_atom = _get_wydata_eq_atom(wydata)
+    eq_atomnames = {}
+    eq_positions = {}
+    # ---------- equivalent atom loop
+    for key, value in sorted(n_uniq.items(), key=lambda x: x[1]):
+        # ------ distribute eq atoms. first, special (num_uniqvar = 0),
+        #            then, others
+        cnt = 0
+        while True:
+            eq_atomnames[key], eq_positions[key] = _gen_eq_atoms(
+                wydata_eq_atom[key])
+            # -- sort in original order
+            atomnames = []
+            positions = []
+            for key_a, value_a in sorted(eq_atomnames.items()):
+                atomnames += eq_atomnames[key_a]
+                positions += eq_positions[key_a]
+            # -- Cartesian coordinate; use clat (not plat)
+            cart = []
+            for p in positions:
+                v = np.zeros(3)
+                for i in range(3):
+                    a = np.array(clat[i])
+                    v += p[i] * a
+                cart.append(v)
+            # -- check minimum distance
+            spgstruc = Structure(plat, atomnames, cart,
+                                    coords_are_cartesian=True)
+            success, mindist_ij, dist = check_distance(spgstruc, atype, mindist)
+            if not success:
+                type0 = atype[mindist_ij[0]]
+                type1 = atype[mindist_ij[1]]
+                logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
+                # failure
+                # num_uniqvar = 0 --> value == 0
+                cnt = maxcnt + 1 if value == 0 else cnt + 1
+                if maxcnt < cnt:
+                    return False, spgstruc    # spgstruc is dummy
             else:
-                spg = random.choice(rin.spgnum)
-            if 1 <= spg <= 2:
-                csys = 'Triclinic'
-            elif 3 <= spg <= 15:
-                csys = 'Monoclinic'
-            elif 16 <= spg <= 74:
-                csys = 'Orthorhombic'
-            elif 75 <= spg <= 142:
-                csys = 'Tetragonal'
-            elif 143 <= spg <= 167:
-                # trigonal includes rhombohedral in find_wy
-                csys = 'Trigonal'
-            elif 168 <= spg <= 194:
-                csys = 'Hexagonal'
-            elif 195 <= spg <= 230:
-                csys = 'Cubic'
+                break    # break while loop --> next eq atoms
+    return True, spgstruc
+
+def _get_wydata_eq_atom(wydata):
+    i = 0    # count eq_atom, not atom
+    n_uniq = {}    # num_uniqvar each eq_atom
+    wydata_eq_atom = {}    # wydata each eq_atom
+    for specie in wydata['atoms']:
+        for wydata2 in specie:    # equivalent atom loop
+            n_uniq[i] = wydata2[0]['num_uniqvar']
+            wydata_eq_atom[i] = wydata2
+            i += 1
+    return n_uniq, wydata_eq_atom
+
+def _gen_eq_atoms(wydata2):
+    eq_atomnames = []
+    eq_positions = []
+    rval = np.random.random_sample(3)
+    for each in wydata2:
+        pos = []
+        for ch in each['xyzch']:
+            if ch == '-2x':
+                pos.append(-2.0 * rval[0])
+            elif ch == '-x+y':
+                pos.append(-rval[0] + rval[1])
+            elif ch == '-z':
+                pos.append(-rval[2])
+            elif ch == '-y':
+                pos.append(-rval[1])
+            elif ch == '-x':
+                pos.append(-rval[0])
+            elif ch == '0':
+                pos.append(0.0)
+            elif ch == 'x':
+                pos.append(rval[0])
+            elif ch == 'y':
+                pos.append(rval[1])
+            elif ch == 'z':
+                pos.append(rval[2])
+            elif ch == 'x-y':
+                pos.append(rval[0] - rval[1])
+            elif ch == '2x':
+                pos.append(2.0 * rval[0])
             else:
-                logger.error('spg is wrong')
+                logger.error('unknown ch in conversion in gen_wycoord')
                 raise SystemExit(1)
-        # ---------- generate lattice constants a, b, c, alpha, beta, gamma
-        if csys == 'Triclinic':
-            t1 = random.uniform(rin.minlen, rin.maxlen)
-            t2 = random.uniform(rin.minlen, rin.maxlen)
-            t3 = random.uniform(rin.minlen, rin.maxlen)
-            t = [t1, t2, t3]
-            t.sort()
-            a, b, c = t
-            r = random.random()
-            if r < 0.5:    # Type I
-                alpha = 90.0 - random.uniform(0, rin.dangle)
-                beta  = 90.0 - random.uniform(0, rin.dangle)
-                gamma = 90.0 - random.uniform(0, rin.dangle)
-            else:    # Type II
-                alpha = 90.0 + random.uniform(0, rin.dangle)
-                beta  = 90.0 + random.uniform(0, rin.dangle)
-                gamma = 90.0 + random.uniform(0, rin.dangle)
-        elif csys == 'Monoclinic':
-            a = random.uniform(rin.minlen, rin.maxlen)
-            b = random.uniform(rin.minlen, rin.maxlen)
-            c = random.uniform(rin.minlen, rin.maxlen)
-            if a > c:
-                a, c = c, a
-            alpha = gamma = 90.0
-            beta = 90.0 + random.uniform(0, rin.dangle)
-        elif csys == 'Orthorhombic':
-            t1 = random.uniform(rin.minlen, rin.maxlen)
-            t2 = random.uniform(rin.minlen, rin.maxlen)
-            t3 = random.uniform(rin.minlen, rin.maxlen)
-            t = [t1, t2, t3]
-            t.sort()
-            a, b, c = t
-            alpha = beta = gamma = 90.0
-        elif csys == 'Tetragonal':
-            a = b = random.uniform(rin.minlen, rin.maxlen)
-            c = random.uniform(rin.minlen, rin.maxlen)
-            alpha = beta = gamma = 90.0
-        elif csys == 'Trigonal':
-            a = b = random.uniform(rin.minlen, rin.maxlen)
-            c = random.uniform(rin.minlen, rin.maxlen)
-            alpha = beta = 90.0
-            gamma = 120.0
-        elif csys == 'Rhombohedral':
-            a = b = c = random.uniform(rin.minlen, rin.maxlen)
-            alpha = beta = gamma = 90 + random.uniform(-rin.dangle,
-                                                       rin.dangle)
-        elif csys == 'Hexagonal':
-            a = b = random.uniform(rin.minlen, rin.maxlen)
-            c = random.uniform(rin.minlen, rin.maxlen)
-            alpha = beta = 90.0
-            gamma = 120.0
-        elif csys == 'Cubic':
-            a = b = c = random.uniform(rin.minlen, rin.maxlen)
-            alpha = beta = gamma = 90.0
-        self.spg = spg
-        self.a = a
-        self.b = b
-        self.c = c
-        self.alpha = alpha
-        self.beta = beta
-        self.gamma = gamma
-
-    def _calc_latvec(self):
-        # ---------- degree to radian
-        alpha_rad = math.radians(self.alpha)
-        beta_rad = math.radians(self.beta)
-        gamma_rad = math.radians(self.gamma)
-        # ---------- calculate components
-        bx = self.b*math.cos(gamma_rad)
-        by = self.b*math.sin(gamma_rad)
-        cx = self.c*math.cos(beta_rad)
-        cy = (self.c*math.cos(alpha_rad)
-              - cx*math.cos(gamma_rad))/math.sin(gamma_rad)
-        cz = math.sqrt(self.c*self.c - cx*cx - cy*cy)
-        # ---------- lattice vector as list
-        self.va = [self.a, 0.0, 0.0]
-        self.vb = [bx, by, 0.0]
-        self.vc = [cx, cy, cz]
-
-    def _calc_cos(self):
-        # ---------- degree to radian
-        a_rad = math.radians(self.alpha)
-        b_rad = math.radians(self.beta)
-        g_rad = math.radians(self.gamma)
-        self.cosa = math.cos(a_rad)
-        self.cosb = math.cos(b_rad)
-        self.cosg = math.cos(g_rad)
-
-    def _gen_struc_wo_spg(self, numIons):
-        '''
-        Success --> return structure data in pymatgen format
-        Failure --> return None
-        '''
-        # ---------- initialize
-        cnt = 0
-        incoord = []
-        natot = sum(numIons)    # do not use rin.natot because of vc
-        # ---------- generate internal coordinates
-        while len(incoord) < natot:
-            tmp_coord = np.random.rand(3)
-            incoord.append(tmp_coord)
-            tmp_struc = Structure([self.va, self.vb, self.vc],
-                                  self.atomlist[:len(incoord)],
-                                  incoord)
-            success, mindist_ij, dist = check_distance(tmp_struc,
-                                                       rin.atype,
-                                                       self.mindist)
-            if not success:
-                type0 = rin.atype[mindist_ij[0]]
-                type1 = rin.atype[mindist_ij[1]]
-                logger.warning(f'mindist in _gen_struc_wo_spg: {type0} - {type1}, {dist}. retry.')
-                incoord.pop(-1)    # cancel
-                cnt += 1
-                if rin.maxcnt < cnt:
-                    return None
-        return tmp_struc
-
-    def _fw_input(self, numIons):
-        with open('input', 'w') as f:
-            f.write('nspecies {}\n'.format(len(rin.atype)))
-            f.write('species_name')
-            for aa in rin.atype:
-                f.write('  {}'.format(aa))
-            f.write('\n')
-            f.write('species_num')
-            for i in numIons:
-                f.write('  {}'.format(i))
-            f.write('\n')
-            f.write('spacegroup  {}\n'.format(self.spg))
-            f.write('originchoice  1\n')
-            f.write('\n')
-            f.write('a  {}\n'.format(self.a))
-            f.write('b  {}\n'.format(self.b))
-            f.write('c  {}\n'.format(self.c))
-            f.write('cosa  {}\n'.format(self.cosa))
-            f.write('cosb  {}\n'.format(self.cosb))
-            f.write('cosc  {}\n'.format(self.cosg))
-            f.write('\n')
-            # f.write('selectone true\n')
-            f.write('randomseed auto\n')
-
-    def _gen_struc_with_spg(self):
-        '''
-        Success --> return True, structure data
-        Failure --> return False, _
-        '''
-        # ---------- load POS_WY_SKEL_ALL.json
-        with open('POS_WY_SKEL_ALL.json', 'r') as f:
-            wydata = json.load(f)
-        # ---------- generate structure
-        plat = wydata['primitivevector']
-        clat = wydata['conventionalvector']
-        n_uniq, wydata_eq_atom = self._get_wydata_eq_atom(wydata)
-        eq_atomnames = {}
-        eq_positions = {}
-        # ---------- equivalent atom loop
-        for key, value in sorted(n_uniq.items(), key=lambda x: x[1]):
-            # ------ distribute eq atoms. first, special (num_uniqvar = 0),
-            #            then, others
-            cnt = 0
-            while True:
-                eq_atomnames[key], eq_positions[key] = self._gen_eq_atoms(
-                    wydata_eq_atom[key])
-                # -- sort in original order
-                atomnames = []
-                positions = []
-                for key_a, value_a in sorted(eq_atomnames.items()):
-                    atomnames += eq_atomnames[key_a]
-                    positions += eq_positions[key_a]
-                # -- Cartesian coordinate; use clat (not plat)
-                cart = []
-                for p in positions:
-                    v = np.zeros(3)
-                    for i in range(3):
-                        a = np.array(clat[i])
-                        v += p[i] * a
-                    cart.append(v)
-                # -- check minimum distance
-                spgstruc = Structure(plat, atomnames, cart,
-                                     coords_are_cartesian=True)
-                success, mindist_ij, dist = check_distance(spgstruc,
-                                                           rin.atype,
-                                                           self.mindist)
-                if not success:
-                    type0 = rin.atype[mindist_ij[0]]
-                    type1 = rin.atype[mindist_ij[1]]
-                    logger.warning(f'mindist in _gen_struc_with_spg: {type0} - {type1}, {dist}. retry.')
-                    # failure
-                    # num_uniqvar = 0 --> value == 0
-                    cnt = rin.maxcnt + 1 if value == 0 else cnt + 1
-                    if rin.maxcnt < cnt:
-                        return False, spgstruc    # spgstruc is dummy
-                else:
-                    break    # break while loop --> next eq atoms
-        return True, spgstruc
-
-    def _get_wydata_eq_atom(self, wydata):
-        i = 0    # count eq_atom, not atom
-        n_uniq = {}    # num_uniqvar each eq_atom
-        wydata_eq_atom = {}    # wydata each eq_atom
-        for specie in wydata['atoms']:
-            for wydata2 in specie:    # equivalent atom loop
-                n_uniq[i] = wydata2[0]['num_uniqvar']
-                wydata_eq_atom[i] = wydata2
-                i += 1
-        return n_uniq, wydata_eq_atom
-
-    def _gen_eq_atoms(self, wydata2):
-        eq_atomnames = []
-        eq_positions = []
-        rval = np.random.random_sample(3)
-        for each in wydata2:
-            pos = []
-            for ch in each['xyzch']:
-                if ch == '-2x':
-                    pos.append(-2.0 * rval[0])
-                elif ch == '-x+y':
-                    pos.append(-rval[0] + rval[1])
-                elif ch == '-z':
-                    pos.append(-rval[2])
-                elif ch == '-y':
-                    pos.append(-rval[1])
-                elif ch == '-x':
-                    pos.append(-rval[0])
-                elif ch == '0':
-                    pos.append(0.0)
-                elif ch == 'x':
-                    pos.append(rval[0])
-                elif ch == 'y':
-                    pos.append(rval[1])
-                elif ch == 'z':
-                    pos.append(rval[2])
-                elif ch == 'x-y':
-                    pos.append(rval[0] - rval[1])
-                elif ch == '2x':
-                    pos.append(2.0 * rval[0])
-                else:
-                    logger.error('unknown ch in conversion in gen_wycoord')
-                    raise SystemExit(1)
-            pos = np.array(pos)
-            eq_positions.append(pos + each['add'])
-            eq_atomnames.append(each['name'])
-        return eq_atomnames, eq_positions
-
-    def _rm_files(self, files=['input', 'POS_WY_SKEL_ALL.json']):
-        for rfile in files:
-            if os.path.isfile(rfile):
-                os.remove(rfile)
+        pos = np.array(pos)
+        eq_positions.append(pos + each['add'])
+        eq_atomnames.append(each['name'])
+    return eq_atomnames, eq_positions
+
+def _rm_files(files=['input', 'POS_WY_SKEL_ALL.json']):
+    for rfile in files:
+        if os.path.isfile(rfile):
+            os.remove(rfile)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/RS/rs_restart.py` & `csp_cryspy-1.3.0/src/cryspy/RS/rs_restart.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-'''
-Restart random search
-'''
-
 from ..IO import io_stat, pkl_data
-from ..IO import read_input as rin
 
 
-def restart(stat, prev_nstruc):
+def restart(rin, prev_nstruc):
     # ---------- load rs data
-    id_queueing, id_running = pkl_data.load_rs_id()
+    id_queueing = pkl_data.load_id_queueing()
 
     # ---------- append id_queueing
     id_queueing.extend([i for i in range(prev_nstruc, rin.tot_struc)])
 
     # ---------- status
+    stat = io_stat.stat_read()
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- save
-    rs_id_data = (id_queueing, id_running)
-    pkl_data.save_rs_id(rs_id_data)
+    pkl_data.save_id_queueing(id_queueing)
 
     # ---------- ext
     if rin.calc_code == 'ext':
         with open('ext/stat_job', 'w') as fstat:
             fstat.write('out\n')
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interactive/energy_plot.py` & `csp_cryspy-1.3.0/src/cryspy/interactive/energy_plot.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/ASE/calc_files_ase.py` & `csp_cryspy-1.3.0/src/cryspy/interface/OMX/calc_files_OMX.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 '''
-Calculation files in ASE
+Calculation files in OpenMX
+written by H. Sawahata 2020/03/09
+info at hikaruri.jp
 '''
 
 from logging import getLogger
 import os
 
-from ...IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def check_input_ase():
-    # ---------- prepare rin.jobfile, POTCAR, INCAR
-    calc_inputs = [rin.jobfile, rin.ase_python]
 
-    # ----- check required files
+def check_input_OMX(rin):
+    # ---------- prepare rin.jobfile, rin.OMX_infile
+    calc_inputs = [rin.jobfile, rin.OMX_infile]
+
+    # ------ check required files
     for f in calc_inputs:
-        if f == rin.ase_python:
-            finfiles = [rin.ase_python + '_{}'.format(i) for i in range(
+        if f == rin.OMX_infile:
+            finfiles = [rin.OMX_infile + f'_{i}' for i in range(
                 1, rin.nstage+1)]
             for ff in finfiles:
-                if not os.path.isfile('./calc_in/'+ff):
-                    logger.error('Could not find ./calc_in/'+ff)
+                if not os.path.isfile('./calc_in/' + ff):
+                    logger.error('Could not find ./calc_in/' + ff)
                     raise SystemExit(1)
         else:
-            if not os.path.isfile('./calc_in/'+f):
-                logger.error('Could not find ./calc_in/'+f)
-                raise SystemExit(1)
+            if not os.path.isfile('./calc_in/' + f):
+                logger.error('Could not find ./calc_in/' + f)
+                raise SystemExit(1)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/ASE/collect_ase.py` & `csp_cryspy-1.3.0/src/cryspy/interface/ASE/collect_ase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-'''
-Collect results in ASE
-'''
-
 from logging import getLogger
 
 import numpy as np
 from pymatgen.core import Structure
 
 
 logger = getLogger('cryspy')
 
+
 def collect_ase(cid, work_path, nat):
     # ---------- natot
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     # ---------- etc
     magmom = np.nan
     check_opt = 'no_file'    # always no_file in ASE for now
     # ---------- collect energy
     try:
         with open(work_path+'log.tote') as f:
             lines = f.readlines()
         energy = float(lines[-1].split()[0])    # in eV/cell
         energy = energy/float(natot)    # eV/cell --> eV/atom
     except Exception as e:
         energy = np.nan    # error
-        logger.warning(str(e.args[0]) + f':    Structure ID {cid}, could not obtain energy from log.tote')
+        logger.warning(f'{e}:    Structure ID {cid}, could not obtain energy from log.tote')
     # ---------- collect CONTCAR
     try:
         opt_struc = Structure.from_file(work_path+'CONTCAR')
     except Exception:
         opt_struc = None
     # ---------- check
     if np.isnan(energy):
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/ASE/ctrl_job_ase.py` & `csp_cryspy-1.3.0/src/cryspy/interface/ASE/ctrl_job_ase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,53 @@
-'''
-Control jobs in ASE
-'''
-
 from logging import getLogger
 import os
 import shutil
 
-from ...IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def next_stage_ase(stage, work_path):
+def next_stage_ase(rin, stage, work_path):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename ASE files at the current stage
     ase_files = ['POSCAR', 'CONTCAR', 'log.tote']
-    for f in ase_files:
-        if not os.path.isfile(work_path+f):
-            logger.error('Not found '+work_path+f)
+    for file in ase_files:
+        if not os.path.isfile(work_path + file):
+            logger.error('Not found ' + work_path + file)
             raise SystemExit(1)
-        os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
+        os.rename(work_path + file, work_path + f'stage{stage}_' + file)
 
     # ---------- cp CONTCAR POSCAR
-    shutil.copyfile(work_path+'stage{}_CONTCAR'.format(stage),
-                    work_path+'POSCAR')
+    shutil.copyfile(work_path + f'stage{stage}_CONTCAR', work_path + 'POSCAR')
 
     # ---------- copy the input file from ./calc_in for the next stage
-    finfile = './calc_in/'+rin.ase_python+'_{}'.format(stage + 1)
+    finfile = './calc_in/' +rin.ase_python + f'_{stage+1}'
     shutil.copyfile(finfile, work_path+rin.ase_python)
 
     # ---------- return
     return skip_flag
 
 
-def next_struc_ase(structure, cid, work_path):
+def next_struc_ase(rin, structure, cid, work_path):
     # ---------- copy files
     calc_inputs = [rin.ase_python]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.ase_python else f
         if not os.path.isfile('./calc_in/' + ff):
             logger.error('Could not find ./calc_in/' + ff)
             raise SystemExit(1)
-        # ------ e.g. cp ./calc_in/INCAR_1 work0001/INCAR
+        # ------ e.g. cp ./calc_in/INCAR_1 work/1/INCAR
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate POSCAR
     structure.to(fmt='poscar', filename=work_path+'POSCAR')
     if not os.path.isfile(work_path+'POSCAR'):
         logger.error(f'Could not find {work_path}POSCAR')
 
     # ---------- Change the title of POSCAR
     with open(work_path+'POSCAR', 'r') as f:
         lines = f.readlines()
-    lines[0] = 'ID_{}\n'.format(cid)
+    lines[0] = f'ID_{cid}\n'
     with open(work_path+'POSCAR', 'w') as f:
         for line in lines:
             f.write(line)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/calc_files_lammps.py` & `csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-'''
-Calculation files in LAMMPS
-'''
-
 from logging import getLogger
 import os
 
-from ...IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def check_input_lammps():
+
+def check_input_lammps(rin):
     # ---------- prepare rin.jobfile, rin.lammps_potential, rin.rammps_infile
     if rin.lammps_potential is None:
         calc_inputs = [rin.jobfile, rin.lammps_infile]
     else:
         calc_inputs = [rin.jobfile, rin.lammps_infile] + rin.lammps_potential
 
     # ----- check required files
     for f in calc_inputs:
         if f == rin.lammps_infile:
-            finfiles = [rin.lammps_infile + '_{}'.format(i) for i in range(
+            finfiles = [rin.lammps_infile + f'_{i}' for i in range(
                 1, rin.nstage+1)]
             for ff in finfiles:
                 if not os.path.isfile('./calc_in/'+ff):
                     logger.error('Could not find ./calc_in/'+ff)
                     raise SystemExit(1)
         else:
             if not os.path.isfile('./calc_in/'+f):
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/collect_lammps.py` & `csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/collect_lammps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-'''
-Collect results in LAMMPS
-'''
-
 from logging import getLogger
 import numpy as np
 
 from . import structure as lammps_structure
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def collect_lammps(cid, work_path, nat):
+
+def collect_lammps(rin, cid, work_path, nat):
     # ---------- natot
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     # ---------- check optimization in current stage & obtain energy
     energy = np.nan
     check_opt = 'not_yet'
     try:
         with open(work_path+rin.lammps_outfile, 'r') as fout:
@@ -27,24 +23,24 @@
                 check_opt = 'not_yet'
                 break
             elif 'Minimization stats:' in line:
                 energy = float(lines[i+3].split()[2])  # in eV (units is metal)
                 energy = energy/float(natot)    # eV/cell --> eV/atom
                 check_opt = 'done'
     except Exception as e:
-        logger.warning(str(e.args[0]) + f':    Structure ID {cid},'
+        logger.warning(f'{e}:    Structure ID {cid},'
                        f'could not obtain energy from {rin.lammps_outfile}')
         energy = np.nan    # error
         check_opt = 'no_file'
 
     # ---------- obtain magmom
     magmom = np.nan    # magnetic moment is not calculated
 
     # ---------- collect the last structure
     try:
-        opt_struc = lammps_structure.from_file(work_path+'log.struc', nat)
+        opt_struc = lammps_structure.from_file(rin, work_path+'log.struc', nat)
     except Exception as e:
-        logger.warning(str(e.args[0]))
+        logger.warning(e)
         opt_struc = None
 
     # ---------- return
     return opt_struc, energy, magmom, check_opt
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py` & `csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-'''
-Control jobs in LAMMPS
-'''
-
 from logging import getLogger
 import os
 import shutil
 
 from . import structure as lammps_structure
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def next_stage_lammps(stage, work_path, nat):
+
+def next_stage_lammps(rin, stage, work_path, nat):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename lammps files at the current stage
     lammps_files = [rin.lammps_infile, rin.lammps_outfile,
                     rin.lammps_data, 'log.struc']
-    for f in lammps_files:
-        if not os.path.isfile(work_path+f):
-            logger.error('Not found '+work_path+f)
+    for file in lammps_files:
+        if not os.path.isfile(work_path + file):
+            logger.error('Not found ' + work_path + file)
             raise SystemExit(1)
-        os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
+        os.rename(work_path + file, work_path + f'stage{stage}_' + file)
 
     # ---------- copy the input file from ./calc_in for the next stage
-    finfile = './calc_in/'+rin.lammps_infile+'_{}'.format(stage + 1)
+    finfile = './calc_in/' + rin.lammps_infile + f'_{stage + 1}'
     shutil.copyfile(finfile, work_path+rin.lammps_infile)
 
     # ---------- generate the structure data file
     try:
         structure = lammps_structure.from_file(
-            work_path+'stage{}_log.struc'.format(stage), nat)
+            rin, work_path + f'stage{stage}_log.struc', nat)
     except ValueError:
         skip_flag = True
         logger.warning('    error in lammps,  skip this structure')
         return skip_flag
-    with open(work_path+'stage{}_'.format(stage)+rin.lammps_data, 'r') as f:
+    with open(work_path + f'stage{stage}_' + rin.lammps_data, 'r') as f:
         lines = f.readlines()
     title = lines[0][7:]    # string following 'data_'
-    lammps_structure.write(structure,
+    lammps_structure.write(rin,
+                           structure,
                            work_path+rin.lammps_data,
                            nat,
                            title=title)
 
     # ---------- return
     return skip_flag
 
 
-def next_struc_lammps(structure, cid, work_path, nat):
+def next_struc_lammps(rin, structure, cid, work_path, nat):
     # ---------- copy files
     if rin.lammps_potential is None:
         calc_inputs = [rin.lammps_infile]
     else:
         calc_inputs = [rin.lammps_infile] + rin.lammps_potential
     for f in calc_inputs:
         ff = f+'_1' if f == rin.lammps_infile else f
         if not os.path.isfile('./calc_in/'+ff):
             logger.error('Could not find ./calc_in/'+ff)
             raise SystemExit(1)
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate the structure data file
-    lammps_structure.write(structure,
+    lammps_structure.write(rin,
+                           structure,
                            work_path+rin.lammps_data, nat,
-                           title='ID_{0:d}'.format(cid))
+                           title=f'ID_{cid}')
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/structure.py` & `csp_cryspy-1.3.0/src/cryspy/interface/LAMMPS/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 '''
 Structure file for LAMMPS
 '''
-
 import itertools
 
 import numpy as np
 from pymatgen.core import Structure
 
-from ...IO import read_input as rin
-
 
-def from_file(name, nat):
+def from_file(rin, name, nat):
     # ---------- natot
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     # ---------- last structure
     with open(name, 'r') as f:
         lines = f.readlines()
     for i, line in enumerate(lines):
         if 'ITEM: TIMESTEP' in line:
@@ -48,15 +45,15 @@
     species = list(itertools.chain.from_iterable(species))
 
     structure = Structure(lattice, species, coords)
 
     return structure
 
 
-def write(structure, output, nat, title="LAMMPS"):
+def write(rin, structure, output, nat, title="LAMMPS"):
     # ---------- convert lattice constants and angles to LAMMPS format
     cos = lambda x: np.cos(np.deg2rad(x))
     sqrt = lambda x: np.sqrt(x)
 
     a, b, c = structure.lattice.abc
     alpha, beta, gamma = structure.lattice.angles
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/OMX/calc_files_OMX.py` & `csp_cryspy-1.3.0/src/cryspy/interface/ASE/calc_files_ase.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-'''
-Calculation files in OpenMX
-written by H. Sawahata 2020/03/09
-info at hikaruri.jp
-'''
-
 from logging import getLogger
 import os
 
-from ...IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def check_input_OMX():
-    # ---------- prepare rin.jobfile, rin.OMX_infile
-    calc_inputs = [rin.jobfile, rin.OMX_infile]
 
-    # ------ check required files
+def check_input_ase(rin):
+    # ---------- prepare rin.jobfile, POTCAR, INCAR
+    calc_inputs = [rin.jobfile, rin.ase_python]
+
+    # ----- check required files
     for f in calc_inputs:
-        if f == rin.OMX_infile:
-            finfiles = [rin.OMX_infile + '_{}'.format(i) for i in range(
+        if f == rin.ase_python:
+            finfiles = [rin.ase_python + f'_{i}' for i in range(
                 1, rin.nstage+1)]
             for ff in finfiles:
-                if not os.path.isfile('./calc_in/' + ff):
-                    logger.error('Could not find ./calc_in/' + ff)
+                if not os.path.isfile('./calc_in/'+ff):
+                    logger.error('Could not find ./calc_in/'+ff)
                     raise SystemExit(1)
         else:
-            if not os.path.isfile('./calc_in/' + f):
-                logger.error('Could not find ./calc_in/' + f)
-                raise SystemExit(1)
+            if not os.path.isfile('./calc_in/'+f):
+                logger.error('Could not find ./calc_in/'+f)
+                raise SystemExit(1)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/OMX/collect_OMX.py` & `csp_cryspy-1.3.0/src/cryspy/interface/OMX/collect_OMX.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 from logging import getLogger
 
 import numpy as np
 import re
 from pymatgen.core.units import Energy
 
 from . import structure as OMX_structure
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def collect_OMX(cid, work_path, nat):
+def collect_OMX(rin, cid, work_path, nat):
     # ---------- check optimization in previous stage (done)
     # If *.out file exists, the calculation is done.
     try:
         with open(work_path+rin.OMX_outfile, 'r') as fpout:
             lines = fpout.readlines()
         check_opt = 'done'
     except Exception as e:
-        logger.warning(str(e.args[0]))
+        logger.warning(e)
         check_opt = 'no_file'
 
     # ---------- obtain energy and magmom (done)
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     try:
         with open(work_path+rin.OMX_outfile, 'r') as fpout:
             lines = fpout.readlines()
@@ -44,36 +43,36 @@
             if line.find("muB") >= 0:
                 muB = line.split()
                 magmom = float(muB[4])
                 break
     except Exception as e:
         energy = np.nan    # error
         magmom = np.nan    # error
-        logger.warning(str(e.args[0]) + f':    Structure ID {cid},'
+        logger.warning(f'{e}:    Structure ID {cid},'
                        f' could not obtain energy from {rin.OMX_outfile}')
 
     # ---------- collect the last structure (yet)
     try:
         lines_cell = OMX_structure.extract_cell_parameters_from_outfile(
             work_path+rin.OMX_outfile)
         if lines_cell is None:
             lines_cell = OMX_structure.extract_cell_parameters_from_infile(
             work_path+rin.OMX_infile)
         lines_atom = OMX_structure.extract_atomic_positions_from_outfile(
             work_path+rin.OMX_outfile, nat)
         if lines_atom is None:
             lines_atom = OMX_structure.extract_atomic_positions_from_infile(
-                work_path+rin.OMX_infile, nat)
+                rin, work_path+rin.OMX_infile, nat)
         opt_struc = OMX_structure.from_lines(lines_cell, lines_atom)
         # ------ opt_OMX-structure
         with open('./data/opt_OMX-structure', 'a') as fstruc:
-            fstruc.write('# ID {0:d}\n'.format(cid))
-        OMX_structure.write(opt_struc, './data/opt_OMX-structure', mode='a')
+            fstruc.write(f'# ID {cid}\n')
+        OMX_structure.write(rin, opt_struc, './data/opt_OMX-structure', mode='a')
     except Exception as e:
-        logger.warning(str(e.args[0]))
+        logger.warning(e)
         opt_struc = None
 
     # ---------- check
     if np.isnan(energy):
         opt_struc = None
     if opt_struc is None:
         energy = np.nan
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/OMX/ctrl_job_OMX.py` & `csp_cryspy-1.3.0/src/cryspy/interface/OMX/ctrl_job_OMX.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,64 +9,63 @@
 import shutil
 
 from pymatgen.io.vasp import Kpoints
 
 from . import structure as OMX_structure
 from ...IO.out_results import out_kpts
 from ...IO import pkl_data
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def next_stage_OMX(stage, work_path, nat, kpt_data, cid):
+def next_stage_OMX(rin, stage, work_path, nat, kpt_data, cid):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename OpenMX files at the current stage
     OMX_files = [rin.OMX_infile, rin.OMX_outfile]
-    for f in OMX_files:
-        if not os.path.isfile(work_path+f):
-            logger.error('Not found '+work_path+f)
+    for file in OMX_files:
+        if not os.path.isfile(work_path + file):
+            logger.error('Not found ' + work_path + file)
             raise SystemExit(1)
-        os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
+        os.rename(work_path + file, work_path + f'stage{stage}_' + file)
 
     # ---------- next structure
     try:
         lines_cell = OMX_structure.extract_cell_parameters_from_outfile(
-            work_path+'stage{}_'.format(stage)+rin.OMX_outfile)
+            work_path+f'stage{stage}_'+rin.OMX_outfile)
         if lines_cell is None:
             lines_cell = OMX_structure.extract_cell_parameters_from_infile(
-                work_path+'stage{}_'.format(stage)+rin.OMX_infile)
+                work_path+f'stage{stage}_'+rin.OMX_infile)
         lines_atom = OMX_structure.extract_atomic_positions_from_outfile(
-            work_path+'stage{}_'.format(stage)+rin.OMX_outfile, nat)
+            work_path+f'stage{stage}_'+rin.OMX_outfile, nat)
         if lines_atom is None:
             lines_atom = OMX_structure.extract_atomic_positions_from_infile(
-                work_path+'stage{}_'.format(stage)+rin.OMX_infile, nat)
+                rin, work_path+f'stage{stage}_'+rin.OMX_infile, nat)
         structure = OMX_structure.from_lines(lines_cell, lines_atom)
     except ValueError:
         skip_flag = True
         kpt_data[cid].append(['skip'])
         pkl_data.save_kpt(kpt_data)
         out_kpts(kpt_data)
         logger.info(f'    error in OpenMX,  skip structure {cid}')
         return skip_flag, kpt_data
 
     # ---------- copy the input file from ./calc_in for the next stage
-    finput = './calc_in/'+rin.OMX_infile+'_{}'.format(stage + 1)
+    finput = './calc_in/'+rin.OMX_infile+f'_{stage + 1}'
     shutil.copyfile(finput, work_path+rin.OMX_infile)
 
     # ---------- "Atoms.Number" (<-- natot) in OMX_infile for EA-vc
     if rin.algo == 'EA-vc':
         _replace_nat(work_path+rin.OMX_infile, nat)
 
     # ---------- append structure info.
     with open(work_path+rin.OMX_infile, 'a') as fin:
         fin.write('\n')
-    OMX_structure.write(structure, work_path+rin.OMX_infile, mode='a')
+    OMX_structure.write(rin, structure, work_path+rin.OMX_infile, mode='a')
 
     # ---------- K_POINTS
     # kppvol[0]: <--> stage 1, kppvol[1] <--> stage2, ...
     #   so (stage - 1): current stage, stage: next stage in kppvol
     kpoints = Kpoints.automatic_density_by_vol(structure=structure,
                                                kppvol=rin.kppvol[stage])
     with open(work_path+rin.OMX_infile, 'a') as f:
@@ -79,15 +78,15 @@
     pkl_data.save_kpt(kpt_data)
     out_kpts(kpt_data)
 
     # ---------- return
     return skip_flag, kpt_data
 
 
-def next_struc_OMX(structure, cid, work_path, nat, kpt_data):
+def next_struc_OMX(rin, structure, cid, work_path, nat, kpt_data):
     # ---------- copy files
     calc_inputs = [rin.OMX_infile]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.OMX_infile else f
         if not os.path.isfile('./calc_in/' + ff):
             logger.error('Could not find ./calc_in/' + ff)
             raise SystemExit(1)
@@ -96,15 +95,15 @@
     # ---------- "Atoms.Number" (<-- natot) in OMX_infile for EA-vc
     if rin.algo == 'EA-vc':
         _replace_nat(work_path+rin.OMX_infile, nat)
 
     # ---------- append structure info. to the input file
     with open(work_path+rin.OMX_infile, 'a') as fin:
         fin.write('\n')
-    OMX_structure.write(structure, work_path+rin.OMX_infile, mode='a')
+    OMX_structure.write(rin, structure, work_path+rin.OMX_infile, mode='a')
 
     # ---------- K_POINTS
     kpoints = Kpoints.automatic_density_by_vol(structure=structure,
                                                kppvol=rin.kppvol[0])
     with open(work_path+rin.OMX_infile, 'a') as f:
         f.write('\n')
         f.write('scf.Kgrid  ')
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/OMX/structure.py` & `csp_cryspy-1.3.0/src/cryspy/interface/OMX/structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 written by H. Sawahata 2020/03/09
 info at hikaruri.jp
 '''
 
 from pymatgen.core import Structure
 from pymatgen.core.units import Length
 
-from ...IO import read_input as rin
 
 import re
 
+
 def extract_cell_parameters_from_outfile(filename):
     # ---------- last Cell vectors a1, a2, a3
     with open(filename, 'r') as f:
         lines = f.readlines()
     lines_cell = None
     for i,line in enumerate(lines):
         if re.search('a1', line):
@@ -47,15 +47,15 @@
         if re.search('final', line):
             ibegin = i + 4
             iend = ibegin + natot
             lines_atom = lines[ibegin:iend]
             break
     return lines_atom
 
-def extract_atomic_positions_from_infile(filename):
+def extract_atomic_positions_from_infile(rin, filename):
     # ---------- last atomic positions
     with open(filename, 'r') as f:
         lines = f.readlines()
     lines_atom = []
     for i,line in enumerate(lines):
         if re.search('<Atoms.SpeciesAndCoordinates', line):
             for j in range(0,rin.natot):
@@ -75,15 +75,15 @@
     for line in lines_atom:
         fields = line.split()
         species.append(fields[1])
         coords.append([float(x) for x in fields[2:5]])
     structure = Structure(lattice, species, coords)
     return structure
 
-def write(structure, output, mode='w'):
+def write(rin, structure, output, mode='w'):
     # ---------- get in POSCAR format
     poscar = structure.to(fmt='poscar')
     lines = poscar.split('\n')[:-1]
     lines = [line+'\n' for line in lines]
     # ---------- write in OMX format (yet)
     with open(output, mode) as f:
         f.write('<Atoms.UnitVectors\n')
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/QE/calc_files_qe.py` & `csp_cryspy-1.3.0/src/cryspy/interface/soiap/calc_files_soiap.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-'''
-Calculation files in Quantum ESPRESSO
-'''
-
 from logging import getLogger
 import os
 
-from ...IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def check_input_qe():
-    # ---------- prepare rin.jobfile, rin.qe_infile
-    calc_inputs = [rin.jobfile, rin.qe_infile]
 
-    # ------ check required files
+def check_input_soiap(rin):
+    # ---------- prepare rin.jobfile, rin.soiap_infile
+    calc_inputs = [rin.jobfile, rin.soiap_infile]
+
+    # ----- check required files
     for f in calc_inputs:
-        if f == rin.qe_infile:
-            finfiles = [rin.qe_infile + '_{}'.format(i) for i in range(
-                1, rin.nstage+1)]
+        if f == rin.soiap_infile:
+            finfiles = [rin.soiap_infile + f'_{i}'
+                        for i in range(1, rin.nstage+1)]
             for ff in finfiles:
-                if not os.path.isfile('./calc_in/' + ff):
-                    logger.error('Could not find ./calc_in/' + ff)
+                if not os.path.isfile('./calc_in/'+ff):
+                    logger.error('Could not find ./calc_in/'+ff)
                     raise SystemExit(1)
         else:
-            if not os.path.isfile('./calc_in/' + f):
-                logger.error('Could not find ./calc_in/' + f)
-                raise SystemExit(1)
+            if not os.path.isfile('./calc_in/'+f):
+                logger.error('Could not find ./calc_in/'+f)
+                raise SystemExit(1)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/QE/collect_qe.py` & `csp_cryspy-1.3.0/src/cryspy/interface/QE/collect_qe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-'''
-Collect results in Quantum ESPRESSO
-'''
-
 from logging import getLogger
 
 import numpy as np
 from pymatgen.core import Structure
 
 from . import structure as qe_structure
 from ...util import constants
 from ...IO import pkl_data
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def collect_qe(cid, work_path, nat):
+def collect_qe(rin, cid, work_path, nat):
     # ---------- check optimization in previous stage
     try:
         with open(work_path+rin.qe_outfile, 'r') as fpout:
             lines = fpout.readlines()
         check_opt = 'not_yet'
         for line in lines:
             if 'End final coordinates' in line:
                 check_opt = 'done'
     except Exception as e:
-        logger.warning(str(e.args[0]))
+        logger.warning(e)
         check_opt = 'no_file'
 
     # ---------- obtain energy and magmom
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     try:
         with open(work_path+rin.qe_outfile, 'r') as fpout:
             lines = fpout.readlines()
@@ -48,15 +43,15 @@
             if line.find("total magnetization") >= 0:
                 muB = line.split()
                 magmom = float(muB[3])
                 break
     except Exception as e:
         energy = np.nan    # error
         magmom = np.nan    # error
-        logger.warning(str(e.args[0]) + f':    Structure ID {cid},'
+        logger.warning(f'{e}:    Structure ID {cid},'
                        f'could not obtain energy from {rin.qe_outfile}')
 
     # ---------- collect the last structure
     try:
         lines_cell = qe_structure.extract_cell_parameters(
             work_path+rin.qe_outfile)
         if lines_cell is None:
@@ -67,32 +62,32 @@
         if lines_atom is None:
             lines_atom = qe_structure.extract_atomic_positions(
                 work_path+rin.qe_infile, nat)
         opt_struc = qe_structure.from_lines(lines_cell, lines_atom)
 
         # ------ opt_qe-structure
         with open('./data/opt_qe-structure', 'a') as fstruc:
-            fstruc.write('# ID {0:d}\n'.format(cid))
+            fstruc.write(f'# ID {cid}\n')
         qe_structure.write(opt_struc, './data/opt_qe-structure', mode='a')
     except Exception as e:
-        logger.warning(str(e.args[0]))
+        logger.warning(e)
         opt_struc = None
 
     # ---------- check
     if np.isnan(energy):
         opt_struc = None
     if opt_struc is None:
         energy = np.nan
         magmom = np.nan
 
     # ---------- return
     return opt_struc, energy, magmom, check_opt
 
 
-def get_energy_step_qe(energy_step_data, cid, work_path, nat):
+def get_energy_step_qe(rin, energy_step_data, cid, work_path, nat):
     '''
     get energy step data in eV/atom
 
     energy_step_data[ID][stage][step]
     energy_step_data[ID][0] <-- stage 1
     energy_step_data[ID][1] <-- stage 2
     '''
@@ -122,29 +117,29 @@
             energy_step = None    # if empty
             logger.warning(f'#### ID: {cid}: failed to parse energy_step')
         else:
             energy_step = constants.RY2EV / natot * np.array(energy_step,
                                                                dtype='float')
     except Exception as e:
         energy_step = None
-        logger.warning(str(e.args[0]) + f'#### ID: {cid}: failed to parse energy_step')
+        logger.warning(f'{e}:    ID {cid}: failed to parse energy_step')
 
     # ---------- append energy_step
     if energy_step_data.get(cid) is None:
         energy_step_data[cid] = []    # initialize
     energy_step_data[cid].append(energy_step)
 
     # ---------- save energy_step_data
     pkl_data.save_energy_step(energy_step_data)
 
     # ---------- return
     return energy_step_data
 
 
-def get_struc_step_qe(struc_step_data, cid, work_path, nat):
+def get_struc_step_qe(rin, struc_step_data, cid, work_path, nat):
     '''
     get structure step data
 
     # ---------- args
     struc_step_data: (dict) the key is structure ID
 
     struc_step_data[ID][stage][step]
@@ -157,15 +152,15 @@
         _extract_struc_qe(work_path+rin.qe_infile, struc_step, nat)
         # ------ struc step from pwscf.out
         _extract_struc_qe(work_path+rin.qe_outfile, struc_step, nat)
         # ------ delete last structure due to duplication
         struc_step.pop(-1)
     except Exception as e:
         struc_step = None
-        logger.warning(str(e.args[0]) + f'#### ID: {cid}: failed to parse in struc_step')
+        logger.warning(f'{e}:    ID {cid}: failed to parse in struc_step')
 
     # ---------- append struc_step_data
     if struc_step_data.get(cid) is None:
         struc_step_data[cid] = []    # initialize
     struc_step_data[cid].append(struc_step)
 
     # ---------- save struc_step_data
@@ -210,15 +205,15 @@
                 struc_step.append(struc)
         if 'ATOMIC_POSITIONS' in line:
             read_coords = True
             species = []
             coords = []
 
 
-def get_force_step_qe(force_step_data, cid, work_path, nat):
+def get_force_step_qe(rin, force_step_data, cid, work_path, nat):
     '''
     get force step data in eV/angstrom
 
     # ---------- args
     force_step_data: (dict) the key is structure ID
 
     force_step_data[ID][stage][step]
@@ -270,15 +265,15 @@
     # ---------- save force_step_data
     pkl_data.save_force_step(force_step_data)
 
     # ---------- return
     return force_step_data
 
 
-def get_stress_step_qe(stress_step_data, cid, work_path):
+def get_stress_step_qe(rin, stress_step_data, cid, work_path):
     '''
     get stress step data in eV/ang**3
 
     # ---------- args
     stress_step_data: (dict) the key is structure ID
 
     stress_step_data[ID][stage][step]
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/QE/ctrl_job_qe.py` & `csp_cryspy-1.3.0/src/cryspy/interface/QE/ctrl_job_qe.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,54 +7,53 @@
 import shutil
 
 from pymatgen.io.vasp import Kpoints
 
 from . import structure as qe_structure
 from ...IO.out_results import out_kpts
 from ...IO import pkl_data
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def next_stage_qe(stage, work_path, nat, kpt_data, cid):
+def next_stage_qe(rin, stage, work_path, nat, kpt_data, cid):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename QE files at the current stage
     qe_files = [rin.qe_infile, rin.qe_outfile]
-    for f in qe_files:
-        if not os.path.isfile(work_path+f):
-            logger.error('Not found '+work_path+f)
+    for file in qe_files:
+        if not os.path.isfile(work_path + file):
+            logger.error('Not found ' + work_path + file)
             raise SystemExit(1)
-        os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
+        os.rename(work_path + file, work_path + f'stage{stage}_' + file)
 
     # ---------- next structure
     try:
         lines_cell = qe_structure.extract_cell_parameters(
-            work_path+'stage{}_'.format(stage)+rin.qe_outfile)
+            work_path+f'stage{stage}_'+rin.qe_outfile)
         if lines_cell is None:
             lines_cell = qe_structure.extract_cell_parameters(
-                work_path+'stage{}_'.format(stage)+rin.qe_infile)
+                work_path+f'stage{stage}_'+rin.qe_infile)
         lines_atom = qe_structure.extract_atomic_positions(
-            work_path+'stage{}_'.format(stage)+rin.qe_outfile, nat)
+            work_path+f'stage{stage}_'+rin.qe_outfile, nat)
         if lines_atom is None:
             lines_atom = qe_structure.extract_atomic_positions(
-                work_path+'stage{}_'.format(stage)+rin.qe_infile, nat)
+                work_path+f'stage{stage}_'+rin.qe_infile, nat)
         structure = qe_structure.from_lines(lines_cell, lines_atom)
     except ValueError:
         skip_flag = True
         kpt_data[cid].append(['skip'])
         pkl_data.save_kpt(kpt_data)
         out_kpts(kpt_data)
         logger.info(f'    error in QE,  skip structure {cid}')
         return skip_flag, kpt_data
 
     # ---------- copy the input file from ./calc_in for the next stage
-    finput = './calc_in/'+rin.qe_infile+'_{}'.format(stage + 1)
+    finput = './calc_in/' + rin.qe_infile + f'_{stage + 1}'
     shutil.copyfile(finput, work_path+rin.qe_infile)
 
     # ---------- "nat" (<-- natot) in qe_infile for EA-vc
     if rin.algo == 'EA-vc':
         _replace_nat(work_path + rin.qe_infile, nat)
 
     # ---------- append structure info.
@@ -77,15 +76,15 @@
     pkl_data.save_kpt(kpt_data)
     out_kpts(kpt_data)
 
     # ---------- return
     return skip_flag, kpt_data
 
 
-def next_struc_qe(structure, cid, work_path, nat, kpt_data):
+def next_struc_qe(rin, structure, cid, work_path, nat, kpt_data):
     # ---------- copy files
     calc_inputs = [rin.qe_infile]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.qe_infile else f
         if not os.path.isfile('./calc_in/' + ff):
             logger.error('Could not find ./calc_in/' + ff)
             raise SystemExit(1)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/QE/structure.py` & `csp_cryspy-1.3.0/src/cryspy/interface/QE/structure.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/VASP/calc_files_vasp.py` & `csp_cryspy-1.3.0/src/cryspy/interface/VASP/calc_files_vasp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-'''
-Calculation files in VASP
-'''
-
 from logging import getLogger
 import os
 
-from ...IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def check_input_vasp():
+
+def check_input_vasp(rin):
     # ---------- prepare rin.jobfile, POTCAR, INCAR
     calc_inputs = [rin.jobfile, 'POTCAR', 'INCAR']
 
     # ------ check required files
     for f in calc_inputs:
         if f == 'INCAR':
-            fincars = ['INCAR_{}'.format(i) for i in range(1, rin.nstage+1)]
+            fincars = [f'INCAR_{i}' for i in range(1, rin.nstage+1)]
             for ff in fincars:
                 if not os.path.isfile('./calc_in/' + ff):
                     logger.error('Could not find ./calc_in/' + ff)
                     raise SystemExit(1)
         else:
             if not os.path.isfile('./calc_in/' + f):
                 logger.error('Could not find ./calc_in/' + f)
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/VASP/collect_vasp.py` & `csp_cryspy-1.3.0/src/cryspy/interface/VASP/collect_vasp.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import xml.etree.ElementTree as ET
 
 import numpy as np
 from pymatgen.core import Structure
 
 from ...util import constants
 from ...IO import pkl_data
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
 def collect_vasp(cid, work_path, nat):
     # ---------- check optimization
     check_opt = check_opt_vasp(work_path+'OUTCAR')
@@ -104,15 +103,15 @@
             else:
                 logger.error('bug in get_energy_step_vasp')
                 raise SystemExit(1)
         # ------ list, str --> array
         energy_step = np.array(energy_step, dtype='float')/float(natot)
     except Exception as e:
         energy_step = None
-        logger.warning(str(e.args[0]) + f': #### ID: {cid}: failed to parse in energy_step')
+        logger.warning(f'{e}:    ID {cid}: failed to parse in energy_step')
 
     # ---------- append energy_step
     if energy_step_data.get(cid) is None:
         energy_step_data[cid] = []    # initialize
     energy_step_data[cid].append(energy_step)
 
     # ---------- save energy_step_data
@@ -161,15 +160,15 @@
                 incoord.append([float(x) for x in a.text.split()])
             # -- structure in pymatgen format
             struc = Structure(lattice, atomlist, incoord)
             # -- append
             struc_step.append(struc)
     except Exception as e:
         struc_step = None
-        logger.warning(str(e.args[0]), f': #### ID: {cid}: failed to parse in struc_step')
+        logger.warning(f'{e}:    ID {cid}: failed to parse in struc_step')
 
     # ---------- append struc_step
     if struc_step_data.get(cid) is None:
         struc_step_data[cid] = []    # initialize
     struc_step_data[cid].append(struc_step)
 
     # ---------- save struc_step_data
@@ -213,15 +212,15 @@
                         force.append(v.text.split())
             # -- list, str --> array
             force = np.array(force, dtype='float')
             # -- appned force_step
             force_step.append(force)
     except Exception as e:
         force_step = None
-        logger.warning(str(e.args[0]) + f': #### ID: {cid}: failed to parse in force_step')
+        logger.warning(f'{e}:    ID {cid}: failed to parse in force_step')
 
     # ---------- append force_step
     if force_step_data.get(cid) is None:
         force_step_data[cid] = []    # initialize
     force_step_data[cid].append(force_step)
 
     # ---------- save force_step_data
@@ -267,15 +266,15 @@
             stress = np.array(stress, dtype='float')
             # -- kbar --> eV/ang**3
             stress = stress * constants.KBAR2eV_ANG3
             # -- appned stress_step
             stress_step.append(stress)
     except Exception as e:
         stress_step = None
-        logger.warning(str(e.args[0]), f': #### ID: {cid}: failed to parse in stress_step')
+        logger.warning(f'{e}:    ID {cid}: failed to parse in stress_step')
 
     # ---------- append stress_step
     if stress_step_data.get(cid) is None:
         stress_step_data[cid] = []    # initialize
     stress_step_data[cid].append(stress_step)
 
     # ---------- save stress_step_data
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/soiap/collect_soiap.py` & `csp_cryspy-1.3.0/src/cryspy/interface/soiap/collect_soiap.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from logging import getLogger
 
 import numpy as np
 
 from . import structure as soiap_structure
 from ...util import constants
 from ...IO import pkl_data
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def collect_soiap(cid, work_path, nat):
+def collect_soiap(rin, cid, work_path, nat):
     # ---------- check optimization in current stage
     try:
         with open(work_path+rin.soiap_outfile, 'r') as fout:
             lines = fout.readlines()
         check_opt = 'not_yet'
         for i, line in enumerate(lines):
             if '*** QMD%loopc' in line:
@@ -34,24 +33,24 @@
     try:
         with open(work_path+'log.tote') as f:
             lines = f.readlines()
         energy = float(lines[-1].split()[4])    # in Hartree/atom
         energy = energy * constants.HRT2EV        # Hartree/atom to eV/atom
     except Exception as e:
         energy = np.nan    # error
-        logger.warning(str(e.args[0]) + f'    Structure ID {cid},'
+        logger.warning(f'{e}:    Structure ID {cid},'
                     f' could not obtain energy from {rin.soiap_outfile}')
 
     # ---------- collect the last structure
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     try:
         with open(work_path+'log.struc', 'r') as f:
             lines = f.readlines()
             lines = lines[-(natot+5):]
-        opt_struc = soiap_structure.from_file(lines, nat)
+        opt_struc = soiap_structure.from_file(rin, lines, nat)
     except Exception:
         opt_struc = None
 
     # ---------- check
     if np.isnan(energy):
         opt_struc = None
     if opt_struc is None:
@@ -81,29 +80,29 @@
             lines = f.readlines()
         for line in lines:
             if line.split()[1] == '1':
                 energy_step.append(line.split()[4])    # collumn 4: Hartree/atom
         energy_step = np.array(energy_step, dtype='float') * constants.HRT2EV
     except Exception as e:
         energy_step = None
-        logger.warning(str(e.args[0]) + f'#### ID: {cid}: failed to parse log.tote')
+        logger.warning(f'{e}:    ID {cid}: failed to parse log.tote')
 
     # ---------- append energy_step
     if energy_step_data.get(cid) is None:
         energy_step_data[cid] = []    # initialize
     energy_step_data[cid].append(energy_step)
 
     # ---------- save energy_step_data
     pkl_data.save_energy_step(energy_step_data)
 
     # ---------- return
     return energy_step_data
 
 
-def get_struc_step_soiap(struc_step_data, cid, work_path, nat):
+def get_struc_step_soiap(rin, struc_step_data, cid, work_path, nat):
     '''
     get structure step data
 
     # ---------- args
     struc_step_data: (dict) the key is structure ID
 
     struc_step_data[ID][stage][step]
@@ -119,20 +118,20 @@
         # ------ init.
         struc_step = []
         # ------ loop for relaxation step
         tmp_lines = []
         for line in lines:
             tmp_lines.append(line)
             if len(tmp_lines) == natot + 5:
-                struc = soiap_structure.from_file(tmp_lines, nat)
+                struc = soiap_structure.from_file(rin, tmp_lines, nat)
                 struc_step.append(struc)
                 tmp_lines = []    # clear
     except Exception as e:
         struc_step = None
-        logger.warning(str(e.args[0]), f'#### ID: {cid}: failed to parse log.struc')
+        logger.warning(f'{e}    ID {cid}: failed to parse log.struc')
 
     # ---------- append struc_step
     if struc_step_data.get(cid) is None:
         struc_step_data[cid] = []    # initialize
     struc_step_data[cid].append(struc_step)
 
     # ---------- save struc_step_data
@@ -170,15 +169,15 @@
                     tmp_lines = np.array(tmp_lines)
                     # Hartree/Bohr --> eV/ang
                     tmp_lines = tmp_lines * constants.HRT2EV / constants.BOHR2ANG
                     force_step.append(tmp_lines)
                     tmp_lines = []    # clear
     except Exception as e:
         force_step = None
-        logger.warning(str(e.args[0]) + f'#### ID: {cid}: failed to parse log.frc')
+        logger.warning(f'{e}    ID {cid}: failed to parse log.frc')
 
     # ---------- append force_step
     if force_step_data.get(cid) is None:
         force_step_data[cid] = []    # initialize
     force_step_data[cid].append(force_step)
 
     # ---------- save force_step_data
@@ -215,15 +214,15 @@
                     tmp_lines = np.array(tmp_lines)
                     # Hartree/Bohr**3 --> eV/ang**3
                     tmp_lines = tmp_lines * constants.HRT2EV / constants.BOHR2ANG**3
                     stress_step.append(tmp_lines)
                     tmp_lines = []    # clear
     except Exception as e:
         stress_step = None
-        logger.warning(str(e.args[0]), f'#### ID: {cid}: failed to parse log.strs')
+        logger.warning(f'{e}:    ID {cid}: failed to parse log.strs')
 
     # ---------- append stress_step
     if stress_step_data.get(cid) is None:
         stress_step_data[cid] = []    # initialize
     stress_step_data[cid].append(stress_step)
 
     # ---------- save stress_step_data
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/soiap/ctrl_job_soiap.py` & `csp_cryspy-1.3.0/src/cryspy/interface/soiap/ctrl_job_soiap.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,67 +3,66 @@
 '''
 
 from logging import getLogger
 import os
 import shutil
 
 from . import structure as soiap_structure
-from ...IO import read_input as rin
 
 
 logger = getLogger('cryspy')
 
-def next_stage_soiap(stage, work_path, nat):
+def next_stage_soiap(rin, stage, work_path, nat):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename soiap files at the current stage
     soiap_files = [rin.soiap_infile, rin.soiap_outfile, rin.soiap_cif,
                    'log.struc', 'log.tote', 'log.frc', 'log.strs']
-    for f in soiap_files:
-        if not os.path.isfile(work_path+f):
-            logger.error('Not found '+work_path+f)
+    for file in soiap_files:
+        if not os.path.isfile(work_path + file):
+            logger.error('Not found ' + work_path + file)
             raise SystemExit(1)
-        os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
+        os.rename(work_path + file, work_path + f'stage{stage}_' + file)
 
     # ---------- copy the input file from ./calc_in for the next stage
-    finfile = './calc_in/'+rin.soiap_infile+'_{}'.format(stage + 1)
+    finfile = './calc_in/' + rin.soiap_infile + f'_{stage + 1}'
     shutil.copyfile(finfile, work_path+rin.soiap_infile)
 
     # ---------- generate the CIF file
     natot = sum(nat)    # do not use rin.natot here for EA-vc
     try:
-        with open(work_path+'stage{}_log.struc'.format(stage), 'r') as f:
+        with open(work_path+f'stage{stage}_log.struc', 'r') as f:
             lines = f.readlines()
             lines = lines[-(natot+5):]
         structure = soiap_structure.from_file(lines, nat)
     except ValueError:
         skip_flag = True
         logger.warning('    error in soiap,  skip this structure')
         return skip_flag
-    with open(work_path+'stage{}_'.format(stage)+rin.soiap_cif, 'r') as f:
+    with open(work_path + f'stage{stage}_' + rin.soiap_cif, 'r') as f:
         lines = f.readlines()
     title = lines[0][5:]    # string following 'data_'
     soiap_structure.write(structure,
                           work_path+rin.soiap_cif,
                           symprec=rin.symprec,
                           title=title)
 
     # ---------- return
     return skip_flag
 
 
-def next_struc_soiap(structure, cid, work_path):
+def next_struc_soiap(rin, structure, cid, work_path):
     # ---------- copy files
     calc_inputs = [rin.soiap_infile]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.soiap_infile else f
         if not os.path.isfile('./calc_in/'+ff):
             logger.error('Could not find ./calc_in/'+ff)
             raise SystemExit(1)
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate the CIF file
     soiap_structure.write(structure,
                           work_path+rin.soiap_cif,
                           symprec=rin.symprec,
-                          title='ID_{0:d}'.format(cid))
+                          title=f'ID_{cid}')
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/interface/soiap/structure.py` & `csp_cryspy-1.3.0/src/cryspy/interface/soiap/structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 '''
 Structure files in soiap
 '''
-
 import itertools
 
 import numpy as np
 from pymatgen.core import Structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
 from ...util import constants
-from ...IO import read_input as rin
 
 
-def from_file(lines, nat):
+def from_file(rin, lines, nat):
     # ---------- lattice
     lattice = [[float(x) for x in line.split()] for line in lines[1:4]]
     #     in Bohr, each column is a lattice vector
     lattice = np.array(lattice) * constants.BOHR2ANG  # Bohr --> Ang
     lattice = lattice.T    # each row is a lattice vector
 
     # ---------- internal coordinates
@@ -28,15 +26,15 @@
     species = list(itertools.chain.from_iterable(species))
 
     structure = Structure(lattice, species, coords)
 
     return structure
 
 
-def write(structure, output, symprec=0.001, title="soiap"):
+def write(structure, output, symprec=0.01, title="soiap"):
     # ---------- symmetrized structure
     analyzer = SpacegroupAnalyzer(structure, symprec=symprec)
     structure_sym = analyzer.get_symmetrized_structure()
 
     # ---------- get written data
     lattice = structure_sym.lattice
     symmetry_operations = structure_sym.spacegroup
@@ -52,15 +50,15 @@
             f.write('{0:17s} {1:12.8f}\n'.format('_cell_length_'+s, value))
         for s, value in zip(['alpha', 'beta', 'gamma'], lattice.angles):
             f.write('{0:17s} {1:12.8f}\n'.format('_cell_angle_'+s, value))
         f.write('\n')
         f.write('loop_\n')
         f.write('  _symmetry_equiv_pos_as_xyz\n')
         for symop in symmetry_operations:
-            f.write("  '{0:s}'\n".format(symop.as_xyz_string()))
+            f.write("  '{0:s}'\n".format(symop.as_xyz_str()))
         f.write('\n')
         f.write('loop_\n')
         f.write('  _atom_site_type_symbol\n')
         for s in ['x', 'y', 'z']:
             f.write('  _atom_site_fract_'+s+'\n')
         for site in sites_inequiv:
             f.write('  {0:5s}  '.format(site.species_string)+' '.join(
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/job/ctrl_ext.py` & `csp_cryspy-1.3.0/src/cryspy/job/ctrl_ext.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,64 @@
+from logging import getLogger
 import os
 import shutil
 
-from logging import getLogger
 import numpy as np
 
 from ..interface import select_code
-from ..IO import read_input as rin
 from ..IO import io_stat, pkl_data
-from ..IO.out_results import out_rslt
+from ..IO.out_results import out_rslt, out_hdist
+from ..util.utility import backup_cryspy
 from ..util.struc_util import out_poscar, out_cif
 
-if rin.algo == 'BO':
-    from ..BO.select_descriptor import select_descriptor
-    from ..BO import bo_next_select
-if rin.algo in ['EA', 'EA-vc']:
-    from ..EA import ea_next_gen
-if rin.algo == 'EA-vc':
-    from ..EA.calc_ef import calc_ef
+# ---------- import later
+#from ..BO.select_descriptor import select_descriptor
+#from ..BO import bo_next_select
+#from ..EA import ea_next_gen
+#from ..EA.calc_ef import calc_ef
 
 
 logger = getLogger('cryspy')
 
+
 class Ctrl_ext:
 
-    def __init__(self, stat, init_struc_data):
-        self.stat = stat
+    def __init__(self, rin, init_struc_data):
+        self.rin = rin
         self.init_struc_data = init_struc_data
         self.opt_struc_data = pkl_data.load_opt_struc()
         self.rslt_data = pkl_data.load_rslt()
+        self.id_queueing = pkl_data.load_id_queueing()
+        self.id_running = pkl_data.load_id_running()
         self.recheck = False
         self.logic_next = False
         # ---------- for each algorithm
         if rin.algo == 'RS':
-            self.id_queueing, self.id_running = pkl_data.load_rs_id()
+            pass
         elif rin.algo == 'BO':
-            (self.n_selection, self.id_queueing,
-             self.id_running, self.id_select_hist) = pkl_data.load_bo_id()
-            (self.init_dscrpt_data, self.opt_dscrpt_data,
-             self.bo_mean, self.bo_var,
-             self.bo_score) = pkl_data.load_bo_data()
+            self.n_selection = pkl_data.load_n_selection()
+            self.id_select_hist = pkl_data.load_id_select_hist()
+            self.init_dscrpt_data = pkl_data.load_init_dscrpt_data()
+            self.opt_dscrpt_data = pkl_data.load_opt_dscrpt_data()
+            self.bo_mean = pkl_data.load_bo_mean()
+            self.bo_var = pkl_data.load_bo_var()
+            self.bo_score = pkl_data.load_bo_score()
         elif rin.rin.algo in ['EA', 'EA-vc']:
-            (self.gen, self.id_queueing,
-             self.id_running) = pkl_data.load_ea_id()
+            self.gen = pkl_data.load_gen()
             if rin.algo == 'EA-vc':
-                self.nat_data, self.ratio_data, self.hdist_data = pkl_data.load_ea_vc_data()
+                self.nat_data = pkl_data.load_nat_data()
+                self.ratio_data = pkl_data.load_ratio_data()
+                self.hdist_data = pkl_data.load_hdist_data()
             # do not have to load ea_data here.
             # ea_data is used only in ea_next_gen.py
 
     def check_job(self):
         # ---------- option: recalc
-        if rin.recalc:
-            self.set_recalc()
+        #if self.rin.recalc is not None:
+        #    self.set_recalc()
         # ---------- check job status
         try:
             with open('ext/stat_job') as fstat:
                 jstat = fstat.readline()    # submitted or done or ...
             if jstat[0:3] == 'sub':
                 self.job_stat = 'submitted'
             elif jstat[0:4] == 'done':
@@ -90,38 +94,39 @@
             logger.error('Unexpected error')
             raise SystemExit(1)
 
     def out_queue(self):
         # ---------- out cifs
         os.makedirs('ext/queue', exist_ok=False)    # if dir exists, error --> stop
         for cid in self.id_queueing:
-            self.init_struc_data[cid].to(fmt='cif', filename='ext/queue/{}.cif'.format(cid))
+            self.init_struc_data[cid].to(fmt='cif', filename=f'ext/queue/{cid}.cif')
         # ---------- queue --> running
         self.id_running = self.id_queueing[:]
         self.id_queueing = []
-        io_stat.set_id(self.stat, 'id_queueing', self.id_queueing)
-        io_stat.write_stat(self.stat)
+        stat = io_stat.stat_read()
+        io_stat.set_id(stat, 'id_queueing', self.id_queueing)
+        io_stat.write_stat(stat)
         self.save_id_data()
         # ---------- stat_job
         with open('ext/stat_job', 'w') as fstat:
             fstat.write('submitted\n')
         # ---------- mkdir calc_data
         os.makedirs('ext/calc_data', exist_ok=True)
 
     def ctrl_done(self):
         # ---------- collect result
         self.ctrl_collect()
 
     def ctrl_collect(self):
         # ---------- each algo
-        if rin.algo == 'RS':
+        if self.rin.algo == 'RS':
             self.ctrl_collect_rs()
-        elif rin.algo == 'BO':
+        elif self.rin.algo == 'BO':
             self.ctrl_collect_bo()
-        elif rin.rin.algo in ['EA', 'EA-vc']:
+        elif self.rin.algo in ['EA', 'EA-vc']:
             self.ctrl_collect_ea()
         else:
             logger.error('Error, algo')
             raise SystemExit(1)
         # ---------- calc_data --> old_calc_data
         if os.path.isdir('ext/old_calc_data'):
             shutil.rmtree('ext/old_calc_data')
@@ -135,29 +140,29 @@
             fstat.write('no queue\n')
         # ---------- update status
         self.id_running = []
         self.save_id_data()
 
     def ctrl_collect_rs(self):
         # ---------- get opt data
-        ext_opt_struc_data, ext_energy_data = select_code.collect('dummy', 'dummy', 'dummy')
+        ext_opt_struc_data, ext_energy_data = select_code.collect(self.rin, 'dummy', 'dummy', 'dummy')
         # ---------- register opt_struc
         ext_magmom, ext_check_opt, ext_spg_sym, ext_spg_num, \
             ext_spg_sym_opt, ext_spg_num_opt = self.regist_opt(ext_opt_struc_data)
         # ---------- save rslt
         for cid, opt_struc in ext_opt_struc_data.items():
             self.rslt_data.loc[cid] = [ext_spg_num[cid], ext_spg_sym[cid],
                                        ext_spg_num_opt[cid], ext_spg_sym_opt[cid],
                                        ext_energy_data[cid], ext_magmom[cid], ext_check_opt[cid]]
         pkl_data.save_rslt(self.rslt_data)
         out_rslt(self.rslt_data)
 
     def ctrl_collect_bo(self):
         # ---------- get opt data
-        ext_opt_struc_data, ext_energy_data = select_code.collect('dummy', 'dummy', 'dummy')
+        ext_opt_struc_data, ext_energy_data = select_code.collect(self.rin, 'dummy', 'dummy', 'dummy')
         # ---------- register opt_struc
         ext_magmom, ext_check_opt, ext_spg_sym, ext_spg_num, \
             ext_spg_sym_opt, ext_spg_num_opt = self.regist_opt(ext_opt_struc_data)
         # ---------- save rslt
         for cid, opt_struc in ext_opt_struc_data.items():
             self.rslt_data.loc[cid] = [self.n_selection,
                                        ext_spg_num[cid], ext_spg_sym[cid],
@@ -165,39 +170,42 @@
                                        ext_energy_data[cid], ext_magmom[cid], ext_check_opt[cid]]
         pkl_data.save_rslt(self.rslt_data)
         out_rslt(self.rslt_data)
         # ---------- descriptor
         for cid, opt_struc in ext_opt_struc_data.items():
             if opt_struc is not None:
                 # ------ calc descriptor for opt structure
-                tmp_dscrpt = select_descriptor({cid: opt_struc})
+                from ..BO.select_descriptor import select_descriptor
+                tmp_dscrpt = select_descriptor(self.rin, {cid: opt_struc})
                 # ------ update descriptors
                 self.opt_dscrpt_data.update(tmp_dscrpt)
                 # ---------- error
             else:
                 # ------ update descriptors and non_error_id
                 self.opt_dscrpt_data[cid] = None
         # ---------- save bo_data
         self.save_data()
 
     def ctrl_collect_ea(self):
         # ---------- get opt data
-        ext_opt_struc_data, ext_energy_data = select_code.collect('dummy', 'dummy', 'dummy')
+        ext_opt_struc_data, ext_energy_data = select_code.collect(self.rin, 'dummy', 'dummy', 'dummy')
         # ---------- register opt_struc
         ext_magmom, ext_check_opt, ext_spg_sym, ext_spg_num, \
             ext_spg_sym_opt, ext_spg_num_opt = self.regist_opt(ext_opt_struc_data)
         # ---------- save rslt
         for cid, opt_struc in ext_opt_struc_data.items():
-            if not rin.algo == 'EA-vc':
+            if not self.rin.algo == 'EA-vc':
                 self.rslt_data.loc[cid] = [self.gen,
                                            ext_spg_num[cid], ext_spg_sym[cid],
                                            ext_spg_num_opt[cid], ext_spg_sym_opt[cid],
                                            ext_energy_data[cid], ext_magmom[cid], ext_check_opt[cid]]
             else:    # for EA-vc
-                ef = calc_ef(ext_energy_data[cid], self.ratio_data[cid], rin.end_point)
+                from ..EA.calc_ef import calc_ef
+                ef = calc_ef(ext_energy_data[cid], self.ratio_data[cid],
+                             self.rin.end_point)
                 self.rslt_data.loc[cid] = [self.gen,
                                            ext_spg_num[cid], ext_spg_sym[cid],
                                            ext_spg_num_opt[cid], ext_spg_sym_opt[cid],
                                            ext_energy_data[cid], ef, ext_magmom[cid], ext_check_opt[cid]]
         pkl_data.save_rslt(self.rslt_data)
         out_rslt(self.rslt_data)
 
@@ -214,32 +222,32 @@
         ext_spg_num_opt = {}
         for cid, opt_struc in ext_opt_struc_data.items():
             ext_magmom[cid] = np.nan
             ext_check_opt[cid] = 'no_file'
             # ------ get initial spg info
             try:
                 ext_spg_sym[cid], ext_spg_num[cid] = self.init_struc_data[
-                    cid].get_space_group_info(symprec=rin.symprec)
+                    cid].get_space_group_info(symprec=self.rin.symprec)
             except TypeError:
                 ext_spg_num[cid] = 0
                 ext_spg_sym[cid] = None
             # ------ success opt
             if ext_opt_struc_data[cid] is not None:
                 # -- get opt spg info
                 try:
                     ext_spg_sym_opt[cid], ext_spg_num_opt[cid] = opt_struc.get_space_group_info(
-                        symprec=rin.symprec)
+                        symprec=self.rin.symprec)
                 except TypeError:
                     ext_spg_num_opt[cid] = 0
                     ext_spg_sym_opt[cid] = None
                 # -- out opt_struc
-                out_poscar(opt_struc, cid, './data/opt_POSCARS')
+                out_poscar({cid:opt_struc}, './data/opt_POSCARS')
                 try:
                     out_cif(opt_struc, cid, './data/',
-                            './data/opt_CIFS.cif', rin.symprec)
+                            './data/opt_CIFS.cif', self.rin.symprec)
                 except TypeError:
                     logger.info('failed to write opt_CIF')
             # ------ error
             else:
                 ext_spg_num_opt[cid] = 0
                 ext_spg_sym_opt[cid] = None
         # ---------- save opt_struc_data
@@ -248,80 +256,97 @@
         # ---------- return
         return ext_magmom, ext_check_opt, ext_spg_sym, ext_spg_num, ext_spg_sym_opt, ext_spg_num_opt
 
     def next_sg(self, noprint=False):
         '''
         next selection or generation
         '''
-        if rin.algo == 'BO':
+        if self.rin.algo == 'BO':
             self.next_select_BO(noprint)
-        if rin.rin.algo in ['EA', 'EA-vc']:
+        if self.rin.algo in ['EA', 'EA-vc']:
             self.next_gen_EA()
 
     def next_select_BO(self, noprint=False):
         # ---------- log
         logger.info(f'Done selection {self.n_selection}')
         # ---------- done all structures
-        if len(self.rslt_data) == rin.tot_struc:
+        if len(self.rslt_data) == self.rin.tot_struc:
             logger.info('\nDone all structures!')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
-        if rin.stop_chkpt == 3:
+        if self.rin.stop_chkpt == 3:
             logger.info('\nStop at check point 3: BO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- max_select_bo
-        if 0 < rin.max_select_bo <= self.n_selection:
-            logger.info(f'\nReached max_select_bo: {rin.max_select_bo}')
+        if 0 < self.rin.max_select_bo <= self.n_selection:
+            logger.info(f'\nReached max_select_bo: {self.rin.max_select_bo}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- BO
         bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
                    self.bo_mean, self.bo_var, self.bo_score)
         bo_id_data = (self.n_selection, self.id_queueing,
                       self.id_running, self.id_select_hist)
-        bo_next_select.next_select(self.stat, self.rslt_data,
+        from ..BO import bo_next_select
+        bo_next_select.next_select(self.rin, self.rslt_data,
                                    bo_id_data, bo_data, noprint)
 
     def next_gen_EA(self):
         # ---------- log
         logger.info(f'Done generation {self.gen}')
         # ---------- check point 3
-        if rin.stop_chkpt == 3:
+        if self.rin.stop_chkpt == 3:
             logger.info('\nStop at check point 3: EA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- maxgen_ea
-        if 0 < rin.maxgen_ea <= self.gen:
-            logger.info(f'\nReached maxgen_ea: {rin.maxgen_ea}')
+        if 0 < self.rin.maxgen_ea <= self.gen:
+            if self.rin.algo == 'EA-vc':
+                # ------ when gen reaches maxgen_ea,  next generation is not created
+                #        so convex hull is calculated here
+                #        update only convex hull and hdist, not elite_struc and elite_fitness
+                c_rslt = self.rslt_data[self.rslt_data['Gen'] == self.gen]
+                c_ids = c_rslt.index.values    # current IDs [array]
+                ef_all = self.rslt_data['Ef_eV_atom'].to_dict()    # formation energy of all structures
+                from ..EA.calc_hull import calc_convex_hull_2d
+                hdist = calc_convex_hull_2d(self.rin, self.ratio_data, ef_all, c_ids, self.gen)
+                out_hdist(self.gen, hdist, self.ratio_data)
+                self.hdist_data[self.gen] = hdist
+                pkl_data.save_hdist_data(self.hdist_data)
+            logger.info(f'\nReached maxgen_ea: {self.rin.maxgen_ea}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- EA
+        backup_cryspy()
         ea_id_data = (self.gen, self.id_queueing, self.id_running)
-        if rin.algo == 'EA-vc':
+        if self.rin.algo == 'EA-vc':
             ea_vc_data = (self.nat_data, self.ratio_data, self.hdist_data)
         else:
             ea_vc_data = None
-        ea_next_gen.next_gen(self.stat, self.init_struc_data, None,
+        from ..EA import ea_next_gen
+        ea_next_gen.next_gen(self.rin, self.init_struc_data, None,
                              self.opt_struc_data, self.rslt_data, ea_id_data, ea_vc_data)
 
     def save_id_data(self):
         # ---------- save id_data
-        if rin.algo == 'RS':
-            rs_id_data = (self.id_queueing, self.id_running)
-            pkl_data.save_rs_id(rs_id_data)
-        if rin.algo == 'BO':
-            bo_id_data = (self.n_selection, self.id_queueing,
-                          self.id_running, self.id_select_hist)
-            pkl_data.save_bo_id(bo_id_data)
-        if rin.rin.algo in ['EA', 'EA-vc']:
-            ea_id_data = (self.gen, self.id_queueing, self.id_running)
-            pkl_data.save_ea_id(ea_id_data)
+        pkl_data.save_id_queueing(self.id_queueing)
+        pkl_data.save_id_running(self.id_running)
+        if self.rin.algo == 'RS':
+            pass
+        if self.rin.algo == 'BO':
+            pkl_data.save_n_selection(self.n_selection)
+            pkl_data.save_id_select_hist(self.id_select_hist)
+        if self.rin.algo in ['EA', 'EA-vc']:
+            pkl_data.save_gen(self.gen)
+
 
     def save_data(self):
         # ---------- save ??_data
-        if rin.algo == 'BO':
-            bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
-                       self.bo_mean, self.bo_var, self.bo_score)
-            pkl_data.save_bo_data(bo_data)
+        if self.rin.algo == 'BO':
+            pkl_data.save_init_dscrpt_data(self.init_dscrpt_data)
+            pkl_data.save_opt_dscrpt_data(self.opt_dscrpt_data)
+            pkl_data.save_bo_mean(self.bo_mean)
+            pkl_data.save_bo_var(self.bo_var)
+            pkl_data.save_bo_score(self.bo_score)
         # ea_data is used only in ea_next_gen.py
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/job/ctrl_job.py` & `csp_cryspy-1.3.0/src/cryspy/job/ctrl_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,122 @@
-'''
-Control jobs
-'''
-
 import itertools
 from logging import getLogger
 import os
 import shutil
 import subprocess
 
 import numpy as np
 
 from ..interface import select_code
-from ..IO import read_input as rin
 from ..IO import change_input, io_stat, pkl_data
 from ..IO.out_results import out_rslt, out_hdist
 from ..util.utility import backup_cryspy
 from ..util.struc_util import out_poscar, out_cif
 
-if rin.algo == 'BO':
-    from ..BO.select_descriptor import select_descriptor
-    from ..BO import bo_next_select
-if rin.algo in ['EA', 'EA-vc']:
-    from ..EA import ea_next_gen
-if rin.algo == 'EA-vc':
-    from ..EA.calc_ef import calc_ef
-    from ..EA.calc_hull import calc_convex_hull_2d
-if rin.algo == 'LAQA':
-    from ..LAQA.calc_score import calc_laqa_bias
-    from ..LAQA import laqa_next_selection
-    from ..IO.out_results import out_laqa_status, out_laqa_step, out_laqa_score
-    from ..IO.out_results import out_laqa_energy, out_laqa_bias
+# ---------- import later
+#from ..BO.select_descriptor import select_descriptor
+#from ..BO import bo_next_select
+#from ..EA import ea_next_gen
+#from ..EA.calc_ef import calc_ef
+#from ..EA.calc_hull import calc_convex_hull_2d
+#from ..LAQA.calc_score import calc_laqa_bias
+#from ..LAQA import laqa_next_selection
+#from ..IO.out_results import out_laqa_status, out_laqa_step, out_laqa_score
+#from ..IO.out_results import out_laqa_energy, out_laqa_bias
 
 
 logger = getLogger('cryspy')
 
+
 class Ctrl_job:
 
-    def __init__(self, stat, init_struc_data):
-        self.stat = stat
+    def __init__(self, rin, init_struc_data):
+        self.rin = rin
         self.init_struc_data = init_struc_data
         self.opt_struc_data = pkl_data.load_opt_struc()
         self.rslt_data = pkl_data.load_rslt()
+        self.id_queueing = pkl_data.load_id_queueing()
+        self.id_running = pkl_data.load_id_running()
         self.recheck = False
         self.logic_next = False
         # ---------- for each algorithm
-        if rin.algo == 'RS':
-            self.id_queueing, self.id_running = pkl_data.load_rs_id()
-        elif rin.algo == 'BO':
-            (self.n_selection, self.id_queueing,
-             self.id_running, self.id_select_hist) = pkl_data.load_bo_id()
-            (self.init_dscrpt_data, self.opt_dscrpt_data,
-             self.bo_mean, self.bo_var, self.bo_score) = pkl_data.load_bo_data()
-            (self.init_dscrpt_data, self.opt_dscrpt_data,
-             self.bo_mean, self.bo_var,
-             self.bo_score) = pkl_data.load_bo_data()
-        elif rin.algo == 'LAQA':
-            (self.id_queueing, self.id_running,
-             self.id_select_hist) = pkl_data.load_laqa_id()
-            (self.tot_step_select, self.laqa_step,
-             self.laqa_struc, self.laqa_energy,
-             self.laqa_bias, self.laqa_score) = pkl_data.load_laqa_data()
-        elif rin.algo in ['EA', 'EA-vc']:
-            (self.gen, self.id_queueing,
-             self.id_running) = pkl_data.load_ea_id()
-            if rin.struc_mode in ['mol', 'mol_bs']:
+        if self.rin.algo == 'RS':
+            pass
+        elif self.rin.algo == 'BO':
+            self.n_selection = pkl_data.load_n_selection()
+            self.id_select_hist = pkl_data.load_id_select_hist()
+            self.init_dscrpt_data = pkl_data.load_init_dscrpt_data()
+            self.opt_dscrpt_data = pkl_data.load_opt_dscrpt_data()
+            self.bo_mean = pkl_data.load_bo_mean()
+            self.bo_var = pkl_data.load_bo_var()
+            self.bo_score = pkl_data.load_bo_score()
+        elif self.rin.algo == 'LAQA':
+            self.id_select_hist = pkl_data.load_id_select_hist()
+            self.tot_step_select = pkl_data.load_tot_step_select()
+            self.laqa_step = pkl_data.load_laqa_step()
+            self.laqa_struc = pkl_data.load_laqa_struc()
+            self.laqa_energy = pkl_data.load_laqa_energy()
+            self.laqa_bias = pkl_data.load_laqa_bias()
+            self.laqa_score = pkl_data.load_laqa_score()
+        elif self.rin.algo in ['EA', 'EA-vc']:
+            self.gen = pkl_data.load_gen()
+            if self.rin.struc_mode in ['mol', 'mol_bs']:
                 self.struc_mol_id = pkl_data.load_struc_mol_id()
-            if rin.algo == 'EA-vc':
-                self.nat_data, self.ratio_data, self.hdist_data = pkl_data.load_ea_vc_data()
+            if self.rin.algo == 'EA-vc':
+                self.nat_data = pkl_data.load_nat_data()
+                self.ratio_data = pkl_data.load_ratio_data()
+                self.hdist_data = pkl_data.load_hdist_data()
             # do not have to load ea_data here.
             # ea_data is used only in ea_next_gen.py
         # ---------- for option
-        if rin.kpt_flag:
+        if self.rin.kpt_flag:
             self.kpt_data = pkl_data.load_kpt()
-        if rin.energy_step_flag:
+        if self.rin.energy_step_flag:
             self.energy_step_data = pkl_data.load_energy_step()
-        if rin.struc_step_flag:
+        if self.rin.struc_step_flag:
             self.struc_step_data = pkl_data.load_struc_step()
-        if rin.force_step_flag:
+        if self.rin.force_step_flag:
             self.force_step_data = pkl_data.load_force_step()
-        if rin.stress_step_flag:
+        if self.rin.stress_step_flag:
             self.stress_step_data = pkl_data.load_stress_step()
         # ---------- flag for next selection or generation
-        if rin.algo in ['BO', 'LAQA', 'EA', 'EA-vc']:
+        if self.rin.algo in ['BO', 'LAQA', 'EA', 'EA-vc']:
             if (self.id_queueing or self.id_running):
                 self.go_next_sg = False
             else:
                 self.go_next_sg = True
 
     def check_job(self):
         # ---------- option: recalc
-        if rin.recalc:
+        if self.rin.recalc is not None:
             self.set_recalc()
         # ---------- temporarily append
         self.tmp_running = self.id_running[:]    # shallow copy
         self.tmp_queueing = self.id_queueing[:]
-        if not rin.stop_next_struc:    # if true --> option: stop_next_struc
-            while len(self.tmp_running) < rin.njob and self.tmp_queueing:
+        if not self.rin.stop_next_struc:    # if true --> option: stop_next_struc
+            while len(self.tmp_running) < self.rin.njob and self.tmp_queueing:
                 self.tmp_running.append(self.tmp_queueing.pop(0))
         # ---------- initialize
         self.stage_stat = {}    # key: Structure ID
         self.job_stat = {}
         # ---------- check job status
-        for cid in self.tmp_running[:rin.njob]:
+        for cid in self.tmp_running[:self.rin.njob]:
             # ------ mkdir
-            if not os.path.isdir(f'work/{cid:06}'):
-                os.mkdir(f'work/{cid:06}')
+            if not os.path.isdir(f'work/{cid}'):
+                os.mkdir(f'work/{cid}')
             # ------ check stat_job file
-            stat_path = f'work/{cid:06}' + '/stat_job'
+            stat_path = f'work/{cid}' + '/stat_job'
             try:
                 with open(stat_path, 'r') as fstat:
                     istat = fstat.readline()    # id
                     sstat = fstat.readline()    # stage
                     jstat = fstat.readline()    # submitted or done or ...
                 self.stage_stat[cid] = int(sstat.split()[0])
                 if not cid == int(istat.split()[0]):
-                    logger.error(f'ID is wrong in work/{cid:06}')
+                    logger.error(f'ID is wrong in work/{cid}')
                     raise SystemExit(1)
                 self.stage_stat[cid] = int(sstat.split()[0])
                 if jstat[0:3] == 'sub':
                     self.job_stat[cid] = 'submitted'
                 elif jstat[0:4] == 'done':
                     self.job_stat[cid] = 'done'
                 elif jstat[0:4] == 'skip':
@@ -127,39 +125,40 @@
                     self.job_stat[cid] = 'else'
             except IOError:
                 self.stage_stat[cid] = 'no_file'
                 self.job_stat[cid] = 'no_file'
 
     def set_recalc(self):
         # ---------- check id
-        for tid in rin.recalc:
+        for tid in self.rin.recalc:
             if tid not in self.opt_struc_data:
                 logger.error(f'ID {tid} has not yet been calculated')
                 raise SystemExit(1)
         # ---------- append IDs to the head of id_queueing
-        self.id_queueing = rin.recalc + self.id_queueing
-        io_stat.set_id(self.stat, 'id_queueing', self.id_queueing)
-        self.save_id_data()
+        self.id_queueing = list(self.rin.recalc) + self.id_queueing
+        # ---------- save and update id_queueing
+        pkl_data.save_id_queueing(self.id_queueing)
+        stat = io_stat.stat_read()
+        io_stat.set_id(stat, 'id_queueing', self.id_queueing)
+        io_stat.write_stat(stat)
         # ---------- log and out
         logger.info('# -- Recalc')
-        logger.info(f'Append {rin.recalc} to the head of id_queueing')
+        logger.info(f'Append {self.rin.recalc} to the head of id_queueing')
         # ---------- clear recalc
-        rin.recalc = []
-        config = change_input.config_read()
-        change_input.change_option(config, 'recalc', '')    # clear
+        self.rin.recalc = None
+        config = change_input.read_config()
+        change_input.change_input(config, 'option', 'recalc', '')    # clear
         change_input.write_config(config)
         logger.info('Clear recalc in cryspy.in')
-        io_stat.set_input_common(self.stat, 'option', 'recalc', '')
-        io_stat.write_stat(self.stat)
 
     def handle_job(self):
         logger.info('# ---------- job status')
-        for cid in self.tmp_running[:rin.njob]:
+        for cid in self.tmp_running[:self.rin.njob]:
             # ---------- set work_path and cid
-            self.work_path = f'./work/{cid:06}/'
+            self.work_path = f'./work/{cid}/'
             self.cid = cid
             # ---------- handle job
             if self.job_stat[cid] == 'submitted':
                 logger.info(f'ID {cid:>6}: still queueing or running')
             elif self.job_stat[cid] == 'done':
                 self.ctrl_done()
             elif self.job_stat[cid] == 'skip':
@@ -172,614 +171,698 @@
                 logger.error(f'Unexpected error in {self.work_path}stat_job')
 
     def ctrl_done(self):
         self.cstage = self.stage_stat[self.cid]
         # ---------- log
         logger.info(f'ID {self.cid:>6}: Stage {self.cstage} Done!')
         # ---------- next stage
-        if self.cstage < rin.nstage:
+        if self.cstage < self.rin.nstage:
             self.ctrl_next_stage()
         # ---------- collect result
-        elif self.cstage == rin.nstage:
+        elif self.cstage == self.rin.nstage:
             self.ctrl_collect()
         # ---------- error
         else:
             logger.error('Wrong stage in '+self.work_path+'stat_job')
             raise SystemExit(1)
 
     def ctrl_next_stage(self):
         # ---------- EA-vc
-        if rin.algo == 'EA-vc':
+        if self.rin.algo == 'EA-vc':
             nat = self.nat_data[self.cid]
         else:
-            nat = rin.nat
+            nat = self.rin.nat
         # ---------- energy step
-        if rin.energy_step_flag:
+        if self.rin.energy_step_flag:
             self.energy_step_data = select_code.get_energy_step(
-                self.energy_step_data, self.cid, self.work_path, nat)
+                self.rin, self.energy_step_data, self.cid, self.work_path, nat)
         # ---------- struc step
-        if rin.struc_step_flag:
+        if self.rin.struc_step_flag:
             self.struc_step_data = select_code.get_struc_step(
-                self.struc_step_data, self.cid, self.work_path, nat)
+                self.rin, self.struc_step_data, self.cid, self.work_path, nat)
         # ---------- force step
-        if rin.force_step_flag:
+        if self.rin.force_step_flag:
             self.force_step_data = select_code.get_force_step(
-                self.force_step_data, self.cid, self.work_path, nat)
+                self.rin, self.force_step_data, self.cid, self.work_path, nat)
         # ---------- stress step
-        if rin.stress_step_flag:
+        if self.rin.stress_step_flag:
             self.stress_step_data = select_code.get_stress_step(
-                self.stress_step_data, self.cid, self.work_path)
+                self.rin, self.stress_step_data, self.cid, self.work_path)
         # ---------- next stage
-        if rin.kpt_flag:
+        if self.rin.kpt_flag:
             skip_flag, self.kpt_data = select_code.next_stage(
-                self.cstage, self.work_path, nat,
+                self.rin, self.cstage, self.work_path, nat,
                 kpt_data=self.kpt_data, cid=self.cid)
         else:
-            skip_flag = select_code.next_stage(self.cstage,
+            skip_flag = select_code.next_stage(self.rin, self.cstage,
                                                self.work_path, nat)
         # ---------- skip
         if skip_flag:
             self.ctrl_skip()
             return
         # ---------- prepare jobfile
-        self.prepare_jobfile()
+        prepare_jobfile(self.rin, self.cid, self.work_path)
         # ---------- submit
         self.submit_next_stage()
 
     def submit_next_stage(self):
         # ---------- submit job
         os.chdir(self.work_path)    # cd work_path
         with open('stat_job', 'w') as fwstat:
             fwstat.write(f'{self.cid:<6}    # Structure ID\n')
             fwstat.write(f'{self.cstage + 1:<6}    # Stage\n')
             fwstat.write('submitted\n')
         with open('sublog', 'w') as logf:
-            subprocess.Popen([rin.jobcmd, rin.jobfile],
+            subprocess.Popen([self.rin.jobcmd, self.rin.jobfile],
                              stdout=logf, stderr=logf)
         os.chdir('../../')    # go back to ..
         # ---------- save status
-        io_stat.set_stage(self.stat, self.cid, self.cstage + 1)
-        io_stat.write_stat(self.stat)
+        stat = io_stat.stat_read()
+        io_stat.set_stage(stat, self.cid, self.cstage + 1)
+        io_stat.write_stat(stat)
         # ---------- log
         logger.info(f'    submitted job, ID {self.cid:>6} Stage {self.cstage + 1}')
 
     def ctrl_collect(self):
         # ---------- EA-vc
-        if rin.algo == 'EA-vc':
+        if self.rin.algo == 'EA-vc':
             nat = self.nat_data[self.cid]
         else:
-            nat = rin.nat
+            nat = self.rin.nat
         # ---------- energy step
-        if rin.energy_step_flag:
+        if self.rin.energy_step_flag:
             self.energy_step_data = select_code.get_energy_step(
-                self.energy_step_data, self.cid, self.work_path, nat)
+                self.rin, self.energy_step_data, self.cid, self.work_path, nat)
         # ---------- struc step
-        if rin.struc_step_flag:
+        if self.rin.struc_step_flag:
             self.struc_step_data = select_code.get_struc_step(
-                self.struc_step_data, self.cid, self.work_path, nat)
+                self.rin, self.struc_step_data, self.cid, self.work_path, nat)
         # ---------- force step
-        if rin.force_step_flag:
+        if self.rin.force_step_flag:
             self.force_step_data = select_code.get_force_step(
-                self.force_step_data, self.cid, self.work_path, nat)
+                self.rin, self.force_step_data, self.cid, self.work_path, nat)
         # ---------- stress step
-        if rin.stress_step_flag:
+        if self.rin.stress_step_flag:
             self.stress_step_data = select_code.get_stress_step(
-                self.stress_step_data, self.cid, self.work_path)
+                self.rin, self.stress_step_data, self.cid, self.work_path)
         # ---------- each algo
-        if rin.algo == 'RS':
+        if self.rin.algo == 'RS':
             self.ctrl_collect_rs(nat)
-        elif rin.algo == 'BO':
+        elif self.rin.algo == 'BO':
             self.ctrl_collect_bo(nat)
-        elif rin.algo == 'LAQA':
+        elif self.rin.algo == 'LAQA':
             self.ctrl_collect_laqa(nat)
-        elif rin.algo in ['EA', 'EA-vc']:
+        elif self.rin.algo in ['EA', 'EA-vc']:
             self.ctrl_collect_ea(nat)
         else:
             logger.error('Error, algo')
             raise SystemExit(1)
         # ---------- move to fin
-        if rin.algo == 'LAQA':
+        if self.rin.algo == 'LAQA':
             if self.fin_laqa:
-                self.mv_fin()
+                mv_fin(self.cid)
             else:
                 os.rename(self.work_path+'stat_job',
                           self.work_path+'prev_stat_job')
         else:
-            self.mv_fin()
+            mv_fin(self.cid)
         # ---------- update status
-        self.update_status(operation='fin')
+        self.id_queueing, self.id_running = update_status(
+                                                self.cid,
+                                                self.id_queueing,
+                                                self.id_running,
+                                                operation='fin',
+                                            )
         # ---------- recheck
         self.recheck = True
 
     def ctrl_collect_rs(self, nat):
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
-            select_code.collect(self.cid, self.work_path, nat)
+            select_code.collect(self.rin, self.cid, self.work_path, nat)
         logger.info(f'    collect results: E = {energy} eV/atom')
-        # ---------- register opt_struc
-        spg_sym, spg_num, spg_sym_opt, spg_num_opt = self.regist_opt(opt_struc)
-        # ---------- save rslt
-        self.rslt_data.loc[self.cid] = [spg_num, spg_sym,
-                                               spg_num_opt, spg_sym_opt,
-                                               energy, magmom, check_opt]
-        pkl_data.save_rslt(self.rslt_data)
-        out_rslt(self.rslt_data)
+        # ---------- register opt data
+        self.opt_struc_data, self.rslt_data = regist_opt(
+            self.rin, self.cid, self.work_path,
+            self.init_struc_data, self.opt_struc_data, self.rslt_data,
+            opt_struc, energy, magmom, check_opt, ef=None, n_selection=None, gen=None)
 
     def ctrl_collect_bo(self, nat):
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
-            select_code.collect(self.cid, self.work_path, nat)
+            select_code.collect(self.rin, self.cid, self.work_path, nat)
         logger.info(f'    collect results: E = {energy} eV/atom')
-        # ---------- register opt_struc
-        spg_sym, spg_num, spg_sym_opt, spg_num_opt = self.regist_opt(opt_struc)
-        # ---------- save rslt
-        self.rslt_data.loc[self.cid] = [self.n_selection,
-                                               spg_num, spg_sym,
-                                               spg_num_opt, spg_sym_opt,
-                                               energy, magmom, check_opt]
-        pkl_data.save_rslt(self.rslt_data)
-        out_rslt(self.rslt_data)
+        # ---------- register opt data
+        self.opt_struc_data, self.rslt_data = regist_opt(
+            self.rin, self.cid, self.work_path,
+            self.init_struc_data, self.opt_struc_data, self.rslt_data,
+            opt_struc, energy, magmom, check_opt,
+            ef=None, n_selection=self.n_selection, gen=None)
         # ---------- success
         if opt_struc is not None:
+            from ..BO.select_descriptor import select_descriptor
             # ------ calc descriptor for opt sturcture
-            tmp_dscrpt = select_descriptor({self.cid: opt_struc})
+            tmp_dscrpt = select_descriptor(self.rin, {self.cid: opt_struc})
             # ------ update descriptors
             self.opt_dscrpt_data.update(tmp_dscrpt)
         # ---------- error
         else:
             # ------ update descriptors and non_error_id
             self.opt_dscrpt_data[self.cid] = None
         # ---------- save bo_data
-        self.save_data()
+        pkl_data.save_opt_dscrpt_data(self.opt_dscrpt_data)
 
     def ctrl_collect_laqa(self, nat):
         # ---------- flag for finish
         self.fin_laqa = False
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
-            select_code.collect(self.cid, self.work_path, nat)
+            select_code.collect(self.rin, self.cid, self.work_path, nat)
         # ---------- total step and laqa_step
         #     force_step_data[ID][stage][step][atom]
         if self.force_step_data[self.cid][-1] is None:
             self.laqa_step[self.cid].append(0)
         else:
             self.tot_step_select[-1] += len(
                 self.force_step_data[self.cid][-1])
             self.laqa_step[self.cid].append(
                 len(self.force_step_data[self.cid][-1]))
         # ------ save status
-        io_stat.set_common(self.stat, 'total_step', sum(self.tot_step_select))
-        io_stat.write_stat(self.stat)
+        stat = io_stat.stat_read()
+        io_stat.set_common(stat, 'total_step', sum(self.tot_step_select))
+        io_stat.write_stat(stat)
         # ---------- append laqa struc
         self.laqa_struc[self.cid].append(opt_struc)
         # ---------- append laqa energy
         self.laqa_energy[self.cid].append(energy)
         # ---------- append laqa bias
         #     force_step_data[ID][stage][step][atom]
         #     stress_step_data[ID][stage][step][atom]
+        from ..LAQA.calc_score import calc_laqa_bias
         tmp_laqa_bias = calc_laqa_bias(
             self.force_step_data[self.cid][-1],
             self.stress_step_data[self.cid][-1],
-            wf=rin.wf, ws=rin.ws)
+            wf=self.rin.wf, ws=self.rin.ws)
         self.laqa_bias[self.cid].append(tmp_laqa_bias)
         # ---------- append laqa score
         if check_opt == 'done' or np.isnan(energy) or np.isnan(tmp_laqa_bias):
             self.laqa_score[self.cid].append(-float('inf'))
         else:
             self.laqa_score[self.cid].append(-energy + tmp_laqa_bias)
         # ---------- save and out laqa data
-        self.save_data()
+        pkl_data.save_tot_step_select(self.tot_step_select)
+        pkl_data.save_laqa_step(self.laqa_step)
+        pkl_data.save_laqa_struc(self.laqa_struc)
+        pkl_data.save_laqa_energy(self.laqa_energy)
+        pkl_data.save_laqa_bias(self.laqa_bias)
+        pkl_data.save_laqa_score(self.laqa_score)
+        from ..IO.out_results import out_laqa_status, out_laqa_step, out_laqa_score
+        from ..IO.out_results import out_laqa_energy, out_laqa_bias
         out_laqa_status(self.laqa_step, self.laqa_score,
                         self.laqa_energy, self.laqa_bias)
         out_laqa_step(self.laqa_step)
         out_laqa_score(self.laqa_score)
         out_laqa_energy(self.laqa_energy)
         out_laqa_bias(self.laqa_bias)
         # ---------- case of 'done' or error
         if check_opt == 'done' or np.isnan(energy) or np.isnan(tmp_laqa_bias):
             self.fin_laqa = True
             logger.info(f'    collect results: E = {energy} eV/atom')
-            # ------ register opt_struc
-            (spg_sym, spg_num,
-             spg_sym_opt, spg_num_opt) = self.regist_opt(opt_struc)
-            # ------ save rslt
-            self.rslt_data.loc[self.cid] = [spg_num, spg_sym,
-                                                   spg_num_opt, spg_sym_opt,
-                                                   energy, magmom, check_opt]
-            pkl_data.save_rslt(self.rslt_data)
-            out_rslt(self.rslt_data)
+            # ------ register opt data
+            self.opt_struc_data, self.rslt_data = regist_opt(
+                self.rin, self.cid, self.work_path,
+                self.init_struc_data, self.opt_struc_data, self.rslt_data,
+                opt_struc, energy, magmom, check_opt, ef=None, n_selection=None, gen=None)
 
     def ctrl_collect_ea(self, nat):
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
-            select_code.collect(self.cid, self.work_path, nat)
+            select_code.collect(self.rin, self.cid, self.work_path, nat)
         logger.info(f'    collect results: E = {energy} eV/atom')
         # ---------- calculate Ef
-        if rin.algo == 'EA-vc':
-            ef = calc_ef(energy, self.ratio_data[self.cid], rin.end_point)
+        if self.rin.algo == 'EA-vc':
+            from ..EA.calc_ef import calc_ef
+            ef = calc_ef(energy, self.ratio_data[self.cid], self.rin.end_point)
             logger.info(f'                     Ef = {ef} eV/atom')
-        # ---------- register opt_struc
-        spg_sym, spg_num, spg_sym_opt, spg_num_opt = self.regist_opt(opt_struc)
-        # ---------- save rslt
-        if not rin.algo == 'EA-vc':
-            self.rslt_data.loc[self.cid] = [self.gen,
-                                            spg_num, spg_sym,
-                                            spg_num_opt, spg_sym_opt,
-                                            energy, magmom, check_opt]
         else:
-            self.rslt_data.loc[self.cid] = [self.gen,
-                                            spg_num, spg_sym,
-                                            spg_num_opt, spg_sym_opt,
-                                            energy, ef, magmom, check_opt]
-        pkl_data.save_rslt(self.rslt_data)
-        if rin.algo == 'EA':
-            out_rslt(self.rslt_data)
-        if rin.algo == 'EA-vc':
-            out_rslt(self.rslt_data, order_ef=True)
-
-    def regist_opt(self, opt_struc):
-        '''
-        Common part in ctrl_collect_*
-        '''
-        # ---------- get initial spg info
-        try:
-            spg_sym, spg_num = self.init_struc_data[
-                self.cid].get_space_group_info(symprec=rin.symprec)
-        except TypeError:
-            spg_num = 0
-            spg_sym = None
-        # ---------- success
-        if opt_struc is not None:
-            # ------ get opt spg info
-            try:
-                spg_sym_opt, spg_num_opt = opt_struc.get_space_group_info(
-                    symprec=rin.symprec)
-            except TypeError:
-                spg_num_opt = 0
-                spg_sym_opt = None
-            # ------ out opt_struc
-            out_poscar(opt_struc, self.cid, './data/opt_POSCARS')
-            try:
-                out_cif(opt_struc, self.cid, self.work_path,
-                        './data/opt_CIFS.cif', rin.symprec)
-            except TypeError:
-                logger.warning('failed to write opt_CIF')
-        # ---------- error
-        else:
-            spg_num_opt = 0
-            spg_sym_opt = None
-        # ---------- register opt_struc
-        self.opt_struc_data[self.cid] = opt_struc
-        pkl_data.save_opt_struc(self.opt_struc_data)
-        # ---------- return
-        return spg_sym, spg_num, spg_sym_opt, spg_num_opt
+            ef = None
+        # ---------- register opt data
+        self.opt_struc_data, self.rslt_data = regist_opt(
+            self.rin, self.cid, self.work_path,
+            self.init_struc_data, self.opt_struc_data, self.rslt_data,
+            opt_struc, energy, magmom, check_opt, ef=ef, n_selection=None, gen=self.gen)
 
     def ctrl_next_struc(self):
-        # ---------- RS
-        if rin.algo == 'RS':
-            next_struc_data = self.init_struc_data[self.cid]
-        # ---------- BO
-        elif rin.algo == 'BO':
+        # ---------- RS, BO, EA, EA-vc
+        if self.rin.algo in ['RS', 'BO', 'EA', 'EA-vc']:
             next_struc_data = self.init_struc_data[self.cid]
         # ---------- LAQA
-        elif rin.algo == 'LAQA':
+        elif self.rin.algo == 'LAQA':
             if self.laqa_struc[self.cid]:    # vacant list?
                 next_struc_data = self.laqa_struc[self.cid][-1]
             else:
                 next_struc_data = self.init_struc_data[self.cid]
-        # ---------- EA
-        elif rin.algo in ['EA', 'EA-vc']:
-            next_struc_data = self.init_struc_data[self.cid]
         # ---------- algo is wrong
         else:
             logger.error('Error, algo in ctrl_next_struc')
             raise SystemExit(1)
         # ---------- nat for EA-vc
-        if rin.algo == 'EA-vc':
+        if self.rin.algo == 'EA-vc':
             nat = self.nat_data[self.cid]
         else:
-            nat = rin.nat
+            nat = self.rin.nat
         # ---------- common part
         # ------ in case there is no initial strucure data
         if next_struc_data is None:
             logger.info(f'ID {self.cid:>6}: initial structure is None')
             self.ctrl_skip()
         # ------ normal initial structure data
         else:
             # -- prepare input files for structure optimization
-            if rin.kpt_flag:
-                self.kpt_data = select_code.next_struc(next_struc_data,
-                                                       self.cid,
-                                                       self.work_path,
-                                                       nat,
-                                                       self.kpt_data)
+            if self.rin.kpt_flag:
+                self.kpt_data = select_code.next_struc(
+                                    self.rin,
+                                    next_struc_data,
+                                    self.cid,
+                                    self.work_path,
+                                    nat,
+                                    self.kpt_data,
+                                )
             else:
-                select_code.next_struc(next_struc_data, self.cid,
-                                       self.work_path, nat)
+                select_code.next_struc(
+                    self.rin,
+                    next_struc_data,
+                    self.cid,
+                    self.work_path,
+                    nat,
+                )
             # -- prepare jobfile
-            self.prepare_jobfile()
+            prepare_jobfile(self.rin, self.cid, self.work_path)
             # -- submit
-            self.submit_next_struc()
+            submit_next_struc(self.rin, self.cid, self.work_path)
             logger.info(f'ID {self.cid:>6}: submit job, Stage 1')
             # -- update status
-            self.update_status(operation='submit')
-
-    def submit_next_struc(self):
-        # ---------- submit job
-        os.chdir(self.work_path)    # cd work_path
-        with open('stat_job', 'w') as fwstat:
-            fwstat.write(f'{self.cid:<6}    # Structure ID\n')
-            fwstat.write(f'{1:<6}    # Stage\n')
-            fwstat.write('submitted\n')
-        with open('sublog', 'w') as logf:
-            subprocess.Popen([rin.jobcmd, rin.jobfile],
-                             stdout=logf, stderr=logf)
-        os.chdir('../../')    # go back to csp root dir
+            self.id_queueing, self.id_running = update_status(
+                                                    self.cid,
+                                                    self.id_queueing,
+                                                    self.id_running,
+                                                    operation='submit'
+                                                )
 
     def ctrl_skip(self):
         # ---------- log
         logger.info(f'ID {self.cid:>6}: Skip')
         # ---------- get initial spg info
         if self.init_struc_data[self.cid] is None:
             spg_sym = None
             spg_num = 0
         else:
             try:
                 spg_sym, spg_num = self.init_struc_data[
-                    self.cid].get_space_group_info(symprec=rin.symprec)
+                    self.cid].get_space_group_info(symprec=self.rin.symprec)
             except TypeError:
                 spg_num = 0
                 spg_sym = None
         # ---------- 'skip' for rslt
         spg_num_opt = 0
         spg_sym_opt = None
         energy = np.nan
         magmom = np.nan
         check_opt = 'skip'
         # ---------- register opt_struc
         self.opt_struc_data[self.cid] = None
         pkl_data.save_opt_struc(self.opt_struc_data)
         # ---------- RS
-        if rin.algo == 'RS':
+        if self.rin.algo == 'RS':
             # ------ save rslt
             self.rslt_data.loc[self.cid] = [spg_num, spg_sym,
                                             spg_num_opt, spg_sym_opt,
                                             energy, magmom, check_opt]
             pkl_data.save_rslt(self.rslt_data)
             out_rslt(self.rslt_data)
         # ---------- BO
-        elif rin.algo == 'BO':
+        elif self.rin.algo == 'BO':
             # ------ save rslt
             self.rslt_data.loc[self.cid] = [self.n_selection,
                                             spg_num, spg_sym,
                                             spg_num_opt, spg_sym_opt,
                                             energy, magmom, check_opt]
             pkl_data.save_rslt(self.rslt_data)
             out_rslt(self.rslt_data)
-            # ------ update descriptors
+            # ------ update and save descriptors
             self.opt_dscrpt_data[self.cid] = None
-            # ------ save
-            self.save_id_data()
-            self.save_data()
+            pkl_data.save_opt_dscrpt_data(self.opt_dscrpt_data)
         # ---------- LAQA
-        elif rin.algo == 'LAQA':
+        elif self.rin.algo == 'LAQA':
             # ------ save rslt
             self.rslt_data.loc[self.cid] = [spg_num, spg_sym,
                                             spg_num_opt, spg_sym_opt,
                                             energy, magmom, check_opt]
             pkl_data.save_rslt(self.rslt_data)
             out_rslt(self.rslt_data)
             # ---------- laqa data
             self.laqa_step[self.cid].append(0)
             self.laqa_struc[self.cid].append(None)
             self.laqa_energy[self.cid].append(energy)
             self.laqa_bias[self.cid].append(np.nan)
             self.laqa_score[self.cid].append(-float('inf'))
             # ---------- save and out laqa data
-            self.save_data()
+            #pkl_data.save_tot_step_select(self.tot_step_select)    # not used here
+            pkl_data.save_laqa_step(self.laqa_step)
+            pkl_data.save_laqa_struc(self.laqa_struc)
+            pkl_data.save_laqa_energy(self.laqa_energy)
+            pkl_data.save_laqa_bias(self.laqa_bias)
+            pkl_data.save_laqa_score(self.laqa_score)
+            from ..IO.out_results import out_laqa_status, out_laqa_step, out_laqa_score
+            from ..IO.out_results import out_laqa_energy, out_laqa_bias
             out_laqa_status(self.laqa_step, self.laqa_score,
                             self.laqa_energy, self.laqa_bias)
             out_laqa_step(self.laqa_step)
             out_laqa_score(self.laqa_score)
             out_laqa_energy(self.laqa_energy)
             out_laqa_bias(self.laqa_bias)
         # ---------- EA
-        elif rin.algo == 'EA':
+        elif self.rin.algo == 'EA':
             self.rslt_data.loc[self.cid] = [self.gen,
                                             spg_num, spg_sym,
                                             spg_num_opt, spg_sym_opt,
                                             energy, magmom, check_opt]
             pkl_data.save_rslt(self.rslt_data)
             out_rslt(self.rslt_data)
-        elif rin.algo == 'EA-vc':
+        elif self.rin.algo == 'EA-vc':
             ef = np.nan
             self.rslt_data.loc[self.cid] = [self.gen,
                                             spg_num, spg_sym,
                                             spg_num_opt, spg_sym_opt,
                                             energy, ef, magmom, check_opt]
             pkl_data.save_rslt(self.rslt_data)
             out_rslt(self.rslt_data)
         # ---------- move to fin
-        self.mv_fin()
+        mv_fin(self.cid)
         # ---------- update status
-        self.update_status(operation='fin')
+        self.id_queueing, self.id_running = update_status(
+                                                self.cid,
+                                                self.id_queueing,
+                                                self.id_running,
+                                                operation='fin',
+                                            )
         # ---------- recheck
         self.recheck = True
 
-    def update_status(self, operation):
-        # ---------- update status
-        if operation == 'submit':
-            self.id_running.append(self.cid)
-            self.id_queueing.remove(self.cid)
-            io_stat.set_stage(self.stat, self.cid, 1)
-        elif operation == 'fin':
-            if self.cid in self.id_queueing:
-                self.id_queueing.remove(self.cid)
-            if self.cid in self.id_running:
-                self.id_running.remove(self.cid)
-            io_stat.clean_id(self.stat, self.cid)
-        else:
-            logger.error('operation is wrong')
-            raise SystemExit(1)
-        io_stat.set_id(self.stat, 'id_queueing', self.id_queueing)
-        io_stat.write_stat(self.stat)
-        # ---------- save id_data
-        self.save_id_data()
-
-    def prepare_jobfile(self):
-        if not os.path.isfile('./calc_in/' + rin.jobfile):
-            logger.error('Could not find ./calc_in' + rin.jobfile)
-            raise SystemExit(1)
-        with open('./calc_in/' + rin.jobfile, 'r') as f:
-            lines = f.readlines()
-        lines2 = []
-        for line in lines:
-            lines2.append(line.replace('CrySPY_ID', str(self.cid)))
-        with open(self.work_path + rin.jobfile, 'w') as f:
-            f.writelines(lines2)
-
-    def mv_fin(self):
-        if not os.path.isdir(f'work/fin/{self.cid:06}'):
-            shutil.move(f'work/{self.cid:06}', 'work/fin/')
-        else:    # rename for recalc
-            for i in itertools.count(1):
-                if not os.path.isdir(f'work/fin/{self.cid:06}_{i}'):
-                    shutil.move(f'work/{self.cid:06}',
-                                f'work/fin/{self.cid:06}_{i}')
-                    break
-
     def next_sg(self, noprint=False):
         '''
         next selection or generation
         '''
-        if rin.algo == 'BO':
+        if self.rin.algo == 'BO':
             self.next_select_BO(noprint)
-        if rin.algo == 'LAQA':
+        if self.rin.algo == 'LAQA':
             self.next_select_LAQA()
-        if rin.algo in ['EA', 'EA-vc']:
-            self.next_gen_EA()
+        if self.rin.algo in ['EA', 'EA-vc']:
+            if self.rin.algo == 'EA-vc':
+                ea_vc_data = (self.nat_data, self.ratio_data, self.hdist_data)
+            else:
+                ea_vc_data = None
+            next_gen_EA(
+                self.rin,
+                self.id_queueing,
+                self.id_running,
+                self.gen,
+                self.go_next_sg,
+                self.init_struc_data,
+                self.opt_struc_data,
+                self.rslt_data,
+                ea_vc_data=ea_vc_data,
+                struc_mol_id=None,
+            )
 
     def next_select_BO(self, noprint=False):
         # ---------- log
         logger.info(f'\nDone selection {self.n_selection}')
         # ---------- done all structures
-        if len(self.rslt_data) == rin.tot_struc:
+        if len(self.rslt_data) == self.rin.tot_struc:
             logger.info('\nDone all structures!')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
             logger.info('\nBO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
-        if rin.stop_chkpt == 3:
+        if self.rin.stop_chkpt == 3:
             logger.info('\nStop at check point 3: BO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- max_select_bo
-        if 0 < rin.max_select_bo <= self.n_selection:
-            logger.info(f'\nReached max_select_bo: {rin.max_select_bo}')
+        if 0 < self.rin.max_select_bo <= self.n_selection:
+            logger.info(f'\nReached max_select_bo: {self.rin.max_select_bo}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- BO
         backup_cryspy()
         bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
                    self.bo_mean, self.bo_var, self.bo_score)
         bo_id_data = (self.n_selection, self.id_queueing,
                       self.id_running, self.id_select_hist)
-        bo_next_select.next_select(self.stat, self.rslt_data,
+        from ..BO import bo_next_select
+        bo_next_select.next_select(self.rin, self.rslt_data,
                                    bo_id_data, bo_data, noprint)
 
     def next_select_LAQA(self):
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
             logger.info('\nLAQA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
-        if rin.stop_chkpt == 3:
+        if self.rin.stop_chkpt == 3:
             logger.info('\nStop at check point 3: LAQA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- selection of LAQA
         backup_cryspy()
         laqa_id_data = (self.id_queueing, self.id_running,
                         self.id_select_hist)
         laqa_data = (self.tot_step_select, self.laqa_step, self.laqa_struc,
                      self.laqa_energy, self.laqa_bias, self.laqa_score)
-        laqa_next_selection.next_selection(self.stat, laqa_id_data, laqa_data)
+        from ..LAQA import laqa_next_selection
+        laqa_next_selection.next_selection(self.rin, laqa_id_data, laqa_data)
 
-    def next_gen_EA(self):
-        # ---------- log
-        logger.info(f'Done generation {self.gen}')
-        # ---------- flag for next selection or generation
-        if not self.go_next_sg:
-            logger.info('\nEA is ready')
-            os.remove('lock_cryspy')
-            raise SystemExit()
-        # ---------- check point 3
-        if rin.stop_chkpt == 3:
-            logger.info('\nStop at check point 3: EA is ready')
-            os.remove('lock_cryspy')
-            raise SystemExit()
-        # ---------- maxgen_ea
-        if 0 < rin.maxgen_ea <= self.gen:
-            if rin.algo == 'EA-vc':
-                # ------ when gen reaches maxgen_ea,  next generation is not created
-                #        so convex hull is calculated here
-                #        update only convex hull and hdist, not elite_struc and elite_fitness
-                c_rslt = self.rslt_data[self.rslt_data['Gen'] == self.gen]
-                c_ids = c_rslt.index.values    # current IDs [array]
-                ef_all = self.rslt_data['Ef_eV_atom'].to_dict()    # formation energy of all structures
-                hdist = calc_convex_hull_2d(self.ratio_data, ef_all, c_ids, self.gen)
-                out_hdist(self.gen, hdist, self.ratio_data)
-                self.hdist_data[self.gen] = hdist
-                ea_vc_data = (self.nat_data, self.ratio_data, self.hdist_data)
-                pkl_data.save_ea_vc_data(ea_vc_data)
-            logger.info(f'\nReached maxgen_ea: {rin.maxgen_ea}')
-            os.remove('lock_cryspy')
-            raise SystemExit()
-        # ---------- EA
-        backup_cryspy()
-        ea_id_data = (self.gen, self.id_queueing, self.id_running)
-        if rin.struc_mode in ['mol', 'mol_bs']:
-            struc_mol_id = self.struc_mol_id
-        else:
-            struc_mol_id = None
+
+#
+#  End Ctrl_job class
+#
+
+
+def prepare_jobfile(rin, cid, work_path):
+    if not os.path.isfile('./calc_in/' + rin.jobfile):
+        logger.error('Could not find ./calc_in' + rin.jobfile)
+        raise SystemExit(1)
+    with open('./calc_in/' + rin.jobfile, 'r') as f:
+        lines = f.readlines()
+    lines2 = []
+    for line in lines:
+        lines2.append(line.replace('CrySPY_ID', str(cid)))
+    with open(work_path + rin.jobfile, 'w') as f:
+        f.writelines(lines2)
+
+
+def submit_next_struc(rin, cid, work_path, wait=False):
+    # ---------- submit job
+    os.chdir(work_path)    # cd work_path
+    # ---------- submit
+    with open('sublog', 'w') as logf:
+        if not wait:
+            subprocess.Popen([rin.jobcmd, rin.jobfile],
+                             stdout=logf, stderr=logf)
+        else:    # wait
+            subprocess.run([rin.jobcmd, rin.jobfile],
+                           stdout=logf, stderr=logf)
+    # ---------- write stat_job
+    with open('stat_job', 'w') as f:
+        f.write(f'{cid:<6}    # Structure ID\n')
+        f.write(f'{1:<6}    # Stage\n')
+        f.write('submitted\n')
+    os.chdir('../../')    # go back to csp root dir
+
+
+def regist_opt(
+        rin,
+        cid,
+        work_path,
+        init_struc_data,
+        opt_struc_data,
+        rslt_data,
+        opt_struc,
+        energy,
+        magmom,
+        check_opt,
+        ef=None,
+        n_selection=None,
+        gen=None
+    ):
+    '''
+    Common part in ctrl_collect_*
+    '''
+    # ---------- get initial spg info
+    try:
+        spg_sym, spg_num = init_struc_data[
+            cid].get_space_group_info(symprec=rin.symprec)
+    except TypeError:
+        spg_num = 0
+        spg_sym = None
+
+    # ---------- success
+    if opt_struc is not None:
+        # ------ get opt spg info
+        try:
+            spg_sym_opt, spg_num_opt = opt_struc.get_space_group_info(
+                symprec=rin.symprec)
+        except TypeError:
+            spg_num_opt = 0
+            spg_sym_opt = None
+        # ------ out opt_struc
+        out_poscar({cid:opt_struc}, './data/opt_POSCARS')
+        try:
+            out_cif(opt_struc, cid, work_path,
+                    './data/opt_CIFS.cif', rin.symprec)
+        except TypeError:
+            logger.warning('failed to write opt_CIF')
+    # ---------- error
+    else:
+        spg_num_opt = 0
+        spg_sym_opt = None
+
+    # ---------- register opt_struc
+    opt_struc_data[cid] = opt_struc
+    pkl_data.save_opt_struc(opt_struc_data)
+    # ---------- return
+    #return spg_sym, spg_num, spg_sym_opt, spg_num_opt
+
+    # ---------- register rslt
+    if rin.algo in ['RS', 'LAQA']:
+        rslt_data.loc[cid] = [spg_num, spg_sym, spg_num_opt, spg_sym_opt,
+                              energy, magmom, check_opt]
+    elif rin.algo == 'BO':
+        rslt_data.loc[cid] = [n_selection,
+                              spg_num, spg_sym, spg_num_opt, spg_sym_opt,
+                              energy, magmom, check_opt]
+    elif rin.algo in ['EA']:
+        rslt_data.loc[cid] = [gen,
+                              spg_num, spg_sym, spg_num_opt, spg_sym_opt,
+                              energy, magmom, check_opt]
+    elif rin.algo in ['EA-vc']:
+        rslt_data.loc[cid] = [gen,
+                              spg_num, spg_sym, spg_num_opt, spg_sym_opt,
+                              energy, ef, magmom, check_opt]
+    pkl_data.save_rslt(rslt_data)
+    if rin.algo != 'EA-vc':
+        out_rslt(rslt_data)
+    else:    # EA-vc
+        out_rslt(rslt_data, order_ef=True)
+
+    # ---------- return
+    return opt_struc_data, rslt_data
+
+
+def update_status(cid, id_queueing, id_running, operation):
+
+    # ---------- read stat
+    stat = io_stat.stat_read()
+
+    # ---------- update status
+    if operation == 'submit':
+        id_running.append(cid)
+        id_queueing.remove(cid)
+        io_stat.set_stage(stat, cid, 1)
+    elif operation == 'fin':
+        if cid in id_queueing:
+            id_queueing.remove(cid)
+        if cid in id_running:
+            id_running.remove(cid)
+        io_stat.clean_id(stat, cid)
+    else:
+        logger.error('operation is wrong')
+        raise SystemExit(1)
+    io_stat.set_id(stat, 'id_queueing', id_queueing)
+    io_stat.write_stat(stat)
+
+    # ---------- save id_queueing and id_running
+    pkl_data.save_id_queueing(id_queueing)
+    pkl_data.save_id_running(id_running)
+
+    # ---------- return
+    return id_queueing, id_running
+
+
+def mv_fin(cid):
+    if not os.path.isdir(f'work/fin/{cid}'):
+        shutil.move(f'work/{cid}', 'work/fin/')
+    else:    # rename for recalc
+        for i in itertools.count(1):
+            if not os.path.isdir(f'work/fin/{cid}_{i}'):
+                shutil.move(f'work/{cid}',
+                            f'work/fin/{cid}_{i}')
+                break
+
+
+def next_gen_EA(
+        rin,
+        id_queueing,
+        id_running,
+        gen,
+        go_next_sg,
+        init_struc_data,
+        opt_struc_data,
+        rslt_data,
+        ea_vc_data=None,
+        struc_mol_id=None,
+    ):
+
+    # ---------- log
+    logger.info(f'Done generation {gen}')
+
+    # ---------- flag for next selection or generation
+    if not go_next_sg:
+        logger.info('\nEA is ready')
+        os.remove('lock_cryspy')
+        raise SystemExit()
+
+    # ---------- check point 3
+    if rin.stop_chkpt == 3:
+        logger.info('\nStop at check point 3: EA is ready')
+        os.remove('lock_cryspy')
+        raise SystemExit()
+
+    # ---------- maxgen_ea
+    if 0 < rin.maxgen_ea <= gen:
         if rin.algo == 'EA-vc':
-            ea_vc_data = (self.nat_data, self.ratio_data, self.hdist_data)
-        else:
-            ea_vc_data = None
-        ea_next_gen.next_gen(self.stat, self.init_struc_data, struc_mol_id,
-                             self.opt_struc_data, self.rslt_data, ea_id_data, ea_vc_data)
-
-    def save_id_data(self):
-        # ---------- save id_data
-        if rin.algo == 'RS':
-            rs_id_data = (self.id_queueing, self.id_running)
-            pkl_data.save_rs_id(rs_id_data)
-        if rin.algo == 'BO':
-            bo_id_data = (self.n_selection, self.id_queueing,
-                          self.id_running, self.id_select_hist)
-            pkl_data.save_bo_id(bo_id_data)
-        if rin.algo == 'LAQA':
-            laqa_id_data = (self.id_queueing, self.id_running,
-                            self.id_select_hist)
-            pkl_data.save_laqa_id(laqa_id_data)
-        if rin.algo in ['EA', 'EA-vc']:
-            ea_id_data = (self.gen, self.id_queueing, self.id_running)
-            pkl_data.save_ea_id(ea_id_data)
-
-    def save_data(self):
-        # ---------- save ??_data
-        if rin.algo == 'BO':
-            bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
-                       self.bo_mean, self.bo_var, self.bo_score)
-            pkl_data.save_bo_data(bo_data)
-        if rin.algo == 'LAQA':
-            laqa_data = (self.tot_step_select, self.laqa_step, self.laqa_struc,
-                         self.laqa_energy, self.laqa_bias, self.laqa_score)
-            pkl_data.save_laqa_data(laqa_data)
-        # ea_data is used only in ea_next_gen.py
-        # ea_vc_data is used in this class, but it is not updated.
-        # ea_vc_data is saved in ea_next_gen.py
+            # ------ when gen reaches maxgen_ea,  next generation is not created
+            #        so convex hull is calculated here
+            #        update only convex hull and hdist, not elite_struc and elite_fitness
+            c_rslt = rslt_data[rslt_data['Gen'] == gen]
+            c_ids = c_rslt.index.values    # current IDs [array]
+            ef_all = rslt_data['Ef_eV_atom'].to_dict()    # formation energy of all structures
+            from ..EA.calc_hull import calc_convex_hull_2d
+            nat_data, ratio_data, hdist_data = ea_vc_data
+            hdist = calc_convex_hull_2d(rin, ratio_data, ef_all, c_ids, gen)
+            out_hdist(gen, hdist, ratio_data)
+            hdist_data[gen] = hdist
+            pkl_data.save_hdist_data(hdist_data)
+        logger.info(f'\nReached maxgen_ea: {rin.maxgen_ea}')
+        os.remove('lock_cryspy')
+        raise SystemExit()
+
+    # ---------- EA
+    backup_cryspy()
+    from ..EA import ea_next_gen
+    ea_next_gen.next_gen(
+        rin,
+        id_queueing,
+        id_running,
+        gen,
+        init_struc_data,
+        opt_struc_data,
+        rslt_data,
+        ea_vc_data,
+        struc_mol_id,
+    )
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/scripts/cryspy.py` & `csp_cryspy-1.3.0/src/cryspy/scripts/cryspy.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Main script
 '''
 
 import argparse
 from logging import getLogger
 import os
 
-from cryspy.IO import read_input as rin
 from cryspy.start import cryspy_init, cryspy_restart
 from cryspy.util.utility import set_logger, backup_cryspy, clean_cryspy
 
 # ---------- import later
 # from mpi4py import MPI
 # from cryspy.job.ctrl_ext import Ctrl_ext
 # from cryspy.job.ctrl_job import Ctrl_job
@@ -37,15 +36,21 @@
     else:
         # ------ normal run
         comm = None
         mpi_rank = 0
         mpi_size = 1
 
     # ---------- logger
-    set_logger(args.noprint, args.debug)
+    set_logger(
+        noprint=args.noprint,
+        debug=args.debug,
+        logfile='log_cryspy',
+        errfile='err_cryspy',
+        debugfile='debug_cryspy',
+    )
     logger = getLogger('cryspy')
 
     # ---------- backup option
     if args.backup:
         if mpi_rank == 0:
             backup_cryspy()
         raise SystemExit()
@@ -75,41 +80,41 @@
         cryspy_init.initialize(comm, mpi_rank, mpi_size)
         if mpi_rank == 0:
             os.remove('lock_cryspy')
         raise SystemExit()
     # ---------- restart
     else:
         # only stat and init_struc_data in rank0 are important
-        stat, init_struc_data = cryspy_restart.restart(comm, mpi_rank, mpi_size)
+        rin, init_struc_data = cryspy_restart.restart(comm, mpi_rank, mpi_size)
     # ########## MPI end
 
     if mpi_rank == 0:
         # ---------- check point 1
         if rin.stop_chkpt == 1:
             logger.info('Stop at check point 1')
             os.remove('lock_cryspy')
             raise SystemExit()
 
         if not rin.calc_code == 'ext':
             # ---------- check calc files in ./calc_in
             from cryspy.interface import select_code
-            select_code.check_calc_files()
+            select_code.check_calc_files(rin)
             # ---------- mkdir work/fin
             os.makedirs('work/fin', exist_ok=True)
 
         # ---------- Perform structure optimization externally
         if rin.calc_code == 'ext':
             # ------ instantiate Ctrl_job class
             from cryspy.job.ctrl_ext import Ctrl_ext
-            jobs = Ctrl_ext(stat, init_struc_data)
+            jobs = Ctrl_ext(rin, init_struc_data)
         # ---------- internally
         else:
             # ---------- instantiate Ctrl_job class
             from cryspy.job.ctrl_job import Ctrl_job
-            jobs = Ctrl_job(stat, init_struc_data)
+            jobs = Ctrl_job(rin, init_struc_data)
 
         # ---------- check job status
         jobs.check_job()
 
         # ---------- handle job
         jobs.handle_job()
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/start/cryspy_init.py` & `csp_cryspy-1.3.0/src/cryspy/start/cryspy_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,84 +3,80 @@
 '''
 
 from datetime import datetime
 from logging import getLogger
 import os
 
 import pandas as pd
+import pkg_resources
 
-from .gen_init_struc import gen_init_struc
-from ..IO import pkl_data, io_stat
-from ..IO import read_input as rin
+from ..IO import pkl_data, io_stat, write_input
+from ..IO.read_input import ReadInput
+from ..RS.rs_gen import gen_random
 from ..util.utility import get_version
 from ..util.struc_util import out_poscar
 
 # ---------- import later
 #from ..RS import rs_init
 #from ..BO import bo_init
 #from ..LAQA import laqa_init
 #from ..EA import ea_init
-#from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
-#from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
 
 
 logger = getLogger('cryspy')
 
+
 def initialize(comm, mpi_rank, mpi_size):
     # ---------- start
     if mpi_rank == 0:
         logger.info('\n\n\nStart CrySPY ' + get_version() + '\n\n')
     # ---------- check versions
     if mpi_rank == 0:
-        logger.info('# ---------- Check version')
+        logger.info('# ---------- Library version info')
         logger.info(f'pandas version: {pd.__version__}')
-
+        v_pymat = pkg_resources.get_distribution('pymatgen').version
+        v_pyxtal = pkg_resources.get_distribution('pyxtal').version
+        logger.info(f'pymatgen version: {v_pymat}')
+        logger.info(f'pyxtal version: {v_pyxtal}')
     # ---------- read input
     if mpi_rank == 0:
         logger.info('# ---------- Read input file, cryspy.in')
     # ########## MPI start
     if mpi_size > 1:
         comm.barrier()
     try:
-        rin.readin()          # read input data, cryspy,in
+        rin = ReadInput()    # read input data, cryspy,in
     except Exception as e:
         if mpi_rank == 0:
-            logger.error(str(e.args[0]))
+            logger.error(e)
         raise SystemExit(1)
     # ########## MPI end
     if mpi_rank == 0:
-        stat = io_stat.stat_init()    # initialize stat
-        rin.save_stat(stat)   # save input variables in cryspy.stat
-
         # ---------- make data directory
         os.makedirs('data/pkl_data', exist_ok=True)
+        # ---------- write and save input file
+        write_input.out_input(rin)    # log
+        pkl_data.save_input(rin)      # input_data.pkl
 
     # ---------- generate initial structures
     if not rin.load_struc_flag:
         if mpi_size > 1:
             comm.barrier()
         if mpi_rank == 0:
             # ------ time
             time_start = datetime.today()
         # ########## MPI start
-        # ------ from scratch
-        init_struc_data = {}
-        if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
-            struc_mol_id = {}
-        # ------ gen_init_struc()
+        # ------ structure generation
         # only init_struc_data in rank0 is important
-        if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
-            init_struc_data, struc_mol_id = gen_init_struc(init_struc_data, struc_mol_id,
-                                                           comm, mpi_rank, mpi_size)
-        else:
-            init_struc_data = gen_init_struc(init_struc_data, None,
-                                             comm, mpi_rank, mpi_size)
+        init_struc_data, struc_mol_id = gen_random(rin, rin.tot_struc, 0,
+                                                       comm, mpi_rank, mpi_size)
         # ########## MPI end
-
         if mpi_rank == 0:
+            # ------ init_POSCARS
+            out_poscar(init_struc_data, './data/init_POSCARS', mode='w')
             # ------ save
             pkl_data.save_init_struc(init_struc_data)
             if rin.algo in ['EA', 'EA-vc'] and rin.struc_mode in ['mol', 'mol_bs']:
                 pkl_data.save_struc_mol_id(struc_mol_id)
             # ------ time
             time_end = datetime.today()
             etime = time_end - time_start
@@ -93,18 +89,20 @@
             init_struc_data = pkl_data.load_init_struc()
             # -- check
             if not rin.tot_struc == len(init_struc_data):
                 logger.error(f'rin.tot_struc = {rin.tot_struc},'
                                 f' len(init_struc_data) = {len(init_struc_data)}')
                 raise SystemExit(1)
             # -- init_POSCARS
-            for cid, struc in init_struc_data.items():
-                out_poscar(struc, cid, './data/init_POSCARS')
+            out_poscar(init_struc_data, './data/init_POSCARS', mode='w')
 
     if mpi_rank == 0:
+        # ---------- initialize stat
+        io_stat.stat_init()
+
         # ---------- initialize opt_struc_data
         opt_struc_data = {}
         pkl_data.save_opt_struc(opt_struc_data)
 
         # ---------- initialize rslt_data
         rslt_data = pd.DataFrame(columns=['Spg_num', 'Spg_sym',
                                         'Spg_num_opt', 'Spg_sym_opt',
@@ -112,24 +110,24 @@
         rslt_data[['Spg_num', 'Spg_num_opt']] = rslt_data[
                                     ['Spg_num', 'Spg_num_opt']].astype(int)
         pkl_data.save_rslt(rslt_data)
 
         # ---------- initialize for each algorithm
         if rin.algo == 'RS':
             from ..RS import rs_init
-            rs_init.initialize(stat)
+            rs_init.initialize(rin)
         elif rin.algo == 'BO':
             from ..BO import bo_init
-            bo_init.initialize(stat, init_struc_data, rslt_data)
+            bo_init.initialize(rin, init_struc_data, rslt_data)
         elif rin.algo == 'LAQA':
             from ..LAQA import laqa_init
-            laqa_init.initialize(stat)
+            laqa_init.initialize(rin)
         elif rin.algo in ['EA', 'EA-vc']:
             from ..EA import ea_init
-            ea_init.initialize(stat, init_struc_data, rslt_data)
+            ea_init.initialize(rin, init_struc_data, rslt_data)
 
         # ---------- initialize etc
         if rin.kpt_flag:
             kpt_data = {}
             pkl_data.save_kpt(kpt_data)
         if rin.energy_step_flag:
             energy_step_data = {}
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/start/cryspy_restart.py` & `csp_cryspy-1.3.0/src/cryspy/start/cryspy_restart.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,145 +2,148 @@
 Restart CrySPY
 '''
 
 from datetime import datetime
 from logging import getLogger
 import os
 
-from .gen_init_struc import gen_init_struc
-from ..IO import io_stat, pkl_data
-from ..IO import read_input as rin
+from ..IO import diff_input, pkl_data
+from ..IO.read_input import ReadInput
+from ..RS.rs_gen import gen_random
 from ..util.utility import get_version, backup_cryspy
+from ..util.struc_util import out_poscar
 
 # ---------- import later
 #from ..RS import rs_restart
 #from ..BO import bo_restart
 #from ..LAQA import laqa_restart
 #from ..EA import ea_append
-#from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
-#from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
 
 
 logger = getLogger('cryspy')
 
 def restart(comm, mpi_rank, mpi_size):
     if mpi_rank == 0:
         logger.info('\n\n\nRestart CrySPY ' + get_version() + '\n\n')
-        # ---------- read stat
-        stat = io_stat.stat_read()
-    else:
-        stat = None
 
     # ########## MPI start
     if mpi_size > 1:
         comm.barrier()
     # ---------- read input and check the change
+    if mpi_rank == 0:
+        logger.info('read input, cryspy.in')
     try:
-        rin.readin()
+        # all processes read input data
+        rin = ReadInput()    # read input data, cryspy,in
     except Exception as e:
         if mpi_rank == 0:
-            logger.error(str(e.args[0]))
+            logger.error(e)
         raise SystemExit(1)
     if mpi_rank == 0:
         try:
-            rin.diffinstat(stat)
+            # only rank0 compares current and previous input
+            pin = pkl_data.load_input()    # load previous input data from input_data.pkl
+            diff_input.diff_in(rin, pin)           # compare current and previous input
+            pkl_data.save_input(rin)       # save input data to input_data.pkl
         except Exception as e:
             if mpi_size > 1:
                 comm.Abort(1)
-            logger.error(str(e.args[0]))
+            logger.error(e)
             raise SystemExit(1)
 
     # ------ load init_struc_data for appending structures
     # In EA, one can not change tot_struc, so struc_mol_id need not be considered here
     # _append_struc is not allowed in EA and EA-vc either
     init_struc_data = pkl_data.load_init_struc()
+    append_flag = False
 
     # ---------- append structures
     if len(init_struc_data) < rin.tot_struc:
+        # ------ append_flag
+        append_flag = True
         # ------ backup
         if mpi_rank == 0:
             backup_cryspy()
         # ------ barrier for MPI
         if mpi_size > 1:
             comm.barrier()
         # ------ append struc.
         if mpi_rank == 0:
             prev_nstruc = len(init_struc_data)
-        init_struc_data = _append_struc(init_struc_data, comm, mpi_rank, mpi_size)
-        # ------ post append
-        if mpi_rank == 0:
-            # -- RS
-            if rin.algo == 'RS':
-                from ..RS import rs_restart
-                rs_restart.restart(stat, prev_nstruc)
-            # -- BO
-            if rin.algo == 'BO':
-                from ..BO import bo_restart
-                bo_restart.restart(init_struc_data, prev_nstruc)
-            # -- LAQA
-            if rin.algo == 'LAQA':
-                from ..LAQA import laqa_restart
-                laqa_restart.restart(stat, prev_nstruc)
-            os.remove('lock_cryspy')
-        raise SystemExit()
+        #        init_struc_data is saved in _append_struc
+        init_struc_data = _append_struc(rin, init_struc_data, comm, mpi_rank, mpi_size)
     elif rin.tot_struc < len(init_struc_data):
         logger.error('tot_struc < len(init_struc_data)')
         raise SystemExit(1)
 
     # ---------- append structures by EA (option)
     # not support MPI
     if rin.append_struc_ea:
+        # ------ append_flag
+        append_flag = True
         if mpi_rank == 0:
             # ------ backup
             backup_cryspy()
     #
     # struc_mol_id has not developed yet here
     #if rin.struc_mode in ['mol', 'mol_bs']:
     #    struc_mol_id = pkl_data.load_struc_mol_id()
     #
             from ..EA import ea_append
             prev_nstruc = len(init_struc_data)
-            init_struc_data = ea_append.append_struc(stat, init_struc_data)
+            # init_struc_data is saved in ea_append.append_struc()
+            init_struc_data = ea_append.append_struc(rin, init_struc_data)
+
+    # ---------- post append
+    if append_flag:
+        if mpi_rank == 0:
             # ------ RS
             if rin.algo == 'RS':
                 from ..RS import rs_restart
-                rs_restart.restart(stat, prev_nstruc)
+                rs_restart.restart(rin, prev_nstruc)
             # ------ BO
             if rin.algo == 'BO':
                 from ..BO import bo_restart
-                bo_restart.restart(init_struc_data, prev_nstruc)
+                bo_restart.restart(rin, init_struc_data, prev_nstruc)
             # ------ LAQA
             if rin.algo == 'LAQA':
                 from ..LAQA import laqa_restart
-                laqa_restart.restart(stat, prev_nstruc)
+                laqa_restart.restart(rin, prev_nstruc)
+            # ------ remove lock_cryspy
             os.remove('lock_cryspy')
         raise SystemExit()
 
     # ---------- return
-    return stat, init_struc_data
+    return rin, init_struc_data
 
 
-def _append_struc(init_struc_data, comm, mpi_rank, mpi_size):
-    # ---------- append initial structures
+def _append_struc(rin, init_struc_data, comm, mpi_rank, mpi_size):
+    # ---------- log
     if mpi_rank == 0:
         logger.info('# ---------- Append structures')
     if mpi_size > 1:
         comm.barrier()
-    # ------ time
+
+    # ---------- time
     if mpi_rank == 0:
         time_start = datetime.today()
 
-    # ---------- gen_init_struc()
+    # ---------- generate structures
     # only init_struc_data in rank0 is important
-    init_struc_data = gen_init_struc(init_struc_data, None,
+    nstruc = rin.tot_struc - len(init_struc_data)
+    tmp_struc_data, tmp_struc_mol_id = gen_random(rin, nstruc, len(init_struc_data),
                                         comm, mpi_rank, mpi_size)
 
     if mpi_rank == 0:
-        # ---------- save
+        out_poscar(tmp_struc_data, './data/init_POSCARS')
+        # ---------- update and save
+        init_struc_data.update(tmp_struc_data)
+        # ToDo: struc_mol_id
         pkl_data.save_init_struc(init_struc_data)
+
         # ---------- time
         time_end = datetime.today()
         etime = time_end - time_start
         logger.info(f'Elapsed time for structure generation: {etime}')
 
     # ---------- return
     # only init_struc_data in rank0 is important
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/util/struc_util.py` & `csp_cryspy-1.3.0/src/cryspy/util/struc_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 '''
 
 from logging import getLogger
 import os
 
 import numpy as np
 
-from pymatgen.core import Structure
+from pymatgen.core import Structure, Molecule
 from pymatgen.io.cif import CifWriter
+from pyxtal.database.collection import Collection
 from pyxtal.tolerance import Tol_matrix
 
-from ..IO import read_input as rin
-
 
 logger = getLogger('cryspy')
 
-def set_mindist(mindist_in, factor, dummy=False, mpi_rank=0):
+
+def set_mindist(atype, mindist_in, factor, struc_mode='crystal',
+                dummy=False, mol_file=None, mpi_rank=0):
     # ---------- dummy atom in mol_bs
     if dummy:
-        atype = get_atype_dummy()
-    else:
-        atype = rin.atype
+        atype = get_atype_dummy(len(mol_file))
 
     # ---------- mindist
     if mindist_in is None:
         # ------ Tol matrix
-        if rin.struc_mode in ['crystal']:
+        if struc_mode in ['crystal']:
             tolmat = Tol_matrix(prototype='atomic', factor=factor)
-        elif rin.struc_mode in ['mol', 'mol_bs']:
+        elif struc_mode in ['mol', 'mol_bs']:
             tolmat = Tol_matrix(prototype='molecular', factor=factor)
         else:
             logger.error('struc_mode is wrong')
             raise SystemExit(1)
         # ------ set mindist
         mindist = []
         for i, itype in enumerate(atype):
@@ -46,60 +45,98 @@
 
     # ---------- log
     if mpi_rank == 0:
         for i, itype in enumerate(atype):
             for j, jtype in enumerate(atype):
                 if i <= j:
                     if dummy:
-                        logger.info(f'{rin.mol_file[i]} - {rin.mol_file[j]}: {mindist[i][j]}')
+                        logger.info(f'{mol_file[i]} - {mol_file[j]}: {mindist[i][j]}')
                     else:
                         logger.info(f'{itype} - {jtype}: {mindist[i][j]}')
-        if rin.struc_mode == 'mol':
+        if struc_mode == 'mol':
             logger.info('When struc_mode is mol (only random structure, not EA part),\n'
             '- tolerance between monoatomic molecules is multiplied by 0.8 inside pyxtal (not printed above)\n'
             '- H-N, H-O, or H-F tolerance is multiplied by 0.9 inside pyxtal (not printed above)')
 
     # ---------- return
     return mindist
 
 
-def get_atype_dummy():
+def get_atype_dummy(n_mol_file):
     noble_gas = ['Rn', 'Xe', 'Kr', 'Ar', 'Ne', 'He']
-    if len(rin.nmol) > len(noble_gas):
-        logger.error('len(nmol) > len(noble_gas)')
+    if n_mol_file > len(noble_gas):
+        logger.error('len(mol_file) > len(noble_gas)')
         raise SystemExit(1)
-    atype = noble_gas[:len(rin.nmol)]
+    atype = noble_gas[:n_mol_file]
     return atype
 
 
-def out_poscar(struc, cid, fpath):
-    # ---------- poscar format
-    pos = struc.to(fmt='poscar')
-    pos = pos.split('\n')
-    blank_indx = pos.index('')    # cut unnecessary parts
-    pos = pos[:blank_indx]
-    pos[0] = 'ID_{}'.format(cid)    # replace with ID
-    lines = [line+'\n' for line in pos]
-
-    # ---------- append POSCAR
-    with open(fpath, 'a') as f:
-        for line in lines:
-            f.write(line)
+def get_mol_data(mol_file):
+    '''
+    get molecular data
+
+    Input:
+        mol_file (tuple)
+            e.g. ('Li.xyz', 'PS4.xyz')
+
+    return:
+        mol_data (list)
+            Molecule data in pymatgen format
+    '''
+    # ----------
+    mol_data = []
+    pyxtal_mol_data = Collection('molecules')
+    pyxtal_mol_names = list(Collection('molecules'))
+    for i, mf in enumerate(mol_file):
+        if os.path.isfile(mf):
+            mol = Molecule.from_file(mf)
+        elif mf in pyxtal_mol_names:
+            mol = pyxtal_mol_data[mf]
+        else:
+            logger.error('no molecular files')
+            raise SystemExit(1)
+        mol_data.append(mol)
+    return mol_data
+
+
+def out_poscar(struc_data: dict, fpath: str, mode='a'):
+    '''
+    # ---------- args
+    struc_data (dict): {'ID': Structure, 'ID': Structure, ...}
+    fpath (str): file path for output
+    mode (str): 'w' or 'a'
+    '''
+    # ---------- if mode='w', clear file
+    with open(fpath, mode):
+        pass
+    # ---------- wrtie POSCAR
+    for cid, struc in struc_data.items():
+        # ---------- poscar format
+        pos = struc.to(fmt='poscar')
+        pos = pos.split('\n')
+        blank_indx = pos.index('')    # cut unnecessary parts
+        pos = pos[:blank_indx]
+        pos[0] = f'ID_{cid}'    # replace with ID
+        lines = [line+'\n' for line in pos]
+        # ---------- always mode='a'
+        with open(fpath, 'a') as f:
+            for line in lines:
+                f.write(line)
 
 
-def out_cif(struc, cid, tmp_path, fpath, symprec=0.1):
+def out_cif(struc, cid, tmp_path, fpath, symprec=0.01):
     # ---------- opt_CIFS
     cif = CifWriter(struc, symprec=symprec)
     cif.write_file(tmp_path+'tmp.cif')
 
     # ---------- correct title for VESTA
     #                (need to delete '_chemical_formula_sum'. i don't know why)
     with open(tmp_path+'tmp.cif', 'r') as fcif:
         ciflines = fcif.readlines()
-    ciflines[1] = 'data_ID_{}\n'.format(cid)
+    ciflines[1] = f'data_ID_{cid}\n'
     if ciflines[11][:21] == '_chemical_formula_sum':
         ciflines.pop(11)
     else:
         logger.error('ciflines[11] is not _chemical_formula_sum,'
                          ' have to fix bag')
         raise SystemExit(1)
 
@@ -433,10 +470,10 @@
                 sorted_mol_id.append(mol_id[j])
                 sorted_group_id.append(group_id[j])
     return sorted_struc, sorted_mol_id, sorted_group_id
 
 
 def get_nat(struc, atype):
     compos = struc.composition.as_dict()
-    nat = [int(compos[at]) for at in atype]
-    ratio = [x/sum(nat) for x in nat]
+    nat = tuple([int(compos[at]) for at in atype])
+    ratio = tuple([x/sum(nat) for x in nat])
     return nat, ratio
```

### Comparing `csp_cryspy-1.2.5/src/cryspy/util/utility.py` & `csp_cryspy-1.3.0/src/cryspy/util/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,47 +9,53 @@
 import subprocess
 import sys
 
 
 logger = getLogger('cryspy')
 
 def get_version():
-    return '1.2.5'
+    return '1.3.0'
 
 
-def set_logger(noprint=False, debug=False):
+def set_logger(noprint=False, debug=False, logfile=None, errfile=None, debugfile=None):
     # ---------- level and formatter
     logger.setLevel(DEBUG)
     fmt = Formatter("[%(asctime)s][%(module)s][%(levelname)s] %(message)s")
 
     # ---------- stream handler for log
     if not noprint:
         shandler = StreamHandler(stream=sys.stdout)
         shandler.setFormatter(fmt)
-        shandler.setLevel(INFO)
+        if debug:
+            shandler.setLevel(DEBUG)
+        else:
+            shandler.setLevel(INFO)
         logger.addHandler(shandler)
 
     # ---------- file handler for log (level == INFO)
-    fhandler = FileHandler('./log_cryspy')
-    fhandler.setFormatter(fmt)
-    fhandler.addFilter(lambda record: record.levelno == INFO)
-    logger.addHandler(fhandler)
+    if logfile is not None:
+        fhandler = FileHandler(logfile)
+        fhandler.setFormatter(fmt)
+        fhandler.addFilter(lambda record: record.levelno == INFO)
+        logger.addHandler(fhandler)
 
     # ---------- file handler for error (WARNING <= level)
-    ehandler = FileHandler('./err_cryspy')
-    ehandler.setFormatter(fmt)
-    ehandler.setLevel(WARNING)
-    logger.addHandler(ehandler)
+    if errfile is not None:
+        ehandler = FileHandler(errfile)
+        ehandler.setFormatter(fmt)
+        ehandler.setLevel(WARNING)
+        logger.addHandler(ehandler)
 
     # ---------- file handler for debug (level == DEBUG)
     if debug:
-        dhandler = FileHandler('./debug_cryspy')
-        dhandler.setFormatter(fmt)
-        dhandler.addFilter(lambda record: record.levelno == DEBUG)
-        logger.addHandler(dhandler)
+        if debugfile is not None:
+            dhandler = FileHandler(debugfile)
+            dhandler.setFormatter(fmt)
+            dhandler.addFilter(lambda record: record.levelno == DEBUG)
+            logger.addHandler(dhandler)
 
 
 def check_fwpath(fwpath):
     if fwpath is None:
         # ---------- check if find_wy is in your path
         sr = subprocess.run(['which', 'find_wy'], capture_output=True, text=True)
         fwpath = sr.stdout.strip()    # to delete \n
@@ -60,30 +66,14 @@
         # ---------- check fwpath written in cryspy.in
         if not os.path.isfile(fwpath):
             logger.error(f'There is no find_wy program in {fwpath}')
             raise SystemExit(1)
     return fwpath
 
 
-def check_fppath(fppath):
-    if fppath is None:
-        # ---------- check if find_wy is in your path
-        sr = subprocess.run(['which', 'cal_fingerprint'], capture_output=True, text=True)
-        fppath = sr.stdout.strip()    # to delete \n
-        if fppath == '':
-            logger.error('There is no cal_fingerprint program in your path')
-            raise SystemExit(1)
-    else:
-        # ---------- check fppath written in cryspy.in
-        if not os.path.isfile(fppath):
-            logger.error(f'There is no cal_fingerprint program in {fppath}')
-            raise SystemExit(1)
-    return fppath
-
-
 def backup_cryspy():
     # ---------- make directory
     dname = datetime.now().strftime("%Y%m%d_%H%M%S")
     dst = 'backup/' + dname + '/'
     os.makedirs(dst, exist_ok=True)
 
     # ---------- file/directory list
@@ -98,22 +88,23 @@
         if os.path.isdir(d):
             shutil.copytree(d, dst + d)
 
     # ---------- print
     logger.info('Backup data')
 
 
-def clean_cryspy():
+def clean_cryspy(skip_yes=False):
     # ---------- yes/no
-    while True:
-        choice = input("Are you sure you want to clean the data? 'yes' or 'no' [y/n]: ").lower()
-        if choice in ['y', 'yes']:
-            break
-        elif choice in ['n', 'no']:
-            return
+    if not skip_yes:
+        while True:
+            choice = input("Are you sure you want to clean the data? 'yes' or 'no' [y/n]: ").lower()
+            if choice in ['y', 'yes']:
+                break
+            elif choice in ['n', 'no']:
+                return
 
     # ---------- file/directory list
     fdlist = ['cryspy.stat', 'debug_cryspy', 'err_cryspy', 'log_cryspy', 'lock_cryspy',
               'data', 'work', 'ext', 'tmp_calc_FP', 'tmp_gen_struc']
 
     # ---------- clean
     dname = datetime.now().strftime("%Y%m%d_%H%M%S")
```

### Comparing `csp_cryspy-1.2.5/src/csp_cryspy.egg-info/PKG-INFO` & `csp_cryspy-1.3.0/src/csp_cryspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.2.5
+Version: 1.3.0
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -43,17 +43,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.2.5 (2024 May 10)
+version 1.3.0 (2024 May 31)
 
 ## News
+- [2024 May 31] CrySPY 1.3.0 released.
+    + There are important changes. See [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info)
 - [2024 May 10] CrySPY 1.2.5 released.
     + bug fix for order_ef in out_results.py
 - [2024 May 7] CrySPY 1.2.4 released.
     + bug fix
 - [2023 October 21] CrySPY 1.2.3 released.
     + bug fix for MPI
 - [2023 October 18] CrySPY 1.2.2 released.
@@ -77,33 +79,31 @@
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
 
 (optional)
-- [COMBO](https://github.com/Tomoki-YAMASHITA/combo3 "COMBO") (required if algo is BO)
-- mpi4py
+- [PHYSBO](https://www.pasums.issp.u-tokyo.ac.jp/physbo/en/about "PHYSBO") (required if algo is BO)
+- [DScribe](https://singroup.github.io/dscribe/latest/ "DScribe") (required if algo is BO)
+- [mpi4py](https://mpi4py.readthedocs.io/en/stable "mpi4py")
 
 
 See [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc/installation/requirements/ "CrySPY document") in detail.
 
 ### Structure optimizer
 At least one optimizer is required.
 
 - [VASP](https://www.vasp.at "VASP") (tested with version 5.4.4)
 - [QUANTUM ESPRESSO](http://www.quantum-espresso.org "Quantum ESPRESSO") (tested with version 6.x, version 5.x does not work)
 - [OpenMX](http://www.openmx-square.org "OpenMX")
 - [soiap](https://github.com/nbsato/soiap "soiap") (tested with version 0.2.2)
 - [LAMMPS](http://lammps.sandia.gov "LAMMPS")
+- [ASE](https://wiki.fysik.dtu.dk/ase "ASE")
 
-### Others
-(optional)
-- cal-fingerprint: (required if algo is BO)
-- [find_wy](https://github.com/nim-hrkn/find_wy "find_wy"): find_wy can randomly select a combination of Wyckoff positions for a given chemical composition and space group. 
 
 ## Document (English/Japanese)
 [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc "CrySPY documment")
 
 ## CrySPY Utility
 [CrySPY Utility](https://github.com/Tomoki-YAMASHITA/CrySPY_utility "CrySPY Utility")
```

### Comparing `csp_cryspy-1.2.5/src/csp_cryspy.egg-info/SOURCES.txt` & `csp_cryspy-1.3.0/src/csp_cryspy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,58 +2,61 @@
 README.md
 pyproject.toml
 src/cryspy/__init__.py
 src/cryspy/BO/__init__.py
 src/cryspy/BO/bo_init.py
 src/cryspy/BO/bo_next_select.py
 src/cryspy/BO/bo_restart.py
-src/cryspy/BO/combo_cryspy.py
 src/cryspy/BO/select_descriptor.py
 src/cryspy/EA/__init__.py
 src/cryspy/EA/calc_ef.py
 src/cryspy/EA/calc_hull.py
 src/cryspy/EA/ea_append.py
 src/cryspy/EA/ea_child.py
 src/cryspy/EA/ea_init.py
 src/cryspy/EA/ea_next_gen.py
+src/cryspy/EA/survival.py
 src/cryspy/EA/gen_struc_EA/__init__.py
 src/cryspy/EA/gen_struc_EA/addition.py
 src/cryspy/EA/gen_struc_EA/adj_comp.py
 src/cryspy/EA/gen_struc_EA/crossover.py
-src/cryspy/EA/gen_struc_EA/ea_generation.py
 src/cryspy/EA/gen_struc_EA/elimination.py
 src/cryspy/EA/gen_struc_EA/permutation.py
 src/cryspy/EA/gen_struc_EA/rotation.py
 src/cryspy/EA/gen_struc_EA/select_parents.py
 src/cryspy/EA/gen_struc_EA/strain.py
 src/cryspy/EA/gen_struc_EA/substitution.py
 src/cryspy/IO/__init__.py
 src/cryspy/IO/change_input.py
+src/cryspy/IO/diff_input.py
 src/cryspy/IO/io_stat.py
 src/cryspy/IO/out_results.py
 src/cryspy/IO/pkl_data.py
 src/cryspy/IO/read_input.py
+src/cryspy/IO/write_input.py
 src/cryspy/LAQA/__init__.py
 src/cryspy/LAQA/calc_score.py
 src/cryspy/LAQA/laqa_init.py
 src/cryspy/LAQA/laqa_next_selection.py
 src/cryspy/LAQA/laqa_restart.py
 src/cryspy/RS/__init__.py
+src/cryspy/RS/rs_gen.py
 src/cryspy/RS/rs_init.py
 src/cryspy/RS/rs_restart.py
 src/cryspy/RS/gen_struc_RS/__init__.py
 src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
 src/cryspy/RS/gen_struc_RS/random_generation.py
 src/cryspy/calc_dscrpt/__init__.py
 src/cryspy/calc_dscrpt/FP/__init__.py
 src/cryspy/calc_dscrpt/FP/calc_FP.py
 src/cryspy/interactive/__init__.py
 src/cryspy/interactive/action.py
 src/cryspy/interactive/energy_plot.py
-src/cryspy/interactive/restart_intract.py
+src/cryspy/interactive/restart_interact.py
+src/cryspy/interactive/restart_interact_subprocess.py
 src/cryspy/interactive/rslt_energy.py
 src/cryspy/interactive/view_atom.py
 src/cryspy/interface/__init__.py
 src/cryspy/interface/select_code.py
 src/cryspy/interface/ASE/calc_files_ase.py
 src/cryspy/interface/ASE/collect_ase.py
 src/cryspy/interface/ASE/ctrl_job_ase.py
@@ -86,15 +89,14 @@
 src/cryspy/job/ctrl_ext.py
 src/cryspy/job/ctrl_job.py
 src/cryspy/scripts/__init__.py
 src/cryspy/scripts/cryspy.py
 src/cryspy/start/__init__.py
 src/cryspy/start/cryspy_init.py
 src/cryspy/start/cryspy_restart.py
-src/cryspy/start/gen_init_struc.py
 src/cryspy/util/constants.py
 src/cryspy/util/struc_util.py
 src/cryspy/util/utility.py
 src/csp_cryspy.egg-info/PKG-INFO
 src/csp_cryspy.egg-info/SOURCES.txt
 src/csp_cryspy.egg-info/dependency_links.txt
 src/csp_cryspy.egg-info/entry_points.txt
```

