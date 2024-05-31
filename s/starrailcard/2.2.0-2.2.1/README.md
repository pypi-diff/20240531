# Comparing `tmp/starrailcard-2.2.0.tar.gz` & `tmp/starrailcard-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.2.0.tar", last modified: Wed May 22 22:14:46 2024, max compression
+gzip compressed data, was "starrailcard-2.2.1.tar", last modified: Fri May 31 21:38:44 2024, max compression
```

## Comparing `starrailcard-2.2.0.tar` & `starrailcard-2.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.132206 starrailcard-2.2.0/
--rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.2.0/LICENSE
--rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4762 2024-05-22 22:14:46.131207 starrailcard-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.2.0/README.md
--rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 22:14:46.132206 starrailcard-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1571 2024-05-11 16:52:16.000000 starrailcard-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.038205 starrailcard-2.2.0/starrailcard/
--rw-rw-rw-   0        0        0     1967 2024-05-22 22:14:43.000000 starrailcard-2.2.0/starrailcard/__init__.py
--rw-rw-rw-   0        0        0    25256 2024-05-20 11:59:09.000000 starrailcard-2.2.0/starrailcard/client.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.028698 starrailcard-2.2.0/starrailcard/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.063660 starrailcard-2.2.0/starrailcard/src/api/
--rw-rw-rw-   0        0        0     3740 2024-05-19 22:23:39.000000 starrailcard-2.2.0/starrailcard/src/api/api.py
--rw-rw-rw-   0        0        0     5892 2024-05-20 10:36:13.000000 starrailcard-2.2.0/starrailcard/src/api/enka.py
--rw-rw-rw-   0        0        0    27773 2024-05-20 10:45:25.000000 starrailcard-2.2.0/starrailcard/src/api/enka_parsed.py
--rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.2.0/starrailcard/src/api/error.py
--rw-rw-rw-   0        0        0     2271 2024-05-20 08:43:12.000000 starrailcard-2.2.0/starrailcard/src/api/hoyolab.py
--rw-rw-rw-   0        0        0    28814 2024-05-20 09:23:13.000000 starrailcard-2.2.0/starrailcard/src/api/hoyolab_parsed.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.028698 starrailcard-2.2.0/starrailcard/src/assets/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.068163 starrailcard-2.2.0/starrailcard/src/assets/font/
--rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.2.0/starrailcard/src/assets/font/font_hsr.ttf
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.091716 starrailcard-2.2.0/starrailcard/src/data/
--rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/avatar.json
--rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/element.json
--rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/keys.json
--rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/paths.json
--rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/relict_sets.json
--rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/stats.json
--rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.094717 starrailcard-2.2.0/starrailcard/src/generator/
--rw-rw-rw-   0        0        0    26195 2024-05-20 11:30:55.000000 starrailcard-2.2.0/starrailcard/src/generator/style_card.py
--rw-rw-rw-   0        0        0     6675 2024-05-17 19:35:00.000000 starrailcard-2.2.0/starrailcard/src/generator/style_profile_phone.py
--rw-rw-rw-   0        0        0    24987 2024-05-20 11:28:47.000000 starrailcard-2.2.0/starrailcard/src/generator/style_relict_score.py
--rw-rw-rw-   0        0        0    30954 2024-05-20 11:29:47.000000 starrailcard-2.2.0/starrailcard/src/generator/style_ticket.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.098223 starrailcard-2.2.0/starrailcard/src/model/
--rw-rw-rw-   0        0        0     4352 2024-05-20 11:35:59.000000 starrailcard-2.2.0/starrailcard/src/model/StarRailCard.py
--rw-rw-rw-   0        0        0    12740 2024-05-20 11:41:22.000000 starrailcard-2.2.0/starrailcard/src/model/api_mihomo.py
--rw-rw-rw-   0        0        0     8565 2024-05-10 22:49:33.000000 starrailcard-2.2.0/starrailcard/src/model/style.py
--rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.2.0/starrailcard/src/model/ukrainization_model.py
--rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.2.0/starrailcard/src/model/utils_model.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.105222 starrailcard-2.2.0/starrailcard/src/tools/
--rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.2.0/starrailcard/src/tools/cache.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.105222 starrailcard-2.2.0/starrailcard/src/tools/calculator/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.106222 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.124700 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/
--rw-rw-rw-   0        0        0      373 2024-05-19 22:33:34.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/max.json
--rw-rw-rw-   0        0        0       49 2024-05-19 22:33:34.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-rw-rw-   0        0        0     3434 2024-05-19 22:33:34.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-rw-rw-   0        0        0   100343 2024-05-19 22:33:35.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/score.json
--rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/utils.py
--rw-rw-rw-   0        0        0     5912 2024-05-19 22:51:06.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/stats.py
--rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.2.0/starrailcard/src/tools/enums.py
--rw-rw-rw-   0        0        0    12292 2024-05-10 21:23:50.000000 starrailcard-2.2.0/starrailcard/src/tools/git.py
--rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.2.0/starrailcard/src/tools/http.py
--rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.2.0/starrailcard/src/tools/json_data.py
--rw-rw-rw-   0        0        0     8371 2024-05-17 19:30:07.000000 starrailcard-2.2.0/starrailcard/src/tools/options.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.130206 starrailcard-2.2.0/starrailcard/src/tools/pill/
--rw-rw-rw-   0        0        0      220 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/color.py
--rw-rw-rw-   0        0        0     2328 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/color_control.py
--rw-rw-rw-   0        0        0     5277 2024-05-10 21:27:12.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/diagrama.py
--rw-rw-rw-   0        0        0     5517 2024-05-10 21:26:51.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/gradient_v2.py
--rw-rw-rw-   0        0        0     3279 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/grandient_v1.py
--rw-rw-rw-   0        0        0     5481 2024-05-12 09:44:45.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/image_control.py
--rw-rw-rw-   0        0        0     5717 2024-05-16 23:08:35.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/style_editor.py
--rw-rw-rw-   0        0        0     2116 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/text_control.py
--rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.2.0/starrailcard/src/tools/translator.py
--rw-rw-rw-   0        0        0     8286 2024-05-09 19:05:04.000000 starrailcard-2.2.0/starrailcard/src/tools/treePaths.py
--rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.2.0/starrailcard/src/tools/ukrainization.py
--rw-rw-rw-   0        0        0     6884 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.130206 starrailcard-2.2.0/starrailcard.egg-info/
--rw-rw-rw-   0        0        0     4762 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2159 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.898784 starrailcard-2.2.1/
+-rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4762 2024-05-31 21:38:44.897282 starrailcard-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.2.1/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 21:38:44.898784 starrailcard-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2024-05-11 16:52:16.000000 starrailcard-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.738833 starrailcard-2.2.1/starrailcard/
+-rw-rw-rw-   0        0        0     1967 2024-05-31 21:38:28.000000 starrailcard-2.2.1/starrailcard/__init__.py
+-rw-rw-rw-   0        0        0    25277 2024-05-28 18:44:44.000000 starrailcard-2.2.1/starrailcard/client.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.727777 starrailcard-2.2.1/starrailcard/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.783108 starrailcard-2.2.1/starrailcard/src/api/
+-rw-rw-rw-   0        0        0     3740 2024-05-19 22:23:39.000000 starrailcard-2.2.1/starrailcard/src/api/api.py
+-rw-rw-rw-   0        0        0     5896 2024-05-28 19:00:51.000000 starrailcard-2.2.1/starrailcard/src/api/enka.py
+-rw-rw-rw-   0        0        0    27773 2024-05-20 10:45:25.000000 starrailcard-2.2.1/starrailcard/src/api/enka_parsed.py
+-rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.2.1/starrailcard/src/api/error.py
+-rw-rw-rw-   0        0        0     2203 2024-05-28 18:53:40.000000 starrailcard-2.2.1/starrailcard/src/api/hoyolab.py
+-rw-rw-rw-   0        0        0    28814 2024-05-20 09:23:13.000000 starrailcard-2.2.1/starrailcard/src/api/hoyolab_parsed.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.726777 starrailcard-2.2.1/starrailcard/src/assets/
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.787108 starrailcard-2.2.1/starrailcard/src/assets/font/
+-rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.2.1/starrailcard/src/assets/font/font_hsr.ttf
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.810665 starrailcard-2.2.1/starrailcard/src/data/
+-rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/avatar.json
+-rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/element.json
+-rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/keys.json
+-rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/paths.json
+-rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/relict_sets.json
+-rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/stats.json
+-rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.2.1/starrailcard/src/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.813667 starrailcard-2.2.1/starrailcard/src/generator/
+-rw-rw-rw-   0        0        0    26195 2024-05-20 11:30:55.000000 starrailcard-2.2.1/starrailcard/src/generator/style_card.py
+-rw-rw-rw-   0        0        0     6675 2024-05-17 19:35:00.000000 starrailcard-2.2.1/starrailcard/src/generator/style_profile_phone.py
+-rw-rw-rw-   0        0        0    24987 2024-05-20 11:28:47.000000 starrailcard-2.2.1/starrailcard/src/generator/style_relict_score.py
+-rw-rw-rw-   0        0        0    30954 2024-05-20 11:29:47.000000 starrailcard-2.2.1/starrailcard/src/generator/style_ticket.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.830676 starrailcard-2.2.1/starrailcard/src/model/
+-rw-rw-rw-   0        0        0     4352 2024-05-20 11:35:59.000000 starrailcard-2.2.1/starrailcard/src/model/StarRailCard.py
+-rw-rw-rw-   0        0        0    12740 2024-05-20 11:41:22.000000 starrailcard-2.2.1/starrailcard/src/model/api_mihomo.py
+-rw-rw-rw-   0        0        0     8565 2024-05-10 22:49:33.000000 starrailcard-2.2.1/starrailcard/src/model/style.py
+-rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.2.1/starrailcard/src/model/ukrainization_model.py
+-rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.2.1/starrailcard/src/model/utils_model.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.861766 starrailcard-2.2.1/starrailcard/src/tools/
+-rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.2.1/starrailcard/src/tools/cache.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.866768 starrailcard-2.2.1/starrailcard/src/tools/calculator/
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.871272 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.891282 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/
+-rw-rw-rw-   0        0        0      373 2024-05-19 22:33:34.000000 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-rw-rw-   0        0        0       49 2024-05-19 22:33:34.000000 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-rw-rw-   0        0        0     3434 2024-05-19 22:33:34.000000 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-rw-rw-   0        0        0   100343 2024-05-19 22:33:35.000000 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.2.1/starrailcard/src/tools/calculator/src/utils.py
+-rw-rw-rw-   0        0        0     5912 2024-05-19 22:51:06.000000 starrailcard-2.2.1/starrailcard/src/tools/calculator/stats.py
+-rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.2.1/starrailcard/src/tools/enums.py
+-rw-rw-rw-   0        0        0    12292 2024-05-10 21:23:50.000000 starrailcard-2.2.1/starrailcard/src/tools/git.py
+-rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.2.1/starrailcard/src/tools/http.py
+-rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.2.1/starrailcard/src/tools/json_data.py
+-rw-rw-rw-   0        0        0     8371 2024-05-17 19:30:07.000000 starrailcard-2.2.1/starrailcard/src/tools/options.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.896282 starrailcard-2.2.1/starrailcard/src/tools/pill/
+-rw-rw-rw-   0        0        0      220 2024-05-10 22:00:17.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-05-10 22:00:17.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/color.py
+-rw-rw-rw-   0        0        0     2328 2024-05-10 22:00:17.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/color_control.py
+-rw-rw-rw-   0        0        0     5277 2024-05-10 21:27:12.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/diagrama.py
+-rw-rw-rw-   0        0        0     5517 2024-05-10 21:26:51.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/gradient_v2.py
+-rw-rw-rw-   0        0        0     3279 2024-05-10 22:00:17.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/grandient_v1.py
+-rw-rw-rw-   0        0        0     5481 2024-05-12 09:44:45.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/image_control.py
+-rw-rw-rw-   0        0        0     5717 2024-05-16 23:08:35.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/style_editor.py
+-rw-rw-rw-   0        0        0     2116 2024-05-10 22:00:17.000000 starrailcard-2.2.1/starrailcard/src/tools/pill/text_control.py
+-rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.2.1/starrailcard/src/tools/translator.py
+-rw-rw-rw-   0        0        0     8286 2024-05-09 19:05:04.000000 starrailcard-2.2.1/starrailcard/src/tools/treePaths.py
+-rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.2.1/starrailcard/src/tools/ukrainization.py
+-rw-rw-rw-   0        0        0     6884 2024-05-10 22:00:17.000000 starrailcard-2.2.1/starrailcard/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 21:38:44.897282 starrailcard-2.2.1/starrailcard.egg-info/
+-rw-rw-rw-   0        0        0     4762 2024-05-31 21:38:44.000000 starrailcard-2.2.1/starrailcard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2024-05-31 21:38:44.000000 starrailcard-2.2.1/starrailcard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 21:38:44.000000 starrailcard-2.2.1/starrailcard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-05-31 21:38:44.000000 starrailcard-2.2.1/starrailcard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 21:38:44.000000 starrailcard-2.2.1/starrailcard.egg-info/top_level.txt
```

### Comparing `starrailcard-2.2.0/LICENSE` & `starrailcard-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/PKG-INFO` & `starrailcard-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.2.0
+Version: 2.2.1
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai,genshin,build,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `starrailcard-2.2.0/README.md` & `starrailcard-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/pyproject.toml` & `starrailcard-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/setup.py` & `starrailcard-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/__init__.py` & `starrailcard-2.2.1/starrailcard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 __title__ = 'StarRailCard.py'
 __author__ = 'DeviantUa'
-__version__ = '2.2.0'
+__version__ = '2.2.1'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 from .client import *
 from .utils import *
 from .src.tools.enums import *
```

### Comparing `starrailcard-2.2.0/starrailcard/client.py` & `starrailcard-2.2.1/starrailcard/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,19 +160,19 @@
                             color = None
                         
                         art = None
                         if self.character_art:
                             if str(key.id) in self.character_art:
                                 art = self.character_art[str(key.id)]
                         if style == 1:
-                            result.append(await style_relict_score.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo, color).start(True))
+                            result.append(await style_relict_score.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo, color).start(hoyo = True))
                         elif style == 2:
-                            result.append(await style_ticket.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo, color).start(True))
+                            result.append(await style_ticket.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo, color).start(hoyo = True))
                         elif style == 3:
-                            result.append(await style_card.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo, color).start(True))
+                            result.append(await style_card.Create(key,self.translateLang,art,hide_uid,uid, self.seeleland,self.remove_logo, color).start(hoyo = True))
                     except Exception as e:
                         print(f"Error in get_result for character {key.id}: {e}")
                         
                 tasks.start_soon(get_result, key)
                     
         response["card"] = result
```

### Comparing `starrailcard-2.2.0/starrailcard/src/api/api.py` & `starrailcard-2.2.1/starrailcard/src/api/api.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/api/enka.py` & `starrailcard-2.2.1/starrailcard/src/api/enka.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         for name in _INDEX_NAME:
             for langs in SUPPORTED_LANGUAGES:
                 if langs == "ua":
                     continue
                 if not lang is None:
                     if langs != lang:
                         continue
-                data = await http.AioSession.get(_INDEX_MIHOMO.format(lang = lang, index=name))
-                if not os.path.exists(PathData.ENKA_INDEX.value / lang):
-                    os.makedirs(PathData.ENKA_INDEX.value / lang)
-                await JsonManager(PathData.ENKA_INDEX.value / lang /f"{name}.json").write(data)
+                data = await http.AioSession.get(_INDEX_MIHOMO.format(lang = langs, index=name))
+                if not os.path.exists(PathData.ENKA_INDEX.value / langs):
+                    os.makedirs(PathData.ENKA_INDEX.value / langs)
+                await JsonManager(PathData.ENKA_INDEX.value / langs /f"{name}.json").write(data)
                 
             print(f"- Updated file: {name}")
         print("===END UPDATE ASSET===")
```

### Comparing `starrailcard-2.2.0/starrailcard/src/api/enka_parsed.py` & `starrailcard-2.2.1/starrailcard/src/api/enka_parsed.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/api/hoyolab.py` & `starrailcard-2.2.1/starrailcard/src/api/hoyolab.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 from typing import Optional, Union
 from .api import ApiMiHoMo
 from ..model import api_mihomo
 from ..tools import http, translator, options, ukrainization
 from .error import StarRailCardError
 from .hoyolab_parsed import AssetHoYoLabParsed
 
-try:
-    import genshin
-    import_genshin = True
-except ImportError as e:
-    import_genshin = False
     
 LANG_MAP = {
     "zh-CN": "zh-cn",
     "zh-TW": "zh-tw",
     "de": "de-de",
     "en": "en-us",
     "es": "es-es",
@@ -45,15 +40,17 @@
             self.lang = "en"
         
         self.convert_lang = LANG_MAP.get(self.lang)
 
 
 
     async def get(self,cookie: dict, uid: Union[str,int] = 0):
-        if not import_genshin:
+        try:
+            import genshin
+        except ImportError:
             raise StarRailCardError(100, "Install the genshin.py module\n- pip install genshin")
         
         if uid == 0:
             uid = self.uid
             if uid == 0:
                 raise StarRailCardError(5, "Specify UID")
```

### Comparing `starrailcard-2.2.0/starrailcard/src/api/hoyolab_parsed.py` & `starrailcard-2.2.1/starrailcard/src/api/hoyolab_parsed.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.2.1/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/data/avatar.json` & `starrailcard-2.2.1/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/data/relict_sets.json` & `starrailcard-2.2.1/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/data/stats.json` & `starrailcard-2.2.1/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/data/weapons.json` & `starrailcard-2.2.1/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/generator/style_card.py` & `starrailcard-2.2.1/starrailcard/src/generator/style_card.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.2.1/starrailcard/src/generator/style_profile_phone.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.2.1/starrailcard/src/generator/style_relict_score.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.2.1/starrailcard/src/generator/style_ticket.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.2.1/starrailcard/src/model/StarRailCard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.2.1/starrailcard/src/model/api_mihomo.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/model/style.py` & `starrailcard-2.2.1/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/model/utils_model.py` & `starrailcard-2.2.1/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/cache.py` & `starrailcard-2.2.1/starrailcard/src/tools/cache.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.2.1/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.2.1/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.2.1/starrailcard/src/tools/calculator/stats.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/enums.py` & `starrailcard-2.2.1/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/git.py` & `starrailcard-2.2.1/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/http.py` & `starrailcard-2.2.1/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/json_data.py` & `starrailcard-2.2.1/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/options.py` & `starrailcard-2.2.1/starrailcard/src/tools/options.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/color.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/color_control.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/color_control.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/diagrama.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/diagrama.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/gradient_v2.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/gradient_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/image_control.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/image_control.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/pill/text_control.py` & `starrailcard-2.2.1/starrailcard/src/tools/pill/text_control.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/translator.py` & `starrailcard-2.2.1/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/treePaths.py` & `starrailcard-2.2.1/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.2.1/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard/utils.py` & `starrailcard-2.2.1/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.2.0/starrailcard.egg-info/PKG-INFO` & `starrailcard-2.2.1/starrailcard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.2.0
+Version: 2.2.1
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai,genshin,build,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `starrailcard-2.2.0/starrailcard.egg-info/SOURCES.txt` & `starrailcard-2.2.1/starrailcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

