# Comparing `tmp/spiakid_simulation-1.24.tar.gz` & `tmp/spiakid_simulation-1.24a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid_simulation-1.24.tar", last modified: Thu May 30 14:53:58 2024, max compression
+gzip compressed data, was "spiakid_simulation-1.24a0.tar", last modified: Fri May 31 07:23:06 2024, max compression
```

## Comparing `spiakid_simulation-1.24.tar` & `spiakid_simulation-1.24a0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10177 2023-08-28 10:56:06.000000 spiakid_simulation-1.24/LICENSE
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      184 2024-02-15 13:53:03.000000 spiakid_simulation-1.24/MANIFEST.in
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1406 2024-02-08 10:38:39.000000 spiakid_simulation-1.24/README.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      643 2024-02-26 13:13:11.000000 spiakid_simulation-1.24/README_for_pip.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-05-30 14:53:15.000000 spiakid_simulation-1.24/pyproject.toml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/setup.cfg
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.104195 spiakid_simulation-1.24/spiakid_simulation/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.104195 spiakid_simulation-1.24/spiakid_simulation/Example/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.104195 spiakid_simulation-1.24/spiakid_simulation/Example/Calib/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      125 2024-04-22 12:39:15.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Calib/Trans.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3627 2024-04-22 12:39:15.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3799 2024-04-23 11:59:54.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Calib/Wv_ph_calib.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4239 2024-03-11 12:55:11.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Sim_10obj.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4538 2024-03-11 12:55:31.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Sim_Gaussian.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4251 2024-05-14 08:30:04.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Sim_phase.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)   199804 2024-05-27 07:53:09.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Sim_psf.ipynb
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.104195 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-03-11 13:03:11.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Template_10obj.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      541 2024-03-11 12:10:32.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Template_Gaussian.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1038 2024-05-30 13:21:46.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Template_phase.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      764 2024-05-28 11:23:18.000000 spiakid_simulation-1.24/spiakid_simulation/Example/Template_psf.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    18606 2024-05-30 13:44:13.000000 spiakid_simulation-1.24/spiakid_simulation/PhotonSimulator.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      978 2024-02-26 13:07:20.000000 spiakid_simulation-1.24/spiakid_simulation/Simulation.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-10-12 08:37:50.000000 spiakid_simulation-1.24/spiakid_simulation/__init__.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/electronics/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      523 2024-02-07 10:08:03.000000 spiakid_simulation-1.24/spiakid_simulation/electronics/Yaml_rw.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12011 2023-11-06 16:00:40.000000 spiakid_simulation-1.24/spiakid_simulation/electronics/cmplxIQ_params.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      677 2023-11-07 14:19:59.000000 spiakid_simulation-1.24/spiakid_simulation/electronics/data_reading.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     7407 2024-05-28 13:37:44.000000 spiakid_simulation-1.24/spiakid_simulation/electronics/filter.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    53144 2023-11-06 15:58:05.000000 spiakid_simulation-1.24/spiakid_simulation/electronics/resonator.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/IQ/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5250 2024-05-14 08:38:06.000000 spiakid_simulation-1.24/spiakid_simulation/functions/IQ/IQ_sim.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/noise/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5029 2024-04-22 13:11:36.000000 spiakid_simulation-1.24/spiakid_simulation/functions/noise/noise.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/output/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2364 2024-04-23 09:17:38.000000 spiakid_simulation-1.24/spiakid_simulation/functions/output/HDF5_creation.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/phase/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1507 2024-02-07 10:11:13.000000 spiakid_simulation-1.24/spiakid_simulation/functions/phase/calib_read.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4624 2024-05-30 12:00:25.000000 spiakid_simulation-1.24/spiakid_simulation/functions/phase/phase_conversion.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/photon/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3431 2024-02-29 09:30:06.000000 spiakid_simulation-1.24/spiakid_simulation/functions/photon/black_body.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      264 2023-11-02 10:55:48.000000 spiakid_simulation-1.24/spiakid_simulation/functions/photon/contamination.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2512 2023-10-06 09:10:32.000000 spiakid_simulation-1.24/spiakid_simulation/functions/photon/photon_gen_image.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4578 2024-05-16 12:49:17.000000 spiakid_simulation-1.24/spiakid_simulation/functions/photon/rot.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     8080 2024-05-30 11:25:37.000000 spiakid_simulation-1.24/spiakid_simulation/functions/photon/sim_image_photon.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/theory/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6198 2023-08-28 15:04:02.000000 spiakid_simulation-1.24/spiakid_simulation/functions/theory/Calc.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14485 2023-09-18 12:50:04.000000 spiakid_simulation-1.24/spiakid_simulation/functions/theory/MKID.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10145 2023-08-28 10:56:06.000000 spiakid_simulation-1.24/spiakid_simulation/functions/theory/SC.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/timeline/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2894 2024-05-30 11:48:11.000000 spiakid_simulation-1.24/spiakid_simulation/functions/timeline/timeline.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      579 2023-08-28 10:56:06.000000 spiakid_simulation-1.24/spiakid_simulation/functions/utils.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/functions/yaml/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      522 2024-02-15 12:49:21.000000 spiakid_simulation-1.24/spiakid_simulation/functions/yaml/yaml_rw.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/image_process/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2757 2024-05-16 13:29:50.000000 spiakid_simulation-1.24/spiakid_simulation/image_process/PSF_interface.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    16411 2023-12-14 15:07:47.000000 spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/interface.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17502 2024-03-08 16:54:53.000000 spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/interface_mult.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1732 2023-12-14 14:48:00.000000 spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/test_displacement.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14003 2024-05-28 11:30:03.000000 spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/turbulence.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3091 2024-05-30 12:54:58.000000 spiakid_simulation-1.24/spiakid_simulation/image_process/image_generation.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/spiakid_simulation.egg-info/
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-30 14:53:58.000000 spiakid_simulation-1.24/spiakid_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3108 2024-05-30 14:53:58.000000 spiakid_simulation-1.24/spiakid_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-05-30 14:53:58.000000 spiakid_simulation-1.24/spiakid_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       69 2024-05-30 14:53:58.000000 spiakid_simulation-1.24/spiakid_simulation.egg-info/requires.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       19 2024-05-30 14:53:58.000000 spiakid_simulation-1.24/spiakid_simulation.egg-info/top_level.txt
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-30 14:53:58.108195 spiakid_simulation-1.24/test/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      157 2023-09-18 12:50:04.000000 spiakid_simulation-1.24/test/test_simu.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10177 2023-08-28 10:56:06.000000 spiakid_simulation-1.24a0/LICENSE
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      184 2024-02-15 13:53:03.000000 spiakid_simulation-1.24a0/MANIFEST.in
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1267 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1406 2024-02-08 10:38:39.000000 spiakid_simulation-1.24a0/README.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      643 2024-02-26 13:13:11.000000 spiakid_simulation-1.24a0/README_for_pip.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      666 2024-05-31 07:21:46.000000 spiakid_simulation-1.24a0/pyproject.toml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/setup.cfg
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.313514 spiakid_simulation-1.24a0/spiakid_simulation/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/Example/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/Example/Calib/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      125 2024-04-22 12:39:15.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Calib/Trans.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3627 2024-04-22 12:39:15.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3799 2024-04-23 11:59:54.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Calib/Wv_ph_calib.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4239 2024-03-11 12:55:11.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_10obj.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4538 2024-03-11 12:55:31.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_Gaussian.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4251 2024-05-14 08:30:04.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_phase.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)   199804 2024-05-27 07:53:09.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_psf.ipynb
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-03-11 13:03:11.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_10obj.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      541 2024-03-11 12:10:32.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_Gaussian.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1036 2024-05-31 07:17:07.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_phase.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      764 2024-05-28 11:23:18.000000 spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_psf.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    18606 2024-05-30 13:44:13.000000 spiakid_simulation-1.24a0/spiakid_simulation/PhotonSimulator.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      978 2024-02-26 13:07:20.000000 spiakid_simulation-1.24a0/spiakid_simulation/Simulation.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-10-12 08:37:50.000000 spiakid_simulation-1.24a0/spiakid_simulation/__init__.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/electronics/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      523 2024-02-07 10:08:03.000000 spiakid_simulation-1.24a0/spiakid_simulation/electronics/Yaml_rw.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12011 2023-11-06 16:00:40.000000 spiakid_simulation-1.24a0/spiakid_simulation/electronics/cmplxIQ_params.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      677 2023-11-07 14:19:59.000000 spiakid_simulation-1.24a0/spiakid_simulation/electronics/data_reading.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     7407 2024-05-28 13:37:44.000000 spiakid_simulation-1.24a0/spiakid_simulation/electronics/filter.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    53144 2023-11-06 15:58:05.000000 spiakid_simulation-1.24a0/spiakid_simulation/electronics/resonator.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/functions/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/functions/IQ/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5250 2024-05-14 08:38:06.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/IQ/IQ_sim.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/functions/noise/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5029 2024-04-22 13:11:36.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/noise/noise.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/functions/output/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2364 2024-04-23 09:17:38.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/output/HDF5_creation.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/functions/phase/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1507 2024-02-07 10:11:13.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/phase/calib_read.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4657 2024-05-31 07:14:58.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/phase/phase_conversion.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.317514 spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3431 2024-02-29 09:30:06.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/black_body.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      264 2023-11-02 10:55:48.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/contamination.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2512 2023-10-06 09:10:32.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/photon_gen_image.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4578 2024-05-16 12:49:17.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/rot.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     8080 2024-05-30 11:25:37.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/sim_image_photon.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6198 2023-08-28 15:04:02.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/Calc.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14485 2023-09-18 12:50:04.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/MKID.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10145 2023-08-28 10:56:06.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/SC.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/spiakid_simulation/functions/timeline/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2894 2024-05-30 11:48:11.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/timeline/timeline.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      579 2023-08-28 10:56:06.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/utils.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/spiakid_simulation/functions/yaml/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      522 2024-02-15 12:49:21.000000 spiakid_simulation-1.24a0/spiakid_simulation/functions/yaml/yaml_rw.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/spiakid_simulation/image_process/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2757 2024-05-16 13:29:50.000000 spiakid_simulation-1.24a0/spiakid_simulation/image_process/PSF_interface.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    16411 2023-12-14 15:07:47.000000 spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/interface.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17502 2024-03-08 16:54:53.000000 spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/interface_mult.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1732 2023-12-14 14:48:00.000000 spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/test_displacement.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14003 2024-05-28 11:30:03.000000 spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/turbulence.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3091 2024-05-30 12:54:58.000000 spiakid_simulation-1.24a0/spiakid_simulation/image_process/image_generation.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/spiakid_simulation.egg-info/
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1267 2024-05-31 07:23:06.000000 spiakid_simulation-1.24a0/spiakid_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3108 2024-05-31 07:23:06.000000 spiakid_simulation-1.24a0/spiakid_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-05-31 07:23:06.000000 spiakid_simulation-1.24a0/spiakid_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       69 2024-05-31 07:23:06.000000 spiakid_simulation-1.24a0/spiakid_simulation.egg-info/requires.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       19 2024-05-31 07:23:06.000000 spiakid_simulation-1.24a0/spiakid_simulation.egg-info/top_level.txt
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-31 07:23:06.321514 spiakid_simulation-1.24a0/test/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      157 2023-09-18 12:50:04.000000 spiakid_simulation-1.24a0/test/test_simu.py
```

### Comparing `spiakid_simulation-1.24/LICENSE` & `spiakid_simulation-1.24a0/LICENSE`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/PKG-INFO` & `spiakid_simulation-1.24a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-simulation
-Version: 1.24
+Version: 1.24a0
 Summary: Data simulation of SPIAKID project
 Author-email: Sebastien Faes <faesebastien@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/simulation/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
```

### Comparing `spiakid_simulation-1.24/README.md` & `spiakid_simulation-1.24a0/README.md`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/README_for_pip.md` & `spiakid_simulation-1.24a0/README_for_pip.md`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/pyproject.toml` & `spiakid_simulation-1.24a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spiakid-simulation"
-version = "1.24"
+version = "1.24a"
 authors = [
     { name="Sebastien Faes", email="faesebastien@gmail.com"}
 ]
 description = "Data simulation of SPIAKID project"
 readme = "README_for_pip.md"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Calib/Wv_ph_calib.csv` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Calib/Wv_ph_calib.csv`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Sim_10obj.ipynb` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_10obj.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Sim_Gaussian.ipynb` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_Gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Sim_phase.ipynb` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_phase.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Sim_psf.ipynb` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Sim_psf.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Template_10obj.yaml` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_10obj.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Template_Gaussian.yaml` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Template_phase.yaml` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_phase.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Simulation
 
 sim_file: /spiakid/data/Simulation_Image/Simulation_phase_1obj.hdf5
 process_nb: 5
 
 1-Photon_Generation:
   telescope:
-    exposition_time: 10
+    exposition_time: 1
     diameter: 3.5
     obscuration: 1
     latitude: 5
     transmittance: spiakid_simulation/Example/Calib/Trans.csv
     detector: 
-      pix_nbr: 10
+      pix_nbr: 5
       pix_size: 0.5
   star:
     number: 5
     distance: 
       min: 35
       max: 37
     wavelength_array:
```

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Example/Template_psf.yaml` & `spiakid_simulation-1.24a0/spiakid_simulation/Example/Template_psf.yaml`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/PhotonSimulator.py` & `spiakid_simulation-1.24a0/spiakid_simulation/PhotonSimulator.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/Simulation.py` & `spiakid_simulation-1.24a0/spiakid_simulation/Simulation.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/electronics/Yaml_rw.py` & `spiakid_simulation-1.24a0/spiakid_simulation/electronics/Yaml_rw.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/electronics/cmplxIQ_params.py` & `spiakid_simulation-1.24a0/spiakid_simulation/electronics/cmplxIQ_params.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/electronics/data_reading.py` & `spiakid_simulation-1.24a0/spiakid_simulation/electronics/data_reading.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/electronics/filter.py` & `spiakid_simulation-1.24a0/spiakid_simulation/electronics/filter.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/electronics/resonator.py` & `spiakid_simulation-1.24a0/spiakid_simulation/electronics/resonator.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/IQ/IQ_sim.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/IQ/IQ_sim.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/noise/noise.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/noise/noise.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/output/HDF5_creation.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/output/HDF5_creation.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/phase/calib_read.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/phase/calib_read.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/phase/phase_conversion.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/phase/phase_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     """
     dim = np.shape(Photon)
     signal = np.zeros(dim,dtype = object)
 
     args = []
     for i in range(len(pix)):
         k,l = np.int64(pix[i].split(sep='_'))
-        
-        args.append([Photon[k,l],conv_wv[i],conv_phase[i],resolution,(k,l)])
+        if k < dim[0] and l < dim[1]:
+            args.append([Photon[k,l],conv_wv[i],conv_phase[i],resolution,(k,l)])
 
     with mp.Pool(processes=process_nb) as pool : 
         res = pool.map(photon2phase,args)
 
     for r in res:
         signal[r[0][0],r[0][1]] = r[1]
```

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/photon/black_body.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/black_body.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/photon/photon_gen_image.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/photon_gen_image.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/photon/rot.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/rot.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/photon/sim_image_photon.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/photon/sim_image_photon.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/theory/Calc.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/Calc.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/theory/MKID.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/MKID.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/theory/SC.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/theory/SC.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/timeline/timeline.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/timeline/timeline.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/utils.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/utils.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/functions/yaml/yaml_rw.py` & `spiakid_simulation-1.24a0/spiakid_simulation/functions/yaml/yaml_rw.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/image_process/PSF_interface.py` & `spiakid_simulation-1.24a0/spiakid_simulation/image_process/PSF_interface.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/interface.py` & `spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/interface.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/interface_mult.py` & `spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/interface_mult.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/test_displacement.py` & `spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/test_displacement.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/image_process/atmosphere/turbulence.py` & `spiakid_simulation-1.24a0/spiakid_simulation/image_process/atmosphere/turbulence.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation/image_process/image_generation.py` & `spiakid_simulation-1.24a0/spiakid_simulation/image_process/image_generation.py`

 * *Files identical despite different names*

### Comparing `spiakid_simulation-1.24/spiakid_simulation.egg-info/PKG-INFO` & `spiakid_simulation-1.24a0/spiakid_simulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-simulation
-Version: 1.24
+Version: 1.24a0
 Summary: Data simulation of SPIAKID project
 Author-email: Sebastien Faes <faesebastien@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/simulation/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
```

### Comparing `spiakid_simulation-1.24/spiakid_simulation.egg-info/SOURCES.txt` & `spiakid_simulation-1.24a0/spiakid_simulation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

