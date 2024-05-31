# Comparing `tmp/enpt-0.20.1.tar.gz` & `tmp/enpt-0.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enpt-0.20.1.tar", last modified: Tue Mar  5 15:17:53 2024, max compression
+gzip compressed data, was "enpt-0.20.2.tar", last modified: Thu May 30 23:58:31 2024, max compression
```

## Comparing `enpt-0.20.1.tar` & `enpt-0.20.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.618575 enpt-0.20.1/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-03-05 15:16:58.000000 enpt-0.20.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-05 15:16:58.000000 enpt-0.20.1/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.582577 enpt-0.20.1/.github/
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-03-05 15:16:58.000000 enpt-0.20.1/.github/ISSUE_TEMPLATE.md
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-03-05 15:16:58.000000 enpt-0.20.1/.github/create_release_from_gitlab_ci.sh
--rw-rw-rw-   0 root         (0) root         (0)     4079 2024-03-05 15:16:58.000000 enpt-0.20.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3532 2024-03-05 15:16:58.000000 enpt-0.20.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3878 2024-03-05 15:16:58.000000 enpt-0.20.1/.zenodo.json
--rw-rw-rw-   0 root         (0) root         (0)      388 2024-03-05 15:16:58.000000 enpt-0.20.1/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1711 2024-03-05 15:16:58.000000 enpt-0.20.1/CITATION
--rw-rw-rw-   0 root         (0) root         (0)     5492 2024-03-05 15:16:58.000000 enpt-0.20.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    23235 2024-03-05 15:16:58.000000 enpt-0.20.1/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1920 2024-03-05 15:16:58.000000 enpt-0.20.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-03-05 15:16:58.000000 enpt-0.20.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-03-05 15:16:58.000000 enpt-0.20.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     6939 2024-03-05 15:17:53.618575 enpt-0.20.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4447 2024-03-05 15:16:58.000000 enpt-0.20.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.582577 enpt-0.20.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6822 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.574578 enpt-0.20.1/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.574578 enpt-0.20.1/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.590577 enpt-0.20.1/docs/_build/html/_images/
--rw-r--r--   0 root         (0) root         (0)     4068 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/EnPT_Logo_clipped.png
--rw-r--r--   0 root         (0) root         (0)   118594 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/screenshot_enpt_enmapboxapp_v0.7.4.png
--rw-r--r--   0 root         (0) root         (0)    81885 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/tut__contents_l2a_output.png
--rw-r--r--   0 root         (0) root         (0)   105427 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/tut__contents_test_dataset.png
--rw-r--r--   0 root         (0) root         (0)   883240 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l1b_swir.png
--rw-r--r--   0 root         (0) root         (0)   797145 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l1b_vnir.png
--rw-r--r--   0 root         (0) root         (0)   305183 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l1b_vnir_swir_shift_striping.png
--rw-r--r--   0 root         (0) root         (0)   462337 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l2a_output.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.590577 enpt-0.20.1/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)     3314 2024-03-05 15:06:47.000000 enpt-0.20.1/docs/_build/html/_static/EnPT_logo_final_clipped_doubleSize.png
--rw-r--r--   0 root         (0) root         (0)      286 2023-09-13 23:25:39.000000 enpt-0.20.1/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-09-13 23:25:39.000000 enpt-0.20.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-09-13 23:25:39.000000 enpt-0.20.1/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.590577 enpt-0.20.1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/_static/wider_theme.css
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/about.rst
--rw-rw-rw-   0 root         (0) root         (0)    22460 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/algorithm_descriptions.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)     9454 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/development.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.598576 enpt-0.20.1/docs/img/
--rw-rw-rw-   0 root         (0) root         (0)    13304 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/EnPT_Logo.png
--rw-rw-rw-   0 root         (0) root         (0)     4068 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/EnPT_Logo_clipped.png
--rw-rw-rw-   0 root         (0) root         (0)     6665 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/EnPT_Logo_transparent.png
--rw-rw-rw-   0 root         (0) root         (0)     1240 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/EnPT_logo_final.png
--rw-rw-rw-   0 root         (0) root         (0)    12452 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/EnPT_logo_final.svg
--rw-rw-rw-   0 root         (0) root         (0)     3314 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/EnPT_logo_final_clipped_doubleSize.png
--rw-rw-rw-   0 root         (0) root         (0)    71218 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/logo3.jpeg
--rw-rw-rw-   0 root         (0) root         (0)   118594 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/screenshot_enpt_enmapboxapp_v0.7.4.png
--rw-rw-rw-   0 root         (0) root         (0)    81885 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/tut__contents_l2a_output.png
--rw-rw-rw-   0 root         (0) root         (0)   105427 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/tut__contents_test_dataset.png
--rw-rw-rw-   0 root         (0) root         (0)   883240 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/tut__enmapbox_l1b_swir.png
--rw-rw-rw-   0 root         (0) root         (0)   797145 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/tut__enmapbox_l1b_vnir.png
--rw-rw-rw-   0 root         (0) root         (0)   305183 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/tut__enmapbox_l1b_vnir_swir_shift_striping.png
--rw-rw-rw-   0 root         (0) root         (0)   462337 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/img/tut__enmapbox_l2a_output.png
--rw-rw-rw-   0 root         (0) root         (0)      438 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6350 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     6455 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.602576 enpt-0.20.1/docs/software_design/
--rw-rw-rw-   0 root         (0) root         (0)  2961861 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/software_design/EnPT_software_design.xmind
--rw-rw-rw-   0 root         (0) root         (0)     9871 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/tutorial.rst
--rw-rw-rw-   0 root         (0) root         (0)     4160 2024-03-05 15:16:58.000000 enpt-0.20.1/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.606576 enpt-0.20.1/enpt/
--rw-rw-rw-   0 root         (0) root         (0)     2635 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12697 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.606576 enpt-0.20.1/enpt/execution/
--rw-rw-rw-   0 root         (0) root         (0)     1783 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10335 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/execution/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.606576 enpt-0.20.1/enpt/io/
--rw-rw-rw-   0 root         (0) root         (0)     1698 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8474 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/io/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.606576 enpt-0.20.1/enpt/model/
--rw-rw-rw-   0 root         (0) root         (0)     1728 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.606576 enpt-0.20.1/enpt/model/images/
--rw-rw-rw-   0 root         (0) root         (0)     1914 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/images/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19590 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/images/image_baseclasses.py
--rw-rw-rw-   0 root         (0) root         (0)    13951 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/images/images_mapgeo.py
--rw-rw-rw-   0 root         (0) root         (0)    50195 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/images/images_sensorgeo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.606576 enpt-0.20.1/enpt/model/metadata/
--rw-rw-rw-   0 root         (0) root         (0)     2566 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23438 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/metadata/metadata_mapgeo.py
--rw-rw-rw-   0 root         (0) root         (0)    35352 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/metadata/metadata_sensorgeo.py
--rw-rw-rw-   0 root         (0) root         (0)     7787 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/model/srf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/options/
--rw-rw-rw-   0 root         (0) root         (0)     1767 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/options/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27236 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/options/config.py
--rw-rw-rw-   0 root         (0) root         (0)     8431 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/options/options_default.json
--rw-rw-rw-   0 root         (0) root         (0)    11124 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/options/options_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/atmospheric_correction/
--rw-rw-rw-   0 root         (0) root         (0)     1824 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/atmospheric_correction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19508 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/atmospheric_correction/atmospheric_correction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/cloud_screening/
--rw-rw-rw-   0 root         (0) root         (0)     1766 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/cloud_screening/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1748 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/cloud_screening/cloud_screening.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/dead_pixel_correction/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/dead_pixel_correction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19311 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/dead_pixel_correction/dead_pixel_correction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/dem_preprocessing/
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/dem_preprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6347 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/dem_preprocessing/dem_preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/image_correction/
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/image_correction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1904 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/image_correction/image_correction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/orthorectification/
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/orthorectification/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20226 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/orthorectification/orthorectification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/radiometric_transform/
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/radiometric_transform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/radiometric_transform/radiometric_transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.610576 enpt-0.20.1/enpt/processors/spatial_module/
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/spatial_module/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/spatial_module/spatial_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt/processors/spatial_optimization/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/spatial_optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17335 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/spatial_optimization/spatial_optimization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt/processors/spatial_transform/
--rw-rw-rw-   0 root         (0) root         (0)     1857 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/spatial_transform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34001 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/processors/spatial_transform/spatial_transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.578577 enpt-0.20.1/enpt/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt/resources/EnMAP_Sensor/
--rw-rw-rw-   0 root         (0) root         (0)    13778 2024-03-05 15:17:01.000000 enpt-0.20.1/enpt/resources/EnMAP_Sensor/EnMAP_Level_1B_SNR.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt/resources/earth_sun_distance/
--rw-rw-rw-   0 root         (0) root         (0)   454623 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/resources/earth_sun_distance/Earth_Sun_distances_per_day_edited__1980_2030.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt/resources/solar_irradiance/
--rw-rw-rw-   0 root         (0) root         (0)   488336 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/resources/solar_irradiance/SUNp1fontenla__350-2500nm_@0.1nm_converted.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1752 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9629 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/utils/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     4317 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/utils/path_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-03-05 15:16:58.000000 enpt-0.20.1/enpt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:17:53.614575 enpt-0.20.1/enpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6939 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3823 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      505 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-05 15:17:53.000000 enpt-0.20.1/enpt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-03-05 15:16:58.000000 enpt-0.20.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-03-05 15:17:53.618575 enpt-0.20.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4518 2024-03-05 15:16:58.000000 enpt-0.20.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-05 15:16:58.000000 enpt-0.20.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.329642 enpt-0.20.2/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-30 23:57:36.000000 enpt-0.20.2/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-30 23:57:36.000000 enpt-0.20.2/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.297644 enpt-0.20.2/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-30 23:57:36.000000 enpt-0.20.2/.github/ISSUE_TEMPLATE.md
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-30 23:57:36.000000 enpt-0.20.2/.github/create_release_from_gitlab_ci.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4079 2024-05-30 23:57:36.000000 enpt-0.20.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2024-05-30 23:57:36.000000 enpt-0.20.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3878 2024-05-30 23:57:36.000000 enpt-0.20.2/.zenodo.json
+-rw-rw-rw-   0 root         (0) root         (0)      388 2024-05-30 23:57:36.000000 enpt-0.20.2/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2024-05-30 23:57:36.000000 enpt-0.20.2/CITATION
+-rw-rw-rw-   0 root         (0) root         (0)     5492 2024-05-30 23:57:36.000000 enpt-0.20.2/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    23393 2024-05-30 23:57:36.000000 enpt-0.20.2/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2024-05-30 23:57:36.000000 enpt-0.20.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-30 23:57:36.000000 enpt-0.20.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-05-30 23:57:36.000000 enpt-0.20.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-05-30 23:58:31.329642 enpt-0.20.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4447 2024-05-30 23:57:36.000000 enpt-0.20.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.301644 enpt-0.20.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.293644 enpt-0.20.2/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.293644 enpt-0.20.2/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.305643 enpt-0.20.2/docs/_build/html/_images/
+-rw-r--r--   0 root         (0) root         (0)     4068 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/EnPT_Logo_clipped.png
+-rw-r--r--   0 root         (0) root         (0)   118594 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/screenshot_enpt_enmapboxapp_v0.7.4.png
+-rw-r--r--   0 root         (0) root         (0)    81885 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/tut__contents_l2a_output.png
+-rw-r--r--   0 root         (0) root         (0)   105427 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/tut__contents_test_dataset.png
+-rw-r--r--   0 root         (0) root         (0)   883240 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l1b_swir.png
+-rw-r--r--   0 root         (0) root         (0)   797145 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l1b_vnir.png
+-rw-r--r--   0 root         (0) root         (0)   305183 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l1b_vnir_swir_shift_striping.png
+-rw-r--r--   0 root         (0) root         (0)   462337 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l2a_output.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.305643 enpt-0.20.2/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)     3314 2024-05-30 23:45:48.000000 enpt-0.20.2/docs/_build/html/_static/EnPT_logo_final_clipped_doubleSize.png
+-rw-r--r--   0 root         (0) root         (0)      286 2023-09-13 23:25:39.000000 enpt-0.20.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-09-13 23:25:39.000000 enpt-0.20.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-09-13 23:25:39.000000 enpt-0.20.2/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.305643 enpt-0.20.2/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/_static/wider_theme.css
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/about.rst
+-rw-rw-rw-   0 root         (0) root         (0)    22460 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/algorithm_descriptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9454 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/development.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.313643 enpt-0.20.2/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)    13304 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/EnPT_Logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/EnPT_Logo_clipped.png
+-rw-rw-rw-   0 root         (0) root         (0)     6665 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/EnPT_Logo_transparent.png
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/EnPT_logo_final.png
+-rw-rw-rw-   0 root         (0) root         (0)    12452 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/EnPT_logo_final.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/EnPT_logo_final_clipped_doubleSize.png
+-rw-rw-rw-   0 root         (0) root         (0)    71218 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/logo3.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)   118594 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/screenshot_enpt_enmapboxapp_v0.7.4.png
+-rw-rw-rw-   0 root         (0) root         (0)    81885 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/tut__contents_l2a_output.png
+-rw-rw-rw-   0 root         (0) root         (0)   105427 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/tut__contents_test_dataset.png
+-rw-rw-rw-   0 root         (0) root         (0)   883240 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/tut__enmapbox_l1b_swir.png
+-rw-rw-rw-   0 root         (0) root         (0)   797145 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/tut__enmapbox_l1b_vnir.png
+-rw-rw-rw-   0 root         (0) root         (0)   305183 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/tut__enmapbox_l1b_vnir_swir_shift_striping.png
+-rw-rw-rw-   0 root         (0) root         (0)   462337 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/img/tut__enmapbox_l2a_output.png
+-rw-rw-rw-   0 root         (0) root         (0)      438 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6350 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6455 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.313643 enpt-0.20.2/docs/software_design/
+-rw-rw-rw-   0 root         (0) root         (0)  2961861 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/software_design/EnPT_software_design.xmind
+-rw-rw-rw-   0 root         (0) root         (0)     9871 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/tutorial.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2024-05-30 23:57:36.000000 enpt-0.20.2/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.317643 enpt-0.20.2/enpt/
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12697 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.317643 enpt-0.20.2/enpt/execution/
+-rw-rw-rw-   0 root         (0) root         (0)     1783 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10335 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/execution/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.317643 enpt-0.20.2/enpt/io/
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8474 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/io/reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/model/
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/model/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/images/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19590 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/images/image_baseclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)    13951 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/images/images_mapgeo.py
+-rw-rw-rw-   0 root         (0) root         (0)    50195 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/images/images_sensorgeo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/model/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)     2566 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23438 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/metadata/metadata_mapgeo.py
+-rw-rw-rw-   0 root         (0) root         (0)    35352 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/metadata/metadata_sensorgeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7787 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/model/srf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/options/
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/options/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27236 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/options/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8431 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/options/options_default.json
+-rw-rw-rw-   0 root         (0) root         (0)    11124 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/options/options_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/processors/
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/processors/atmospheric_correction/
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/atmospheric_correction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19494 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/atmospheric_correction/atmospheric_correction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/processors/cloud_screening/
+-rw-rw-rw-   0 root         (0) root         (0)     1766 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/cloud_screening/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/cloud_screening/cloud_screening.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/processors/dead_pixel_correction/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/dead_pixel_correction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19311 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/dead_pixel_correction/dead_pixel_correction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.321642 enpt-0.20.2/enpt/processors/dem_preprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/dem_preprocessing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6347 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/dem_preprocessing/dem_preprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/processors/image_correction/
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/image_correction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/image_correction/image_correction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/processors/orthorectification/
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/orthorectification/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20226 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/orthorectification/orthorectification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/processors/radiometric_transform/
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/radiometric_transform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/radiometric_transform/radiometric_transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/processors/spatial_module/
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/spatial_module/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/spatial_module/spatial_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/processors/spatial_optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/spatial_optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17335 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/spatial_optimization/spatial_optimization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/processors/spatial_transform/
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/spatial_transform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34001 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/processors/spatial_transform/spatial_transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.297644 enpt-0.20.2/enpt/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/resources/EnMAP_Sensor/
+-rw-rw-rw-   0 root         (0) root         (0)    13778 2024-05-30 23:57:39.000000 enpt-0.20.2/enpt/resources/EnMAP_Sensor/EnMAP_Level_1B_SNR.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/resources/earth_sun_distance/
+-rw-rw-rw-   0 root         (0) root         (0)   454623 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/resources/earth_sun_distance/Earth_Sun_distances_per_day_edited__1980_2030.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.325642 enpt-0.20.2/enpt/resources/solar_irradiance/
+-rw-rw-rw-   0 root         (0) root         (0)   488336 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/resources/solar_irradiance/SUNp1fontenla__350-2500nm_@0.1nm_converted.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.329642 enpt-0.20.2/enpt/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9629 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/utils/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     4317 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/utils/path_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-05-30 23:57:36.000000 enpt-0.20.2/enpt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 23:58:31.329642 enpt-0.20.2/enpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6939 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-30 23:58:31.000000 enpt-0.20.2/enpt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-30 23:57:36.000000 enpt-0.20.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-05-30 23:58:31.333642 enpt-0.20.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2024-05-30 23:57:36.000000 enpt-0.20.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-30 23:57:36.000000 enpt-0.20.2/tox.ini
```

### Comparing `enpt-0.20.1/.coveragerc` & `enpt-0.20.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/.github/create_release_from_gitlab_ci.sh` & `enpt-0.20.2/.github/create_release_from_gitlab_ci.sh`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/.gitignore` & `enpt-0.20.2/.gitignore`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/.gitlab-ci.yml` & `enpt-0.20.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/.zenodo.json` & `enpt-0.20.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/CITATION` & `enpt-0.20.2/CITATION`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/CONTRIBUTING.rst` & `enpt-0.20.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/HISTORY.rst` & `enpt-0.20.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+0.20.2 (2024-05-30)
+-------------------
+
+* !107: Re-enabled first guess retrievals for water vapour, liquid water, and ice after fixing issues #90 and #92.
+
+
 0.20.1 (2024-03-05)
 -------------------
 
 * !105: Replaced legacy scipy.interpolate.interp1d with similar 1-dimensional interpolation functions.
 
 
 0.20.0 (2024-02-09)
```

### Comparing `enpt-0.20.1/LICENSE` & `enpt-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/Makefile` & `enpt-0.20.2/Makefile`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/PKG-INFO` & `enpt-0.20.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enpt
-Version: 0.20.1
+Version: 0.20.2
 Summary: EnMAP Processing Tool
 Home-page: https://git.gfz-potsdam.de/EnMAP/GFZ_Tools_EnMAP_BOX/EnPT
 Author: Karl Segl, Daniel Scheffler, Niklas Bohn, Stéphane Guillaso, Brenner Silva, Leonardo Alvarado
 Author-email: segl@gfz-potsdam.de, danschef@gfz-potsdam.de, nbohn@gfz-potsdam.de, stephane.guillaso@gfz-potsdam.de, brenner.silva@awi.de, leonardo.alvarado@awi.de
 License: GPL-3.0-or-later
 Keywords: EnPT,EnMAP,EnMAP-Box,hyperspectral,remote sensing,satellite,processing chain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `enpt-0.20.1/README.rst` & `enpt-0.20.2/README.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/Makefile` & `enpt-0.20.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/EnPT_Logo_clipped.png` & `enpt-0.20.2/docs/_build/html/_images/EnPT_Logo_clipped.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/screenshot_enpt_enmapboxapp_v0.7.4.png` & `enpt-0.20.2/docs/_build/html/_images/screenshot_enpt_enmapboxapp_v0.7.4.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/tut__contents_l2a_output.png` & `enpt-0.20.2/docs/_build/html/_images/tut__contents_l2a_output.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/tut__contents_test_dataset.png` & `enpt-0.20.2/docs/_build/html/_images/tut__contents_test_dataset.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l1b_swir.png` & `enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l1b_swir.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l1b_vnir.png` & `enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l1b_vnir.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l1b_vnir_swir_shift_striping.png` & `enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l1b_vnir_swir_shift_striping.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_images/tut__enmapbox_l2a_output.png` & `enpt-0.20.2/docs/_build/html/_images/tut__enmapbox_l2a_output.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/_build/html/_static/EnPT_logo_final_clipped_doubleSize.png` & `enpt-0.20.2/docs/_build/html/_static/EnPT_logo_final_clipped_doubleSize.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/about.rst` & `enpt-0.20.2/docs/about.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/algorithm_descriptions.rst` & `enpt-0.20.2/docs/algorithm_descriptions.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/conf.py` & `enpt-0.20.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/development.rst` & `enpt-0.20.2/docs/development.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/EnPT_Logo.png` & `enpt-0.20.2/docs/img/EnPT_Logo.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/EnPT_Logo_clipped.png` & `enpt-0.20.2/docs/img/EnPT_Logo_clipped.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/EnPT_Logo_transparent.png` & `enpt-0.20.2/docs/img/EnPT_Logo_transparent.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/EnPT_logo_final.png` & `enpt-0.20.2/docs/img/EnPT_logo_final.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/EnPT_logo_final.svg` & `enpt-0.20.2/docs/img/EnPT_logo_final.svg`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/EnPT_logo_final_clipped_doubleSize.png` & `enpt-0.20.2/docs/img/EnPT_logo_final_clipped_doubleSize.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/logo3.jpeg` & `enpt-0.20.2/docs/img/logo3.jpeg`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/screenshot_enpt_enmapboxapp_v0.7.4.png` & `enpt-0.20.2/docs/img/screenshot_enpt_enmapboxapp_v0.7.4.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/tut__contents_l2a_output.png` & `enpt-0.20.2/docs/img/tut__contents_l2a_output.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/tut__contents_test_dataset.png` & `enpt-0.20.2/docs/img/tut__contents_test_dataset.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/tut__enmapbox_l1b_swir.png` & `enpt-0.20.2/docs/img/tut__enmapbox_l1b_swir.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/tut__enmapbox_l1b_vnir.png` & `enpt-0.20.2/docs/img/tut__enmapbox_l1b_vnir.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/tut__enmapbox_l1b_vnir_swir_shift_striping.png` & `enpt-0.20.2/docs/img/tut__enmapbox_l1b_vnir_swir_shift_striping.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/img/tut__enmapbox_l2a_output.png` & `enpt-0.20.2/docs/img/tut__enmapbox_l2a_output.png`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/installation.rst` & `enpt-0.20.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/make.bat` & `enpt-0.20.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/software_design/EnPT_software_design.xmind` & `enpt-0.20.2/docs/software_design/EnPT_software_design.xmind`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/tutorial.rst` & `enpt-0.20.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/docs/usage.rst` & `enpt-0.20.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/__init__.py` & `enpt-0.20.2/enpt/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/cli.py` & `enpt-0.20.2/enpt/cli.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/execution/__init__.py` & `enpt-0.20.2/enpt/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/execution/controller.py` & `enpt-0.20.2/enpt/execution/controller.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/io/__init__.py` & `enpt-0.20.2/enpt/io/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/io/reader.py` & `enpt-0.20.2/enpt/io/reader.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/__init__.py` & `enpt-0.20.2/enpt/model/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/images/__init__.py` & `enpt-0.20.2/enpt/model/images/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/images/image_baseclasses.py` & `enpt-0.20.2/enpt/model/images/image_baseclasses.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/images/images_mapgeo.py` & `enpt-0.20.2/enpt/model/images/images_mapgeo.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/images/images_sensorgeo.py` & `enpt-0.20.2/enpt/model/images/images_sensorgeo.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/metadata/__init__.py` & `enpt-0.20.2/enpt/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/metadata/metadata_mapgeo.py` & `enpt-0.20.2/enpt/model/metadata/metadata_mapgeo.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/metadata/metadata_sensorgeo.py` & `enpt-0.20.2/enpt/model/metadata/metadata_sensorgeo.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/model/srf.py` & `enpt-0.20.2/enpt/model/srf.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/options/__init__.py` & `enpt-0.20.2/enpt/options/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/options/config.py` & `enpt-0.20.2/enpt/options/config.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/options/options_default.json` & `enpt-0.20.2/enpt/options/options_default.json`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/options/options_schema.py` & `enpt-0.20.2/enpt/options/options_schema.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/__init__.py` & `enpt-0.20.2/enpt/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/atmospheric_correction/__init__.py` & `enpt-0.20.2/enpt/processors/atmospheric_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/atmospheric_correction/atmospheric_correction.py` & `enpt-0.20.2/enpt/processors/atmospheric_correction/atmospheric_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,33 +69,34 @@
 
             # adjust options
             if enmap_ImageL1.meta.aot is not None:
                 options["retrieval"]["default_aot_value"] = enmap_ImageL1.meta.aot
 
             options["retrieval"]["cpu"] = self.cfg.CPUs or cpu_count()
             options["retrieval"]["disable_progressbars"] = self.cfg.disable_progress_bars
+            options["retrieval"]["segmentation"] = True
 
             # TODO: issue is closed -> revise
             # temporarily disable uncertainty measures to avoid https://git.gfz-potsdam.de/EnMAP/sicor/-/issues/86
             # if set to False, uncertainty values are not contained in the additional output of SICOR
             options["retrieval"]["inversion"]["full"] = False
 
             # set land_only mode
             options["retrieval"]["land_only"] = land_only
 
-            # disable first guess water vapor retrieval for now
-            options["retrieval"]["state_vector"]["water_vapor"]["use_prior_mean"] = True
-            options["retrieval"]["state_vector"]["water_vapor"]["prior_mean"] = \
-                enmap_ImageL1.meta.water_vapour  # = default = 2.5
+            # disable first guess water vapor retrieval
+            # options["retrieval"]["state_vector"]["water_vapor"]["use_prior_mean"] = True
+            # options["retrieval"]["state_vector"]["water_vapor"]["prior_mean"] = \
+            #     enmap_ImageL1.meta.water_vapour  # = default = 2.5
 
             # disable first guess liquid water retrieval for now
-            options["retrieval"]["state_vector"]["liquid_water"]["use_prior_mean"] = True
+            # options["retrieval"]["state_vector"]["liquid_water"]["use_prior_mean"] = True
 
             # disable first guess ice retrieval for now
-            options["retrieval"]["state_vector"]["ice"]["use_prior_mean"] = True
+            # options["retrieval"]["state_vector"]["ice"]["use_prior_mean"] = True
 
         except FileNotFoundError:
             raise FileNotFoundError(f'Could not locate options file for atmospheric correction at {path_opts}')
 
         enmap_ImageL1.logger.debug('SICOR AC configuration: \n' +
                                    pprint.pformat(options))
 
@@ -134,15 +135,15 @@
                 logger.warning(f"The atmospheric correction mode was set to '{self.cfg.mode_ac}' but "
                                f"Polymer cannot be imported (Error was: {e.msg}). "
                                f"As a fallback, SICOR is applied to water surfaces instead.")
             return False
 
         return True
 
-    def _run_AC__land_mode(self,
+    def _run_ac__land_mode(self,
                            enmap_ImageL1: EnMAPL1Product_SensorGeo
                            ) -> (np.ndarray, np.ndarray, dict):
         """Run atmospheric correction in 'land' mode, i.e., use SICOR for all surfaces."""
         if 2 in enmap_ImageL1.vnir.mask_landwater[:]:
             enmap_ImageL1.logger.info(
                 "Running atmospheric correction in 'land' mode, i.e., SICOR is applied to ALL surfaces. "
                 "Uncertainty is expected for water surfaces because SICOR is designed for land only.")
@@ -162,15 +163,15 @@
             sicor_ac_enmap(enmap_l1b=enmap_ImageL1,
                            options=self._get_sicor_options(enmap_ImageL1, land_only=False),
                            unknowns=True,
                            logger=enmap_ImageL1.logger)
 
         return boa_ref_vnir, boa_ref_swir, land_additional_results
 
-    def _run_AC__water_mode(self, enmap_ImageL1: EnMAPL1Product_SensorGeo
+    def _run_ac__water_mode(self, enmap_ImageL1: EnMAPL1Product_SensorGeo
                             ) -> (np.ndarray, np.ndarray):
         """Run atmospheric correction in 'water' mode, i.e., use ACWater/Polymer for water surfaces only.
 
         NOTE:
             - Land surfaces are NOT included in the EnMAP L2A product.
             - The output radiometric unit for water surfaces is 'water leaving reflectance'.
         """
@@ -204,15 +205,15 @@
                 "Alternatively, you may run EnPT in the 'land' atmospheric correction mode based on SICOR.\n"
                 "The error message is now raised:"
             )
             raise
 
         return wl_ref_vnir, wl_ref_swir, water_additional_results
 
-    def _run_AC__combined_mode(self,
+    def _run_ac__combined_mode(self,
                                enmap_ImageL1: EnMAPL1Product_SensorGeo
                                ) -> (np.ndarray, np.ndarray, dict):
         """Run atmospheric corr. in 'combined' mode, i.e., use SICOR for land and ACWater/Polymer for water surfaces.
 
         NOTE:
             - The output radiometric units are:
                 - 'surface reflectance' for land surfaces
@@ -266,15 +267,15 @@
         water_mask_swir = enmap_ImageL1.swir.mask_landwater[:] == 2  # 2 = water
         wlboa_ref_vnir = np.where(water_mask_vnir[:, :, None], wl_ref_vnir_water, boa_ref_vnir_land)
         wlboa_ref_swir = np.where(water_mask_swir[:, :, None], wl_ref_swir_water, boa_ref_swir_land)
 
         return wlboa_ref_vnir, wlboa_ref_swir, water_additional_results, land_additional_results
 
     @staticmethod
-    def _validate_AC_results(reflectance_vnir: np.ndarray,
+    def _validate_ac_results(reflectance_vnir: np.ndarray,
                              reflectance_swir: np.ndarray,
                              logger: Logger):
         for detectordata, detectorname in zip([reflectance_vnir, reflectance_swir],
                                               ['VNIR', 'SWIR']):
             mean0 = np.nanmean(detectordata[:, :, 0])
             std0 = np.nanstd(detectordata[:, :, 0])
 
@@ -294,46 +295,45 @@
         """
         enmap_ImageL1.set_SWIRattr_with_transformedVNIRattr('mask_landwater', src_nodata=0, tgt_nodata=0)
 
         enmap_ImageL1.logger.info(
             f"Starting atmospheric correction for VNIR and SWIR detector in '{self.cfg.mode_ac}' mode. "
             f"Source radiometric unit code is '{enmap_ImageL1.meta.vnir.unitcode}'.")
 
-        # set initial values for land_additional_results and water_additional_results
-        land_additional_results = None
+        # set initial value water_additional_results
         water_additional_results = None
 
         # run the AC
         acwater_operable = self._is_acwater_operable(enmap_ImageL1.logger)
 
         if self.cfg.mode_ac in ['water', 'combined'] and not acwater_operable:
             # use SICOR as fallback AC for water surfaces if ACWater/Polymer is not installed
             reflectance_vnir, reflectance_swir, land_additional_results = \
-                self._run_AC__land_mode(enmap_ImageL1)
+                self._run_ac__land_mode(enmap_ImageL1)
 
         else:
             if self.cfg.mode_ac == 'combined':
                 reflectance_vnir, reflectance_swir, water_additional_results, land_additional_results = \
-                    self._run_AC__combined_mode(enmap_ImageL1)
+                    self._run_ac__combined_mode(enmap_ImageL1)
 
             elif self.cfg.mode_ac == 'water':
                 reflectance_vnir, reflectance_swir, water_additional_results = \
-                    self._run_AC__water_mode(enmap_ImageL1)
+                    self._run_ac__water_mode(enmap_ImageL1)
 
             elif self.cfg.mode_ac == 'land':
                 reflectance_vnir, reflectance_swir, land_additional_results = \
-                    self._run_AC__land_mode(enmap_ImageL1)
+                    self._run_ac__land_mode(enmap_ImageL1)
 
             else:
                 raise ValueError(self.cfg.mode_ac,
                                  "Unexpected 'mode_ac' parameter. "
                                  "Choose one out of 'land', 'water', 'combined'.")
 
         # validate outputs
-        self._validate_AC_results(reflectance_vnir, reflectance_swir, logger=enmap_ImageL1.logger)
+        self._validate_ac_results(reflectance_vnir, reflectance_swir, logger=enmap_ImageL1.logger)
 
         # join results
         enmap_ImageL1.logger.info('Joining results of atmospheric correction.')
 
         for in_detector, out_detector in zip([enmap_ImageL1.vnir, enmap_ImageL1.swir],
                                              [reflectance_vnir, reflectance_swir]):
             data_ac_scaled_float = out_detector * self.cfg.scale_factor_boa_ref
```

### Comparing `enpt-0.20.1/enpt/processors/cloud_screening/__init__.py` & `enpt-0.20.2/enpt/processors/cloud_screening/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/cloud_screening/cloud_screening.py` & `enpt-0.20.2/enpt/processors/cloud_screening/cloud_screening.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/dead_pixel_correction/__init__.py` & `enpt-0.20.2/enpt/processors/dead_pixel_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/dead_pixel_correction/dead_pixel_correction.py` & `enpt-0.20.2/enpt/processors/dead_pixel_correction/dead_pixel_correction.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/dem_preprocessing/__init__.py` & `enpt-0.20.2/enpt/processors/dem_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/dem_preprocessing/dem_preprocessing.py` & `enpt-0.20.2/enpt/processors/dem_preprocessing/dem_preprocessing.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/image_correction/__init__.py` & `enpt-0.20.2/enpt/processors/image_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/image_correction/image_correction.py` & `enpt-0.20.2/enpt/processors/image_correction/image_correction.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/orthorectification/__init__.py` & `enpt-0.20.2/enpt/processors/orthorectification/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/orthorectification/orthorectification.py` & `enpt-0.20.2/enpt/processors/orthorectification/orthorectification.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/radiometric_transform/__init__.py` & `enpt-0.20.2/enpt/processors/radiometric_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/radiometric_transform/radiometric_transform.py` & `enpt-0.20.2/enpt/processors/radiometric_transform/radiometric_transform.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/spatial_module/__init__.py` & `enpt-0.20.2/enpt/processors/spatial_module/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/spatial_module/spatial_module.py` & `enpt-0.20.2/enpt/processors/spatial_module/spatial_module.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/spatial_optimization/__init__.py` & `enpt-0.20.2/enpt/processors/spatial_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/spatial_optimization/spatial_optimization.py` & `enpt-0.20.2/enpt/processors/spatial_optimization/spatial_optimization.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/spatial_transform/__init__.py` & `enpt-0.20.2/enpt/processors/spatial_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/processors/spatial_transform/spatial_transform.py` & `enpt-0.20.2/enpt/processors/spatial_transform/spatial_transform.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/resources/EnMAP_Sensor/EnMAP_Level_1B_SNR.zip` & `enpt-0.20.2/enpt/resources/EnMAP_Sensor/EnMAP_Level_1B_SNR.zip`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/resources/earth_sun_distance/Earth_Sun_distances_per_day_edited__1980_2030.csv` & `enpt-0.20.2/enpt/resources/earth_sun_distance/Earth_Sun_distances_per_day_edited__1980_2030.csv`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/resources/solar_irradiance/SUNp1fontenla__350-2500nm_@0.1nm_converted.txt` & `enpt-0.20.2/enpt/resources/solar_irradiance/SUNp1fontenla__350-2500nm_@0.1nm_converted.txt`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/utils/__init__.py` & `enpt-0.20.2/enpt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/utils/logging.py` & `enpt-0.20.2/enpt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/utils/path_generator.py` & `enpt-0.20.2/enpt/utils/path_generator.py`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/enpt/version.py` & `enpt-0.20.2/enpt/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.20.1'
-__versionalias__ = '20240305.01'
+__version__ = '0.20.2'
+__versionalias__ = '20240530.01'
 __author__ = 'Daniel Scheffler'
```

### Comparing `enpt-0.20.1/enpt.egg-info/PKG-INFO` & `enpt-0.20.2/enpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enpt
-Version: 0.20.1
+Version: 0.20.2
 Summary: EnMAP Processing Tool
 Home-page: https://git.gfz-potsdam.de/EnMAP/GFZ_Tools_EnMAP_BOX/EnPT
 Author: Karl Segl, Daniel Scheffler, Niklas Bohn, Stéphane Guillaso, Brenner Silva, Leonardo Alvarado
 Author-email: segl@gfz-potsdam.de, danschef@gfz-potsdam.de, nbohn@gfz-potsdam.de, stephane.guillaso@gfz-potsdam.de, brenner.silva@awi.de, leonardo.alvarado@awi.de
 License: GPL-3.0-or-later
 Keywords: EnPT,EnMAP,EnMAP-Box,hyperspectral,remote sensing,satellite,processing chain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `enpt-0.20.1/enpt.egg-info/SOURCES.txt` & `enpt-0.20.2/enpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enpt-0.20.1/setup.py` & `enpt-0.20.2/setup.py`

 * *Files identical despite different names*

