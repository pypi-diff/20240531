# Comparing `tmp/mhmzx_little_paimon-3.0.15.tar.gz` & `tmp/mhmzx_little_paimon-3.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhmzx_little_paimon-3.0.15.tar", max compression
+gzip compressed data, was "mhmzx_little_paimon-3.0.16.tar", max compression
```

## Comparing `mhmzx_little_paimon-3.0.15.tar` & `mhmzx_little_paimon-3.0.16.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0    34523 2023-10-03 11:58:12.363188 mhmzx_little_paimon-3.0.15/LICENSE
--rw-r--r--   0        0        0     3118 2023-10-04 07:14:41.385648 mhmzx_little_paimon-3.0.15/LittlePaimon/__init__.py
--rw-r--r--   0        0        0      186 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/__init__.py
--rw-r--r--   0        0        0     1665 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/command/__init__.py
--rw-r--r--   0        0        0     1752 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/manage.py
--rw-r--r--   0        0        0     3423 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/model.py
--rw-r--r--   0        0        0    37053 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/alias.json
--rw-r--r--   0        0        0    35968 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/artifact.json
--rw-r--r--   0        0        0    25724 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/ban_word.txt
--rw-r--r--   0        0        0    57930 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/genshin_info.json
--rw-r--r--   0        0        0     1508 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/prop.json
--rw-r--r--   0        0        0    44920 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_skill.json
--rw-r--r--   0        0        0    34331 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_talent.json
--rw-r--r--   0        0        0  1377336 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/roles_data.json
--rw-r--r--   0        0        0    25343 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/score.json
--rw-r--r--   0        0        0      949 2023-10-03 14:13:02.126748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/upheaval.json
--rw-r--r--   0        0        0    22390 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/weapon.json
--rw-r--r--   0        0        0     7744 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/类型.json
--rw-r--r--   0        0        0     8927 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/manage.py
--rw-r--r--   0        0        0      795 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/model.py
--rw-r--r--   0        0        0     4161 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/__init__.py
--rw-r--r--   0        0        0      308 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/__init__.py
--rw-r--r--   0        0        0    11634 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/abyss_info.py
--rw-r--r--   0        0        0    20220 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/character.py
--rw-r--r--   0        0        0     2602 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/cookie.py
--rw-r--r--   0        0        0     1234 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/genshin_voice.py
--rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/manage.py
--rw-r--r--   0        0        0      451 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/memory_db.py
--rw-r--r--   0        0        0      782 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/other.py
--rw-r--r--   0        0        0    12879 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/player_info.py
--rw-r--r--   0        0        0     3546 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/subscription.py
--rw-r--r--   0        0        0     4573 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/__init__.py
--rw-r--r--   0        0        0     6849 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/event.py
--rw-r--r--   0        0        0     2540 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/generate.py
--rw-r--r--   0        0        0     2466 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html
--rw-r--r--   0        0        0     6882 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/index.css
--rw-r--r--   0        0        0   315626 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/iview.css
--rw-r--r--   0        0        0     6346 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css
--rw-r--r--   0        0        0   158333 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg
--rw-r--r--   0        0        0     4436 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/__init__.py
--rw-r--r--   0        0        0     2535 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/draw.py
--rw-r--r--   0        0        0     5816 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/handler.py
--rw-r--r--   0        0        0     3565 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/resources.py
--rw-r--r--   0        0        0     3382 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/__init__.py
--rw-r--r--   0        0        0     3046 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/config.py
--rw-r--r--   0        0        0     6587 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/genshin_word.txt
--rw-r--r--   0        0        0    30915 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/handler.py
--rw-r--r--   0        0        0     3970 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/models.py
--rw-r--r--   0        0        0     9972 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_api.py
--rw-r--r--   0        0        0    23060 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_page.py
--rw-r--r--   0        0        0     1306 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Mihoyo_bbs/__init__.py
--rw-r--r--   0        0        0    10040 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/__init__.py
--rw-r--r--   0        0        0     1235 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/config.py
--rw-r--r--   0        0        0     3343 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/__init__.py
--rw-r--r--   0        0        0    16481 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py
--rw-r--r--   0        0        0    13495 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py
--rw-r--r--   0        0        0       28 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/__init__.py
--rw-r--r--   0        0        0     1727 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py
--rw-r--r--   0        0        0     3552 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py
--rw-r--r--   0        0        0      991 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py
--rw-r--r--   0        0        0     8135 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/__init__.py
--rw-r--r--   0        0        0    14974 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py
--rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/draw.py
--rw-r--r--   0        0        0     8833 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py
--rw-r--r--   0        0        0    20499 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/__init__.py
--rw-r--r--   0        0        0    11054 2023-12-07 13:48:58.774988 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/get_cookie.py
--rw-r--r--   0        0        0     4387 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py
--rw-r--r--   0        0        0     1768 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/api.py
--rw-r--r--   0        0        0     3894 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py
--rw-r--r--   0        0        0     3147 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/__init__.py
--rw-r--r--   0        0        0     9780 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/draw.py
--rw-r--r--   0        0        0     7660 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/handler.py
--rw-r--r--   0        0        0    10565 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/__init__.py
--rw-r--r--   0        0        0     1341 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_handle.py
--rw-r--r--   0        0        0     7925 2023-11-29 06:20:17.596561 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_source.py
--rw-r--r--   0        0        0     4364 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/draw.py
--rw-r--r--   0        0        0     8158 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py
--rw-r--r--   0        0        0    10507 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py
--rw-r--r--   0        0        0    13429 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py
--rw-r--r--   0        0        0     3852 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/models.py
--rw-r--r--   0        0        0    15959 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/__init__.py
--rw-r--r--   0        0        0    11703 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_cal.py
--rw-r--r--   0        0        0    65408 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_model.py
--rw-r--r--   0        0        0    10845 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py
--rw-r--r--   0        0        0     7799 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_card.py
--rw-r--r--   0        0        0    14100 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py
--rw-r--r--   0        0        0     9721 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_player_card.py
--rw-r--r--   0        0        0     1502 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py
--rw-r--r--   0        0        0     3990 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/draw.py
--rw-r--r--   0        0        0     1431 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/handler.py
--rw-r--r--   0        0        0      123 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/Atlas/__init__.py
--rw-r--r--   0        0        0     2029 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py
--rw-r--r--   0        0        0       37 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/__init__.py
--rw-r--r--   0        0        0     3357 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py
--rw-r--r--   0        0        0     5089 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py
--rw-r--r--   0        0        0      209 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/models.py
--rw-r--r--   0        0        0    22279 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/__init__.py
--rw-r--r--   0        0        0     7572 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py
--rw-r--r--   0        0        0     8754 2023-11-29 04:10:49.880595 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_map.py
--rw-r--r--   0        0        0      888 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py
--rw-r--r--   0        0        0      446 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/exc.py
--rw-r--r--   0        0        0     2600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py
--rw-r--r--   0        0        0     3573 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py
--rw-r--r--   0        0        0     4320 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py
--rw-r--r--   0        0        0     2902 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py
--rw-r--r--   0        0        0     1231 2023-11-02 02:35:17.358460 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py
--rw-r--r--   0        0        0     7228 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/bot_manager/__init__.py
--rw-r--r--   0        0        0     4615 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/news60s/__init__.py
--rw-r--r--   0        0        0     8537 2023-12-07 12:31:51.791454 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/__init__.py
--rw-r--r--   0        0        0     5192 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/draw_help.py
--rw-r--r--   0        0        0     1443 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/tools/__init__.py
--rw-r--r--   0        0        0      607 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/__init__.py
--rw-r--r--   0        0        0     6214 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/alias.py
--rw-r--r--   0        0        0    18691 2024-05-03 13:28:19.726888 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/api.py
--rw-r--r--   0        0        0     3844 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/browser.py
--rw-r--r--   0        0        0     2695 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/files.py
--rw-r--r--   0        0        0     2420 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/filter.py
--rw-r--r--   0        0        0    19469 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/genshin.py
--rw-r--r--   0        0        0    22406 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/image.py
--rw-r--r--   0        0        0     1380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/logger.py
--rw-r--r--   0        0        0    14786 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/message.py
--rw-r--r--   0        0        0     2380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/path.py
--rw-r--r--   0        0        0     9531 2023-11-29 04:13:41.406015 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/requests.py
--rw-r--r--   0        0        0     1254 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/scheduler.py
--rw-r--r--   0        0        0     1600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/status.py
--rw-r--r--   0        0        0     5838 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/tool.py
--rw-r--r--   0        0        0     3829 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/typing.py
--rw-r--r--   0        0        0     4568 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/update.py
--rw-r--r--   0        0        0     2576 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.15/LittlePaimon/web/__init__.py
--rw-r--r--   0        0        0      655 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/__init__.py
--rw-r--r--   0        0        0     4853 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/bot_info.py
--rw-r--r--   0        0        0     1807 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/command_alias.py
--rw-r--r--   0        0        0    15631 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/cookie.py
--rw-r--r--   0        0        0      791 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/login.py
--rw-r--r--   0        0        0     6463 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/plugin.py
--rw-r--r--   0        0        0     1974 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/status.py
--rw-r--r--   0        0        0     1081 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/utils.py
--rw-r--r--   0        0        0      112 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/__init__.py
--rw-r--r--   0        0        0     1651 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/bind_cookie.py
--rw-r--r--   0        0        0     3525 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/command_alias.py
--rw-r--r--   0        0        0    16990 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/config_manage.py
--rw-r--r--   0        0        0      347 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/constants.py
--rw-r--r--   0        0        0     5482 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/home_page.py
--rw-r--r--   0        0        0     1903 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/login.py
--rw-r--r--   0        0        0     1816 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/main.py
--rw-r--r--   0        0        0     8089 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/plugin_manage.py
--rw-r--r--   0        0        0     6613 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/private_cookie.py
--rw-r--r--   0        0        0     3067 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/public_cookie.py
--rw-r--r--   0        0        0     1251 2024-05-03 13:29:30.667635 mhmzx_little_paimon-3.0.15/pyproject.toml
--rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mhmzx_little_paimon-3.0.15/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-10-03 11:58:12.363188 mhmzx_little_paimon-3.0.16/LICENSE
+-rw-r--r--   0        0        0     3118 2023-10-04 07:14:41.385648 mhmzx_little_paimon-3.0.16/LittlePaimon/__init__.py
+-rw-r--r--   0        0        0      186 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/__init__.py
+-rw-r--r--   0        0        0     1665 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/command/__init__.py
+-rw-r--r--   0        0        0     1752 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/config/manage.py
+-rw-r--r--   0        0        0     3423 2024-05-31 10:02:11.059629 mhmzx_little_paimon-3.0.16/LittlePaimon/config/config/model.py
+-rw-r--r--   0        0        0    37053 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/alias.json
+-rw-r--r--   0        0        0    35968 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/artifact.json
+-rw-r--r--   0        0        0    25724 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/ban_word.txt
+-rw-r--r--   0        0        0    57930 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/genshin_info.json
+-rw-r--r--   0        0        0     1508 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/prop.json
+-rw-r--r--   0        0        0    44920 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/role_skill.json
+-rw-r--r--   0        0        0    34331 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/role_talent.json
+-rw-r--r--   0        0        0  1377336 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/roles_data.json
+-rw-r--r--   0        0        0    25343 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/score.json
+-rw-r--r--   0        0        0      949 2023-10-03 14:13:02.126748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/upheaval.json
+-rw-r--r--   0        0        0    22390 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/weapon.json
+-rw-r--r--   0        0        0     7744 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/类型.json
+-rw-r--r--   0        0        0     8927 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.16/LittlePaimon/config/plugin/manage.py
+-rw-r--r--   0        0        0      795 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/config/plugin/model.py
+-rw-r--r--   0        0        0     4161 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/__init__.py
+-rw-r--r--   0        0        0      308 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/__init__.py
+-rw-r--r--   0        0        0    11634 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/abyss_info.py
+-rw-r--r--   0        0        0    20220 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/character.py
+-rw-r--r--   0        0        0     2602 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/cookie.py
+-rw-r--r--   0        0        0     1234 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/genshin_voice.py
+-rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/manage.py
+-rw-r--r--   0        0        0      451 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/memory_db.py
+-rw-r--r--   0        0        0      782 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/other.py
+-rw-r--r--   0        0        0    12879 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/player_info.py
+-rw-r--r--   0        0        0     3546 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/subscription.py
+-rw-r--r--   0        0        0     4573 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/__init__.py
+-rw-r--r--   0        0        0     6849 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/event.py
+-rw-r--r--   0        0        0     2540 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/generate.py
+-rw-r--r--   0        0        0     2466 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html
+-rw-r--r--   0        0        0     6882 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/index.css
+-rw-r--r--   0        0        0   315626 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/iview.css
+-rw-r--r--   0        0        0     6346 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css
+-rw-r--r--   0        0        0   158333 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg
+-rw-r--r--   0        0        0     4436 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/__init__.py
+-rw-r--r--   0        0        0     2535 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/draw.py
+-rw-r--r--   0        0        0     5816 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/handler.py
+-rw-r--r--   0        0        0     3565 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/resources.py
+-rw-r--r--   0        0        0     3382 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/__init__.py
+-rw-r--r--   0        0        0     3046 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/config.py
+-rw-r--r--   0        0        0     6587 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/genshin_word.txt
+-rw-r--r--   0        0        0    30915 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/handler.py
+-rw-r--r--   0        0        0     3970 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/models.py
+-rw-r--r--   0        0        0     9972 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/web_api.py
+-rw-r--r--   0        0        0    23060 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/web_page.py
+-rw-r--r--   0        0        0     1306 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Mihoyo_bbs/__init__.py
+-rw-r--r--   0        0        0    10040 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/NoticeAndRequest/__init__.py
+-rw-r--r--   0        0        0     1235 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/NoticeAndRequest/config.py
+-rw-r--r--   0        0        0     3343 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/__init__.py
+-rw-r--r--   0        0        0    16481 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py
+-rw-r--r--   0        0        0    13495 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py
+-rw-r--r--   0        0        0       28 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/__init__.py
+-rw-r--r--   0        0        0     1727 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py
+-rw-r--r--   0        0        0     3552 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py
+-rw-r--r--   0        0        0      991 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py
+-rw-r--r--   0        0        0     8135 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/__init__.py
+-rw-r--r--   0        0        0    14974 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py
+-rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/draw.py
+-rw-r--r--   0        0        0     8833 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py
+-rw-r--r--   0        0        0    20499 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Bind/__init__.py
+-rw-r--r--   0        0        0    11054 2023-12-07 13:48:58.774988 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Bind/get_cookie.py
+-rw-r--r--   0        0        0     4387 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py
+-rw-r--r--   0        0        0     1768 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_CloudGenshin/api.py
+-rw-r--r--   0        0        0     3894 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py
+-rw-r--r--   0        0        0     3147 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_DailyNote/__init__.py
+-rw-r--r--   0        0        0     9780 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_DailyNote/draw.py
+-rw-r--r--   0        0        0     7660 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_DailyNote/handler.py
+-rw-r--r--   0        0        0    10565 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/__init__.py
+-rw-r--r--   0        0        0     1341 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/data_handle.py
+-rw-r--r--   0        0        0     7925 2023-11-29 06:20:17.596561 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/data_source.py
+-rw-r--r--   0        0        0     4364 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/draw.py
+-rw-r--r--   0        0        0     8158 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py
+-rw-r--r--   0        0        0    10507 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py
+-rw-r--r--   0        0        0    13429 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py
+-rw-r--r--   0        0        0     3852 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/models.py
+-rw-r--r--   0        0        0    15959 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/__init__.py
+-rw-r--r--   0        0        0    11703 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/damage_cal.py
+-rw-r--r--   0        0        0    65408 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/damage_model.py
+-rw-r--r--   0        0        0    10845 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py
+-rw-r--r--   0        0        0     7799 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_character_card.py
+-rw-r--r--   0        0        0    14100 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py
+-rw-r--r--   0        0        0     9721 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_player_card.py
+-rw-r--r--   0        0        0     1502 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py
+-rw-r--r--   0        0        0     3990 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_MonthInfo/draw.py
+-rw-r--r--   0        0        0     1431 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_MonthInfo/handler.py
+-rw-r--r--   0        0        0      123 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/Atlas/__init__.py
+-rw-r--r--   0        0        0     2029 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py
+-rw-r--r--   0        0        0       37 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/__init__.py
+-rw-r--r--   0        0        0     3357 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py
+-rw-r--r--   0        0        0     5089 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py
+-rw-r--r--   0        0        0      209 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/models.py
+-rw-r--r--   0        0        0    22279 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/__init__.py
+-rw-r--r--   0        0        0     7572 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py
+-rw-r--r--   0        0        0     8754 2023-11-29 04:10:49.880595 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/draw_map.py
+-rw-r--r--   0        0        0      888 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py
+-rw-r--r--   0        0        0      446 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/exc.py
+-rw-r--r--   0        0        0     2600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py
+-rw-r--r--   0        0        0     3573 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py
+-rw-r--r--   0        0        0     4320 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py
+-rw-r--r--   0        0        0     2902 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py
+-rw-r--r--   0        0        0     1231 2023-11-02 02:35:17.358460 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py
+-rw-r--r--   0        0        0     7228 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/bot_manager/__init__.py
+-rw-r--r--   0        0        0     4615 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/news60s/__init__.py
+-rw-r--r--   0        0        0     8537 2023-12-07 12:31:51.791454 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/plugin_manager/__init__.py
+-rw-r--r--   0        0        0     5192 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/plugin_manager/draw_help.py
+-rw-r--r--   0        0        0     1443 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/tools/__init__.py
+-rw-r--r--   0        0        0      607 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/__init__.py
+-rw-r--r--   0        0        0     6214 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/alias.py
+-rw-r--r--   0        0        0    18691 2024-05-03 13:28:19.726888 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/api.py
+-rw-r--r--   0        0        0     3844 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/browser.py
+-rw-r--r--   0        0        0     2695 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/files.py
+-rw-r--r--   0        0        0     2420 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/filter.py
+-rw-r--r--   0        0        0    19469 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/genshin.py
+-rw-r--r--   0        0        0    22406 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/image.py
+-rw-r--r--   0        0        0     1380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/logger.py
+-rw-r--r--   0        0        0    14786 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/message.py
+-rw-r--r--   0        0        0     2380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/path.py
+-rw-r--r--   0        0        0     9531 2023-11-29 04:13:41.406015 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/requests.py
+-rw-r--r--   0        0        0     1254 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/scheduler.py
+-rw-r--r--   0        0        0     1600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/status.py
+-rw-r--r--   0        0        0     5805 2024-05-31 10:02:11.059629 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/tool.py
+-rw-r--r--   0        0        0     3829 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/typing.py
+-rw-r--r--   0        0        0     4568 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/utils/update.py
+-rw-r--r--   0        0        0     2576 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.16/LittlePaimon/web/__init__.py
+-rw-r--r--   0        0        0      655 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/__init__.py
+-rw-r--r--   0        0        0     4853 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/bot_info.py
+-rw-r--r--   0        0        0     1807 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/command_alias.py
+-rw-r--r--   0        0        0    15631 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/cookie.py
+-rw-r--r--   0        0        0      791 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/login.py
+-rw-r--r--   0        0        0     6463 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/plugin.py
+-rw-r--r--   0        0        0     1974 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/status.py
+-rw-r--r--   0        0        0     1081 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/utils.py
+-rw-r--r--   0        0        0      112 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/__init__.py
+-rw-r--r--   0        0        0     1651 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/bind_cookie.py
+-rw-r--r--   0        0        0     3525 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/command_alias.py
+-rw-r--r--   0        0        0    16990 2024-05-31 10:02:11.059629 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/config_manage.py
+-rw-r--r--   0        0        0      347 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/constants.py
+-rw-r--r--   0        0        0     5482 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/home_page.py
+-rw-r--r--   0        0        0     1903 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/login.py
+-rw-r--r--   0        0        0     1816 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/main.py
+-rw-r--r--   0        0        0     8089 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/plugin_manage.py
+-rw-r--r--   0        0        0     6613 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/private_cookie.py
+-rw-r--r--   0        0        0     3067 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/public_cookie.py
+-rw-r--r--   0        0        0     1251 2024-05-31 10:02:41.887630 mhmzx_little_paimon-3.0.16/pyproject.toml
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mhmzx_little_paimon-3.0.16/PKG-INFO
```

### Comparing `mhmzx_little_paimon-3.0.15/LICENSE` & `mhmzx_little_paimon-3.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/command/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/command/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/manage.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/config/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/model.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/config/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     command_alias_enable: bool = Field(True, alias='启用命令别名')
     browser_type: Literal['chromium', 'firefox', 'webkit'] = Field('firefox', alias='浏览器内核')
 
     # 早报60s
     morning_news: str = Field('https://api.vvhan.com/api/60s', alias='早报60s')
 
-    github_proxy: str = Field('https://github.cherishmoon.fun/', alias='github资源地址')
+    github_proxy: str = Field('https://github.cherishmoon.top/', alias='github资源地址')
 
     @property
     def alias_dict(self):
         return {v.alias: k for k, v in self.__fields__.items()}
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
```

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/alias.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/alias.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/artifact.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/artifact.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/ban_word.txt` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/ban_word.txt`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/genshin_info.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/genshin_info.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/prop.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/prop.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_skill.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/role_skill.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_talent.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/role_talent.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/roles_data.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/roles_data.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/score.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/score.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/upheaval.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/upheaval.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/weapon.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/weapon.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/类型.json` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/data/类型.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/manage.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/plugin/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/model.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/config/plugin/model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/abyss_info.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/abyss_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/character.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/character.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/cookie.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/genshin_voice.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/genshin_voice.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/manage.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/other.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/other.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/player_info.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/player_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/subscription.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/database/models/subscription.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/event.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/event.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/generate.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/generate.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/index.css` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/index.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/iview.css` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/iview.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/handler.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/resources.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Genshin_Voice/resources.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/config.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/config.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/genshin_word.txt` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/genshin_word.txt`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/handler.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/models.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/web_api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_page.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Learning_Chat/web_page.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Mihoyo_bbs/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Mihoyo_bbs/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/NoticeAndRequest/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/config.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/NoticeAndRequest/config.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Bind/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/get_cookie.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Bind/get_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_CloudGenshin/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_DailyNote/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_DailyNote/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/handler.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_DailyNote/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_handle.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/data_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_source.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/data_source.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/models.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Gacha_Log/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_cal.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/damage_cal.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_model.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/damage_model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_card.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_character_card.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_player_card.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Info/draw_player_card.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_MonthInfo/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/handler.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_MonthInfo/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_map.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/draw_map.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/bot_manager/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/bot_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/news60s/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/news60s/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/plugin_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/draw_help.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/plugin_manager/draw_help.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/tools/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/plugins/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/alias.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/api.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/browser.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/browser.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/files.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/files.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/filter.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/filter.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/genshin.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/genshin.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/image.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/image.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/logger.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/message.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/message.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/path.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/path.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/requests.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/requests.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/scheduler.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/status.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/status.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/tool.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,32 +89,32 @@
 async def check_resource():
     logger.info('资源检查', '开始检查资源')
     if not (
             (RESOURCE_BASE_PATH / 'LittlePaimon').is_dir() and
             len(list((RESOURCE_BASE_PATH / 'LittlePaimon').rglob('*'))) >= 50):
         try:
             await aiorequests.download(
-                url=f'{config.github_proxy}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/resources.zip',
+                url=f'{config.github_proxy}https://github.com/CMHopeSunshine/LittlePaimonRes/raw/main/resources.zip',
                 save_path=RESOURCE_BASE_PATH / '小派蒙基础资源.zip')
             zipfile.ZipFile(RESOURCE_BASE_PATH / '小派蒙基础资源.zip').extractall(RESOURCE_BASE_PATH)
             (RESOURCE_BASE_PATH / '小派蒙基础资源.zip').unlink()
 
             await aiorequests.download(
-                url=f'{config.github_proxy}https://raw.githubusercontent.com/CMHopeSunshine/GenshinWikiMap/master/resources/genshin_resources.zip',
+                url=f'{config.github_proxy}https://github.com/CMHopeSunshine/GenshinWikiMap/raw/master/resources/genshin_resources.zip',
                 save_path=RESOURCE_BASE_PATH / '原神图标资源.zip')
             zipfile.ZipFile(RESOURCE_BASE_PATH / '原神图标资源.zip').extractall(RESOURCE_BASE_PATH / 'LittlePaimon')
             (RESOURCE_BASE_PATH / '原神图标资源.zip').unlink()
             logger.info('资源检查', '<g>资源下载完成</g>')
         except Exception:
             logger.warning('资源检查', '下载<m>资源包</m>时<r>出错</r>，请尝试更换<m>github资源地址</m>')
     else:
         if not (RESOURCE_BASE_PATH / 'LittlePaimon' / 'star_rail').is_dir():
             try:
                 await aiorequests.download(
-                    url=f'{config.github_proxy}https://raw.githubusercontent.com/CMHopeSunshine/LittlePaimonRes/main/star_rail.zip',
+                    url=f'{config.github_proxy}https://github.com/CMHopeSunshine/LittlePaimonRes/raw/main/star_rail.zip',
                     save_path=RESOURCE_BASE_PATH / 'star_rail.zip')
                 zipfile.ZipFile(RESOURCE_BASE_PATH / 'star_rail.zip').extractall(RESOURCE_BASE_PATH / 'LittlePaimon' / 'star_rail')
                 (RESOURCE_BASE_PATH / 'star_rail.zip').unlink()
                 logger.info('资源检查', '<g>星穹铁道相关资源下载完成</g>')
             except Exception:
                 logger.warning('资源检查', '下载<m>星穹铁道资源</m>时<r>出错</r>，请尝试更换<m>github资源地址</m>')
         try:
```

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/typing.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/typing.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/update.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/utils/update.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/__init__.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/bot_info.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/bot_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/command_alias.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/command_alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/cookie.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/login.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/login.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/plugin.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/plugin.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/status.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/status.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/utils.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/bind_cookie.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/bind_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/command_alias.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/command_alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/config_manage.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/config_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,16 +374,16 @@
             creatable=True,
             options=[
                 {
                     'label': 'ghproxy.com代理',
                     'value': 'https://ghproxy.com/'
                 },
                 {
-                    'label': 'github.cherishmoon.fun代理',
-                    'value': 'https://github.cherishmoon.fun/'
+                    'label': 'github.cherishmoon.top代理',
+                    'value': 'https://github.cherishmoon.top/'
                 },
                 {
                     'label': 'github.91chi.fun代理',
                     'value': 'https://github.91chi.fun/'
                 },
                 {
                     'label': 'github原地址',
```

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/home_page.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/login.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/login.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/main.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/main.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/plugin_manage.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/private_cookie.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/private_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/public_cookie.py` & `mhmzx_little_paimon-3.0.16/LittlePaimon/web/pages/public_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.15/pyproject.toml` & `mhmzx_little_paimon-3.0.16/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mhmzx-little-paimon"
-version = "3.0.15"
+version = "3.0.16"
 description = "（非官方）小派蒙！原神qq群机器人，基于NoneBot2的UID查询、抽卡导出分析、模拟抽卡、实时便签、札记等多功能小助手。"
 authors = ["Madray Haven <sgpublic2002@gmail.com>"]
 license = "AGPL"
 packages = [
     { include = "LittlePaimon" },
 ]
```

### Comparing `mhmzx_little_paimon-3.0.15/PKG-INFO` & `mhmzx_little_paimon-3.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhmzx-little-paimon
-Version: 3.0.15
+Version: 3.0.16
 Summary: （非官方）小派蒙！原神qq群机器人，基于NoneBot2的UID查询、抽卡导出分析、模拟抽卡、实时便签、札记等多功能小助手。
 License: AGPL
 Author: Madray Haven
 Author-email: sgpublic2002@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

