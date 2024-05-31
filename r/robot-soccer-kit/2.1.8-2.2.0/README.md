# Comparing `tmp/robot-soccer-kit-2.1.8.tar.gz` & `tmp/robot-soccer-kit-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-soccer-kit-2.1.8.tar", last modified: Fri May 24 13:34:47 2024, max compression
+gzip compressed data, was "robot-soccer-kit-2.2.0.tar", last modified: Fri May 31 14:31:52 2024, max compression
```

## Comparing `robot-soccer-kit-2.1.8.tar` & `robot-soccer-kit-2.2.0.tar`

### file list

```diff
@@ -1,162 +1,163 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1161 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/README.md
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/
--rw-r--r--   0 gregwar   (1000) gregwar   (1000)     1161 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4883 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      176 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2024-05-24 13:34:47.000000 robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/rsk/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/api.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5578 2024-05-21 08:27:22.000000 robot-soccer-kit-2.1.8/rsk/backend.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14312 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3696 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/constants.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.8/rsk/control.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.1.8/rsk/detection.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/dump_referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/field.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/game_controller.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/kinematics.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/logger.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/place.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24336 2023-11-22 10:48:11.000000 robot-soccer-kit-2.1.8/rsk/referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2368 2024-05-21 08:26:43.000000 robot-soccer-kit-2.1.8/rsk/robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11630 2024-05-21 08:24:01.000000 robot-soccer-kit-2.1.8/rsk/robot_serial.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      142 2024-05-21 08:25:36.000000 robot-soccer-kit-2.1.8/rsk/robot_wifi.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/robots.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10208 2024-05-21 08:24:28.000000 robot-soccer-kit-2.1.8/rsk/simulator.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/state.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/rsk/static/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.292004 robot-soccer-kit-2.1.8/rsk/static/bootstrap/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/camera-setting.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3721 2024-05-24 13:31:39.000000 robot-soccer-kit-2.1.8/rsk/static/css/app.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/favicon.ico
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.browserslistrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.editorconfig
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.eslintignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.eslintrc.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.fantasticonrc.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.gitattributes
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/.github/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/dependabot.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/preview.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/release-drafter.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.296004 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/codeql.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/deploy.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/release-notes.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/test.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/.stylelintrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/LICENSE.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/bootstrap-icons.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/composer.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/config.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/icons/font/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.json
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff2
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/font/index.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/package-lock.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/package.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/svg-sprite.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/icons/svgo.config.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/imgs/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_16x16.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_24x24.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_256x256.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_32x32.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/ball_48x48.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/field.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/field.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robot.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    33731 2024-05-24 13:33:34.000000 robot-soccer-kit-2.1.8/rsk/static/index.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/jquery/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/jquery/jquery.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2225 2024-05-24 13:33:49.000000 robot-soccer-kit-2.1.8/rsk/static/js/app.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1738 2023-06-26 12:35:06.000000 robot-soccer-kit-2.1.8/rsk/static/js/competition.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1585 2024-04-11 05:52:39.000000 robot-soccer-kit-2.1.8/rsk/static/js/control.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13475 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/static/js/referee.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/js/robots.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:35:04.000000 robot-soccer-kit-2.1.8/rsk/static/js/simulator.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/js/tabs.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/js/utils.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.1.8/rsk/static/js/video.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/rsk/static/markers/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/blue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/blue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/green1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/markers/green2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/referee_event_neutral.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/referee_event_team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/static/robot.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.1.8/rsk/static/team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4186 2023-11-10 16:33:26.000000 robot-soccer-kit-2.1.8/rsk/tasks.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.1.8/rsk/video.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2024-05-24 13:34:47.300004 robot-soccer-kit-2.1.8/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1420 2024-05-24 13:34:34.000000 robot-soccer-kit-2.1.8/setup.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1161 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/README.md
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.284283 robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/
+-rw-r--r--   0 gregwar   (1000) gregwar   (1000)     1161 2024-05-31 14:31:52.000000 robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4898 2024-05-31 14:31:52.000000 robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2024-05-31 14:31:52.000000 robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      176 2024-05-31 14:31:52.000000 robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2024-05-31 14:31:52.000000 robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.288284 robot-soccer-kit-2.2.0/rsk/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/api.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5657 2024-05-31 14:31:10.000000 robot-soccer-kit-2.2.0/rsk/backend.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14312 2023-11-10 16:33:26.000000 robot-soccer-kit-2.2.0/rsk/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3696 2023-11-10 16:33:26.000000 robot-soccer-kit-2.2.0/rsk/constants.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-06-26 12:24:11.000000 robot-soccer-kit-2.2.0/rsk/control.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.2.0/rsk/detection.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/dump_referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/field.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2766 2024-05-31 14:31:10.000000 robot-soccer-kit-2.2.0/rsk/game_controller.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/kinematics.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/logger.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4384 2024-05-31 14:31:10.000000 robot-soccer-kit-2.2.0/rsk/packets.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/place.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24336 2023-11-22 10:48:11.000000 robot-soccer-kit-2.2.0/rsk/referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2415 2024-05-31 14:31:10.000000 robot-soccer-kit-2.2.0/rsk/robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     8610 2024-05-31 14:31:10.000000 robot-soccer-kit-2.2.0/rsk/robot_serial.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     7884 2024-05-31 14:31:10.000000 robot-soccer-kit-2.2.0/rsk/robot_wifi.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2024-05-31 12:31:49.000000 robot-soccer-kit-2.2.0/rsk/robots.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10208 2024-05-21 08:24:28.000000 robot-soccer-kit-2.2.0/rsk/simulator.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/state.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.288284 robot-soccer-kit-2.2.0/rsk/static/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.284283 robot-soccer-kit-2.2.0/rsk/static/bootstrap/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/camera-setting.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3721 2024-05-24 13:31:39.000000 robot-soccer-kit-2.2.0/rsk/static/css/app.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/favicon.ico
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/icons/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.browserslistrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.editorconfig
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.eslintignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.eslintrc.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.fantasticonrc.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.gitattributes
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/icons/.github/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/icons/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/dependabot.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/preview.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/release-drafter.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/codeql.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/deploy.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/release-notes.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/test.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/.stylelintrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/LICENSE.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/bootstrap-icons.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/composer.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/config.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/icons/font/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/font/bootstrap-icons.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/font/bootstrap-icons.json
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.292284 robot-soccer-kit-2.2.0/rsk/static/icons/font/fonts/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/font/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/font/fonts/bootstrap-icons.woff2
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/font/index.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/package-lock.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/package.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/svg-sprite.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/icons/svgo.config.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/rsk/static/imgs/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/ball.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/ball_16x16.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/ball_24x24.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/ball_256x256.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/ball_32x32.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/ball_48x48.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/field.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/field.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/robot.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/robotblue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/robotblue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/robotgreen1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/imgs/robotgreen2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    33731 2024-05-24 13:33:34.000000 robot-soccer-kit-2.2.0/rsk/static/index.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/rsk/static/jquery/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/jquery/jquery.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/rsk/static/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2225 2024-05-24 13:33:49.000000 robot-soccer-kit-2.2.0/rsk/static/js/app.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1738 2023-06-26 12:35:06.000000 robot-soccer-kit-2.2.0/rsk/static/js/competition.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1585 2024-04-11 05:52:39.000000 robot-soccer-kit-2.2.0/rsk/static/js/control.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13475 2023-11-10 16:33:26.000000 robot-soccer-kit-2.2.0/rsk/static/js/referee.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/js/robots.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    14606 2023-06-26 12:35:04.000000 robot-soccer-kit-2.2.0/rsk/static/js/simulator.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/js/tabs.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/js/utils.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-06-26 12:24:11.000000 robot-soccer-kit-2.2.0/rsk/static/js/video.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/rsk/static/markers/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/markers/blue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/markers/blue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/markers/green1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/markers/green2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/referee_event_neutral.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/referee_event_team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/static/robot.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.2.0/rsk/static/team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4186 2023-11-10 16:33:26.000000 robot-soccer-kit-2.2.0/rsk/tasks.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/utils.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.2.0/rsk/video.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2024-05-31 14:31:52.296284 robot-soccer-kit-2.2.0/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1420 2024-05-31 14:31:35.000000 robot-soccer-kit-2.2.0/setup.py
```

### Comparing `robot-soccer-kit-2.1.8/PKG-INFO` & `robot-soccer-kit-2.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.1.8
+Version: 2.2.0
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl sct robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.1.8/README.md` & `robot-soccer-kit-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/PKG-INFO` & `robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.1.8
+Version: 2.2.0
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl sct robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.1.8/robot_soccer_kit.egg-info/SOURCES.txt` & `robot-soccer-kit-2.2.0/robot_soccer_kit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 rsk/control.py
 rsk/detection.py
 rsk/dump_referee.py
 rsk/field.py
 rsk/game_controller.py
 rsk/kinematics.py
 rsk/logger.py
+rsk/packets.py
 rsk/place.py
 rsk/referee.py
 rsk/robot.py
 rsk/robot_serial.py
 rsk/robot_wifi.py
 rsk/robots.py
 rsk/simulator.py
```

### Comparing `robot-soccer-kit-2.1.8/rsk/api.py` & `robot-soccer-kit-2.2.0/rsk/api.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/backend.py` & `robot-soccer-kit-2.2.0/rsk/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from . import api
 from . import (
     state,
     video,
     robots,
     robot_serial,
+    robot_wifi,
     control,
     referee,
     detection,
     utils,
     constants,
     simulator,
 )
 
 
 class Backend:
     def __init__(self, simulated=False, competition=False):
         super().__init__()
         robots.Robots.protocols["serial"] = robot_serial.RobotSerial
+        robots.Robots.protocols["wifi"] = robot_wifi.RobotWifi
 
         self.simulated = simulated
         self.competition = competition
 
         self.state: state.State = state.State(30, self.simulated)
         self.state.start_pub()
```

### Comparing `robot-soccer-kit-2.1.8/rsk/client.py` & `robot-soccer-kit-2.2.0/rsk/client.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/constants.py` & `robot-soccer-kit-2.2.0/rsk/constants.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/control.py` & `robot-soccer-kit-2.2.0/rsk/control.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/detection.py` & `robot-soccer-kit-2.2.0/rsk/detection.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/dump_referee.py` & `robot-soccer-kit-2.2.0/rsk/dump_referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/field.py` & `robot-soccer-kit-2.2.0/rsk/field.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/game_controller.py` & `robot-soccer-kit-2.2.0/rsk/game_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,34 @@
 import time
 import logging
 import threading
 import waitress
 from flask import Flask, send_from_directory, jsonify, request
 from flask_cors import CORS
 from .backend import Backend
-from . import api
+from . import api, robot_wifi
 
 
 # Setting up the logger
 logging.basicConfig(format="[%(levelname)s] %(asctime)s - %(name)s - %(message)s", level=logging.INFO)
 logging.getLogger("werkzeug").setLevel(logging.CRITICAL)
 logging.getLogger("robot-soccer-kit").info("Starting robot-soccer-kit Game Controller")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--port", "-p", type=str, default="7070")
 parser.add_argument("--ip", "-ip", type=str, default="127.0.0.1")
 parser.add_argument("--simulated", "-s", action="store_true")
 parser.add_argument("--competition", "-c", action="store_true")
+parser.add_argument("--wifi-network", "-w", type=str, default="192.168.100.0")
+parser.add_argument("--wifi-subnet", "-ws", type=str, default="255.255.255.0")
 args = parser.parse_args()
 
+robot_wifi.RobotWifi.network = args.wifi_network
+robot_wifi.RobotWifi.netmask = args.wifi_subnet
+robot_wifi.RobotWifi.start_service()
 
 has_client: bool = False
 backend: Backend = Backend(args.simulated, args.competition)
 api.register(backend)
 
 # Starting a Flask app serving API requests and files of static/ directory
 static = os.path.dirname(__file__) + "/static/"
```

### Comparing `robot-soccer-kit-2.1.8/rsk/kinematics.py` & `robot-soccer-kit-2.2.0/rsk/kinematics.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/place.py` & `robot-soccer-kit-2.2.0/rsk/place.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/referee.py` & `robot-soccer-kit-2.2.0/rsk/referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/robot.py` & `robot-soccer-kit-2.2.0/rsk/robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         self.last_message = None
 
         # Marker on the top of this robot
         self.marker = None
 
     def available_urls() -> list:
         return []
+    
+    def close(self) -> None:
+        pass
 
     def set_marker(self, marker: str) -> None:
         """
         Sets the robot's marker
 
         :param str marker: the robot marker
         """
```

### Comparing `robot-soccer-kit-2.1.8/rsk/robot_serial.py` & `robot-soccer-kit-2.2.0/rsk/robot_serial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,19 @@
 import numpy as np
 import threading
 import time
 import serial
 from serial.tools import list_ports
 import logging
 from . import robot, robots
-
-# Constants for binary protocol
-PACKET_ACK = 0
-PACKET_MONITOR = 1
-PACKET_HOLO = 80
-PACKET_HOLO_CONTROL = 2
-PACKET_HOLO_BEEP = 3
-PACKET_HOLO_LEDS_CUSTOM = 7
-PACKET_HOLO_LEDS_BREATH = 8
-PACKET_HOLO_KICK = 12
-PACKET_MONITOR_DATA = 5
+from .packets import *
 
 logger: logging.Logger = logging.getLogger("robot")
 
 
-class Packet:
-    """
-    Represents a physical packet that is sent or received (binary protocol)
-    """
-
-    def __init__(self, type_: int, payload=bytearray()):
-        self.type: int = type_
-        self.payload = payload.copy()
-
-    def available(self):
-        return len(self.payload)
-
-    def append_byte(self, char):
-        char = char & 0xFF
-        if type(char) == int:
-            self.payload += bytearray((char,))
-        else:
-            self.payload += bytearray(char)
-
-    def append_short(self, short):
-        b1 = (short >> 8) & 0xFF
-        b2 = short & 0xFF
-
-        self.payload += bytearray((b1, b2))
-
-    def append_int(self, short):
-        b1 = (short >> 24) & 0xFF
-        b2 = (short >> 16) & 0xFF
-        b3 = (short >> 8) & 0xFF
-        b4 = short & 0xFF
-
-        self.payload += bytearray((b1, b2, b3, b4))
-
-    def appendFloat(self, f):
-        self.append_int(f * 1000.0)
-
-    def appendSmallFloat(self, f):
-        self.append_short(f * 10.0)
-
-    def readByte(self):
-        byte = self.payload[0]
-        self.payload = self.payload[1:]
-
-        return byte
-
-    def read_int(self):
-        n = self.readByte() << 24
-        n = n | (self.readByte() << 16)
-        n = n | (self.readByte() << 8)
-        n = n | (self.readByte() << 0)
-
-        return int(np.int32(n))
-
-    def read_short(self):
-        n = (self.readByte() << 8) | self.readByte()
-
-        return int(np.int16(n))
-
-    def read_float(self):
-        return self.read_int() / 1000.0
-
-    def read_small_float(self):
-        return self.read_short() / 10.0
-
-    def to_raw(self):
-        raw = bytearray()
-        raw += bytearray((0xFF, 0xAA, self.type, len(self.payload)))
-        raw += self.payload
-        raw += bytearray((self.checksum(),))
-
-        return raw
-
-    def checksum(self):
-        return sum(self.payload) % 256
-
-
 class RobotSerial(robot.Robot):
     """
     Connection with a physical robot
     """
 
     def __init__(self, url: str):
         super().__init__(url)
@@ -217,59 +131,59 @@
     def beep(self, frequency: int, duration: int):
         """
         Gets the robot beeping
 
         :param int frequency: frequency (Hz)
         :param int duration: duration (ms)
         """
-        packet = Packet(PACKET_HOLO)
-        packet.append_byte(PACKET_HOLO_BEEP)
+        packet = Packet(PACKET_ROBOT)
+        packet.append_byte(PACKET_ROBOT_BEEP)
         packet.append_short(frequency)
         packet.append_short(duration)
         self.add_packet("beep", packet)
 
     def kick(self, power: float = 1.0):
         """
         Gets the robot kicking
 
         :param float power: kick intensity (0 to 1), defaults to 1.
         """
-        packet = Packet(PACKET_HOLO)
-        packet.append_byte(PACKET_HOLO_KICK)
+        packet = Packet(PACKET_ROBOT)
+        packet.append_byte(PACKET_ROBOT_KICK)
         packet.append_byte(int(100 * power))
         self.add_packet("kick", packet)
 
     def control(self, dx: float, dy: float, dturn: float):
         """
         Sends some chassis speed order fo the robot
 
         :param float dx: x speed (m/s)
         :param float dy: y speed (m/s)
         :param float dturn: rotational speed (rad/s)
         """
-        packet = Packet(PACKET_HOLO)
-        packet.append_byte(PACKET_HOLO_CONTROL)
+        packet = Packet(PACKET_ROBOT)
+        packet.append_byte(PACKET_ROBOT_CONTROL)
         packet.append_short(int(1000 * dx))
         packet.append_short(int(1000 * dy))
         packet.append_short(int(np.rad2deg(dturn)))
         self.add_packet("control", packet)
 
-    def leds(self, r: int, g: int, b: int) -> None:
+    def leds(self, red: int, green: int, blue: int) -> None:
         """
         Sets the robot LEDs
 
         :param int r: R intensity (0-255)
         :param int g: G intensity (0-255)
         :param int b: B intensity (0-255)
         """
-        packet = Packet(PACKET_HOLO)
-        packet.append_byte(PACKET_HOLO_LEDS_CUSTOM)
-        packet.append_byte(r)
-        packet.append_byte(g)
-        packet.append_byte(b)
+        packet = Packet(PACKET_ROBOT)
+        packet.append_byte(PACKET_ROBOT_LEDS_CUSTOM)
+        packet.append_byte(red)
+        packet.append_byte(green)
+        packet.append_byte(blue)
         self.add_packet("leds", packet)
 
     def stop(self):
         """
         Stops the robot from moving
         """
         self.control(0, 0, 0)
@@ -280,14 +194,16 @@
         """
         self.running = False
 
     def run_thread(self):
         """
         Process the main thread
         """
+        packet_reader = PacketReader()
+
         while self.running:
             try:
                 if self.init:
                     logger.info(f"Opening connection with {self.url}")
                     self.init = False
                     if self.bt is not None:
                         self.bt.close()
@@ -295,48 +211,24 @@
                     self.bt = serial.Serial(self.url, timeout=0.02)
                     time.sleep(0.1)
                     self.bt.write(b"rhock\r\nrhock\r\nrhock\r\n")
                     time.sleep(0.1)
                     self.monitor(5)
                     self.control(0, 0, 0)
                     self.beep(880, 250)
+                    packet_reader.reset()
                     self.last_init = time.time()
                     self.last_sent_message = None
-                    state = 0
-                    type_, length, payload = 0, 0, bytearray()
 
                 # Receiving data
                 byte = self.bt.read(1)
                 if len(byte):
-                    byte = ord(byte)
-                    if state == 0:  # First header
-                        if byte == 0xFF:
-                            state += 1
-                        else:
-                            state = 0
-                    elif state == 1:  # Second header
-                        if byte == 0xAA:
-                            state += 1
-                        else:
-                            state = 0
-                    elif state == 2:  # Packet type
-                        type_ = byte
-                        state += 1
-                    elif state == 3:  # Packet length
-                        length = byte
-                        state += 1
-                    elif state == 4:  # Payload
-                        payload += bytearray((byte,))
-                        if len(payload) >= length:
-                            state += 1
-                    elif state == 5:  # Checksum
-                        if sum(payload) % 256 == byte:
-                            self.process(Packet(type_, payload))
-                            type_, length, payload = 0, 0, bytearray()
-                        state = 0
+                    packet_reader.push(ord(byte))
+                    if packet_reader.has_packet():
+                        self.process(packet_reader.pop_packet())
 
                 # Asking periodically for robot monitor status
                 if self.last_sent_message is None or time.time() - self.last_sent_message > 1.0:
                     self.monitor(1)
 
                 # Sending pending packets
                 packet = self.pop_packet()
```

### Comparing `robot-soccer-kit-2.1.8/rsk/robots.py` & `robot-soccer-kit-2.2.0/rsk/robots.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/simulator.py` & `robot-soccer-kit-2.2.0/rsk/simulator.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/state.py` & `robot-soccer-kit-2.2.0/rsk/state.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.js.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.js.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.esm.min.js.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.js.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/bootstrap/js/bootstrap.min.js.map` & `robot-soccer-kit-2.2.0/rsk/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/css/app.css` & `robot-soccer-kit-2.2.0/rsk/static/css/app.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/favicon.ico` & `robot-soccer-kit-2.2.0/rsk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.fantasticonrc.js` & `robot-soccer-kit-2.2.0/rsk/static/icons/.fantasticonrc.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md` & `robot-soccer-kit-2.2.0/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.github/preview.png` & `robot-soccer-kit-2.2.0/rsk/static/icons/.github/preview.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.github/release-drafter.yml` & `robot-soccer-kit-2.2.0/rsk/static/icons/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/codeql.yml` & `robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/deploy.yml` & `robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/.github/workflows/test.yml` & `robot-soccer-kit-2.2.0/rsk/static/icons/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/LICENSE.md` & `robot-soccer-kit-2.2.0/rsk/static/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/README.md` & `robot-soccer-kit-2.2.0/rsk/static/icons/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/bootstrap-icons.svg` & `robot-soccer-kit-2.2.0/rsk/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/config.yml` & `robot-soccer-kit-2.2.0/rsk/static/icons/config.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.css` & `robot-soccer-kit-2.2.0/rsk/static/icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/font/bootstrap-icons.json` & `robot-soccer-kit-2.2.0/rsk/static/icons/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff` & `robot-soccer-kit-2.2.0/rsk/static/icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/font/fonts/bootstrap-icons.woff2` & `robot-soccer-kit-2.2.0/rsk/static/icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/font/index.html` & `robot-soccer-kit-2.2.0/rsk/static/icons/font/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/package-lock.json` & `robot-soccer-kit-2.2.0/rsk/static/icons/package-lock.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/package.json` & `robot-soccer-kit-2.2.0/rsk/static/icons/package.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/svg-sprite.json` & `robot-soccer-kit-2.2.0/rsk/static/icons/svg-sprite.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/icons/svgo.config.js` & `robot-soccer-kit-2.2.0/rsk/static/icons/svgo.config.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/ball.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/ball.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_16x16.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/ball_16x16.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_24x24.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/ball_24x24.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_256x256.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/ball_256x256.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_32x32.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/ball_32x32.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/ball_48x48.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/ball_48x48.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/field.png` & `robot-soccer-kit-2.2.0/rsk/static/imgs/field.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/field.svg` & `robot-soccer-kit-2.2.0/rsk/static/imgs/field.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/robot.svg` & `robot-soccer-kit-2.2.0/rsk/static/imgs/robot.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue1.svg` & `robot-soccer-kit-2.2.0/rsk/static/imgs/robotblue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/robotblue2.svg` & `robot-soccer-kit-2.2.0/rsk/static/imgs/robotblue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen1.svg` & `robot-soccer-kit-2.2.0/rsk/static/imgs/robotgreen1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/imgs/robotgreen2.svg` & `robot-soccer-kit-2.2.0/rsk/static/imgs/robotgreen2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/index.html` & `robot-soccer-kit-2.2.0/rsk/static/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/jquery/jquery.js` & `robot-soccer-kit-2.2.0/rsk/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/app.js` & `robot-soccer-kit-2.2.0/rsk/static/js/app.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/competition.js` & `robot-soccer-kit-2.2.0/rsk/static/js/competition.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/control.js` & `robot-soccer-kit-2.2.0/rsk/static/js/control.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/referee.js` & `robot-soccer-kit-2.2.0/rsk/static/js/referee.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/robots.js` & `robot-soccer-kit-2.2.0/rsk/static/js/robots.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/simulator.js` & `robot-soccer-kit-2.2.0/rsk/static/js/simulator.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/js/video.js` & `robot-soccer-kit-2.2.0/rsk/static/js/video.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/markers/blue1.svg` & `robot-soccer-kit-2.2.0/rsk/static/markers/blue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/markers/blue2.svg` & `robot-soccer-kit-2.2.0/rsk/static/markers/blue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/markers/green1.svg` & `robot-soccer-kit-2.2.0/rsk/static/markers/green1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/markers/green2.svg` & `robot-soccer-kit-2.2.0/rsk/static/markers/green2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/referee_event_team.html` & `robot-soccer-kit-2.2.0/rsk/static/referee_event_team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/robot.html` & `robot-soccer-kit-2.2.0/rsk/static/robot.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/static/team.html` & `robot-soccer-kit-2.2.0/rsk/static/team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/tasks.py` & `robot-soccer-kit-2.2.0/rsk/tasks.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/utils.py` & `robot-soccer-kit-2.2.0/rsk/utils.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/rsk/video.py` & `robot-soccer-kit-2.2.0/rsk/video.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.1.8/setup.py` & `robot-soccer-kit-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         for filename in filenames:
             if "__pycache__" not in path:
                 paths.append(os.path.join("..", path, filename))
     return paths
 
 setuptools.setup(
     name="robot-soccer-kit",
-    version="2.1.8",
+    version="2.2.0",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Robot Soccer Kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/robot-soccer-kit/",
     packages=setuptools.find_packages(),
```

