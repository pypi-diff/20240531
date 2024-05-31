# Comparing `tmp/pyft-0.2.1.tar.gz` & `tmp/pyft-0.2.2.tar.gz`

## Comparing `pyft-0.2.1.tar` & `pyft-0.2.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-------   0      501       20     2767 2024-04-19 18:47:57.000000 pyft-0.2.1/Cargo.toml
--rw-r--r--   0      501       20      428 2024-03-21 19:08:49.000000 pyft-0.2.1/.cargo/config.toml
--rw-r--r--   0      501       20      284 2023-10-20 17:58:19.000000 pyft-0.2.1/.dockerignore
--rw-r--r--   0      501       20       29 2024-03-18 17:54:48.000000 pyft-0.2.1/.gitattributes
--rw-r--r--   0      501       20      468 2023-10-30 21:58:54.000000 pyft-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      433 2024-03-21 20:39:06.000000 pyft-0.2.1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0      501       20     1181 2024-01-11 23:03:28.000000 pyft-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20    11301 2024-04-09 21:26:17.000000 pyft-0.2.1/.github/workflows/release.yml
--rw-r--r--   0      501       20      261 2024-01-24 15:42:11.000000 pyft-0.2.1/.gitignore
--rw-r--r--   0      501       20      475 2023-07-30 04:16:53.000000 pyft-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0      501       20      377 2024-03-13 02:37:48.000000 pyft-0.2.1/.readthedocs.yaml
--rw-------   0      501       20   188717 2024-03-21 20:40:43.000000 pyft-0.2.1/CHANGELOG.md
--rw-r--r--   0      501       20      571 2024-03-21 20:39:06.000000 pyft-0.2.1/CONTRIBUTING.md
--rw-r--r--   0      501       20   115889 2024-03-26 15:18:33.000000 pyft-0.2.1/Cargo.lock
--rw-r--r--   0      501       20      863 2023-10-24 18:55:03.000000 pyft-0.2.1/Dockerfile
--rw-r--r--   0      501       20     1519 2024-03-13 02:37:48.000000 pyft-0.2.1/INSTALL.md
--rw-r--r--   0      501       20      296 2024-03-20 16:43:55.000000 pyft-0.2.1/NOTES.md
--rw-r--r--   0      501       20     3522 2024-03-21 20:39:06.000000 pyft-0.2.1/README.md
--rw-r--r--   0      501       20      297 2023-07-30 04:16:53.000000 pyft-0.2.1/_config.yml
--rw-r--r--   0      501       20   670134 2023-07-30 04:16:53.000000 pyft-0.2.1/assets/img/center.png
--rw-r--r--   0      501       20   160734 2023-07-30 04:16:53.000000 pyft-0.2.1/assets/img/fiber_tools_grey.png
--rw-r--r--   0      501       20   159267 2023-07-30 04:16:53.000000 pyft-0.2.1/assets/img/fiber_tools_teal.png
--rw-r--r--   0      501       20   220557 2023-07-30 04:16:53.000000 pyft-0.2.1/assets/img/ft-extract-all.png
--rw-r--r--   0      501       20   303252 2023-07-30 04:16:53.000000 pyft-0.2.1/assets/img/logo.png
--rw-r--r--   0      501       20     1020 2024-03-21 20:39:06.000000 pyft-0.2.1/build.rs
--rw-r--r--   0      501       20     3421 2023-10-08 04:44:35.000000 pyft-0.2.1/docs/center.md
--rw-r--r--   0      501       20     4687 2024-05-28 15:22:42.000000 pyft-0.2.1/docs/extract.md
--rw-r--r--   0      501       20     2976 2024-03-20 02:07:03.000000 pyft-0.2.1/docs/footprint.md
--rw-r--r--   0      501       20     1322 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft--help.md
--rw-r--r--   0      501       20     1273 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-add-nucleosomes-help.md
--rw-r--r--   0      501       20     1794 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-center-help.md
--rw-r--r--   0      501       20      489 2024-03-21 03:21:43.000000 pyft-0.2.1/docs/ft-clear-kinetics-help.md
--rw-r--r--   0      501       20     1519 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-extract-help.md
--rw-r--r--   0      501       20     2401 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-fire-help.md
--rw-r--r--   0      501       20      677 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-footprint-help.md
--rw-r--r--   0      501       20     1883 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-predict-m6a-help.md
--rw-r--r--   0      501       20      601 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/ft-strip-basemods-help.md
--rw-r--r--   0      501       20      744 2024-03-21 03:21:47.000000 pyft-0.2.1/docs/ft-track-decorators-help.md
--rwxr-xr-x   0      501       20      451 2024-03-21 20:39:06.000000 pyft-0.2.1/docs/make_help_docs.sh
--rw-r--r--   0      501       20      294 2023-07-30 04:16:53.000000 pyft-0.2.1/env.yaml
--rw-r--r--   0      501       20     5008 2023-07-30 04:16:53.000000 pyft-0.2.1/models/2.0_semi_torch.json
--rw-r--r--   0      501       20     8502 2023-07-30 04:16:53.000000 pyft-0.2.1/models/2.2_semi_torch.json
--rw-r--r--   0      501       20    15472 2023-07-30 04:16:53.000000 pyft-0.2.1/models/3.2_semi_torch.json
--rw-r--r--   0      501       20    69919 2023-12-02 03:58:23.000000 pyft-0.2.1/models/FIRE.conf.json
--rw-r--r--   0      501       20  1458572 2023-12-02 03:58:23.000000 pyft-0.2.1/models/FIRE.gbdt.json
--rw-r--r--   0      501       20     4491 2023-07-30 04:16:53.000000 pyft-0.2.1/models/Revio_semi_torch.json
--rwxr-xr-x   0      501       20      646 2024-03-20 02:07:03.000000 pyft-0.2.1/models/convert-pt-to-onnx.py
--rw-r--r--   0      501       20    10587 2024-01-13 04:25:34.000000 pyft-0.2.1/src/bamlift/mod.rs
--rw-r--r--   0      501       20     9600 2024-03-13 02:37:48.000000 pyft-0.2.1/src/bamranges.rs
--rw-r--r--   0      501       20    12549 2024-01-13 04:25:34.000000 pyft-0.2.1/src/basemods/mod.rs
--rw-r--r--   0      501       20    12683 2024-03-21 20:39:06.000000 pyft-0.2.1/src/bio_io/mod.rs
--rw-r--r--   0      501       20    13751 2024-01-14 06:01:13.000000 pyft-0.2.1/src/center.rs
--rw-r--r--   0      501       20    15444 2024-05-28 15:42:55.000000 pyft-0.2.1/src/cli.rs
--rw-r--r--   0      501       20     6758 2024-01-12 01:45:18.000000 pyft-0.2.1/src/decorator.rs
--rw-r--r--   0      501       20     4583 2024-03-20 02:07:03.000000 pyft-0.2.1/src/extract.rs
--rw-r--r--   0      501       20    17551 2024-05-28 15:25:51.000000 pyft-0.2.1/src/fiber.rs
--rw-r--r--   0      501       20    22122 2024-03-13 02:37:48.000000 pyft-0.2.1/src/fire.rs
--rw-r--r--   0      501       20    11686 2024-03-13 02:37:48.000000 pyft-0.2.1/src/footprint.rs
--rw-r--r--   0      501       20     4301 2024-04-11 03:11:08.000000 pyft-0.2.1/src/lib.rs
--rw-r--r--   0      501       20     3848 2024-03-26 15:13:17.000000 pyft-0.2.1/src/m6a_burn/mod.rs
--rw-r--r--   0      501       20    57302 2024-03-20 02:07:03.000000 pyft-0.2.1/src/m6a_burn/revio.onnx
--rw-r--r--   0      501       20    51494 2024-03-20 02:07:03.000000 pyft-0.2.1/src/m6a_burn/three_two.onnx
--rw-r--r--   0      501       20    51671 2024-03-20 02:07:03.000000 pyft-0.2.1/src/m6a_burn/two_two.onnx
--rw-r--r--   0      501       20    51666 2024-03-20 02:07:03.000000 pyft-0.2.1/src/m6a_burn/two_zero.onnx
--rw-r--r--   0      501       20     5151 2024-04-11 16:00:05.000000 pyft-0.2.1/src/main.rs
--rw-r--r--   0      501       20    10831 2024-05-28 21:58:01.000000 pyft-0.2.1/src/nucleosomes.rs
--rw-r--r--   0      501       20     8816 2024-04-11 16:00:15.000000 pyft-0.2.1/src/pileup.rs
--rw-r--r--   0      501       20    18287 2024-03-20 02:07:03.000000 pyft-0.2.1/src/predict_m6a/mod.rs
--rw-r--r--   0      501       20     1051 2023-10-29 16:36:23.000000 pyft-0.2.1/src/strip_basemods.rs
--rw-r--r--   0      501       20     2220 2023-12-09 03:44:15.000000 pyft-0.2.1/src/unused-code/sorted_write.rs
--rw-r--r--   0      501       20     2064 2024-01-13 04:25:34.000000 pyft-0.2.1/tests/extract_test.rs
--rw-r--r--   0      501       20     2050 2024-03-20 02:07:03.000000 pyft-0.2.1/tests/m6a_prediction_test.rs
--rw-r--r--   0      501       20     2651 2024-03-20 02:27:40.000000 pyft-0.2.1/tests/run_test.rs
--rwxr-xr-x   0      501       20     1178 2023-12-09 04:09:55.000000 pyft-0.2.1/tests/test-decorator.sh
--rw-r--r--   0      501       20   648359 2024-05-28 10:54:28.000000 pyft-0.2.1/view.bam
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 pyft-0.2.1/py-ft/Cargo.toml
--rw-r--r--   0      501       20     2807 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/.github/workflows/CI.yml
--rw-r--r--   0      501       20      692 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/.gitignore
--rw-r--r--   0      501       20      341 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/DEV-NOTES.md
--rw-r--r--   0      501       20      396 2024-03-21 03:14:56.000000 pyft-0.2.1/py-ft/README.md
--rw-r--r--   0      501       20      634 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/docs/Makefile
--rw-r--r--   0      501       20     2216 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/docs/_static/css/rtd_dark.css
--rw-r--r--   0      501       20   160734 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/docs/_static/img/fiber_tools_grey.png
--rw-r--r--   0      501       20      294 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/docs/_templates/layout.html
--rw-r--r--   0      501       20      241 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/docs/api.rst
--rw-r--r--   0      501       20     1808 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/docs/conf.py
--rw-r--r--   0      501       20       76 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/docs/environment.yml
--rw-r--r--   0      501       20     1052 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/docs/index.rst
--rw-r--r--   0      501       20      800 2023-07-30 04:16:53.000000 pyft-0.2.1/py-ft/docs/make.bat
--rw-r--r--   0      501       20      180 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/docs/requirements.txt
--rw-r--r--   0      501       20    17851 2024-05-28 23:34:48.000000 pyft-0.2.1/py-ft/docs/vignettes/basic-usage-examples.ipynb
--rw-r--r--   0      501       20 13807746 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/docs/vignettes/centered-plot.ipynb
--rw-r--r--   0      501       20      162 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/docs/vignettes/index.rst
--rw-r--r--   0      501       20      177 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/python/pyft/__init__.py
--rw-r--r--   0      501       20     6249 2024-05-28 22:45:00.000000 pyft-0.2.1/py-ft/python/pyft/plot.py
--rw-r--r--   0      501       20     7310 2024-03-13 02:37:48.000000 pyft-0.2.1/py-ft/python/pyft/utils.py
--rw-r--r--   0      501       20    14290 2024-05-28 23:39:19.000000 pyft-0.2.1/py-ft/src/fiberdata.rs
--rw-r--r--   0      501       20      746 2024-01-11 21:55:03.000000 pyft-0.2.1/py-ft/src/lib.rs
--rw-r--r--   0      501       20   116437 2024-05-28 23:40:08.000000 pyft-0.2.1/py-ft/Cargo.lock
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 pyft-0.2.1/pyproject.toml
--rw-r--r--   0      501       20     6249 2024-05-28 22:45:00.000000 pyft-0.2.1/python/pyft/plot.py
--rw-r--r--   0      501       20      177 2024-03-13 02:37:48.000000 pyft-0.2.1/python/pyft/__init__.py
--rw-r--r--   0      501       20     7310 2024-03-13 02:37:48.000000 pyft-0.2.1/python/pyft/utils.py
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 pyft-0.2.1/PKG-INFO
+-rw-------   0      501       20     2770 2024-05-31 18:34:01.000000 pyft-0.2.2/Cargo.toml
+-rw-r--r--   0      501       20      428 2024-03-21 19:08:49.000000 pyft-0.2.2/.cargo/config.toml
+-rw-r--r--   0      501       20      284 2023-10-20 17:58:19.000000 pyft-0.2.2/.dockerignore
+-rw-r--r--   0      501       20       29 2024-03-18 17:54:48.000000 pyft-0.2.2/.gitattributes
+-rw-r--r--   0      501       20      468 2023-10-30 21:58:54.000000 pyft-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      433 2024-03-21 20:39:06.000000 pyft-0.2.2/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0      501       20     1181 2024-01-11 23:03:28.000000 pyft-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0      501       20    11301 2024-04-09 21:26:17.000000 pyft-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0      501       20      261 2024-01-24 15:42:11.000000 pyft-0.2.2/.gitignore
+-rw-r--r--   0      501       20      475 2023-07-30 04:16:53.000000 pyft-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      376 2024-05-31 18:32:10.000000 pyft-0.2.2/.readthedocs.yaml
+-rw-------   0      501       20   188717 2024-03-21 20:40:43.000000 pyft-0.2.2/CHANGELOG.md
+-rw-r--r--   0      501       20      571 2024-03-21 20:39:06.000000 pyft-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0      501       20   115889 2024-05-31 18:34:03.000000 pyft-0.2.2/Cargo.lock
+-rw-r--r--   0      501       20      863 2023-10-24 18:55:03.000000 pyft-0.2.2/Dockerfile
+-rw-r--r--   0      501       20     1519 2024-03-13 02:37:48.000000 pyft-0.2.2/INSTALL.md
+-rw-r--r--   0      501       20      296 2024-03-20 16:43:55.000000 pyft-0.2.2/NOTES.md
+-rw-r--r--   0      501       20     3522 2024-03-21 20:39:06.000000 pyft-0.2.2/README.md
+-rw-r--r--   0      501       20      297 2023-07-30 04:16:53.000000 pyft-0.2.2/_config.yml
+-rw-r--r--   0      501       20   670134 2023-07-30 04:16:53.000000 pyft-0.2.2/assets/img/center.png
+-rw-r--r--   0      501       20   160734 2023-07-30 04:16:53.000000 pyft-0.2.2/assets/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20   159267 2023-07-30 04:16:53.000000 pyft-0.2.2/assets/img/fiber_tools_teal.png
+-rw-r--r--   0      501       20   220557 2023-07-30 04:16:53.000000 pyft-0.2.2/assets/img/ft-extract-all.png
+-rw-r--r--   0      501       20   303252 2023-07-30 04:16:53.000000 pyft-0.2.2/assets/img/logo.png
+-rw-r--r--   0      501       20     1020 2024-03-21 20:39:06.000000 pyft-0.2.2/build.rs
+-rw-r--r--   0      501       20     3421 2023-10-08 04:44:35.000000 pyft-0.2.2/docs/center.md
+-rw-r--r--   0      501       20     4687 2024-05-28 15:22:42.000000 pyft-0.2.2/docs/extract.md
+-rw-r--r--   0      501       20     2976 2024-03-20 02:07:03.000000 pyft-0.2.2/docs/footprint.md
+-rw-r--r--   0      501       20     1322 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft--help.md
+-rw-r--r--   0      501       20     1273 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-add-nucleosomes-help.md
+-rw-r--r--   0      501       20     1794 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-center-help.md
+-rw-r--r--   0      501       20      489 2024-03-21 03:21:43.000000 pyft-0.2.2/docs/ft-clear-kinetics-help.md
+-rw-r--r--   0      501       20     1519 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-extract-help.md
+-rw-r--r--   0      501       20     2401 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-fire-help.md
+-rw-r--r--   0      501       20      677 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-footprint-help.md
+-rw-r--r--   0      501       20     1883 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-predict-m6a-help.md
+-rw-r--r--   0      501       20      601 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/ft-strip-basemods-help.md
+-rw-r--r--   0      501       20      744 2024-03-21 03:21:47.000000 pyft-0.2.2/docs/ft-track-decorators-help.md
+-rwxr-xr-x   0      501       20      451 2024-03-21 20:39:06.000000 pyft-0.2.2/docs/make_help_docs.sh
+-rw-r--r--   0      501       20      294 2023-07-30 04:16:53.000000 pyft-0.2.2/env.yaml
+-rw-r--r--   0      501       20     5008 2023-07-30 04:16:53.000000 pyft-0.2.2/models/2.0_semi_torch.json
+-rw-r--r--   0      501       20     8502 2023-07-30 04:16:53.000000 pyft-0.2.2/models/2.2_semi_torch.json
+-rw-r--r--   0      501       20    15472 2023-07-30 04:16:53.000000 pyft-0.2.2/models/3.2_semi_torch.json
+-rw-r--r--   0      501       20    69919 2023-12-02 03:58:23.000000 pyft-0.2.2/models/FIRE.conf.json
+-rw-r--r--   0      501       20  1458572 2023-12-02 03:58:23.000000 pyft-0.2.2/models/FIRE.gbdt.json
+-rw-r--r--   0      501       20     4491 2023-07-30 04:16:53.000000 pyft-0.2.2/models/Revio_semi_torch.json
+-rwxr-xr-x   0      501       20      646 2024-03-20 02:07:03.000000 pyft-0.2.2/models/convert-pt-to-onnx.py
+-rw-r--r--   0      501       20    10587 2024-01-13 04:25:34.000000 pyft-0.2.2/src/bamlift/mod.rs
+-rw-r--r--   0      501       20     9600 2024-03-13 02:37:48.000000 pyft-0.2.2/src/bamranges.rs
+-rw-r--r--   0      501       20    12549 2024-01-13 04:25:34.000000 pyft-0.2.2/src/basemods/mod.rs
+-rw-r--r--   0      501       20    12683 2024-03-21 20:39:06.000000 pyft-0.2.2/src/bio_io/mod.rs
+-rw-r--r--   0      501       20    13751 2024-01-14 06:01:13.000000 pyft-0.2.2/src/center.rs
+-rw-r--r--   0      501       20    15855 2024-05-30 21:32:49.000000 pyft-0.2.2/src/cli.rs
+-rw-r--r--   0      501       20     6758 2024-01-12 01:45:18.000000 pyft-0.2.2/src/decorator.rs
+-rw-r--r--   0      501       20     4583 2024-03-20 02:07:03.000000 pyft-0.2.2/src/extract.rs
+-rw-r--r--   0      501       20    17639 2024-05-31 18:40:20.000000 pyft-0.2.2/src/fiber.rs
+-rw-r--r--   0      501       20    22122 2024-03-13 02:37:48.000000 pyft-0.2.2/src/fire.rs
+-rw-r--r--   0      501       20    11686 2024-03-13 02:37:48.000000 pyft-0.2.2/src/footprint.rs
+-rw-r--r--   0      501       20     4301 2024-05-30 04:24:13.000000 pyft-0.2.2/src/lib.rs
+-rw-r--r--   0      501       20     3848 2024-03-26 15:13:17.000000 pyft-0.2.2/src/m6a_burn/mod.rs
+-rw-r--r--   0      501       20    57302 2024-03-20 02:07:03.000000 pyft-0.2.2/src/m6a_burn/revio.onnx
+-rw-r--r--   0      501       20    51494 2024-03-20 02:07:03.000000 pyft-0.2.2/src/m6a_burn/three_two.onnx
+-rw-r--r--   0      501       20    51671 2024-03-20 02:07:03.000000 pyft-0.2.2/src/m6a_burn/two_two.onnx
+-rw-r--r--   0      501       20    51666 2024-03-20 02:07:03.000000 pyft-0.2.2/src/m6a_burn/two_zero.onnx
+-rw-r--r--   0      501       20     5151 2024-04-11 16:00:05.000000 pyft-0.2.2/src/main.rs
+-rw-r--r--   0      501       20    10699 2024-05-30 01:44:27.000000 pyft-0.2.2/src/nucleosomes.rs
+-rw-r--r--   0      501       20    12826 2024-05-30 21:42:27.000000 pyft-0.2.2/src/pileup.rs
+-rw-r--r--   0      501       20    18287 2024-03-20 02:07:03.000000 pyft-0.2.2/src/predict_m6a/mod.rs
+-rw-r--r--   0      501       20     1051 2023-10-29 16:36:23.000000 pyft-0.2.2/src/strip_basemods.rs
+-rw-r--r--   0      501       20     2220 2023-12-09 03:44:15.000000 pyft-0.2.2/src/unused-code/sorted_write.rs
+-rw-r--r--   0      501       20     2064 2024-01-13 04:25:34.000000 pyft-0.2.2/tests/extract_test.rs
+-rw-r--r--   0      501       20     2032 2024-05-30 22:27:18.000000 pyft-0.2.2/tests/m6a_prediction_test.rs
+-rw-r--r--   0      501       20     2651 2024-03-20 02:27:40.000000 pyft-0.2.2/tests/run_test.rs
+-rwxr-xr-x   0      501       20     1178 2023-12-09 04:09:55.000000 pyft-0.2.2/tests/test-decorator.sh
+-rw-r--r--   0      501       20   648359 2024-05-28 10:54:28.000000 pyft-0.2.2/view.bam
+-rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 pyft-0.2.2/py-ft/Cargo.toml
+-rw-r--r--   0      501       20     2807 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      692 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/.gitignore
+-rw-r--r--   0      501       20      341 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/DEV-NOTES.md
+-rw-r--r--   0      501       20      396 2024-03-21 03:14:56.000000 pyft-0.2.2/py-ft/README.md
+-rw-r--r--   0      501       20      634 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/docs/Makefile
+-rw-r--r--   0      501       20     2216 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/docs/_static/css/rtd_dark.css
+-rw-r--r--   0      501       20   160734 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/docs/_static/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20      294 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/docs/_templates/layout.html
+-rw-r--r--   0      501       20      241 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/docs/api.rst
+-rw-r--r--   0      501       20     1808 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/docs/conf.py
+-rw-r--r--   0      501       20       76 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/docs/environment.yml
+-rw-r--r--   0      501       20     1052 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-07-30 04:16:53.000000 pyft-0.2.2/py-ft/docs/make.bat
+-rw-r--r--   0      501       20      180 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/docs/requirements.txt
+-rw-r--r--   0      501       20    17851 2024-05-28 23:34:48.000000 pyft-0.2.2/py-ft/docs/vignettes/basic-usage-examples.ipynb
+-rw-r--r--   0      501       20 13807746 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/docs/vignettes/centered-plot.ipynb
+-rw-r--r--   0      501       20      162 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/docs/vignettes/index.rst
+-rw-r--r--   0      501       20      177 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/python/pyft/__init__.py
+-rw-r--r--   0      501       20     6249 2024-05-28 22:45:00.000000 pyft-0.2.2/py-ft/python/pyft/plot.py
+-rw-r--r--   0      501       20     7310 2024-03-13 02:37:48.000000 pyft-0.2.2/py-ft/python/pyft/utils.py
+-rw-r--r--   0      501       20    14673 2024-05-31 18:51:00.000000 pyft-0.2.2/py-ft/src/fiberdata.rs
+-rw-r--r--   0      501       20      746 2024-01-11 21:55:03.000000 pyft-0.2.2/py-ft/src/lib.rs
+-rw-r--r--   0      501       20   116437 2024-05-31 18:50:40.000000 pyft-0.2.2/py-ft/Cargo.lock
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 pyft-0.2.2/pyproject.toml
+-rw-r--r--   0      501       20     6249 2024-05-28 22:45:00.000000 pyft-0.2.2/python/pyft/plot.py
+-rw-r--r--   0      501       20      177 2024-03-13 02:37:48.000000 pyft-0.2.2/python/pyft/__init__.py
+-rw-r--r--   0      501       20     7310 2024-03-13 02:37:48.000000 pyft-0.2.2/python/pyft/utils.py
+-rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 pyft-0.2.2/PKG-INFO
```

### Comparing `pyft-0.2.1/Cargo.toml` & `pyft-0.2.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 edition = "2021"
 homepage = "https://fiberseq.github.io/fibertools-rs/"
 keywords = ["cli", "bam", "bfx"]
 license = "MIT"
 name = "fibertools-rs"
 readme = "README.md"
 repository = "https://github.com/fiberseq/fibertools-rs"
-version = "0.4.2"
+version = "0.4.3"
 # exclude py-ft and test data from cargo publish since they are too large
 exclude = ["py-ft/", "tests/data/"]
 
 [workspace]
 exclude = ["py-ft"]
 
 [[bin]]
@@ -35,15 +35,16 @@
 indicatif = {version = "0.17.7", features = ["rayon"]}
 itertools = "0.10.5"
 lazy_static = "1.4.0"
 log = "0.4"
 ordered-float = "3.4.0"
 rayon = "1.8"
 regex = "1.9.1"
-rust-htslib = "0.43"
+rust-htslib = "0.43.0"
+
 serde = {version = "1.0.104", features = ["derive"], optional = false}
 serde_json = {version = "1.0.48", optional = false}
 serde_yaml = "0.9"
 spin = "0.9.8"
 tch = {version = "0.15.0", optional = true}
 tempfile = "3.3.0"
 derive_builder = "0.12.0"
```

### Comparing `pyft-0.2.1/.github/workflows/CI.yml` & `pyft-0.2.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/.github/workflows/release.yml` & `pyft-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/CHANGELOG.md` & `pyft-0.2.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/CONTRIBUTING.md` & `pyft-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/Cargo.lock` & `pyft-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1383,15 +1383,15 @@
 name = "feature-probe"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "835a3dc7d1ec9e75e2b5fb4ba75396837112d2060b03f7d43bc1897c7f7211da"
 
 [[package]]
 name = "fibertools-rs"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "anstyle",
  "anyhow",
  "assert_cmd",
  "bio",
  "burn",
  "burn-import",
@@ -2007,17 +2007,17 @@
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "hts-sys"
-version = "2.1.1"
+version = "2.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deebfb779c734d542e7f14c298597914b9b5425e4089aef482eacb5cab941915"
+checksum = "e9f348d14cb4e50444e39fcd6b00302fe2ed2bc88094142f6278391d349a386d"
 dependencies = [
  "bzip2-sys",
  "cc",
  "curl-sys",
  "fs-utils",
  "glob",
  "libz-sys",
```

### Comparing `pyft-0.2.1/Dockerfile` & `pyft-0.2.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/INSTALL.md` & `pyft-0.2.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/README.md` & `pyft-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/assets/img/center.png` & `pyft-0.2.2/assets/img/center.png`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/assets/img/fiber_tools_grey.png` & `pyft-0.2.2/assets/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/assets/img/fiber_tools_teal.png` & `pyft-0.2.2/assets/img/fiber_tools_teal.png`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/assets/img/ft-extract-all.png` & `pyft-0.2.2/assets/img/ft-extract-all.png`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/assets/img/logo.png` & `pyft-0.2.2/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/build.rs` & `pyft-0.2.2/build.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/center.md` & `pyft-0.2.2/docs/center.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/extract.md` & `pyft-0.2.2/docs/extract.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/footprint.md` & `pyft-0.2.2/docs/footprint.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft--help.md` & `pyft-0.2.2/docs/ft--help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-add-nucleosomes-help.md` & `pyft-0.2.2/docs/ft-add-nucleosomes-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-center-help.md` & `pyft-0.2.2/docs/ft-center-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-extract-help.md` & `pyft-0.2.2/docs/ft-extract-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-fire-help.md` & `pyft-0.2.2/docs/ft-fire-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-footprint-help.md` & `pyft-0.2.2/docs/ft-footprint-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-predict-m6a-help.md` & `pyft-0.2.2/docs/ft-predict-m6a-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-strip-basemods-help.md` & `pyft-0.2.2/docs/ft-strip-basemods-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/docs/ft-track-decorators-help.md` & `pyft-0.2.2/docs/ft-track-decorators-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/2.0_semi_torch.json` & `pyft-0.2.2/models/2.0_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/2.2_semi_torch.json` & `pyft-0.2.2/models/2.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/3.2_semi_torch.json` & `pyft-0.2.2/models/3.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/FIRE.conf.json` & `pyft-0.2.2/models/FIRE.conf.json`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/FIRE.gbdt.json` & `pyft-0.2.2/models/FIRE.gbdt.json`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/Revio_semi_torch.json` & `pyft-0.2.2/models/Revio_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/models/convert-pt-to-onnx.py` & `pyft-0.2.2/models/convert-pt-to-onnx.py`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/bamlift/mod.rs` & `pyft-0.2.2/src/bamlift/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/bamranges.rs` & `pyft-0.2.2/src/bamranges.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/basemods/mod.rs` & `pyft-0.2.2/src/basemods/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/bio_io/mod.rs` & `pyft-0.2.2/src/bio_io/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/center.rs` & `pyft-0.2.2/src/center.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/cli.rs` & `pyft-0.2.2/src/cli.rs`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     ///  See https://fiberseq.github.io/fibertools-rs/docs/center.html for a description of the output.
     #[clap(visible_aliases = &["c", "ct"])]
     Center(CenterOptions),
     /// Infer footprints from fiberseq data
     Footprint(FootprintOptions),
     /// Make decorated bed files for fiberseq data
     TrackDecorators(DecoratorOptions),
-    /// make a pileup track from a FIRE bam
+    /// Make a pileup track of Fiber-seq features from a FIRE bam
     Pileup(PileupOptions),
     /// Remove HiFi kinetics tags from the input bam file
     ClearKinetics(ClearKineticsOptions),
     /// Strip out select base modifications
     StripBasemods(StripBasemodsOptions),
     /// Make command line completions
     #[clap(hide = true)]
@@ -399,11 +399,23 @@
     /// Region string to make a pileup of.
     /// If not provided will make a pileup of the whole genome
     #[clap(default_value = None)]
     pub rgn: Option<String>,
     /// Output file
     #[clap(short, long, default_value = "-")]
     pub out: String,
+    /// include m6A calls
+    #[clap(short, long)]
+    pub m6a: bool,
+    /// include 5mC calls
+    #[clap(short, long)]
+    pub cpg: bool,
+    /// For each column add two new columns with the hap1 and hap2 specific data.
+    #[clap(short, long)]
+    pub haps: bool,
     /// Keep zero coverage regions
     #[clap(short, long)]
     pub keep_zeros: bool,
+    /// Write output one base at a time even if the values do not change
+    #[clap(short, long)]
+    pub per_base: bool,
 }
```

### Comparing `pyft-0.2.1/src/decorator.rs` & `pyft-0.2.2/src/decorator.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/extract.rs` & `pyft-0.2.2/src/extract.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/fiber.rs` & `pyft-0.2.2/src/fiber.rs`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,17 @@
             target_name,
             rg,
             center_position: None,
         }
     }
 
     pub fn dict_from_head_view(head_view: &HeaderView) -> HashMap<i32, String> {
+        if head_view.target_count() == 0 {
+            return HashMap::new();
+        }
         let target_u8s = head_view.target_names();
         let tids = target_u8s
             .iter()
             .map(|t| head_view.tid(t).expect("Unable to get tid"));
         let target_names = target_u8s
             .iter()
             .map(|&a| String::from_utf8_lossy(a).to_string());
```

### Comparing `pyft-0.2.1/src/fire.rs` & `pyft-0.2.2/src/fire.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/footprint.rs` & `pyft-0.2.2/src/footprint.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/lib.rs` & `pyft-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/m6a_burn/mod.rs` & `pyft-0.2.2/src/m6a_burn/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/m6a_burn/revio.onnx` & `pyft-0.2.2/src/m6a_burn/revio.onnx`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/m6a_burn/three_two.onnx` & `pyft-0.2.2/src/m6a_burn/three_two.onnx`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/m6a_burn/two_two.onnx` & `pyft-0.2.2/src/m6a_burn/two_two.onnx`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/m6a_burn/two_zero.onnx` & `pyft-0.2.2/src/m6a_burn/two_zero.onnx`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/main.rs` & `pyft-0.2.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/nucleosomes.rs` & `pyft-0.2.2/src/nucleosomes.rs`

 * *Files 0% similar despite different names*

```diff
@@ -228,19 +228,14 @@
     }
 }
 
 pub fn add_nucleosomes_to_bam(nuc_opts: &AddNucleosomeOptions, threads: usize) {
     let mut bam = bam_reader(&nuc_opts.bam, threads);
     let mut out = bam_writer(&nuc_opts.out, &bam, threads);
 
-    log::info!(
-        "Adding nucleosomes to bam file using m6a with an ML of at least {}",
-        nuc_opts.min_ml_score
-    );
-
     // read in bam data
     let bam_chunk_iter = BamChunk::new(bam.records(), None);
 
     // iterate over chunks
     for mut chunk in bam_chunk_iter {
         // add nuc calls
         let records: Vec<&mut Record> = chunk
```

### Comparing `pyft-0.2.1/src/pileup.rs` & `pyft-0.2.2/src/pileup.rs`

 * *Files 26% similar despite different names*

```diff
@@ -10,40 +10,70 @@
 /// This module is used to extract the fire calls as well as nucs and msps from a bam file
 /// for every position in the bam file and output the results to a bed file.
 /// all calculations are done in total as well as for haplotype 1 and haplotype 2.
 
 const MIN_FIRE_COVERAGE: i32 = 4;
 const MIN_FIRE_QUAL: u8 = 229; // floor(255*0.9)
 
-pub struct FireTrack {
+#[derive(Debug, PartialEq)]
+pub struct FireRow<'a> {
+    pub coverage: &'a i32,
+    pub fire_coverage: &'a i32,
+    pub score: &'a f32,
+    pub nuc_coverage: &'a i32,
+    pub msp_coverage: &'a i32,
+    pub cpg_coverage: &'a i32,
+    pub m6a_coverage: &'a i32,
+    pileup_opts: &'a PileupOptions,
+}
+
+impl std::fmt::Display for FireRow<'_> {
+    fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
+        let mut rtn = format!(
+            "\t{}\t{}\t{}\t{}\t{}",
+            self.coverage, self.fire_coverage, self.score, self.nuc_coverage, self.msp_coverage
+        );
+        if self.pileup_opts.m6a {
+            rtn += &format!("\t{}", self.m6a_coverage);
+        }
+        if self.pileup_opts.cpg {
+            rtn += &format!("\t{}", self.cpg_coverage);
+        }
+        write!(f, "{}", rtn)
+    }
+}
+
+pub struct FireTrack<'a> {
     pub chrom_len: usize,
     pub raw_scores: Vec<f32>,
     pub scores: Vec<f32>,
     pub coverage: Vec<i32>,
     pub fire_coverage: Vec<i32>,
     pub msp_coverage: Vec<i32>,
     pub nuc_coverage: Vec<i32>,
     pub cpg_coverage: Vec<i32>,
     pub m6a_coverage: Vec<i32>,
+    pileup_opts: &'a PileupOptions,
 }
 
-impl FireTrack {
-    pub fn new(chrom_len: usize) -> Self {
+impl<'a> FireTrack<'a> {
+    pub fn new(chrom_len: usize, pileup_opts: &'a PileupOptions) -> Self {
         let raw_scores = vec![-1.0; chrom_len];
         let scores = vec![-1.0; chrom_len];
         Self {
             chrom_len,
             raw_scores,
             scores,
             coverage: vec![0; chrom_len],
             fire_coverage: vec![0; chrom_len],
             msp_coverage: vec![0; chrom_len],
             nuc_coverage: vec![0; chrom_len],
             cpg_coverage: vec![0; chrom_len],
             m6a_coverage: vec![0; chrom_len],
+            pileup_opts,
         }
     }
 
     #[inline]
     fn add_range_set(array: &mut [i32], ranges: &super::bamranges::Ranges) {
         let shuffle_offset = 0;
         for (_, _, _, _, r) in ranges {
@@ -83,46 +113,64 @@
                         self.fire_coverage[i] += 1;
                         self.raw_scores[i] += score_update;
                     }
                 }
                 _ => continue,
             }
         }
+
         Self::add_range_set(&mut self.nuc_coverage, &fiber.nuc);
         Self::add_range_set(&mut self.msp_coverage, &fiber.msp);
-        Self::add_range_set(&mut self.m6a_coverage, &fiber.m6a);
-        Self::add_range_set(&mut self.cpg_coverage, &fiber.cpg);
+        if self.pileup_opts.m6a {
+            Self::add_range_set(&mut self.m6a_coverage, &fiber.m6a);
+        }
+        if self.pileup_opts.cpg {
+            Self::add_range_set(&mut self.cpg_coverage, &fiber.cpg);
+        }
     }
 
     pub fn calculate_scores(&mut self) {
         for i in 0..self.chrom_len {
             if self.fire_coverage[i] < MIN_FIRE_COVERAGE {
                 self.scores[i] = -1.0;
             } else {
                 self.scores[i] = self.raw_scores[i] / self.coverage[i] as f32;
             }
         }
     }
+
+    pub fn row(&self, i: usize) -> FireRow {
+        FireRow {
+            score: &self.scores[i],
+            coverage: &self.coverage[i],
+            fire_coverage: &self.fire_coverage[i],
+            msp_coverage: &self.msp_coverage[i],
+            nuc_coverage: &self.nuc_coverage[i],
+            cpg_coverage: &self.cpg_coverage[i],
+            m6a_coverage: &self.m6a_coverage[i],
+            pileup_opts: self.pileup_opts,
+        }
+    }
 }
 
 pub struct FiberseqPileup<'a> {
-    pub all_data: FireTrack,
-    pub hap1_data: FireTrack,
-    pub hap2_data: FireTrack,
+    pub all_data: FireTrack<'a>,
+    pub hap1_data: FireTrack<'a>,
+    pub hap2_data: FireTrack<'a>,
     pub chrom: String,
     pub chrom_len: usize,
     has_data: bool,
     pileup_opts: &'a PileupOptions,
 }
 
 impl<'a> FiberseqPileup<'a> {
     pub fn new(chrom: &str, chrom_len: usize, pileup_opts: &'a PileupOptions) -> Self {
-        let all_data = FireTrack::new(chrom_len);
-        let hap1_data = FireTrack::new(chrom_len);
-        let hap2_data = FireTrack::new(chrom_len);
+        let all_data = FireTrack::new(chrom_len, pileup_opts);
+        let hap1_data = FireTrack::new(chrom_len, pileup_opts);
+        let hap2_data = FireTrack::new(chrom_len, pileup_opts);
         Self {
             all_data,
             hap1_data,
             hap2_data,
             chrom: chrom.to_string(),
             chrom_len,
             has_data: false,
@@ -132,15 +180,15 @@
 
     pub fn has_data(&self) -> bool {
         self.has_data
     }
 
     pub fn add_records(
         &mut self,
-        records: bam::Records<'a, IndexedReader>,
+        records: std::iter::Peekable<bam::Records<'a, IndexedReader>>,
     ) -> Result<(), anyhow::Error> {
         records
             .map(|r| r.unwrap())
             .filter(|r| !(r.is_secondary() || r.is_supplementary() || r.is_unmapped()))
             .chunks(1000)
             .into_iter()
             .map(|r| r.collect::<Vec<_>>())
@@ -150,103 +198,175 @@
                     .map(|r| FiberseqData::new(r.clone(), None, 0))
                     .collect();
                 if !fibers.is_empty() {
                     self.has_data = true;
                 }
                 for fiber in fibers {
                     self.all_data.update_with_fiber(&fiber);
-                    if fiber.get_hp() == "H1" {
+                    if fiber.get_hp() == "H1" && self.pileup_opts.haps {
                         self.hap1_data.update_with_fiber(&fiber);
-                    } else if fiber.get_hp() == "H2" {
+                    } else if fiber.get_hp() == "H2" && self.pileup_opts.haps {
                         self.hap2_data.update_with_fiber(&fiber);
                     }
                 }
             });
+        self.calculate_scores();
         Ok(())
     }
 
-    pub fn header() -> String {
-        format!(
-            "{}\t{}\t{}\t{}\n",
-            "#chrom\tpos",
-            "coverage\tfire_coverage\tscore\tnuc_coverage\tmsp_coverage\tm6a_coverage\tcpg_coverage",
-            "coverage_H1\tfire_coverage_H1\tscore_H1\tnuc_coverage_H1\tmsp_coverage_H1\tm6a_coverage_H1\tcpg_coverage_H1",
-            "coverage_H2\tfire_coverage_H2\tscore_H2\tnuc_coverage_H2\tmsp_coverage_H2\tm6a_coverage_H2\tcpg_coverage_H2",
-        )
+    pub fn header(pileup_opts: &PileupOptions) -> String {
+        let mut header = format!("{}\t{}\t{}", "#chrom", "start", "end");
+
+        let haps = if pileup_opts.haps {
+            vec!["", "_H1", "_H2"]
+        } else {
+            vec![""]
+        };
+        for hap in haps {
+            header += &format!(
+                "\t{}{hap}\t{}{hap}\t{}{hap}\t{}{hap}\t{}{hap}",
+                "coverage", "fire_coverage", "score", "nuc_coverage", "msp_coverage",
+            );
+            if pileup_opts.m6a {
+                header += &format!("\t{}{hap}", "m6a_coverage");
+            }
+            if pileup_opts.cpg {
+                header += &format!("\t{}{hap}", "cpg_coverage");
+            }
+        }
+        header += "\n";
+        header
     }
 
-    pub fn calculate_scores(&mut self) {
+    fn calculate_scores(&mut self) {
         self.all_data.calculate_scores();
         self.hap1_data.calculate_scores();
         self.hap2_data.calculate_scores();
     }
 
+    /// check if the ith row has the same data as the previous row
+    /// if it does, return true, otherwise return false
+    /// this is used to determine if the data should be written to the output
+    pub fn is_same_as_previous(&self, i: usize) -> bool {
+        if i == 0
+            || (self.all_data.row(i) == self.all_data.row(i - 1)
+                && self.hap1_data.row(i) == self.hap1_data.row(i - 1)
+                && self.hap2_data.row(i) == self.hap2_data.row(i - 1))
+        {
+            return true;
+        }
+        false
+    }
+
+    fn wait_to_write(&self, i: usize) -> bool {
+        // write every row
+        if self.pileup_opts.per_base {
+            return false;
+        }
+        self.is_same_as_previous(i) && i != self.chrom_len - 1
+    }
+
     pub fn write(&self, out: &mut Box<dyn Write>) -> Result<(), anyhow::Error> {
         if !self.has_data {
             return Ok(());
         }
-
+        let mut write_start_index = 0;
+        let mut write_end_index = 0;
         for i in 0..self.chrom_len {
-            if !self.pileup_opts.keep_zeros && self.all_data.coverage[i] == 0 {
+            // do we have the same data as the previous row?
+            if self.wait_to_write(i) {
+                write_end_index = i;
                 continue;
-            }
-            let mut line = format!("{}\t{}\t", self.chrom, i);
-            for data in [&self.all_data, &self.hap1_data, &self.hap2_data] {
-                line += &format!(
-                    "{}\t{}\t{}\t{}\t{}\t{}\t{}\t",
-                    data.coverage[i],
-                    data.fire_coverage[i],
-                    data.scores[i],
-                    data.nuc_coverage[i],
-                    data.msp_coverage[i],
-                    data.m6a_coverage[i],
-                    data.cpg_coverage[i],
+            } else {
+                let mut line = format!(
+                    "{}\t{}\t{}",
+                    self.chrom,
+                    write_start_index,
+                    write_end_index + 1
                 );
+                // add in the data
+                let hap_data = if self.pileup_opts.haps {
+                    vec![&self.all_data, &self.hap1_data, &self.hap2_data]
+                } else {
+                    vec![&self.all_data]
+                };
+                for data in hap_data {
+                    line += data.row(write_start_index).to_string().as_str();
+                }
+                // don't write empty lines unless keep_zeros is set
+                if self.pileup_opts.keep_zeros || self.all_data.coverage[write_start_index] > 0 {
+                    line += "\n";
+                    out.write_all(line.as_bytes())?;
+                }
+                // reset the write indexes
+                write_start_index = i;
+                write_end_index = i;
             }
-            // remove the last tab
-            line.pop();
-            line += "\n";
-
-            out.write_all(line.as_bytes())?;
         }
         out.flush()?;
         Ok(())
     }
 }
 
+/// split up a FetchDefinition into multiple regions of a certain size
+/// TODO set up run_rgn to take a list of regions and multithread it
+pub fn split_fetch_definition(
+    rgn: &FetchDefinition,
+    chrom_len: usize,
+    window_size: usize,
+) -> Vec<(i64, i64)> {
+    let (start, end) = match rgn {
+        FetchDefinition::RegionString(_chrom, start, end) => (*start, *end),
+        _ => (0, chrom_len as i64),
+    };
+    let mut rgns = vec![];
+    let mut cur_start = start;
+    while cur_start < end {
+        let cur_end = std::cmp::min(cur_start + window_size as i64, end);
+        rgns.push((cur_start, cur_end));
+        cur_start = cur_end;
+    }
+    rgns
+}
+
 fn run_rgn(
     chrom: &str,
     rgn: FetchDefinition,
     bam: &mut IndexedReader,
     out: &mut Box<dyn Write>,
     pileup_opts: &PileupOptions,
 ) -> Result<(), anyhow::Error> {
-    log::info!("Processing region: {}", chrom);
     let tid = bam.header().tid(chrom.as_bytes()).unwrap();
     let chrom_len = bam.header().target_len(tid).unwrap() as usize;
+
     bam.fetch(rgn)?;
-    let records = bam.records();
+    let mut records = bam.records().peekable();
+    // skip if there are no records and keep_zeros is not set
+    if records.peek().is_none() && !pileup_opts.keep_zeros {
+        return Ok(());
+    }
     // make the pileup
     let mut pileup = FiberseqPileup::new(chrom, chrom_len, pileup_opts);
+    log::info!("Processing records for {}", chrom);
     pileup.add_records(records)?;
-    pileup.calculate_scores();
+    log::info!("Writing pileup for {}", chrom);
     pileup.write(out)?;
     Ok(())
 }
 
 /// extract existing fire calls into a bed9+ like file
 pub fn pileup_track(pileup_opts: &PileupOptions) -> Result<(), anyhow::Error> {
     // read in the bam from stdin or from a file
     let mut bam = bam::IndexedReader::from_path(pileup_opts.bam.clone())?;
     let header = bam.header().clone();
     bam.set_threads(8).unwrap();
 
     let mut out = bio_io::writer(&pileup_opts.out)?;
     // add the header
-    out.write_all(FiberseqPileup::header().as_bytes())?;
+    out.write_all(FiberseqPileup::header(pileup_opts).as_bytes())?;
 
     match &pileup_opts.rgn {
         // if a region is specified, only process that region
         Some(rgn) => {
             let (rgn, chrom) = region_parser(rgn);
             run_rgn(&chrom, rgn, &mut bam, &mut out, pileup_opts)?;
         }
```

### Comparing `pyft-0.2.1/src/predict_m6a/mod.rs` & `pyft-0.2.2/src/predict_m6a/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/strip_basemods.rs` & `pyft-0.2.2/src/strip_basemods.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/src/unused-code/sorted_write.rs` & `pyft-0.2.2/src/unused-code/sorted_write.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/tests/extract_test.rs` & `pyft-0.2.2/tests/extract_test.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/tests/m6a_prediction_test.rs` & `pyft-0.2.2/tests/m6a_prediction_test.rs`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         sum += fiber
             .m6a
             .qual
             .into_iter()
             .map(|x| x as usize)
             .sum::<usize>();
     }
+    eprintln!("sum {:?}", sum);
     // now count for the input bam file as well
     sum
 }
 
 fn run_prediction_and_count_qual(inbam: String) -> usize {
     let named_tmp_bam_out = NamedTempFile::new().unwrap();
     let out_str = named_tmp_bam_out.path().to_str().unwrap();
@@ -32,29 +33,36 @@
     }
 
     // read in the output bam and check the sum of the quality scores
     let mut predicted_bam = bio_io::bam_reader(out_str, 1);
     sum_qual(&mut predicted_bam)
 }
 
-/// This function predicts m6A for all the fibers in a the test bam file and test the sum of their quality scores against the expected value.
+fn run_comparison(file: &str) {
+    let files = vec![file];
+    eprintln!("{:?}", files);
+    let results_before_this_predict = sum_qual(&mut bio_io::bam_reader(file, 1));
+    eprintln!("{:?}", results_before_this_predict);
+    let results = run_prediction_and_count_qual(file.to_string());
+    eprintln!("{:?}", results);
+    assert_eq!(results, results_before_this_predict);
+}
+
 #[test]
-fn test_m6a_prediction() {
-    let files = vec![
-        "tests/data/all.bam",       // tests 2.0 chemistry
-        "tests/data/two_two.bam",   // tests 2.2 chemistry
-        "tests/data/three_two.bam", // tests 3.2 chemistry
-        "tests/data/revio.bam",     // tests revio chemistry
-    ];
-
-    let results_before_this_predict = files
-        .iter()
-        .map(|x| sum_qual(&mut bio_io::bam_reader(x, 1)))
-        .collect::<Vec<usize>>();
-
-    let results: Vec<usize> = files
-        .iter()
-        .map(|x| run_prediction_and_count_qual(x.to_string()))
-        .collect();
+fn test_two_zero_prediction() {
+    run_comparison("tests/data/all.bam");
+}
 
-    assert_eq!(results, results_before_this_predict);
+#[test]
+fn test_two_two_m6a_prediction() {
+    run_comparison("tests/data/two_two.bam");
+}
+
+#[test]
+fn test_three_two_m6a_prediction() {
+    run_comparison("tests/data/three_two.bam");
+}
+
+#[test]
+fn test_revio_m6a_prediction() {
+    run_comparison("tests/data/revio.bam");
 }
```

### Comparing `pyft-0.2.1/tests/run_test.rs` & `pyft-0.2.2/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/tests/test-decorator.sh` & `pyft-0.2.2/tests/test-decorator.sh`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/view.bam` & `pyft-0.2.2/view.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/.github/workflows/CI.yml` & `pyft-0.2.2/py-ft/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/.gitignore` & `pyft-0.2.2/py-ft/.gitignore`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/Makefile` & `pyft-0.2.2/py-ft/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/_static/css/rtd_dark.css` & `pyft-0.2.2/py-ft/docs/_static/css/rtd_dark.css`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/_static/img/fiber_tools_grey.png` & `pyft-0.2.2/py-ft/docs/_static/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/conf.py` & `pyft-0.2.2/py-ft/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/index.rst` & `pyft-0.2.2/py-ft/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/make.bat` & `pyft-0.2.2/py-ft/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/vignettes/basic-usage-examples.ipynb` & `pyft-0.2.2/py-ft/docs/vignettes/basic-usage-examples.ipynb`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/docs/vignettes/centered-plot.ipynb` & `pyft-0.2.2/py-ft/docs/vignettes/centered-plot.ipynb`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/python/pyft/plot.py` & `pyft-0.2.2/py-ft/python/pyft/plot.py`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/python/pyft/utils.py` & `pyft-0.2.2/py-ft/python/pyft/utils.py`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/src/fiberdata.rs` & `pyft-0.2.2/py-ft/src/fiberdata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use fibertools_rs::bamlift;
 //use fibertools_rs::bio_io;
 use fibertools_rs::fiber::FiberseqData;
 use pyo3::iter::IterNextOutput;
 use pyo3::prelude::*;
 use rust_htslib::{bam, bam::ext::BamRecordExtensions, bam::record::Aux, bam::Read};
+use std::collections::HashMap;
 use std::time;
 use std::vec::IntoIter;
 #[pyclass]
 /// Class for fiberseq data. This class corresponds to a single record in the bam file.
 pub struct Fiberdata {
     /// Number of c_s
     #[pyo3(get, set)]
@@ -215,14 +216,15 @@
 
 #[pyclass]
 /// Open a fiberseq bam file. Must have an index.
 pub struct Fiberbam {
     bam: bam::IndexedReader,
     reader: bam::Reader,
     header: bam::Header,
+    target_dict: HashMap<i32, String>,
     start: time::Instant,
 }
 
 /// pure rust functions for Fiberbam
 impl Fiberbam {
     fn _fetch_helper(
         &mut self,
@@ -232,14 +234,16 @@
     ) -> Vec<FiberseqData> {
         let fetch_args = match (start, end) {
             (Some(start), Some(end)) => bam::FetchDefinition::from((chrom, start, end)),
             _ => bam::FetchDefinition::from(chrom),
         };
 
         let head_view = bam::HeaderView::from_header(&self.header);
+        let target_dict = FiberseqData::dict_from_head_view(&head_view);
+
         self.bam.fetch(fetch_args).expect("unable to fetch region");
         let records: Vec<bam::Record> = self.bam.records().map(|r| r.unwrap()).collect();
 
         log::info!(
             "{} records fetched in {:.2}s",
             records.len(),
             self._time_from_last()
@@ -263,19 +267,22 @@
             bam::IndexedReader::from_path(bam_file).expect("unable to open indexed bam file");
         bam.set_threads(threads).unwrap();
 
         let mut reader = bam::Reader::from_path(bam_file).expect("unable to open bam file");
         reader.set_threads(threads).unwrap();
 
         let header = bam::Header::from_template(bam.header());
+        let head_view = bam::HeaderView::from_header(&header);
+        let target_dict = FiberseqData::dict_from_head_view(&head_view);
         let start = time::Instant::now();
         Self {
             bam,
             reader,
             header,
+            target_dict,
             start,
         }
     }
 
     /// Returns an iterator over :class:`~pyft.Fiberdata` objects for the selected region.
     /// Arguments for the region to fetch can be provided in multiple ways, e.g.:
     ///
@@ -320,15 +327,16 @@
     }
 
     fn __next__(&mut self) -> IterNextOutput<Fiberdata, &'static str> {
         let data = self.reader.records().next();
         match data {
             Some(record) => {
                 let record = record.unwrap();
-                let fiber = FiberseqData::new(record, None, 0);
+                let target_name = self.target_dict.get(&record.tid());
+                let fiber = FiberseqData::new(record, target_name, 0);
                 IterNextOutput::Yield(Fiberdata::new(fiber, None))
             }
             None => IterNextOutput::Return("Ended"),
         }
     }
 
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
```

### Comparing `pyft-0.2.1/py-ft/src/lib.rs` & `pyft-0.2.2/py-ft/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/py-ft/Cargo.lock` & `pyft-0.2.2/py-ft/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1358,15 +1358,15 @@
 name = "feature-probe"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "835a3dc7d1ec9e75e2b5fb4ba75396837112d2060b03f7d43bc1897c7f7211da"
 
 [[package]]
 name = "fibertools-rs"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "anstyle",
  "anyhow",
  "bio",
  "burn",
  "burn-import",
  "clap",
@@ -1970,17 +1970,17 @@
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "hts-sys"
-version = "2.1.1"
+version = "2.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deebfb779c734d542e7f14c298597914b9b5425e4089aef482eacb5cab941915"
+checksum = "e9f348d14cb4e50444e39fcd6b00302fe2ed2bc88094142f6278391d349a386d"
 dependencies = [
  "bzip2-sys",
  "cc",
  "curl-sys",
  "fs-utils",
  "glob",
  "libz-sys",
@@ -2975,15 +2975,15 @@
  "libm",
  "num-complex",
  "reborrow",
 ]
 
 [[package]]
 name = "pyft"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "colored",
  "env_logger 0.10.2",
  "fibertools-rs",
  "itertools 0.10.5",
  "lazy_static",
```

### Comparing `pyft-0.2.1/pyproject.toml` & `pyft-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/python/pyft/plot.py` & `pyft-0.2.2/python/pyft/plot.py`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/python/pyft/utils.py` & `pyft-0.2.2/python/pyft/utils.py`

 * *Files identical despite different names*

### Comparing `pyft-0.2.1/PKG-INFO` & `pyft-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyft
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=2.0
 Requires-Dist: altair >=5.0
 Requires-Dist: vegafusion[embed]
 Requires-Dist: tqdm
```

