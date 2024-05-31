# Comparing `tmp/xsuite-0.9.3.tar.gz` & `tmp/xsuite-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsuite-0.9.3.tar", last modified: Thu May  2 19:34:56 2024, max compression
+gzip compressed data, was "xsuite-0.9.4.tar", last modified: Fri May  3 14:31:39 2024, max compression
```

## Comparing `xsuite-0.9.3.tar` & `xsuite-0.9.4.tar`

### file list

```diff
@@ -1,158 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.851442 xsuite-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.819442 xsuite-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.823442 xsuite-0.9.3/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/scripts/install_branches.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/scripts/run_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.823442 xsuite-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/cron_test_gh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/cron_test_gh_omp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/cron_test_gpu_cl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/cron_test_gpu_cuda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/cron_test_sh_cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/manual_test_gh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/manual_test_sh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/test_gh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-02 19:34:31.000000 xsuite-0.9.3/.github/workflows/test_sh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-02 19:34:31.000000 xsuite-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-02 19:34:31.000000 xsuite-0.9.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 19:34:31.000000 xsuite-0.9.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-02 19:34:31.000000 xsuite-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 19:34:31.000000 xsuite-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-02 19:34:56.851442 xsuite-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 19:34:31.000000 xsuite-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 19:34:31.000000 xsuite-0.9.3/contributors.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.831442 xsuite-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/acceleration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/apireference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/autogeneration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/beambeam.rst
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/citing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/collective.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/collective_intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/collimation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/combined_cpu_gpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/dev_guide_xtbe_data_structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/dev_guide_xtbe_internal_record.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/dev_guide_xtbe_lost_part_codes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/dev_guide_xtbe_tracking_code.rst
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/dev_guide_xtrack_beam_elements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/dynamic_aperture.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/exciter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/fast_lattice_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.843443 xsuite-0.9.3/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)   296224 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/acceleration.png
--rw-r--r--   0 runner    (1001) docker     (127)    38807 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/beambeam_sigmapi.png
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/beambeamkick.png
--rw-r--r--   0 runner    (1001) docker     (127)   108018 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/crossing_bump.png
--rw-r--r--   0 runner    (1001) docker     (127)   395863 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/dynamic_aperture.png
--rw-r--r--   0 runner    (1001) docker     (127)   201057 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/elena_w_chrom.png
--rw-r--r--   0 runner    (1001) docker     (127)    76009 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/exciter_signals.png
--rw-r--r--   0 runner    (1001) docker     (127)    64395 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/footprint_HO2D.png
--rw-r--r--   0 runner    (1001) docker     (127)   140959 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/footprint_bb_no_rescale.png
--rw-r--r--   0 runner    (1001) docker     (127)   128051 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/footprint_bb_with_rescale.png
--rw-r--r--   0 runner    (1001) docker     (127)   143371 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/footprint_polar.png
--rw-r--r--   0 runner    (1001) docker     (127)   179030 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/footprint_unif_action.png
--rw-r--r--   0 runner    (1001) docker     (127)   179734 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/gaussian.png
--rw-r--r--   0 runner    (1001) docker     (127)   121485 2024-05-02 19:34:31.000000 xsuite-0.9.3/docs/figures/halo.png
--rw-r--r--   0 runner    (1001) docker     (127)   465172 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/loss_location_refinement.png
--rw-r--r--   0 runner    (1001) docker     (127)    70669 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/orbit_bump.png
--rw-r--r--   0 runner    (1001) docker     (127)   203281 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/pencil.png
--rw-r--r--   0 runner    (1001) docker     (127)    67404 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/phasespacedistortion.png
--rw-r--r--   0 runner    (1001) docker     (127)   206008 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/radial_steering.png
--rw-r--r--   0 runner    (1001) docker     (127)    38610 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/stabilitydiagram.png
--rw-r--r--   0 runner    (1001) docker     (127)   112097 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/time_dep_knob_pwlin_tracking.png
--rw-r--r--   0 runner    (1001) docker     (127)   153741 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/time_dep_knob_pwlin_twiss.png
--rw-r--r--   0 runner    (1001) docker     (127)   109560 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/time_dep_knob_sin_pulse_tracking.png
--rw-r--r--   0 runner    (1001) docker     (127)   123326 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/time_dep_knob_sin_tracking.png
--rw-r--r--   0 runner    (1001) docker     (127)   130156 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/time_dep_knob_sin_twiss.png
--rw-r--r--   0 runner    (1001) docker     (127)   140876 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/twiss.png
--rw-r--r--   0 runner    (1001) docker     (127)   183220 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/twiss_beam_sizes.png
--rw-r--r--   0 runner    (1001) docker     (127)    88689 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/twiss_periodic.png
--rw-r--r--   0 runner    (1001) docker     (127)   136677 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/twiss_range.png
--rw-r--r--   0 runner    (1001) docker     (127)    77880 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/twiss_reverse.png
--rw-r--r--   0 runner    (1001) docker     (127)    67165 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/twiss_vs_delta.png
--rw-r--r--   0 runner    (1001) docker     (127)    88492 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/figures/xsuite_logo_alpha.png
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/footprint.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/freeze_longitudinal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/full_table_of_contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.843443 xsuite-0.9.3/docs/generated_code_snippets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/generated_code_snippets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/intrabeam_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/jupyter_tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/match.rst
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/method_4d.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/numericalreproducibility.rst
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/optimize_for_tracking.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/particles_monitor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/particlesmanip.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.847442 xsuite-0.9.3/docs/physics_manual/
--rw-r--r--   0 runner    (1001) docker     (127)    56659 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/bb6d.tex
--rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/bbconfig.tex
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/bibliography.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.847442 xsuite-0.9.3/docs/physics_manual/figures/
--rw-r--r--   0 runner    (1001) docker     (127)   310545 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/b1ip1.png
--rw-r--r--   0 runner    (1001) docker     (127)   298299 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/b1ip5.png
--rw-r--r--   0 runner    (1001) docker     (127)   306208 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/b4ip1.png
--rw-r--r--   0 runner    (1001) docker     (127)   303009 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/b4ip5.png
--rw-r--r--   0 runner    (1001) docker     (127)    62776 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/bhabha_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/bs_1.png
--rw-r--r--   0 runner    (1001) docker     (127)   234007 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/figures/xang_xplane.png
--rw-r--r--   0 runner    (1001) docker     (127)  1450972 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/physics_man.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/physics_man.tex
--rw-r--r--   0 runner    (1001) docker     (127)    72587 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/xfields.tex
--rw-r--r--   0 runner    (1001) docker     (127)    97215 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physics_manual/xtrack.tex
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/physicsguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/pyhtinterface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/singlepart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/spacechargeauto.rst
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/synchrotron_radiation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/tapering.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/time_dependent_knobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/track.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/twiss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/usersguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/v020changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/xmask.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/xobjexample.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-05-02 19:34:32.000000 xsuite-0.9.3/docs/xsuite_data_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-02 19:34:32.000000 xsuite-0.9.3/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-02 19:34:32.000000 xsuite-0.9.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1597 2024-05-02 19:34:32.000000 xsuite-0.9.3/release.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 19:34:32.000000 xsuite-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-02 19:34:32.000000 xsuite-0.9.3/run_on_gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-02 19:34:32.000000 xsuite-0.9.3/run_release_tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:34:56.851442 xsuite-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-02 19:34:32.000000 xsuite-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.851442 xsuite-0.9.3/xsuite/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.851442 xsuite-0.9.3/xsuite/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/__pycache__/kernel_definitions.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/__pycache__/prebuild_kernels.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/kernel_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.851442 xsuite-0.9.3/xsuite/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-02 19:34:32.000000 xsuite-0.9.3/xsuite/prebuild_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:34:56.851442 xsuite-0.9.3/xsuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-02 19:34:56.000000 xsuite-0.9.3/xsuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-02 19:34:56.000000 xsuite-0.9.3/xsuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:34:56.000000 xsuite-0.9.3/xsuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 19:34:56.000000 xsuite-0.9.3/xsuite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 19:34:56.000000 xsuite-0.9.3/xsuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 19:34:56.000000 xsuite-0.9.3/xsuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.167943 xsuite-0.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.135942 xsuite-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.139943 xsuite-0.9.4/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/scripts/install_branches.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/scripts/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.143942 xsuite-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/cron_test_gh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/cron_test_gh_omp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/cron_test_gpu_cl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/cron_test_gpu_cuda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/cron_test_sh_cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/manual_test_gh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/manual_test_sh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/test_gh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-03 14:31:16.000000 xsuite-0.9.4/.github/workflows/test_sh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-03 14:31:16.000000 xsuite-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-03 14:31:16.000000 xsuite-0.9.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-03 14:31:16.000000 xsuite-0.9.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 14:31:16.000000 xsuite-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 14:31:16.000000 xsuite-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-03 14:31:39.167943 xsuite-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-03 14:31:16.000000 xsuite-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-03 14:31:16.000000 xsuite-0.9.4/contributors.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.151943 xsuite-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/acceleration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/apireference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/autogeneration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/beambeam.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/collective.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/collective_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/collimation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/combined_cpu_gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/dev_guide_xtbe_data_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/dev_guide_xtbe_internal_record.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/dev_guide_xtbe_lost_part_codes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/dev_guide_xtbe_tracking_code.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/dev_guide_xtrack_beam_elements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/dynamic_aperture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/exciter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/fast_lattice_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.159943 xsuite-0.9.4/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   296224 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/acceleration.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38807 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/beambeam_sigmapi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/beambeamkick.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108018 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/crossing_bump.png
+-rw-r--r--   0 runner    (1001) docker     (127)   395863 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/dynamic_aperture.png
+-rw-r--r--   0 runner    (1001) docker     (127)   201057 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/elena_w_chrom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76009 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/exciter_signals.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64395 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/footprint_HO2D.png
+-rw-r--r--   0 runner    (1001) docker     (127)   140959 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/footprint_bb_no_rescale.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128051 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/footprint_bb_with_rescale.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143371 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/footprint_polar.png
+-rw-r--r--   0 runner    (1001) docker     (127)   179030 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/footprint_unif_action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   179734 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/gaussian.png
+-rw-r--r--   0 runner    (1001) docker     (127)   121485 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/halo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   465172 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/loss_location_refinement.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70669 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/orbit_bump.png
+-rw-r--r--   0 runner    (1001) docker     (127)   203281 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67404 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/phasespacedistortion.png
+-rw-r--r--   0 runner    (1001) docker     (127)   206008 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/radial_steering.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38610 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/stabilitydiagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112097 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/time_dep_knob_pwlin_tracking.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153741 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/time_dep_knob_pwlin_twiss.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109560 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/time_dep_knob_sin_pulse_tracking.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123326 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/time_dep_knob_sin_tracking.png
+-rw-r--r--   0 runner    (1001) docker     (127)   130156 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/time_dep_knob_sin_twiss.png
+-rw-r--r--   0 runner    (1001) docker     (127)   140876 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/twiss.png
+-rw-r--r--   0 runner    (1001) docker     (127)   183220 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/twiss_beam_sizes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88689 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/twiss_periodic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136677 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/twiss_range.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77880 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/twiss_reverse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67165 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/twiss_vs_delta.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88492 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/figures/xsuite_logo_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/footprint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/freeze_longitudinal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/full_table_of_contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.159943 xsuite-0.9.4/docs/generated_code_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/generated_code_snippets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/intrabeam_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/jupyter_tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/match.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/method_4d.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/numericalreproducibility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/optimize_for_tracking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/particles_monitor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/particlesmanip.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.163943 xsuite-0.9.4/docs/physics_manual/
+-rw-r--r--   0 runner    (1001) docker     (127)    56659 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/bb6d.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/bbconfig.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/bibliography.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.167943 xsuite-0.9.4/docs/physics_manual/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   310545 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/b1ip1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   298299 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/b1ip5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   306208 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/b4ip1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303009 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/b4ip5.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62776 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/bhabha_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/bs_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   234007 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/figures/xang_xplane.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1450972 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/physics_man.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/physics_man.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    72587 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/xfields.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    97215 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physics_manual/xtrack.tex
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/physicsguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/pyhtinterface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/singlepart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/spacechargeauto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/synchrotron_radiation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/tapering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/time_dependent_knobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/track.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/twiss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/usersguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/v020changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/xmask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/xobjexample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-05-03 14:31:16.000000 xsuite-0.9.4/docs/xsuite_data_management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-03 14:31:16.000000 xsuite-0.9.4/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-03 14:31:16.000000 xsuite-0.9.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1597 2024-05-03 14:31:16.000000 xsuite-0.9.4/release.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 14:31:16.000000 xsuite-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-03 14:31:16.000000 xsuite-0.9.4/run_on_gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-03 14:31:16.000000 xsuite-0.9.4/run_release_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:31:39.167943 xsuite-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-03 14:31:16.000000 xsuite-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.167943 xsuite-0.9.4/xsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-03 14:31:16.000000 xsuite-0.9.4/xsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 14:31:16.000000 xsuite-0.9.4/xsuite/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-03 14:31:16.000000 xsuite-0.9.4/xsuite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-03 14:31:16.000000 xsuite-0.9.4/xsuite/kernel_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.167943 xsuite-0.9.4/xsuite/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:16.000000 xsuite-0.9.4/xsuite/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-03 14:31:16.000000 xsuite-0.9.4/xsuite/prebuild_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:31:39.167943 xsuite-0.9.4/xsuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-03 14:31:39.000000 xsuite-0.9.4/xsuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-03 14:31:39.000000 xsuite-0.9.4/xsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:31:39.000000 xsuite-0.9.4/xsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 14:31:39.000000 xsuite-0.9.4/xsuite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 14:31:39.000000 xsuite-0.9.4/xsuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 14:31:39.000000 xsuite-0.9.4/xsuite.egg-info/top_level.txt
```

### Comparing `xsuite-0.9.3/.github/scripts/install_branches.sh` & `xsuite-0.9.4/.github/scripts/install_branches.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 #!/bin/bash
 # copyright ############################### #
 # This file is part of the Xsuite project.  #
 # Copyright (c) CERN, 2024.                 #
 # ######################################### #
 set -xe
 
-repos=(xobjects xdeps xpart xtrack xfields xmask xcoll xsuite-kernels)
+repos=(xobjects xdeps xpart xtrack xfields xmask xcoll)
 xsuite_prefix="${xsuite_prefix:-.}"
 
 # Expects the following environment variables:
 # - $prefix, where to clone the packages
 # - ${repo}_branch, where $repo is one of the repos above (replace - with _)
 # - $precompile_kernels set to "true" or "false"
 
+# Expect Xsuite already cloned by the main workflow
+if [ "${precompile_kernels:-false}" == "false" ]; then
+  export SKIP_KERNEL_BUILD=1
+fi
+pip install --no-deps -v -e "${xsuite_prefix}/xsuite"
+
+# Clone the repos and install them in the correct branch
 for project in "${repos[@]}"; do
   branch_varname="${project//-/_}_branch"
   project_branch=${!branch_varname}  # get value of the variable [project]_branch
 
   IFS=':' read -r -a parts <<< "$project_branch"
   user="${parts[0]}"
   branch="${parts[1]}"
 
   cd "$xsuite_prefix"
   git clone \
     --recursive \
     --single-branch -b "$branch" \
     "https://github.com/${user}/${project}.git"
 
-   if [ "$project" == "xsuite" ]; then
-      if [ "${precompile_kernels:-false}" == "false" ]; then
-          echo export SKIP_KERNEL_BUILD=1
-      fi
-      pip install --no-deps -e -v "${xsuite_prefix}/${project}"
-  else
-      pip install -e "${xsuite_prefix}/${project}[tests]"
-  fi
+    pip install -e "${xsuite_prefix}/${project}[tests]"
 done
```

### Comparing `xsuite-0.9.3/.github/scripts/run_tests.sh` & `xsuite-0.9.4/.github/scripts/run_tests.sh`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/.github/workflows/cron_test_gh.yaml` & `xsuite-0.9.4/.github/workflows/cron_test_gh.yaml`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/.github/workflows/cron_test_sh_cpu.yaml` & `xsuite-0.9.4/.github/workflows/cron_test_sh_cpu.yaml`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/.github/workflows/manual_test_gh.yaml` & `xsuite-0.9.4/.github/workflows/manual_test_gh.yaml`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/.github/workflows/manual_test_sh.yaml` & `xsuite-0.9.4/.github/workflows/manual_test_sh.yaml`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/.github/workflows/release.yaml` & `xsuite-0.9.4/.github/workflows/release.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,16 @@
       - name: Install cibuildwheel
         run: python -m pip install cibuildwheel==2.17.0
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
         env:
           CIBW_BUILD: ${{ matrix.pyver }}-*
+          CIBW_ENVIRONMENT_PASS_LINUX: LDFLAGS
+          LDFLAGS: "-Wl,-S"  # Strip debug symbols: otherwise added by manylinux
 
       - uses: actions/upload-artifact@v4
         with:
           name: dist-wheels-${{ matrix.os }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
 
   build-sdist:
```

### Comparing `xsuite-0.9.3/.github/workflows/test_gh.yaml` & `xsuite-0.9.4/.github/workflows/test_gh.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,14 @@
         required: false
         default: "xsuite:main"
         type: string
       xcoll_location:
         required: false
         default: "xsuite:main"
         type: string
-      xsuite_kernels_location:
-        required: false
-        default: "xsuite:main"
-        type: string
       precompile_kernels:
         required: false
         default: false
         type: boolean
       xobjects_test_contexts:
         required: false
         default: "ContextCpu;ContextCpu:auto"
@@ -99,24 +95,22 @@
         xobjects_branch: ${{ inputs.xobjects_location }}
         xdeps_branch: ${{ inputs.xdeps_location }}
         xpart_branch: ${{ inputs.xpart_location }}
         xtrack_branch: ${{ inputs.xtrack_location }}
         xfields_branch: ${{ inputs.xfields_location }}
         xmask_branch: ${{ inputs.xmask_location }}
         xcoll_branch: ${{ inputs.xcoll_location }}
-        xsuite_kernels_branch: ${{ inputs.xsuite_kernels_location }}
         precompile_kernels: ${{ inputs.precompile_kernels }}
       run: |
         export xsuite_prefix="$GITHUB_WORKSPACE"
-        chmod +x $GITHUB_WORKSPACE/xsuite/.github/scripts/install_branches.sh
-        $GITHUB_WORKSPACE/xsuite/.github/scripts/install_branches.sh
+        bash $GITHUB_WORKSPACE/xsuite/.github/scripts/install_branches.sh
     - name: Precompile kernels
       if: ${{ inputs.precompile_kernels == true }}
       run: |
-        xsuite-kernels regenerate
+        xsuite-prebuild r
     - name: Print versions
       run: conda list
     - name: Run tests (${{ matrix.test-suite }})
       env:
         XOBJECTS_TEST_CONTEXTS: ${{ inputs.xobjects_test_contexts }}
       run: |
         cd $GITHUB_WORKSPACE/${{ matrix.test-suite }}
```

### Comparing `xsuite-0.9.3/.github/workflows/test_sh.yaml` & `xsuite-0.9.4/.github/workflows/test_sh.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,14 @@
         required: false
         default: "xsuite:main"
         type: string
       xcoll_location:
         required: false
         default: "xsuite:main"
         type: string
-      xsuite_kernels_location:
-        required: false
-        default: "xsuite:main"
-        type: string
       test_contexts:
         required: false
         type: string
         default: 'ContextCpu;ContextCpu:auto;ContextCupy;ContextPyopencl'
       platform:
         required: true
         type: string
@@ -73,29 +69,27 @@
           xobjects_branch: ${{ inputs.xobjects_location }}
           xdeps_branch: ${{ inputs.xdeps_location }}
           xpart_branch: ${{ inputs.xpart_location }}
           xtrack_branch: ${{ inputs.xtrack_location }}
           xfields_branch: ${{ inputs.xfields_location }}
           xmask_branch: ${{ inputs.xmask_location }}
           xcoll_branch: ${{ inputs.xcoll_location }}
-          xsuite_kernels_branch: ${{ inputs.xsuite_kernels_location }}
         run: |
           IMAGE="xsuite-test-runner-$(cat /proc/sys/kernel/random/uuid)"
           echo "image_id=$IMAGE" >> $GITHUB_OUTPUT
           docker build \
             --network=host \
             --no-cache=true \
             --build-arg xobjects_branch=${xobjects_branch} \
             --build-arg xdeps_branch=${xdeps_branch} \
             --build-arg xpart_branch=${xpart_branch} \
             --build-arg xtrack_branch=${xtrack_branch} \
             --build-arg xfields_branch=${xfields_branch} \
             --build-arg xmask_branch=${xmask_branch} \
             --build-arg xcoll_branch=${xcoll_branch} \
-            --build-arg xsuite_kernels_branch=${xsuite_kernels_branch} \
             --build-arg with_gpu=${with_gpu} \
             -t $IMAGE .
 
   # Print out some stuff about the test environment
   image-sanity-checks:
     runs-on: [self-hosted, "${{ inputs.platform }}"]
     needs: build-test-image
```

### Comparing `xsuite-0.9.3/.gitignore` & `xsuite-0.9.4/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 xsuite/lib/*.so
 xsuite/lib/*.c
 xsuite/lib/*.json
 
+docs/physics_manual/physics_man.aux
+docs/physics_manual/physics_man.bbl
+docs/physics_manual/physics_man.blg
+docs/physics_manual/physics_man.log
+docs/physics_manual/physics_man.out
+docs/physics_manual/physics_man.toc
+
 # Created by https://www.toptal.com/developers/gitignore/api/macos,linux,python
 # Edit at https://www.toptal.com/developers/gitignore?templates=macos,linux,python
 
 ### Linux ###
 *~
 
 # temporary files which can be created if a process still has a handle open of a deleted file
```

### Comparing `xsuite-0.9.3/.readthedocs.yaml` & `xsuite-0.9.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/Dockerfile` & `xsuite-0.9.4/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         && pip install --no-cache-dir pyopencl mako \
         && git clone --depth 1 https://github.com/geggo/gpyfft.git \
         && pip install ./gpyfft; \
     fi
 
 # Install all the Xsuite packages in the required versions
 WORKDIR /opt/xsuite
-COPY .github/scripts/install_branches.sh /opt/xsuite/
-RUN bash /opt/xsuite/install_branches.sh && pip cache purge
+COPY ./ /opt/xsuite/xsuite/
+RUN bash /opt/xsuite/xsuite/.github/scripts/install_branches.sh && pip cache purge
 
 # Copy the test runner script into the image
 WORKDIR /opt
-COPY .github/scripts/run_tests.sh /opt/
+RUN ln -s /opt/xsuite/xsuite/.github/scripts/run_tests.sh /opt/
 RUN chmod +x run_tests.sh
 
 CMD python /opt/xsuite/xtrack/examples/print_package_paths.py
```

### Comparing `xsuite-0.9.3/LICENSE` & `xsuite-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/PKG-INFO` & `xsuite-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsuite
-Version: 0.9.3
+Version: 0.9.4
 Summary: Integrated suite for particle accelerator simulations.
 Author: Riccardo De Maria, Giovanni Iadarola, Szymon Łopaciuk, et al.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -207,15 +207,15 @@
 Project-URL: Download, https://pypi.python.org/pypi/xsuite
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
 Project-URL: Source Code, https://github.com/xsuite/xsuite
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: xtrack==0.59.0
+Requires-Dist: xtrack==0.59.1
 Requires-Dist: xfields==0.16.0
 Requires-Dist: xcoll==0.3.6
 Requires-Dist: xobjects==0.4.1
 Requires-Dist: xdeps==0.5.7
 Requires-Dist: xpart==0.18.2
 
 # Xsuite
```

### Comparing `xsuite-0.9.3/README.md` & `xsuite-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/Makefile` & `xsuite-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/apireference.rst` & `xsuite-0.9.4/docs/apireference.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/autogeneration.rst` & `xsuite-0.9.4/docs/autogeneration.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/beambeam.rst` & `xsuite-0.9.4/docs/beambeam.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/citing.rst` & `xsuite-0.9.4/docs/citing.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/collective_intro.rst` & `xsuite-0.9.4/docs/collective_intro.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/collimation.rst` & `xsuite-0.9.4/docs/collimation.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/combined_cpu_gpu.rst` & `xsuite-0.9.4/docs/combined_cpu_gpu.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/conf.py` & `xsuite-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/contexts.rst` & `xsuite-0.9.4/docs/contexts.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/dev_guide_xtbe_data_structure.rst` & `xsuite-0.9.4/docs/dev_guide_xtbe_data_structure.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/dev_guide_xtbe_internal_record.rst` & `xsuite-0.9.4/docs/dev_guide_xtbe_internal_record.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/dev_guide_xtbe_lost_part_codes.rst` & `xsuite-0.9.4/docs/dev_guide_xtbe_lost_part_codes.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/dev_guide_xtbe_tracking_code.rst` & `xsuite-0.9.4/docs/dev_guide_xtbe_tracking_code.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/exciter.rst` & `xsuite-0.9.4/docs/exciter.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/fast_lattice_changes.rst` & `xsuite-0.9.4/docs/fast_lattice_changes.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/acceleration.png` & `xsuite-0.9.4/docs/figures/acceleration.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/beambeam_sigmapi.png` & `xsuite-0.9.4/docs/figures/beambeam_sigmapi.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/beambeamkick.png` & `xsuite-0.9.4/docs/figures/beambeamkick.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/crossing_bump.png` & `xsuite-0.9.4/docs/figures/crossing_bump.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/dynamic_aperture.png` & `xsuite-0.9.4/docs/figures/dynamic_aperture.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/elena_w_chrom.png` & `xsuite-0.9.4/docs/figures/elena_w_chrom.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/exciter_signals.png` & `xsuite-0.9.4/docs/figures/exciter_signals.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/footprint_HO2D.png` & `xsuite-0.9.4/docs/figures/footprint_HO2D.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/footprint_bb_no_rescale.png` & `xsuite-0.9.4/docs/figures/footprint_bb_no_rescale.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/footprint_bb_with_rescale.png` & `xsuite-0.9.4/docs/figures/footprint_bb_with_rescale.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/footprint_polar.png` & `xsuite-0.9.4/docs/figures/footprint_polar.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/footprint_unif_action.png` & `xsuite-0.9.4/docs/figures/footprint_unif_action.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/gaussian.png` & `xsuite-0.9.4/docs/figures/gaussian.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/halo.png` & `xsuite-0.9.4/docs/figures/halo.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/loss_location_refinement.png` & `xsuite-0.9.4/docs/figures/loss_location_refinement.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/orbit_bump.png` & `xsuite-0.9.4/docs/figures/orbit_bump.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/pencil.png` & `xsuite-0.9.4/docs/figures/pencil.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/phasespacedistortion.png` & `xsuite-0.9.4/docs/figures/phasespacedistortion.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/radial_steering.png` & `xsuite-0.9.4/docs/figures/radial_steering.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/stabilitydiagram.png` & `xsuite-0.9.4/docs/figures/stabilitydiagram.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/time_dep_knob_pwlin_tracking.png` & `xsuite-0.9.4/docs/figures/time_dep_knob_pwlin_tracking.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/time_dep_knob_pwlin_twiss.png` & `xsuite-0.9.4/docs/figures/time_dep_knob_pwlin_twiss.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/time_dep_knob_sin_pulse_tracking.png` & `xsuite-0.9.4/docs/figures/time_dep_knob_sin_pulse_tracking.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/time_dep_knob_sin_tracking.png` & `xsuite-0.9.4/docs/figures/time_dep_knob_sin_tracking.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/time_dep_knob_sin_twiss.png` & `xsuite-0.9.4/docs/figures/time_dep_knob_sin_twiss.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/twiss.png` & `xsuite-0.9.4/docs/figures/twiss.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/twiss_beam_sizes.png` & `xsuite-0.9.4/docs/figures/twiss_beam_sizes.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/twiss_periodic.png` & `xsuite-0.9.4/docs/figures/twiss_periodic.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/twiss_range.png` & `xsuite-0.9.4/docs/figures/twiss_range.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/twiss_reverse.png` & `xsuite-0.9.4/docs/figures/twiss_reverse.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/twiss_vs_delta.png` & `xsuite-0.9.4/docs/figures/twiss_vs_delta.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/figures/xsuite_logo_alpha.png` & `xsuite-0.9.4/docs/figures/xsuite_logo_alpha.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/footprint.rst` & `xsuite-0.9.4/docs/footprint.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/freeze_longitudinal.rst` & `xsuite-0.9.4/docs/freeze_longitudinal.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/index.rst` & `xsuite-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/installation.rst` & `xsuite-0.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/intrabeam_scattering.rst` & `xsuite-0.9.4/docs/intrabeam_scattering.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/jupyter_tutorials.rst` & `xsuite-0.9.4/docs/jupyter_tutorials.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/line.rst` & `xsuite-0.9.4/docs/line.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/make.bat` & `xsuite-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/match.rst` & `xsuite-0.9.4/docs/match.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/method_4d.rst` & `xsuite-0.9.4/docs/method_4d.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/numericalreproducibility.rst` & `xsuite-0.9.4/docs/numericalreproducibility.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/particles_monitor.rst` & `xsuite-0.9.4/docs/particles_monitor.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/particlesmanip.rst` & `xsuite-0.9.4/docs/particlesmanip.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/bb6d.tex` & `xsuite-0.9.4/docs/physics_manual/bb6d.tex`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/bbconfig.tex` & `xsuite-0.9.4/docs/physics_manual/bbconfig.tex`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/bibliography.bib` & `xsuite-0.9.4/docs/physics_manual/bibliography.bib`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/b1ip1.png` & `xsuite-0.9.4/docs/physics_manual/figures/b1ip1.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/b1ip5.png` & `xsuite-0.9.4/docs/physics_manual/figures/b1ip5.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/b4ip1.png` & `xsuite-0.9.4/docs/physics_manual/figures/b4ip1.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/b4ip5.png` & `xsuite-0.9.4/docs/physics_manual/figures/b4ip5.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/bhabha_1.png` & `xsuite-0.9.4/docs/physics_manual/figures/bhabha_1.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/bs_1.png` & `xsuite-0.9.4/docs/physics_manual/figures/bs_1.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/figures/xang_xplane.png` & `xsuite-0.9.4/docs/physics_manual/figures/xang_xplane.png`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/physics_man.pdf` & `xsuite-0.9.4/docs/physics_manual/physics_man.pdf`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/physics_man.tex` & `xsuite-0.9.4/docs/physics_manual/physics_man.tex`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/xfields.tex` & `xsuite-0.9.4/docs/physics_manual/xfields.tex`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/physics_manual/xtrack.tex` & `xsuite-0.9.4/docs/physics_manual/xtrack.tex`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/pipeline.rst` & `xsuite-0.9.4/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/pyhtinterface.rst` & `xsuite-0.9.4/docs/pyhtinterface.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/singlepart.rst` & `xsuite-0.9.4/docs/singlepart.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/spacechargeauto.rst` & `xsuite-0.9.4/docs/spacechargeauto.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/synchrotron_radiation.rst` & `xsuite-0.9.4/docs/synchrotron_radiation.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/tapering.rst` & `xsuite-0.9.4/docs/tapering.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/testing.rst` & `xsuite-0.9.4/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/time_dependent_knobs.rst` & `xsuite-0.9.4/docs/time_dependent_knobs.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/track.rst` & `xsuite-0.9.4/docs/track.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/twiss.rst` & `xsuite-0.9.4/docs/twiss.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/v020changes.rst` & `xsuite-0.9.4/docs/v020changes.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/xmask.rst` & `xsuite-0.9.4/docs/xmask.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/xobjexample.rst` & `xsuite-0.9.4/docs/xobjexample.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/docs/xsuite_data_management.rst` & `xsuite-0.9.4/docs/xsuite_data_management.rst`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/make_changelog.py` & `xsuite-0.9.4/make_changelog.py`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/pyproject.toml` & `xsuite-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     'setuptools>=64',
     'setuptools-scm[toml]>=8',
-    "xtrack==0.59.0",
+    "xtrack==0.59.1",
     "xfields==0.16.0",
     "xcoll==0.3.6",
     "xobjects==0.4.1",
     "xdeps==0.5.7",
     "xpart==0.18.2",
 ]
 build-backend = 'setuptools.build_meta'
@@ -20,15 +20,15 @@
     {name = "et al."},
 ]
 description = "Integrated suite for particle accelerator simulations."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 dependencies = [
-    "xtrack==0.59.0",
+    "xtrack==0.59.1",
     "xfields==0.16.0",
     "xcoll==0.3.6",
     "xobjects==0.4.1",
     "xdeps==0.5.7",
     "xpart==0.18.2",
 ]
 dynamic = ["version"]
```

### Comparing `xsuite-0.9.3/release.sh` & `xsuite-0.9.4/release.sh`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/run_on_gh.py` & `xsuite-0.9.4/run_on_gh.py`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/run_release_tests.sh` & `xsuite-0.9.4/run_release_tests.sh`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/setup.py` & `xsuite-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/xsuite/cli.py` & `xsuite-0.9.4/xsuite/cli.py`

 * *Files identical despite different names*

### Comparing `xsuite-0.9.3/xsuite/kernel_definitions.py` & `xsuite-0.9.4/xsuite/kernel_definitions.py`

 * *Files 21% similar despite different names*

```diff
@@ -92,79 +92,90 @@
     Quadrupole,
     Sextupole,
     Octupole,
     SecondOrderTaylorMap,
     Exciter,
 ]
 
+# Xfields elements
+DEFAULT_XF_ELEMENTS = [
+    xf.BeamBeamBiGaussian2D,
+    xf.BeamBeamBiGaussian3D,
+    xf.SpaceChargeBiGaussian,
+]
+
+# Xcoll elements
+DEFAULT_XCOLL_ELEMENTS = [
+    ZetaShift,
+    xc.BlackAbsorber,
+    xc.EverestBlock,
+    xc.EverestCollimator,
+    xc.EverestCrystal
+]
+
 NON_TRACKING_ELEMENTS = [
     RandomUniform,
     RandomExponential,
     RandomNormal,
     RandomRutherford,
     MultiSetter,
 ]
 
 # These are enumerated in order specified below: the highest priority at the top
 kernel_definitions = [
-    # ('default_only_xtrack_no_config', {
-    #     'config': {},
-    #     'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
-    # }),
-    ('default_only_xtrack', {
+    ('non_tracking_kernels', {
         'config': BASE_CONFIG,
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': [],
+        'extra_classes': NON_TRACKING_ELEMENTS
     }),
-    ('default_only_xtrack_exact_drifts', {
+    ('default_no_config', {
+        'config': {},
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
+    }),
+    ('default_base_config', {
+        'config': BASE_CONFIG,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
+    }),
+    ('exact_drifts', {
         'config': {
             **BASE_CONFIG,
             'XTRACK_USE_EXACT_DRIFTS': True,
         },
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
-    ('default_only_xtrack_no_limit', {
+    ('default_no_limit', {
         'config': {
             **{k: v for k, v in BASE_CONFIG.items()
                 if k != 'XTRACK_GLOBAL_XY_LIMIT'}
         },
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
-    }),
-    ('only_xtrack_non_tracking_kernels_no_config', {
-        'config': {},
-        'classes': [],
-        'extra_classes': NON_TRACKING_ELEMENTS
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
-    ('only_xtrack_non_tracking_kernels', {
-        'config': BASE_CONFIG,
-        'classes': [],
-        'extra_classes': NON_TRACKING_ELEMENTS
-    }),
-    ('default_only_xtrack_backtrack', {
+    ('default_backtrack', {
         'config': {**BASE_CONFIG, 'XSUITE_BACKTRACK': True},
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
-    ('default_only_xtrack_backtrack_no_limit', {
+    ('only_xtrack_backtrack_no_limit', {
         'config': {
-            **{k: v for k, v in BASE_CONFIG.items()
-                if k != 'XTRACK_GLOBAL_XY_LIMIT'},
-            'XSUITE_BACKTRACK': True
+            **BASE_CONFIG,
+            'XSUITE_BACKTRACK': True,
+            'XTRACK_GLOBAL_XY_LIMIT': False,
         },
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
-    ('only_xtrack_frozen_longitudinal', {
+    ('frozen_longitudinal', {
         'config': {**BASE_CONFIG, **FREEZE_LONGITUDINAL},
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
-    ('only_xtrack_frozen_energy', {
+    ('frozen_energy', {
         'config': {**BASE_CONFIG, **FREEZE_ENERGY},
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
-    ('only_xtrack_backtrack_frozen_energy', {
+    ('backtrack_frozen_energy', {
         'config': {**BASE_CONFIG, **FREEZE_ENERGY, 'XSUITE_BACKTRACK': True},
-        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS,
+        'classes': ONLY_XTRACK_ELEMENTS + NO_SYNRAD_ELEMENTS + DEFAULT_XF_ELEMENTS + DEFAULT_XCOLL_ELEMENTS,
     }),
     ('only_xtrack_taper', {
         'config': {
             **BASE_CONFIG,
             'XTRACK_MULTIPOLE_NO_SYNRAD': False,
             'XTRACK_MULTIPOLE_TAPER': True,
             'XTRACK_DIPOLEEDGE_TAPER': True,
@@ -179,88 +190,7 @@
         'config': {
             **BASE_CONFIG, 'XTRACK_MULTIPOLE_NO_SYNRAD': False,
             'XTRACK_SYNRAD_KICK_SAME_AS_FIRST': True
         },
         'classes': ONLY_XTRACK_ELEMENTS,
     }),
 ]
-
-
-# Xfields elements
-DEFAULT_XF_ELEMENTS = [
-    *ONLY_XTRACK_ELEMENTS,
-    xf.BeamBeamBiGaussian2D,
-    xf.BeamBeamBiGaussian3D,
-    xf.SpaceChargeBiGaussian,
-]
-
-kernel_definitions += [
-    ('default_xfields', {
-        'config': BASE_CONFIG,
-        'classes': [*DEFAULT_XF_ELEMENTS],
-    }),
-    ('default_xfields_no_config', {
-        'config': {},
-        'classes': [*DEFAULT_XF_ELEMENTS],
-    }),
-    ('default_xfields_frozen_longitudinal', {
-        'config': {**BASE_CONFIG, **FREEZE_LONGITUDINAL},
-        'classes': DEFAULT_XF_ELEMENTS,
-    }),
-    ('default_xfields_frozen_energy', {
-        'config': {**BASE_CONFIG, **FREEZE_ENERGY},
-        'classes': DEFAULT_XF_ELEMENTS,
-    }),
-]
-
-# Xcoll elements
-DEFAULT_XCOLL_ELEMENTS = [
-    *ONLY_XTRACK_ELEMENTS,
-    *NO_SYNRAD_ELEMENTS,
-    ZetaShift,
-    xc.BlackAbsorber,
-    xc.EverestBlock,
-    xc.EverestCollimator,
-    xc.EverestCrystal
-]
-
-kernel_definitions += [
-    ('default_xcoll', {
-        'config': BASE_CONFIG,
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_no_config', {
-        'config': {},
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_no_limit', {
-        'config': {
-            **{k: v for k, v in BASE_CONFIG.items()
-                if k != 'XTRACK_GLOBAL_XY_LIMIT'}
-        },
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_frozen_longitudinal', {
-        'config': {**BASE_CONFIG, **FREEZE_LONGITUDINAL},
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_frozen_energy', {
-        'config': {**BASE_CONFIG, **FREEZE_ENERGY},
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_backtrack', {
-        'config': {**BASE_CONFIG, 'XSUITE_BACKTRACK': True},
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_backtrack_no_limit', {
-        'config': {
-            **{k: v for k, v in BASE_CONFIG.items()
-                if k != 'XTRACK_GLOBAL_XY_LIMIT'},
-            'XSUITE_BACKTRACK': True
-        },
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-    ('default_xcoll_backtrack_frozen_energy', {
-        'config': {**BASE_CONFIG, **FREEZE_ENERGY, 'XSUITE_BACKTRACK': True},
-        'classes': DEFAULT_XCOLL_ELEMENTS,
-    }),
-]
```

### Comparing `xsuite-0.9.3/xsuite/prebuild_kernels.py` & `xsuite-0.9.4/xsuite/prebuild_kernels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # copyright ############################### #
 # This file is part of the Xsuite project.  #
 # Copyright (c) CERN, 2024.                 #
 # ######################################### #
 import json
 import os
+from multiprocessing import Pool
 from pathlib import Path
 from pprint import pformat
-from multiprocessing import Pool
 from typing import Iterator, Optional, Tuple
 
 import numpy as np
 
+import xsuite as xs
+import xcoll as xc
+import xfields as xf
 import xobjects as xo
-import xsuite
 import xtrack as xt
+from xsuite.kernel_definitions import kernel_definitions
 from xtrack.general import _print
 
-XSK_PREBUILT_KERNELS_LOCATION = Path(xsuite.__file__).parent / 'lib'
+XSK_PREBUILT_KERNELS_LOCATION = Path(xs.__file__).parent / 'lib'
 
 BEAM_ELEMENTS_INIT_DEFAULTS = {
     'Bend': {
         'length': 1.,
     },
     'Quadrupole': {
         'length': 1.,
@@ -70,36 +73,35 @@
     'SpaceChargeBiGaussian': {
         'longitudinal_profile': {
             '__class__': 'LongitudinalProfileQGaussian',
             'number_of_particles': 1,
             'sigma_z': 0,
         }
     },
+    'EverestBlock': {
+        'material': xc.materials.Silicon,
+    },
+    'EverestCollimator': {
+        'material': xc.materials.Silicon,
+    },
+    'EverestCrystal': {
+        'material': xc.materials.SiliconCrystal,
+    }
 }
 
 # SpaceChargeBiGaussian is not included for now (different issues -
 # circular import, incompatible compilation flags)
 
 
 def get_element_class_by_name(name: str) -> type:
-    try:
-        from xfields import element_classes as xf_element_classes
-    except ModuleNotFoundError:
-        xf_element_classes = ()
-
-    try:
-        from xcoll import element_classes as xc_element_classes
-    except ModuleNotFoundError:
-        xc_element_classes = ()
-
-    xt_multisetter = (xt.MultiSetter, )
-
-    element_classes = (xt.element_classes + xt.rng_classes
-                       + xt.monitor_classes + xt_multisetter
-                       + xf_element_classes + xc_element_classes)
+    extra_classes = (xt.MultiSetter, )
+
+    element_classes = (xt.element_classes + xt.rng_classes + xt.monitor_classes
+                       + xf.element_classes + xc.element_classes
+                       + extra_classes)
 
     for cls in element_classes:
         if cls.__name__ == name:
             return cls
 
     raise ValueError(f'No element class with name {name} available.')
 
@@ -109,81 +111,67 @@
         config: dict,
         kernel_element_classes,
         location,
 ):
     location = Path(location)
     out_file = location / f'{module_name}.json'
 
-    try:
-        import xfields
-        xf_version = xfields.__version__
-    except ModuleNotFoundError:
-        xf_version = None
-
-    try:
-        import xcoll
-        xc_version = xcoll.__version__
-    except ModuleNotFoundError:
-        xc_version = None
-
     kernel_metadata = {
         'config': config.data,
         'classes': [cls._DressingClass.__name__ for cls in kernel_element_classes],
         'versions': {
             'xtrack': xt.__version__,
-            'xfields': xf_version,
-            'xcoll': xc_version,
+            'xfields': xf.__version__,
+            'xcoll': xc.__version__,
             'xobjects': xo.__version__,
         }
     }
 
     with out_file.open('w') as fd:
         json.dump(kernel_metadata, fd, indent=4)
 
 
-def enumerate_kernels() -> Iterator[Tuple[str, dict]]:
+def enumerate_kernels(verbose=False) -> Iterator[Tuple[str, dict]]:
     """
     Iterate over the prebuilt kernels compatible with the current version of
     xsuite. The first element of the tuple is the name of the kernel module
     and the second is a dictionary with the kernel metadata.
     """
-    from xsuite.kernel_definitions import kernel_definitions
     for kernel_name, _ in kernel_definitions:
         metadata_file = XSK_PREBUILT_KERNELS_LOCATION / f'{kernel_name}.json'
 
         if not metadata_file.exists():
             continue
 
         with metadata_file.open('r') as fd:
             kernel_metadata = json.load(fd)
 
-        try:
-            import xfields
-            xf_version = xfields.__version__
-        except ModuleNotFoundError:
-            xf_version = None
-
-        try:
-            import xcoll
-            xc_version = xcoll.__version__
-        except ModuleNotFoundError:
-            xc_version = None
-
-        if kernel_metadata['versions']['xtrack'] != xt.__version__:
-            continue
+        needed_versions = kernel_metadata['versions']
+        have_versions = {
+            'xtrack': xt.__version__,
+            'xfields': xf.__version__,
+            'xcoll': xc.__version__,
+            'xobjects': xo.__version__,
+        }
 
-        if kernel_metadata['versions']['xobjects'] != xo.__version__:
-            continue
+        version_mismatch = False
+        for package in needed_versions.keys():
+            need = needed_versions[package]
+            have = have_versions[package]
+            if need == have:
+                continue
 
-        if (kernel_metadata['versions']['xfields'] != xf_version
-                and xf_version is not None):
-            continue
+            version_mismatch = True
+            if verbose:
+                _print(
+                    f'Version mismatch for kernel `{kernel_name}`: needs '
+                    f'{package}=={need}, but have {package}=={have}.'
+                )
 
-        if (kernel_metadata['versions']['xcoll'] != xc_version
-                and xc_version is not None):
+        if version_mismatch:
             continue
 
         yield metadata_file.stem, kernel_metadata
 
 
 def get_suitable_kernel(
         config: dict,
@@ -192,27 +180,29 @@
 ) -> Optional[Tuple[str, list]]:
     """
     Given a configuration and a list of element classes, return a tuple with
     the name of a suitable prebuilt kernel module together with the list of
     element classes that were used to build it. Set `verbose` to True, to
     obtain a justification of the choice (or lack thereof) on standard output.
     """
-    _print.suppress = False
     env_var = os.environ.get("XSUITE_PREBUILT_KERNELS")
     if env_var and env_var == '0':
         if verbose:
             _print('Skipping the search for a suitable kernel, as the '
                    'environment variable XSUITE_PREBUILT_KERNELS == "0".')
         return
 
+    if os.environ.get("XSUITE_VERBOSE", None) is not None:
+        verbose = True
+
     requested_class_names = [
         cls._DressingClass.__name__ for cls in line_element_classes
     ]
 
-    for module_name, kernel_metadata in enumerate_kernels():
+    for module_name, kernel_metadata in enumerate_kernels(verbose=verbose):
         if verbose:
             _print(f"==> Considering the precompiled kernel `{module_name}`...")
 
         available_classes_names = kernel_metadata['classes']
         if kernel_metadata['config'] != config:
             if verbose:
                 lhs = kernel_metadata['config']
@@ -263,46 +253,34 @@
         kernels = [kernels]
 
     location = Path(location)
 
     # Delete existing kernels to avoid accidentally loading in existing C code
     clear_kernels(kernels=kernels, location=location)
 
-    from xsuite.kernel_definitions import kernel_definitions
-    try:
-        import xcoll as xc
-        BEAM_ELEMENTS_INIT_DEFAULTS['EverestBlock'] = {
-                'material': xc.materials.Silicon,
-                'use_prebuilt_kernels': False
-            }
-        BEAM_ELEMENTS_INIT_DEFAULTS['EverestCollimator'] = {
-                'material': xc.materials.Silicon,
-                'use_prebuilt_kernels': False
-            }
-        BEAM_ELEMENTS_INIT_DEFAULTS['EverestCrystal'] = {
-                'material': xc.materials.SiliconCrystal,
-                'use_prebuilt_kernels': False
-            }
-    except ImportError:
-        pass
-
     kernels_to_build = []
     for module_name, metadata in kernel_definitions:
         if kernels is not None and module_name not in kernels:
             continue
         kernels_to_build.append((module_name, metadata))
 
     thread_pool = Pool(processes=n_threads)
+    results = []
     for idx, (module_name, metadata) in enumerate(kernels_to_build):
         args = (idx, len(kernels_to_build), location, metadata, module_name)
-        thread_pool.apply_async(build_single_kernel, args=args)
+        result = thread_pool.apply_async(build_single_kernel, args=args)
+        results.append(result)
 
     thread_pool.close()
     thread_pool.join()
 
+    # Ensure no errors
+    for result in results:
+        result.get()
+
     _print(f'Built {len(kernels_to_build)} kernels.')
 
 
 def build_single_kernel(idx, total, location, metadata, module_name):
     _print(f'[{idx + 1}/{total}] Building `{module_name}`...')
 
     config = metadata['config']
```

### Comparing `xsuite-0.9.3/xsuite.egg-info/PKG-INFO` & `xsuite-0.9.4/xsuite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsuite
-Version: 0.9.3
+Version: 0.9.4
 Summary: Integrated suite for particle accelerator simulations.
 Author: Riccardo De Maria, Giovanni Iadarola, Szymon Łopaciuk, et al.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -207,15 +207,15 @@
 Project-URL: Download, https://pypi.python.org/pypi/xsuite
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
 Project-URL: Source Code, https://github.com/xsuite/xsuite
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: xtrack==0.59.0
+Requires-Dist: xtrack==0.59.1
 Requires-Dist: xfields==0.16.0
 Requires-Dist: xcoll==0.3.6
 Requires-Dist: xobjects==0.4.1
 Requires-Dist: xdeps==0.5.7
 Requires-Dist: xpart==0.18.2
 
 # Xsuite
```

### Comparing `xsuite-0.9.3/xsuite.egg-info/SOURCES.txt` & `xsuite-0.9.4/xsuite.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -131,13 +131,8 @@
 xsuite/prebuild_kernels.py
 xsuite.egg-info/PKG-INFO
 xsuite.egg-info/SOURCES.txt
 xsuite.egg-info/dependency_links.txt
 xsuite.egg-info/entry_points.txt
 xsuite.egg-info/requires.txt
 xsuite.egg-info/top_level.txt
-xsuite/__pycache__/__init__.cpython-310.pyc
-xsuite/__pycache__/_version.cpython-310.pyc
-xsuite/__pycache__/cli.cpython-310.pyc
-xsuite/__pycache__/kernel_definitions.cpython-310.pyc
-xsuite/__pycache__/prebuild_kernels.cpython-310.pyc
 xsuite/lib/__init__.py
```

