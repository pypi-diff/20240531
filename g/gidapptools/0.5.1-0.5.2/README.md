# Comparing `tmp/gidapptools-0.5.1.tar.gz` & `tmp/gidapptools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gidapptools-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gidapptools-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gidapptools-0.5.1.tar` & `gidapptools-0.5.2.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rw-r--r--   0        0        0     1064 2021-08-31 18:36:20.520000 gidapptools-0.5.1/LICENSE
--rw-r--r--   0        0        0      649 2023-04-07 20:25:45.102049 gidapptools-0.5.1/README.rst
--rw-r--r--   0        0        0      716 2024-05-28 01:33:43.196158 gidapptools-0.5.1/gidapptools/__init__.py
--rw-r--r--   0        0        0      667 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/__main__.py
--rw-r--r--   0        0        0      106 2021-09-20 21:57:04.325557 gidapptools-0.5.1/gidapptools/abstract_classes/__init__.py
--rw-r--r--   0        0        0     2098 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/abstract_classes/abstract_meta_factory.py
--rw-r--r--   0        0        0     1324 2023-01-07 14:13:46.164752 gidapptools-0.5.1/gidapptools/abstract_classes/abstract_meta_item.py
--rw-r--r--   0        0        0      585 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/cli_info.py
--rw-r--r--   0        0        0       21 2024-04-25 20:13:17.822555 gidapptools-0.5.1/gidapptools/code_generation/__init__.py
--rw-r--r--   0        0        0     5890 2024-04-25 21:29:19.094195 gidapptools-0.5.1/gidapptools/code_generation/python.py
--rw-r--r--   0        0        0      769 2023-06-19 19:52:38.610215 gidapptools-0.5.1/gidapptools/custom_types.py
--rw-r--r--   0        0        0       69 2022-01-12 13:50:02.703044 gidapptools-0.5.1/gidapptools/data/__init__.py
--rw-r--r--   0        0        0     3374 2023-08-16 03:08:15.130796 gidapptools-0.5.1/gidapptools/data/conversion_data.py
--rw-r--r--   0        0        0      126 2022-11-02 13:03:47.066458 gidapptools-0.5.1/gidapptools/data/general_data.py
--rw-r--r--   0        0        0     1035 2022-03-20 03:11:40.597216 gidapptools-0.5.1/gidapptools/data/gifs/__init__.py
--rw-r--r--   0        0        0    21837 2022-03-04 16:17:21.627813 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_1.gif
--rw-r--r--   0        0        0    28904 2022-03-04 16:31:53.112866 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_2.gif
--rw-r--r--   0        0        0   780846 2022-03-04 16:16:38.588118 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_3.gif
--rw-r--r--   0        0        0   126652 2022-03-04 16:35:31.028357 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_4.gif
--rw-r--r--   0        0        0    72232 2022-03-05 00:49:16.857127 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_5.gif
--rw-r--r--   0        0        0    77029 2022-03-05 00:49:38.490391 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_6.gif
--rw-r--r--   0        0        0    75110 2022-03-05 00:49:54.683726 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_7.gif
--rw-r--r--   0        0        0    24880 2022-03-05 00:48:39.458832 gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_cat.gif
--rw-r--r--   0        0        0      115 2023-04-02 21:48:20.214187 gidapptools-0.5.1/gidapptools/data/json/__init__.py
--rw-r--r--   0        0        0    23364 2023-04-13 23:13:08.036055 gidapptools-0.5.1/gidapptools/data/json/webcolors.json
--rw-r--r--   0        0        0       80 2021-12-14 11:09:57.360075 gidapptools-0.5.1/gidapptools/data/py/__init__.py
--rw-r--r--   0        0        0    13608 2024-05-27 23:40:41.217006 gidapptools-0.5.1/gidapptools/errors.py
--rw-r--r--   0        0        0        0 2023-04-02 21:48:15.322224 gidapptools-0.5.1/gidapptools/general_helper/__init__.py
--rw-r--r--   0        0        0     2949 2023-03-29 11:24:17.430146 gidapptools-0.5.1/gidapptools/general_helper/ast_helper.py
--rw-r--r--   0        0        0      686 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/general_helper/checker.py
--rw-r--r--   0        0        0     2607 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/general_helper/class_helper.py
--rw-r--r--   0        0        0     1341 2023-03-25 00:28:35.426969 gidapptools-0.5.1/gidapptools/general_helper/compress.py
--rw-r--r--   0        0        0        0 2021-11-20 18:26:05.665295 gidapptools-0.5.1/gidapptools/general_helper/concurrency/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-16 18:59:55.715194 gidapptools-0.5.1/gidapptools/general_helper/concurrency/events.py
--rw-r--r--   0        0        0     2244 2023-06-19 19:55:25.461422 gidapptools-0.5.1/gidapptools/general_helper/concurrency/locks.py
--rw-r--r--   0        0        0     1708 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/general_helper/concurrency/switch.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:32.741650 gidapptools-0.5.1/gidapptools/general_helper/concurrency/threadpools.py
--rw-r--r--   0        0        0    15290 2024-05-25 23:05:36.995810 gidapptools-0.5.1/gidapptools/general_helper/conversion.py
--rw-r--r--   0        0        0    10460 2024-05-28 01:32:16.099085 gidapptools-0.5.1/gidapptools/general_helper/date_time.py
--rw-r--r--   0        0        0       60 2022-03-03 04:10:34.793253 gidapptools-0.5.1/gidapptools/general_helper/development/__init__.py
--rw-r--r--   0        0        0     6408 2024-05-28 01:32:51.634635 gidapptools-0.5.1/gidapptools/general_helper/development/class_hierachy_inspect.py
--rw-r--r--   0        0        0    11546 2023-04-02 21:27:25.104771 gidapptools-0.5.1/gidapptools/general_helper/development/inspect_helpers.py
--rw-r--r--   0        0        0     3411 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/general_helper/development/misc.py
--rw-r--r--   0        0        0    15131 2023-01-07 14:13:32.741650 gidapptools-0.5.1/gidapptools/general_helper/dict_helper.py
--rw-r--r--   0        0        0     5290 2023-01-07 14:12:32.946563 gidapptools-0.5.1/gidapptools/general_helper/dispatch_table.py
--rw-r--r--   0        0        0     2282 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/general_helper/enums.py
--rw-r--r--   0        0        0        0 2023-03-18 16:54:11.952129 gidapptools-0.5.1/gidapptools/general_helper/font/__init__.py
--rw-r--r--   0        0        0     7904 2023-03-25 00:44:51.605615 gidapptools-0.5.1/gidapptools/general_helper/font/font_locating.py
--rw-r--r--   0        0        0     5995 2023-03-25 00:41:16.101915 gidapptools-0.5.1/gidapptools/general_helper/general.py
--rw-r--r--   0        0        0     3116 2023-01-07 14:13:32.742648 gidapptools-0.5.1/gidapptools/general_helper/general_classes.py
--rw-r--r--   0        0        0     1748 2023-06-13 19:40:27.991615 gidapptools-0.5.1/gidapptools/general_helper/hashing.py
--rw-r--r--   0        0        0     2921 2023-06-17 04:04:12.834423 gidapptools-0.5.1/gidapptools/general_helper/import_helper.py
--rw-r--r--   0        0        0     2828 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/general_helper/io_helper.py
--rw-r--r--   0        0        0        0 2022-08-06 19:27:50.929033 gidapptools-0.5.1/gidapptools/general_helper/meta_helper/__init__.py
--rw-r--r--   0        0        0     5641 2023-04-29 22:15:25.791172 gidapptools-0.5.1/gidapptools/general_helper/meta_helper/single_running_instance.py
--rw-r--r--   0        0        0        0 2021-09-27 16:39:28.396464 gidapptools-0.5.1/gidapptools/general_helper/mixins/__init__.py
--rw-r--r--   0        0        0     8434 2023-03-25 00:18:50.510201 gidapptools-0.5.1/gidapptools/general_helper/mixins/file_mixin.py
--rw-r--r--   0        0        0        0 2024-04-25 20:10:07.945114 gidapptools-0.5.1/gidapptools/general_helper/output_helper/__init__.py
--rw-r--r--   0        0        0    10403 2024-04-27 18:44:31.954748 gidapptools-0.5.1/gidapptools/general_helper/output_helper/console_colors.py
--rw-r--r--   0        0        0      188 2022-03-31 12:52:12.827634 gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/__init__.py
--rw-r--r--   0        0        0     4545 2023-02-15 16:01:15.425910 gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/rich_helper.py
--rw-r--r--   0        0        0      621 2023-05-24 23:00:14.061622 gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/rich_styles.py
--rw-r--r--   0        0        0     4350 2023-05-25 07:17:35.605342 gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/rich_themes.py
--rw-r--r--   0        0        0     5112 2023-04-29 21:16:12.721551 gidapptools-0.5.1/gidapptools/general_helper/path_helper.py
--rw-r--r--   0        0        0        0 2021-10-27 16:15:21.832963 gidapptools-0.5.1/gidapptools/general_helper/regex/__init__.py
--rw-r--r--   0        0        0     1754 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/general_helper/regex/datetime_regex.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:32.742648 gidapptools-0.5.1/gidapptools/general_helper/ressource_classes.py
--rw-r--r--   0        0        0    16114 2023-06-13 19:16:50.176014 gidapptools-0.5.1/gidapptools/general_helper/string_helper.py
--rw-r--r--   0        0        0     4965 2023-01-07 15:48:23.927013 gidapptools-0.5.1/gidapptools/general_helper/timing.py
--rw-r--r--   0        0        0     1025 2023-01-07 14:13:32.665853 gidapptools-0.5.1/gidapptools/general_helper/typing_helper.py
--rw-r--r--   0        0        0      752 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/general_helper/web_helper.py
--rw-r--r--   0        0        0       61 2022-09-23 14:25:48.373107 gidapptools-0.5.1/gidapptools/gid_argparse/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 13:44:44.191704 gidapptools-0.5.1/gidapptools/gid_argparse/custom_actions/__init__.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gid_argparse/custom_actions/base_actions.py
--rw-r--r--   0        0        0     5675 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gid_argparse/custom_parser.py
--rw-r--r--   0        0        0      669 2022-10-08 05:04:32.804406 gidapptools-0.5.1/gidapptools/gid_config/__init__.py
--rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.5.1/gidapptools/gid_config/conversion/__init__.py
--rw-r--r--   0        0        0    13101 2024-05-27 23:40:05.042182 gidapptools-0.5.1/gidapptools/gid_config/conversion/base_converters.py
--rw-r--r--   0        0        0     3113 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/gid_config/conversion/conversion_table.py
--rw-r--r--   0        0        0     3083 2023-02-26 14:34:28.683848 gidapptools-0.5.1/gidapptools/gid_config/conversion/converter_grammar.py
--rw-r--r--   0        0        0     1365 2023-01-07 14:13:32.660866 gidapptools-0.5.1/gidapptools/gid_config/conversion/extra_base_typus.py
--rw-r--r--   0        0        0     7978 2024-05-26 17:01:31.981447 gidapptools-0.5.1/gidapptools/gid_config/conversion/spec_data.py
--rw-r--r--   0        0        0     4895 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/gid_config/conversion/spec_item.py
--rw-r--r--   0        0        0      613 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/gid_config/enums.py
--rw-r--r--   0        0        0    12005 2024-05-26 17:25:49.550783 gidapptools-0.5.1/gidapptools/gid_config/interface.py
--rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.5.1/gidapptools/gid_config/parser/__init__.py
--rw-r--r--   0        0        0     9761 2024-05-26 17:25:01.962688 gidapptools-0.5.1/gidapptools/gid_config/parser/config_data.py
--rw-r--r--   0        0        0     4553 2023-01-07 14:13:32.741650 gidapptools-0.5.1/gidapptools/gid_config/parser/grammar.py
--rw-r--r--   0        0        0     6121 2023-02-26 14:34:28.689832 gidapptools-0.5.1/gidapptools/gid_config/parser/ini_parser.py
--rw-r--r--   0        0        0     4797 2023-02-26 14:34:28.688835 gidapptools-0.5.1/gidapptools/gid_config/parser/tokens.py
--rw-r--r--   0        0        0        0 2022-09-23 03:58:23.085387 gidapptools-0.5.1/gidapptools/gid_database/__init__.py
--rw-r--r--   0        0        0      145 2022-09-23 04:02:35.172766 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/__init__.py
--rw-r--r--   0        0        0      153 2022-09-23 03:59:53.337430 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/__init__.py
--rw-r--r--   0        0        0    14235 2024-05-28 01:32:51.492648 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py
--rw-r--r--   0        0        0     1520 2023-01-07 14:13:34.168833 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/constants.py
--rw-r--r--   0        0        0        0 2022-09-23 10:53:55.853779 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/custom_base_models/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 11:29:26.257182 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/custom_fields/__init__.py
--rw-r--r--   0        0        0        0 2022-10-08 05:05:38.373765 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/__init__.py
--rw-r--r--   0        0        0      670 2023-01-07 14:13:40.530819 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py
--rw-r--r--   0        0        0     1071 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py
--rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py
--rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py
--rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py
--rw-r--r--   0        0        0     7754 2023-02-15 16:09:50.560537 gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py
--rw-r--r--   0        0        0      139 2023-01-03 18:51:48.004792 gidapptools-0.5.1/gidapptools/gid_image/__init__.py
--rw-r--r--   0        0        0     3247 2023-01-07 14:13:32.626957 gidapptools-0.5.1/gidapptools/gid_image/size_manipulation.py
--rw-r--r--   0        0        0        0 2021-11-04 00:01:05.741311 gidapptools-0.5.1/gidapptools/gid_logger/__init__.py
--rw-r--r--   0        0        0     5368 2023-02-15 17:01:23.731015 gidapptools-0.5.1/gidapptools/gid_logger/enums.py
--rw-r--r--   0        0        0    10633 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/gid_logger/fake_logger.py
--rw-r--r--   0        0        0    17749 2023-07-20 21:33:22.892575 gidapptools-0.5.1/gidapptools/gid_logger/formatter.py
--rw-r--r--   0        0        0     8175 2023-02-26 14:34:28.767869 gidapptools-0.5.1/gidapptools/gid_logger/handler.py
--rw-r--r--   0        0        0    16292 2023-07-16 19:55:21.898252 gidapptools-0.5.1/gidapptools/gid_logger/logger.py
--rw-r--r--   0        0        0     4177 2023-03-13 09:56:15.401301 gidapptools-0.5.1/gidapptools/gid_logger/misc.py
--rw-r--r--   0        0        0     3697 2023-03-13 09:56:48.681021 gidapptools-0.5.1/gidapptools/gid_logger/records.py
--rw-r--r--   0        0        0      149 2022-08-06 19:27:51.411743 gidapptools-0.5.1/gidapptools/gid_parsing/__init__.py
--rw-r--r--   0        0        0     4219 2023-05-25 22:29:50.274352 gidapptools-0.5.1/gidapptools/gid_parsing/py_log_parsing.py
--rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.5.1/gidapptools/gid_parsing/tokens/__init__.py
--rw-r--r--   0        0        0     1171 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/gid_parsing/tokens/base_tokens.py
--rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.5.1/gidapptools/gid_parsing/universal/__init__.py
--rw-r--r--   0        0        0     2971 2023-01-07 14:13:32.626957 gidapptools-0.5.1/gidapptools/gid_parsing/universal/character_elements.py
--rw-r--r--   0        0        0     4576 2023-01-07 14:13:32.741650 gidapptools-0.5.1/gidapptools/gid_parsing/universal/datetime_elements.py
--rw-r--r--   0        0        0        0 2022-08-06 19:27:51.547380 gidapptools-0.5.1/gidapptools/gid_pytest/__init__.py
--rw-r--r--   0        0        0      492 2023-01-07 14:13:32.665853 gidapptools-0.5.1/gidapptools/gid_pytest/parameter.py
--rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.5.1/gidapptools/gid_signal/__init__.py
--rw-r--r--   0        0        0     1418 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/gid_signal/interface.py
--rw-r--r--   0        0        0     1679 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/gid_signal/signal_registry.py
--rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.5.1/gidapptools/gid_signal/signals/__init__.py
--rw-r--r--   0        0        0     3451 2023-01-07 14:13:32.626957 gidapptools-0.5.1/gidapptools/gid_signal/signals/abstract_signal.py
--rw-r--r--   0        0        0     2345 2023-01-07 14:13:32.655879 gidapptools-0.5.1/gidapptools/gid_signal/signals/basic_signal.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:32.652887 gidapptools-0.5.1/gidapptools/gid_signal/signals/qt_signal.py
--rw-r--r--   0        0        0       29 2022-03-11 23:29:54.398628 gidapptools-0.5.1/gidapptools/gid_utility/__init__.py
--rw-r--r--   0        0        0     3773 2023-01-07 14:13:32.627954 gidapptools-0.5.1/gidapptools/gid_utility/version_item.py
--rw-r--r--   0        0        0        0 2022-03-21 03:01:51.190903 gidapptools-0.5.1/gidapptools/gid_warning/__init__.py
--rw-r--r--   0        0        0     3378 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/gid_warning/deprecation.py
--rw-r--r--   0        0        0     1300 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/gid_warning/experimental.py
--rw-r--r--   0        0        0      229 2022-04-18 18:34:33.321765 gidapptools-0.5.1/gidapptools/gidapptools_qt/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 20:52:02.729934 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/__init__.py
--rw-r--r--   0        0        0     1249 2023-01-16 14:23:56.282011 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/__init__.py
--rw-r--r--   0        0        0    32565 2023-01-16 14:18:24.219793 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/debugging_icon.png
--rw-r--r--   0        0        0    12608 2022-08-18 05:21:13.655846 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/default_app_icon.png
--rw-r--r--   0        0        0   134024 2021-12-11 23:04:26.441608 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/placeholder.png
--rw-r--r--   0        0        0      421 2022-08-24 18:17:31.865700 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/__init__.py
--rw-r--r--   0        0        0      220 2022-08-24 18:35:31.118550 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/about_stylesheet.css
--rw-r--r--   0        0        0      598 2022-08-24 18:40:47.966025 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html
--rw-r--r--   0        0        0      826 2022-08-24 18:14:01.808478 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html
--rw-r--r--   0        0        0      218 2022-08-24 18:15:48.522228 gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/arg_doc_markdown_template.jinja_md
--rw-r--r--   0        0        0        0 2023-01-16 14:30:23.631080 gidapptools-0.5.1/gidapptools/gidapptools_qt/abc/__init__.py
--rw-r--r--   0        0        0     5923 2023-01-16 14:32:05.111343 gidapptools-0.5.1/gidapptools/gidapptools_qt/abc/abstract_syntax_highlighting_rule.py
--rw-r--r--   0        0        0        0 2021-11-25 19:55:33.355786 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/__init__.py
--rw-r--r--   0        0        0    27397 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/application.py
--rw-r--r--   0        0        0     1068 2023-01-07 14:13:34.168833 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/application_info.py
--rw-r--r--   0        0        0     2054 2023-02-13 22:15:48.019581 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/application_new.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/command_line_parser.py
--rw-r--r--   0        0        0     2830 2023-01-07 14:13:40.480953 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/main_window.py
--rw-r--r--   0        0        0     5829 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/menu_bar.py
--rw-r--r--   0        0        0     1452 2023-01-07 14:13:34.162849 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/status_bar.py
--rw-r--r--   0        0        0     6475 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/sys_tray.py
--rw-r--r--   0        0        0        0 2022-01-06 22:29:45.436190 gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/__init__.py
--rw-r--r--   0        0        0      723 2023-01-25 04:12:40.770472 gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_value_widgets/__init__.py
--rw-r--r--   0        0        0     5143 2023-01-25 02:03:04.006135 gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_value_widgets/_checks.py
--rw-r--r--   0        0        0    10979 2023-01-25 05:15:16.953587 gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_value_widgets/standard_types.py
--rw-r--r--   0        0        0    19709 2024-05-28 01:32:17.141129 gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_widget.py
--rw-r--r--   0        0        0     7339 2023-02-15 16:01:08.996748 gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/event_analyzer.py
--rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.5.1/gidapptools/gidapptools_qt/dialogs/__init__.py
--rw-r--r--   0        0        0     1791 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py
--rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/__init__.py
--rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/command_line_parser/__init__.py
--rw-r--r--   0        0        0     1493 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py
--rw-r--r--   0        0        0     1831 2023-03-15 23:35:57.577116 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/misc.py
--rw-r--r--   0        0        0      747 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/object_name.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/signal_bridge.py
--rw-r--r--   0        0        0        0 2023-01-16 14:32:52.231212 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/syntax_highlighting/__init__.py
--rw-r--r--   0        0        0     8783 2023-01-18 12:53:20.806844 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/syntax_highlighting/rules.py
--rw-r--r--   0        0        0     1354 2023-10-21 23:10:32.561981 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/window_geometry_helper.py
--rw-r--r--   0        0        0     2519 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/window_reference_keeper.py
--rw-r--r--   0        0        0        0 2022-02-27 16:36:21.918865 gidapptools-0.5.1/gidapptools/gidapptools_qt/layouts/__init__.py
--rw-r--r--   0        0        0     7553 2023-02-15 10:01:30.255286 gidapptools-0.5.1/gidapptools/gidapptools_qt/layouts/sorted_layout.py
--rw-r--r--   0        0        0      823 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py
--rw-r--r--   0        0        0        0 2021-12-02 11:38:53.174893 gidapptools-0.5.1/gidapptools/gidapptools_qt/models/__init__.py
--rw-r--r--   0        0        0     1798 2023-01-10 12:47:37.778095 gidapptools-0.5.1/gidapptools/gidapptools_qt/models/basic_model.py
--rw-r--r--   0        0        0        0 2023-07-15 17:20:27.983921 gidapptools-0.5.1/gidapptools/gidapptools_qt/protocols/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 22:01:16.199629 gidapptools-0.5.1/gidapptools/gidapptools_qt/resources/__init__.py
--rw-r--r--   0        0        0     1628 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/resources/placeholder.py
--rw-r--r--   0        0        0     5394 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/resources/resources_helper.py
--rw-r--r--   0        0        0     5126 2023-07-15 17:32:48.110111 gidapptools-0.5.1/gidapptools/gidapptools_qt/sub_typing.py
--rw-r--r--   0        0        0        0 2021-12-02 11:32:36.936086 gidapptools-0.5.1/gidapptools/gidapptools_qt/views/__init__.py
--rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/views/basic_view.py
--rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/__init__.py
--rw-r--r--   0        0        0    12484 2024-05-28 00:54:33.315218 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/app_log_viewer.py
--rw-r--r--   0        0        0    10939 2023-01-24 15:57:36.849714 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/category_select_widget.py
--rw-r--r--   0        0        0     7519 2023-03-15 23:37:04.290567 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/collapsible_widget.py
--rw-r--r--   0        0        0     2841 2023-03-16 00:11:13.454353 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/hyperlink_label.py
--rw-r--r--   0        0        0     3579 2023-03-31 22:17:40.477649 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/icon_text_button.py
--rw-r--r--   0        0        0     1066 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/json_editor.py
--rw-r--r--   0        0        0     6239 2023-07-29 00:25:52.761350 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/scrollable_widget.py
--rw-r--r--   0        0        0     6380 2023-01-13 19:24:03.785389 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/separator_lines.py
--rw-r--r--   0        0        0     5507 2023-07-08 12:51:52.873532 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/spinner_widget.py
--rw-r--r--   0        0        0     6645 2023-01-07 14:13:46.165750 gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/std_stream_widget.py
--rw-r--r--   0        0        0        0 2021-10-04 15:25:35.923246 gidapptools-0.5.1/gidapptools/gidcolor/__init__.py
--rw-r--r--   0        0        0    10859 2023-09-12 18:49:22.065364 gidapptools-0.5.1/gidapptools/gidcolor/color.py
--rw-r--r--   0        0        0    13948 2023-09-12 18:43:16.982322 gidapptools-0.5.1/gidapptools/gidcolor/color_item.py
--rw-r--r--   0        0        0     6746 2023-04-28 16:48:17.765325 gidapptools-0.5.1/gidapptools/gidcolor/color_string_formatter.py
--rw-r--r--   0        0        0     3995 2023-08-15 22:43:07.163783 gidapptools-0.5.1/gidapptools/gidcolor/coversion.py
--rw-r--r--   0        0        0     4284 2023-05-01 20:54:30.254114 gidapptools-0.5.1/gidapptools/gidcolor/misc_calculations.py
--rw-r--r--   0        0        0     3737 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/gidcolor/palette.py
--rw-r--r--   0        0        0        0 2021-12-14 11:01:49.256730 gidapptools-0.5.1/gidapptools/gidcolor/preset_colors/__init__.py
--rw-r--r--   0        0        0     1660 2023-04-02 21:57:49.861549 gidapptools-0.5.1/gidapptools/gidcolor/preset_colors/web_colors.py
--rw-r--r--   0        0        0       96 2021-09-14 19:29:19.689941 gidapptools-0.5.1/gidapptools/meta_data/__init__.py
--rw-r--r--   0        0        0     2816 2023-01-07 14:13:33.733996 gidapptools-0.5.1/gidapptools/meta_data/config_kwargs.py
--rw-r--r--   0        0        0     7502 2023-01-07 14:13:32.665853 gidapptools-0.5.1/gidapptools/meta_data/interface.py
--rw-r--r--   0        0        0       65 2021-09-19 15:57:06.694208 gidapptools-0.5.1/gidapptools/meta_data/meta_info/__init__.py
--rw-r--r--   0        0        0     6335 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/meta_data/meta_info/meta_info_factory.py
--rw-r--r--   0        0        0     6027 2023-06-04 19:32:02.729405 gidapptools-0.5.1/gidapptools/meta_data/meta_info/meta_info_item.py
--rw-r--r--   0        0        0       67 2021-09-19 15:57:36.351976 gidapptools-0.5.1/gidapptools/meta_data/meta_paths/__init__.py
--rw-r--r--   0        0        0     2420 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/meta_data/meta_paths/appdirs_implementations.py
--rw-r--r--   0        0        0     2955 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/meta_data/meta_paths/meta_paths_factory.py
--rw-r--r--   0        0        0     6482 2023-01-09 20:46:11.912758 gidapptools-0.5.1/gidapptools/meta_data/meta_paths/meta_paths_item.py
--rw-r--r--   0        0        0        0 2021-09-22 03:09:38.138175 gidapptools-0.5.1/gidapptools/utility/__init__.py
--rw-r--r--   0        0        0     3029 2023-01-07 14:13:32.664855 gidapptools-0.5.1/gidapptools/utility/enums.py
--rw-r--r--   0        0        0     8794 2023-05-03 05:48:40.390181 gidapptools-0.5.1/gidapptools/utility/helper.py
--rw-r--r--   0        0        0     2529 2023-01-07 14:13:33.732999 gidapptools-0.5.1/gidapptools/utility/kwarg_dict.py
--rw-r--r--   0        0        0        0 2022-08-06 21:26:08.033946 gidapptools-0.5.1/gidapptools/vendored/__init__.py
--rw-r--r--   0        0        0     7128 2022-11-02 13:03:50.593217 gidapptools-0.5.1/gidapptools/vendored/atomic_writes.py
--rw-r--r--   0        0        0     1069 2022-06-30 02:44:23.800813 gidapptools-0.5.1/gidapptools/vendored/atomic_writes_LICENSE
--rw-r--r--   0        0        0     3424 2024-05-26 17:04:20.571571 gidapptools-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 gidapptools-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-08-31 18:36:20.520000 gidapptools-0.5.2/LICENSE
+-rw-r--r--   0        0        0      649 2023-04-07 20:25:45.102049 gidapptools-0.5.2/README.rst
+-rw-r--r--   0        0        0      716 2024-05-31 01:33:53.208089 gidapptools-0.5.2/gidapptools/__init__.py
+-rw-r--r--   0        0        0      667 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/__main__.py
+-rw-r--r--   0        0        0      106 2021-09-20 21:57:04.325557 gidapptools-0.5.2/gidapptools/abstract_classes/__init__.py
+-rw-r--r--   0        0        0     2098 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/abstract_classes/abstract_meta_factory.py
+-rw-r--r--   0        0        0     1324 2023-01-07 14:13:46.164752 gidapptools-0.5.2/gidapptools/abstract_classes/abstract_meta_item.py
+-rw-r--r--   0        0        0      585 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/cli_info.py
+-rw-r--r--   0        0        0       21 2024-04-25 20:13:17.822555 gidapptools-0.5.2/gidapptools/code_generation/__init__.py
+-rw-r--r--   0        0        0     5890 2024-04-25 21:29:19.094195 gidapptools-0.5.2/gidapptools/code_generation/python.py
+-rw-r--r--   0        0        0      769 2023-06-19 19:52:38.610215 gidapptools-0.5.2/gidapptools/custom_types.py
+-rw-r--r--   0        0        0       69 2022-01-12 13:50:02.703044 gidapptools-0.5.2/gidapptools/data/__init__.py
+-rw-r--r--   0        0        0     3374 2023-08-16 03:08:15.130796 gidapptools-0.5.2/gidapptools/data/conversion_data.py
+-rw-r--r--   0        0        0      126 2022-11-02 13:03:47.066458 gidapptools-0.5.2/gidapptools/data/general_data.py
+-rw-r--r--   0        0        0     1035 2022-03-20 03:11:40.597216 gidapptools-0.5.2/gidapptools/data/gifs/__init__.py
+-rw-r--r--   0        0        0    21837 2022-03-04 16:17:21.627813 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_1.gif
+-rw-r--r--   0        0        0    28904 2022-03-04 16:31:53.112866 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_2.gif
+-rw-r--r--   0        0        0   780846 2022-03-04 16:16:38.588118 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_3.gif
+-rw-r--r--   0        0        0   126652 2022-03-04 16:35:31.028357 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_4.gif
+-rw-r--r--   0        0        0    72232 2022-03-05 00:49:16.857127 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_5.gif
+-rw-r--r--   0        0        0    77029 2022-03-05 00:49:38.490391 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_6.gif
+-rw-r--r--   0        0        0    75110 2022-03-05 00:49:54.683726 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_7.gif
+-rw-r--r--   0        0        0    24880 2022-03-05 00:48:39.458832 gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_cat.gif
+-rw-r--r--   0        0        0      115 2023-04-02 21:48:20.214187 gidapptools-0.5.2/gidapptools/data/json/__init__.py
+-rw-r--r--   0        0        0    23364 2023-04-13 23:13:08.036055 gidapptools-0.5.2/gidapptools/data/json/webcolors.json
+-rw-r--r--   0        0        0       80 2021-12-14 11:09:57.360075 gidapptools-0.5.2/gidapptools/data/py/__init__.py
+-rw-r--r--   0        0        0    13608 2024-05-27 23:40:41.217006 gidapptools-0.5.2/gidapptools/errors.py
+-rw-r--r--   0        0        0        0 2023-04-02 21:48:15.322224 gidapptools-0.5.2/gidapptools/general_helper/__init__.py
+-rw-r--r--   0        0        0     2949 2023-03-29 11:24:17.430146 gidapptools-0.5.2/gidapptools/general_helper/ast_helper.py
+-rw-r--r--   0        0        0      686 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/general_helper/checker.py
+-rw-r--r--   0        0        0     2607 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/general_helper/class_helper.py
+-rw-r--r--   0        0        0     1341 2023-03-25 00:28:35.426969 gidapptools-0.5.2/gidapptools/general_helper/compress.py
+-rw-r--r--   0        0        0        0 2021-11-20 18:26:05.665295 gidapptools-0.5.2/gidapptools/general_helper/concurrency/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-16 18:59:55.715194 gidapptools-0.5.2/gidapptools/general_helper/concurrency/events.py
+-rw-r--r--   0        0        0     2244 2023-06-19 19:55:25.461422 gidapptools-0.5.2/gidapptools/general_helper/concurrency/locks.py
+-rw-r--r--   0        0        0     1708 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/general_helper/concurrency/switch.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:32.741650 gidapptools-0.5.2/gidapptools/general_helper/concurrency/threadpools.py
+-rw-r--r--   0        0        0    15290 2024-05-25 23:05:36.995810 gidapptools-0.5.2/gidapptools/general_helper/conversion.py
+-rw-r--r--   0        0        0    10460 2024-05-28 01:32:16.099085 gidapptools-0.5.2/gidapptools/general_helper/date_time.py
+-rw-r--r--   0        0        0       60 2022-03-03 04:10:34.793253 gidapptools-0.5.2/gidapptools/general_helper/development/__init__.py
+-rw-r--r--   0        0        0     6408 2024-05-28 01:32:51.634635 gidapptools-0.5.2/gidapptools/general_helper/development/class_hierachy_inspect.py
+-rw-r--r--   0        0        0    11546 2023-04-02 21:27:25.104771 gidapptools-0.5.2/gidapptools/general_helper/development/inspect_helpers.py
+-rw-r--r--   0        0        0     3411 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/general_helper/development/misc.py
+-rw-r--r--   0        0        0    15131 2023-01-07 14:13:32.741650 gidapptools-0.5.2/gidapptools/general_helper/dict_helper.py
+-rw-r--r--   0        0        0     5290 2023-01-07 14:12:32.946563 gidapptools-0.5.2/gidapptools/general_helper/dispatch_table.py
+-rw-r--r--   0        0        0     2282 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/general_helper/enums.py
+-rw-r--r--   0        0        0        0 2023-03-18 16:54:11.952129 gidapptools-0.5.2/gidapptools/general_helper/font/__init__.py
+-rw-r--r--   0        0        0     7904 2023-03-25 00:44:51.605615 gidapptools-0.5.2/gidapptools/general_helper/font/font_locating.py
+-rw-r--r--   0        0        0     5995 2023-03-25 00:41:16.101915 gidapptools-0.5.2/gidapptools/general_helper/general.py
+-rw-r--r--   0        0        0     3116 2023-01-07 14:13:32.742648 gidapptools-0.5.2/gidapptools/general_helper/general_classes.py
+-rw-r--r--   0        0        0     1748 2023-06-13 19:40:27.991615 gidapptools-0.5.2/gidapptools/general_helper/hashing.py
+-rw-r--r--   0        0        0     2921 2023-06-17 04:04:12.834423 gidapptools-0.5.2/gidapptools/general_helper/import_helper.py
+-rw-r--r--   0        0        0     2828 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/general_helper/io_helper.py
+-rw-r--r--   0        0        0        0 2022-08-06 19:27:50.929033 gidapptools-0.5.2/gidapptools/general_helper/meta_helper/__init__.py
+-rw-r--r--   0        0        0     5641 2023-04-29 22:15:25.791172 gidapptools-0.5.2/gidapptools/general_helper/meta_helper/single_running_instance.py
+-rw-r--r--   0        0        0        0 2021-09-27 16:39:28.396464 gidapptools-0.5.2/gidapptools/general_helper/mixins/__init__.py
+-rw-r--r--   0        0        0     8434 2023-03-25 00:18:50.510201 gidapptools-0.5.2/gidapptools/general_helper/mixins/file_mixin.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:10:07.945114 gidapptools-0.5.2/gidapptools/general_helper/output_helper/__init__.py
+-rw-r--r--   0        0        0    10403 2024-04-27 18:44:31.954748 gidapptools-0.5.2/gidapptools/general_helper/output_helper/console_colors.py
+-rw-r--r--   0        0        0      188 2022-03-31 12:52:12.827634 gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/__init__.py
+-rw-r--r--   0        0        0     4545 2023-02-15 16:01:15.425910 gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/rich_helper.py
+-rw-r--r--   0        0        0      621 2023-05-24 23:00:14.061622 gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/rich_styles.py
+-rw-r--r--   0        0        0     4350 2023-05-25 07:17:35.605342 gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/rich_themes.py
+-rw-r--r--   0        0        0     5112 2023-04-29 21:16:12.721551 gidapptools-0.5.2/gidapptools/general_helper/path_helper.py
+-rw-r--r--   0        0        0        0 2021-10-27 16:15:21.832963 gidapptools-0.5.2/gidapptools/general_helper/regex/__init__.py
+-rw-r--r--   0        0        0     1754 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/general_helper/regex/datetime_regex.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:32.742648 gidapptools-0.5.2/gidapptools/general_helper/ressource_classes.py
+-rw-r--r--   0        0        0    16114 2023-06-13 19:16:50.176014 gidapptools-0.5.2/gidapptools/general_helper/string_helper.py
+-rw-r--r--   0        0        0     4965 2023-01-07 15:48:23.927013 gidapptools-0.5.2/gidapptools/general_helper/timing.py
+-rw-r--r--   0        0        0     1025 2023-01-07 14:13:32.665853 gidapptools-0.5.2/gidapptools/general_helper/typing_helper.py
+-rw-r--r--   0        0        0      752 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/general_helper/web_helper.py
+-rw-r--r--   0        0        0       61 2022-09-23 14:25:48.373107 gidapptools-0.5.2/gidapptools/gid_argparse/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-23 13:44:44.191704 gidapptools-0.5.2/gidapptools/gid_argparse/custom_actions/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gid_argparse/custom_actions/base_actions.py
+-rw-r--r--   0        0        0     5675 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gid_argparse/custom_parser.py
+-rw-r--r--   0        0        0      669 2022-10-08 05:04:32.804406 gidapptools-0.5.2/gidapptools/gid_config/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.5.2/gidapptools/gid_config/conversion/__init__.py
+-rw-r--r--   0        0        0    13101 2024-05-27 23:40:05.042182 gidapptools-0.5.2/gidapptools/gid_config/conversion/base_converters.py
+-rw-r--r--   0        0        0     3113 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/gid_config/conversion/conversion_table.py
+-rw-r--r--   0        0        0     3083 2023-02-26 14:34:28.683848 gidapptools-0.5.2/gidapptools/gid_config/conversion/converter_grammar.py
+-rw-r--r--   0        0        0     1365 2023-01-07 14:13:32.660866 gidapptools-0.5.2/gidapptools/gid_config/conversion/extra_base_typus.py
+-rw-r--r--   0        0        0     7978 2024-05-26 17:01:31.981447 gidapptools-0.5.2/gidapptools/gid_config/conversion/spec_data.py
+-rw-r--r--   0        0        0     4895 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/gid_config/conversion/spec_item.py
+-rw-r--r--   0        0        0      613 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/gid_config/enums.py
+-rw-r--r--   0        0        0    12005 2024-05-26 17:25:49.550783 gidapptools-0.5.2/gidapptools/gid_config/interface.py
+-rw-r--r--   0        0        0        0 2021-09-23 00:22:27.273740 gidapptools-0.5.2/gidapptools/gid_config/parser/__init__.py
+-rw-r--r--   0        0        0     9761 2024-05-26 17:25:01.962688 gidapptools-0.5.2/gidapptools/gid_config/parser/config_data.py
+-rw-r--r--   0        0        0     4553 2023-01-07 14:13:32.741650 gidapptools-0.5.2/gidapptools/gid_config/parser/grammar.py
+-rw-r--r--   0        0        0     6121 2023-02-26 14:34:28.689832 gidapptools-0.5.2/gidapptools/gid_config/parser/ini_parser.py
+-rw-r--r--   0        0        0     4797 2023-02-26 14:34:28.688835 gidapptools-0.5.2/gidapptools/gid_config/parser/tokens.py
+-rw-r--r--   0        0        0        0 2022-09-23 03:58:23.085387 gidapptools-0.5.2/gidapptools/gid_database/__init__.py
+-rw-r--r--   0        0        0      145 2022-09-23 04:02:35.172766 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/__init__.py
+-rw-r--r--   0        0        0      153 2022-09-23 03:59:53.337430 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/__init__.py
+-rw-r--r--   0        0        0    14235 2024-05-28 01:32:51.492648 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py
+-rw-r--r--   0        0        0     1520 2023-01-07 14:13:34.168833 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/constants.py
+-rw-r--r--   0        0        0        0 2022-09-23 10:53:55.853779 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/custom_base_models/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-23 11:29:26.257182 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/custom_fields/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-08 05:05:38.373765 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/__init__.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.530819 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py
+-rw-r--r--   0        0        0     1071 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py
+-rw-r--r--   0        0        0      670 2023-01-07 14:13:40.480953 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py
+-rw-r--r--   0        0        0     7754 2023-02-15 16:09:50.560537 gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py
+-rw-r--r--   0        0        0      139 2023-01-03 18:51:48.004792 gidapptools-0.5.2/gidapptools/gid_image/__init__.py
+-rw-r--r--   0        0        0     3247 2023-01-07 14:13:32.626957 gidapptools-0.5.2/gidapptools/gid_image/size_manipulation.py
+-rw-r--r--   0        0        0        0 2021-11-04 00:01:05.741311 gidapptools-0.5.2/gidapptools/gid_logger/__init__.py
+-rw-r--r--   0        0        0     5368 2023-02-15 17:01:23.731015 gidapptools-0.5.2/gidapptools/gid_logger/enums.py
+-rw-r--r--   0        0        0    10633 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/gid_logger/fake_logger.py
+-rw-r--r--   0        0        0    17749 2023-07-20 21:33:22.892575 gidapptools-0.5.2/gidapptools/gid_logger/formatter.py
+-rw-r--r--   0        0        0    11617 2024-05-31 00:49:34.618374 gidapptools-0.5.2/gidapptools/gid_logger/handler.py
+-rw-r--r--   0        0        0    16292 2023-07-16 19:55:21.898252 gidapptools-0.5.2/gidapptools/gid_logger/logger.py
+-rw-r--r--   0        0        0     4177 2023-03-13 09:56:15.401301 gidapptools-0.5.2/gidapptools/gid_logger/misc.py
+-rw-r--r--   0        0        0     3697 2023-03-13 09:56:48.681021 gidapptools-0.5.2/gidapptools/gid_logger/records.py
+-rw-r--r--   0        0        0      149 2022-08-06 19:27:51.411743 gidapptools-0.5.2/gidapptools/gid_parsing/__init__.py
+-rw-r--r--   0        0        0     4219 2023-05-25 22:29:50.274352 gidapptools-0.5.2/gidapptools/gid_parsing/py_log_parsing.py
+-rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.5.2/gidapptools/gid_parsing/tokens/__init__.py
+-rw-r--r--   0        0        0     1171 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/gid_parsing/tokens/base_tokens.py
+-rw-r--r--   0        0        0        0 2022-01-15 19:38:52.874584 gidapptools-0.5.2/gidapptools/gid_parsing/universal/__init__.py
+-rw-r--r--   0        0        0     2971 2023-01-07 14:13:32.626957 gidapptools-0.5.2/gidapptools/gid_parsing/universal/character_elements.py
+-rw-r--r--   0        0        0     4576 2023-01-07 14:13:32.741650 gidapptools-0.5.2/gidapptools/gid_parsing/universal/datetime_elements.py
+-rw-r--r--   0        0        0        0 2022-08-06 19:27:51.547380 gidapptools-0.5.2/gidapptools/gid_pytest/__init__.py
+-rw-r--r--   0        0        0      492 2023-01-07 14:13:32.665853 gidapptools-0.5.2/gidapptools/gid_pytest/parameter.py
+-rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.5.2/gidapptools/gid_signal/__init__.py
+-rw-r--r--   0        0        0     1418 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/gid_signal/interface.py
+-rw-r--r--   0        0        0     1679 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/gid_signal/signal_registry.py
+-rw-r--r--   0        0        0        0 2021-09-29 21:44:28.330981 gidapptools-0.5.2/gidapptools/gid_signal/signals/__init__.py
+-rw-r--r--   0        0        0     3451 2023-01-07 14:13:32.626957 gidapptools-0.5.2/gidapptools/gid_signal/signals/abstract_signal.py
+-rw-r--r--   0        0        0     2345 2023-01-07 14:13:32.655879 gidapptools-0.5.2/gidapptools/gid_signal/signals/basic_signal.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:32.652887 gidapptools-0.5.2/gidapptools/gid_signal/signals/qt_signal.py
+-rw-r--r--   0        0        0       29 2022-03-11 23:29:54.398628 gidapptools-0.5.2/gidapptools/gid_utility/__init__.py
+-rw-r--r--   0        0        0     3773 2023-01-07 14:13:32.627954 gidapptools-0.5.2/gidapptools/gid_utility/version_item.py
+-rw-r--r--   0        0        0        0 2022-03-21 03:01:51.190903 gidapptools-0.5.2/gidapptools/gid_warning/__init__.py
+-rw-r--r--   0        0        0     3378 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/gid_warning/deprecation.py
+-rw-r--r--   0        0        0     1300 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/gid_warning/experimental.py
+-rw-r--r--   0        0        0      229 2022-04-18 18:34:33.321765 gidapptools-0.5.2/gidapptools/gidapptools_qt/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 20:52:02.729934 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/__init__.py
+-rw-r--r--   0        0        0     1249 2023-01-16 14:23:56.282011 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/__init__.py
+-rw-r--r--   0        0        0    32565 2023-01-16 14:18:24.219793 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/debugging_icon.png
+-rw-r--r--   0        0        0    12608 2022-08-18 05:21:13.655846 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/default_app_icon.png
+-rw-r--r--   0        0        0   134024 2021-12-11 23:04:26.441608 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/placeholder.png
+-rw-r--r--   0        0        0      421 2022-08-24 18:17:31.865700 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/__init__.py
+-rw-r--r--   0        0        0      220 2022-08-24 18:35:31.118550 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/about_stylesheet.css
+-rw-r--r--   0        0        0      598 2022-08-24 18:40:47.966025 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html
+-rw-r--r--   0        0        0      826 2022-08-24 18:14:01.808478 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html
+-rw-r--r--   0        0        0      218 2022-08-24 18:15:48.522228 gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/arg_doc_markdown_template.jinja_md
+-rw-r--r--   0        0        0        0 2023-01-16 14:30:23.631080 gidapptools-0.5.2/gidapptools/gidapptools_qt/abc/__init__.py
+-rw-r--r--   0        0        0     5923 2023-01-16 14:32:05.111343 gidapptools-0.5.2/gidapptools/gidapptools_qt/abc/abstract_syntax_highlighting_rule.py
+-rw-r--r--   0        0        0        0 2021-11-25 19:55:33.355786 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/__init__.py
+-rw-r--r--   0        0        0    27397 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/application.py
+-rw-r--r--   0        0        0     1068 2023-01-07 14:13:34.168833 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/application_info.py
+-rw-r--r--   0        0        0     2054 2023-02-13 22:15:48.019581 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/application_new.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/command_line_parser.py
+-rw-r--r--   0        0        0     2830 2023-01-07 14:13:40.480953 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/main_window.py
+-rw-r--r--   0        0        0     5829 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/menu_bar.py
+-rw-r--r--   0        0        0     1452 2023-01-07 14:13:34.162849 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/status_bar.py
+-rw-r--r--   0        0        0     6475 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/sys_tray.py
+-rw-r--r--   0        0        0        0 2022-01-06 22:29:45.436190 gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/__init__.py
+-rw-r--r--   0        0        0      723 2023-01-25 04:12:40.770472 gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_value_widgets/__init__.py
+-rw-r--r--   0        0        0     5143 2023-01-25 02:03:04.006135 gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_value_widgets/_checks.py
+-rw-r--r--   0        0        0    10979 2023-01-25 05:15:16.953587 gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_value_widgets/standard_types.py
+-rw-r--r--   0        0        0    19709 2024-05-28 01:32:17.141129 gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_widget.py
+-rw-r--r--   0        0        0     7339 2023-02-15 16:01:08.996748 gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/event_analyzer.py
+-rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.5.2/gidapptools/gidapptools_qt/dialogs/__init__.py
+-rw-r--r--   0        0        0     1791 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py
+-rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-07 22:19:08.564742 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/command_line_parser/__init__.py
+-rw-r--r--   0        0        0     1493 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py
+-rw-r--r--   0        0        0     1831 2023-03-15 23:35:57.577116 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/misc.py
+-rw-r--r--   0        0        0      747 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/object_name.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/signal_bridge.py
+-rw-r--r--   0        0        0        0 2023-01-16 14:32:52.231212 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/syntax_highlighting/__init__.py
+-rw-r--r--   0        0        0     8783 2023-01-18 12:53:20.806844 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/syntax_highlighting/rules.py
+-rw-r--r--   0        0        0     1354 2023-10-21 23:10:32.561981 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/window_geometry_helper.py
+-rw-r--r--   0        0        0     2519 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/window_reference_keeper.py
+-rw-r--r--   0        0        0        0 2022-02-27 16:36:21.918865 gidapptools-0.5.2/gidapptools/gidapptools_qt/layouts/__init__.py
+-rw-r--r--   0        0        0     7553 2023-02-15 10:01:30.255286 gidapptools-0.5.2/gidapptools/gidapptools_qt/layouts/sorted_layout.py
+-rw-r--r--   0        0        0      823 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py
+-rw-r--r--   0        0        0        0 2021-12-02 11:38:53.174893 gidapptools-0.5.2/gidapptools/gidapptools_qt/models/__init__.py
+-rw-r--r--   0        0        0     1798 2023-01-10 12:47:37.778095 gidapptools-0.5.2/gidapptools/gidapptools_qt/models/basic_model.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:27.983921 gidapptools-0.5.2/gidapptools/gidapptools_qt/protocols/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 22:01:16.199629 gidapptools-0.5.2/gidapptools/gidapptools_qt/resources/__init__.py
+-rw-r--r--   0        0        0     1628 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/resources/placeholder.py
+-rw-r--r--   0        0        0     5394 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/resources/resources_helper.py
+-rw-r--r--   0        0        0     5126 2023-07-15 17:32:48.110111 gidapptools-0.5.2/gidapptools/gidapptools_qt/sub_typing.py
+-rw-r--r--   0        0        0        0 2021-12-02 11:32:36.936086 gidapptools-0.5.2/gidapptools/gidapptools_qt/views/__init__.py
+-rw-r--r--   0        0        0      496 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/views/basic_view.py
+-rw-r--r--   0        0        0        0 2021-12-07 00:05:58.701876 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/__init__.py
+-rw-r--r--   0        0        0    26025 2024-05-31 00:13:56.189045 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/app_log_viewer.py
+-rw-r--r--   0        0        0    10939 2023-01-24 15:57:36.849714 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/category_select_widget.py
+-rw-r--r--   0        0        0     7519 2023-03-15 23:37:04.290567 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/collapsible_widget.py
+-rw-r--r--   0        0        0     2841 2023-03-16 00:11:13.454353 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/hyperlink_label.py
+-rw-r--r--   0        0        0     3579 2023-03-31 22:17:40.477649 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/icon_text_button.py
+-rw-r--r--   0        0        0     1066 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/json_editor.py
+-rw-r--r--   0        0        0     6239 2023-07-29 00:25:52.761350 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/scrollable_widget.py
+-rw-r--r--   0        0        0     6380 2023-01-13 19:24:03.785389 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/separator_lines.py
+-rw-r--r--   0        0        0     5507 2023-07-08 12:51:52.873532 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/spinner_widget.py
+-rw-r--r--   0        0        0     6645 2023-01-07 14:13:46.165750 gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/std_stream_widget.py
+-rw-r--r--   0        0        0        0 2021-10-04 15:25:35.923246 gidapptools-0.5.2/gidapptools/gidcolor/__init__.py
+-rw-r--r--   0        0        0    10859 2023-09-12 18:49:22.065364 gidapptools-0.5.2/gidapptools/gidcolor/color.py
+-rw-r--r--   0        0        0    13948 2023-09-12 18:43:16.982322 gidapptools-0.5.2/gidapptools/gidcolor/color_item.py
+-rw-r--r--   0        0        0     6746 2023-04-28 16:48:17.765325 gidapptools-0.5.2/gidapptools/gidcolor/color_string_formatter.py
+-rw-r--r--   0        0        0     3995 2023-08-15 22:43:07.163783 gidapptools-0.5.2/gidapptools/gidcolor/coversion.py
+-rw-r--r--   0        0        0     4284 2023-05-01 20:54:30.254114 gidapptools-0.5.2/gidapptools/gidcolor/misc_calculations.py
+-rw-r--r--   0        0        0     3737 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/gidcolor/palette.py
+-rw-r--r--   0        0        0        0 2021-12-14 11:01:49.256730 gidapptools-0.5.2/gidapptools/gidcolor/preset_colors/__init__.py
+-rw-r--r--   0        0        0     1660 2023-04-02 21:57:49.861549 gidapptools-0.5.2/gidapptools/gidcolor/preset_colors/web_colors.py
+-rw-r--r--   0        0        0       96 2021-09-14 19:29:19.689941 gidapptools-0.5.2/gidapptools/meta_data/__init__.py
+-rw-r--r--   0        0        0     2816 2023-01-07 14:13:33.733996 gidapptools-0.5.2/gidapptools/meta_data/config_kwargs.py
+-rw-r--r--   0        0        0     7502 2023-01-07 14:13:32.665853 gidapptools-0.5.2/gidapptools/meta_data/interface.py
+-rw-r--r--   0        0        0       65 2021-09-19 15:57:06.694208 gidapptools-0.5.2/gidapptools/meta_data/meta_info/__init__.py
+-rw-r--r--   0        0        0     6335 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/meta_data/meta_info/meta_info_factory.py
+-rw-r--r--   0        0        0     6027 2023-06-04 19:32:02.729405 gidapptools-0.5.2/gidapptools/meta_data/meta_info/meta_info_item.py
+-rw-r--r--   0        0        0       67 2021-09-19 15:57:36.351976 gidapptools-0.5.2/gidapptools/meta_data/meta_paths/__init__.py
+-rw-r--r--   0        0        0     2420 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/meta_data/meta_paths/appdirs_implementations.py
+-rw-r--r--   0        0        0     2955 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/meta_data/meta_paths/meta_paths_factory.py
+-rw-r--r--   0        0        0     6482 2023-01-09 20:46:11.912758 gidapptools-0.5.2/gidapptools/meta_data/meta_paths/meta_paths_item.py
+-rw-r--r--   0        0        0        0 2021-09-22 03:09:38.138175 gidapptools-0.5.2/gidapptools/utility/__init__.py
+-rw-r--r--   0        0        0     3029 2023-01-07 14:13:32.664855 gidapptools-0.5.2/gidapptools/utility/enums.py
+-rw-r--r--   0        0        0     8794 2023-05-03 05:48:40.390181 gidapptools-0.5.2/gidapptools/utility/helper.py
+-rw-r--r--   0        0        0     2529 2023-01-07 14:13:33.732999 gidapptools-0.5.2/gidapptools/utility/kwarg_dict.py
+-rw-r--r--   0        0        0        0 2022-08-06 21:26:08.033946 gidapptools-0.5.2/gidapptools/vendored/__init__.py
+-rw-r--r--   0        0        0     7128 2022-11-02 13:03:50.593217 gidapptools-0.5.2/gidapptools/vendored/atomic_writes.py
+-rw-r--r--   0        0        0     1069 2022-06-30 02:44:23.800813 gidapptools-0.5.2/gidapptools/vendored/atomic_writes_LICENSE
+-rw-r--r--   0        0        0     3424 2024-05-26 17:04:20.571571 gidapptools-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 gidapptools-0.5.2/PKG-INFO
```

### Comparing `gidapptools-0.5.1/LICENSE` & `gidapptools-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/README.rst` & `gidapptools-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/__init__.py` & `gidapptools-0.5.2/gidapptools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 WiP
 """
 
 from gidapptools.meta_data.interface import setup_meta_data, get_meta_info, get_meta_item, get_meta_paths
 from gidapptools.gid_logger.logger import setup_main_logger, get_logger, setup_main_logger_with_file_logging, get_main_logger, get_handlers
 
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 from pathlib import Path
 from tzlocal import reload_localzone
 
 THIS_FILE_DIR = Path(__file__).resolve().parent
```

### Comparing `gidapptools-0.5.1/gidapptools/__main__.py` & `gidapptools-0.5.2/gidapptools/__main__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/abstract_classes/abstract_meta_factory.py` & `gidapptools-0.5.2/gidapptools/abstract_classes/abstract_meta_factory.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/abstract_classes/abstract_meta_item.py` & `gidapptools-0.5.2/gidapptools/abstract_classes/abstract_meta_item.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/cli_info.py` & `gidapptools-0.5.2/gidapptools/cli_info.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/code_generation/python.py` & `gidapptools-0.5.2/gidapptools/code_generation/python.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/custom_types.py` & `gidapptools-0.5.2/gidapptools/custom_types.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/conversion_data.py` & `gidapptools-0.5.2/gidapptools/data/conversion_data.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/__init__.py` & `gidapptools-0.5.2/gidapptools/data/gifs/__init__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_1.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_1.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_2.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_2.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_3.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_3.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_4.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_4.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_5.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_5.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_6.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_6.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_7.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_7.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/gifs/busy_spinner_cat.gif` & `gidapptools-0.5.2/gidapptools/data/gifs/busy_spinner_cat.gif`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/data/json/webcolors.json` & `gidapptools-0.5.2/gidapptools/data/json/webcolors.json`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/errors.py` & `gidapptools-0.5.2/gidapptools/errors.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/ast_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/ast_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/checker.py` & `gidapptools-0.5.2/gidapptools/general_helper/checker.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/class_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/class_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/compress.py` & `gidapptools-0.5.2/gidapptools/general_helper/compress.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/concurrency/events.py` & `gidapptools-0.5.2/gidapptools/general_helper/concurrency/events.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/concurrency/locks.py` & `gidapptools-0.5.2/gidapptools/general_helper/concurrency/locks.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/concurrency/switch.py` & `gidapptools-0.5.2/gidapptools/general_helper/concurrency/switch.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/conversion.py` & `gidapptools-0.5.2/gidapptools/general_helper/conversion.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/date_time.py` & `gidapptools-0.5.2/gidapptools/general_helper/date_time.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/development/class_hierachy_inspect.py` & `gidapptools-0.5.2/gidapptools/general_helper/development/class_hierachy_inspect.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/development/inspect_helpers.py` & `gidapptools-0.5.2/gidapptools/general_helper/development/inspect_helpers.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/development/misc.py` & `gidapptools-0.5.2/gidapptools/general_helper/development/misc.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/dict_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/dict_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/dispatch_table.py` & `gidapptools-0.5.2/gidapptools/general_helper/dispatch_table.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/enums.py` & `gidapptools-0.5.2/gidapptools/general_helper/enums.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/font/font_locating.py` & `gidapptools-0.5.2/gidapptools/general_helper/font/font_locating.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/general.py` & `gidapptools-0.5.2/gidapptools/general_helper/general.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/general_classes.py` & `gidapptools-0.5.2/gidapptools/general_helper/general_classes.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/hashing.py` & `gidapptools-0.5.2/gidapptools/general_helper/hashing.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/import_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/import_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/io_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/io_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/meta_helper/single_running_instance.py` & `gidapptools-0.5.2/gidapptools/general_helper/meta_helper/single_running_instance.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/mixins/file_mixin.py` & `gidapptools-0.5.2/gidapptools/general_helper/mixins/file_mixin.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/output_helper/console_colors.py` & `gidapptools-0.5.2/gidapptools/general_helper/output_helper/console_colors.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/rich_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/rich_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/rich_styles.py` & `gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/rich_styles.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/output_helper/rich_helper/rich_themes.py` & `gidapptools-0.5.2/gidapptools/general_helper/output_helper/rich_helper/rich_themes.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/path_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/path_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/regex/datetime_regex.py` & `gidapptools-0.5.2/gidapptools/general_helper/regex/datetime_regex.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/string_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/string_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/timing.py` & `gidapptools-0.5.2/gidapptools/general_helper/timing.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/typing_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/typing_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/general_helper/web_helper.py` & `gidapptools-0.5.2/gidapptools/general_helper/web_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_argparse/custom_parser.py` & `gidapptools-0.5.2/gidapptools/gid_argparse/custom_parser.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/__init__.py` & `gidapptools-0.5.2/gidapptools/gid_config/__init__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/conversion/base_converters.py` & `gidapptools-0.5.2/gidapptools/gid_config/conversion/base_converters.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/conversion/conversion_table.py` & `gidapptools-0.5.2/gidapptools/gid_config/conversion/conversion_table.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/conversion/converter_grammar.py` & `gidapptools-0.5.2/gidapptools/gid_config/conversion/converter_grammar.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/conversion/extra_base_typus.py` & `gidapptools-0.5.2/gidapptools/gid_config/conversion/extra_base_typus.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/conversion/spec_data.py` & `gidapptools-0.5.2/gidapptools/gid_config/conversion/spec_data.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/conversion/spec_item.py` & `gidapptools-0.5.2/gidapptools/gid_config/conversion/spec_item.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/enums.py` & `gidapptools-0.5.2/gidapptools/gid_config/enums.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/interface.py` & `gidapptools-0.5.2/gidapptools/gid_config/interface.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/parser/config_data.py` & `gidapptools-0.5.2/gidapptools/gid_config/parser/config_data.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/parser/grammar.py` & `gidapptools-0.5.2/gidapptools/gid_config/parser/grammar.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/parser/ini_parser.py` & `gidapptools-0.5.2/gidapptools/gid_config/parser/ini_parser.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_config/parser/tokens.py` & `gidapptools-0.5.2/gidapptools/gid_config/parser/tokens.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/apsw_database.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/constants.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/constants.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/commit_hook_functions.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/profile_hook_functions.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/rollback_hook_functions.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/update_hook_functions.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/hook_functions/wal_hook_functions.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py` & `gidapptools-0.5.2/gidapptools/gid_database/orm_peewee/sqlite/pragma_info.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_image/size_manipulation.py` & `gidapptools-0.5.2/gidapptools/gid_image/size_manipulation.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/enums.py` & `gidapptools-0.5.2/gidapptools/gid_logger/enums.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/fake_logger.py` & `gidapptools-0.5.2/gidapptools/gid_logger/fake_logger.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/formatter.py` & `gidapptools-0.5.2/gidapptools/gid_logger/formatter.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/handler.py` & `gidapptools-0.5.2/gidapptools/gid_logger/handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 """
 
 # region [Imports]
 
 # * Standard Library Imports ---------------------------------------------------------------------------->
 import re
 import logging
+from time import perf_counter
+from threading import Lock, RLock
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Union
+from typing import TYPE_CHECKING, Any, Union, Literal, Callable
 from pathlib import Path
 from datetime import datetime, timezone
 from collections import deque
 from logging.handlers import BaseRotatingHandler
-
+from frozendict import frozendict
 # * Gid Imports ----------------------------------------------------------------------------------------->
 from gidapptools.general_helper.conversion import human2bytes
 from gidapptools.general_helper.regex.datetime_regex import datetime_format_to_regex
 
 # * Type-Checking Imports --------------------------------------------------------------------------------->
 if TYPE_CHECKING:
     from gidapptools.custom_types import PATH_TYPE
@@ -185,57 +187,128 @@
 LOG_DEQUE_TYPE = deque["LOG_RECORD_TYPES"]
 
 
 class GidStoringHandler(logging.Handler):
 
     def __init__(self, max_storage_size: int = None) -> None:
         super().__init__()
+        self.emit_lock = RLock()
+        self._callbacks: dict[str, list[Callable[["LOG_RECORD_TYPES"], None]]] = {"ALL": [],
+                                                                                  "DEBUG": [],
+                                                                                  "INFO": [],
+                                                                                  "WARNING": [],
+                                                                                  "CRITICAL": [],
+                                                                                  "ERROR": []}
         self.debug_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
         self.info_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
         self.warning_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
         self.critical_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
         self.error_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
         self.other_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
 
-        self.table = {'CRITICAL': self.critical_messages,
-                      'FATAL': self.critical_messages,
-                      'ERROR': self.error_messages,
-                      'WARN': self.warning_messages,
-                      'WARNING': self.warning_messages,
-                      'INFO': self.info_messages,
-                      'DEBUG': self.debug_messages,
-                      "OTHER": self.other_messages}
+        self._all_messages: "LOG_DEQUE_TYPE" = deque(maxlen=max_storage_size)
+
+        self.table = frozendict({'CRITICAL': self.critical_messages,
+                                 'FATAL': self.critical_messages,
+                                 'ERROR': self.error_messages,
+                                 'WARN': self.warning_messages,
+                                 'WARNING': self.warning_messages,
+                                 'INFO': self.info_messages,
+                                 'DEBUG': self.debug_messages,
+                                 "OTHER": self.other_messages})
+
+    @property
+    def all_deques(self) -> tuple["LOG_DEQUE_TYPE"]:
+        # dupicates = {"FATAL", "WARN"}
+        return tuple({k: v for k, v in self.table.items() if k not in {"FATAL", "WARN"}}.values())
+        # _out = []
+        # for table in self.table.values():
+        #     if table not in _out:
+        #         _out.append(table)
+
+        # return tuple(_out)
+
+    def add_callback(self, typus: Literal["ALL", "DEBUG", "INFO", "WARNING", "CRITICAL", "ERROR"], callback: Callable[["LOG_RECORD_TYPES"], None]):
+        callback_list = self._callbacks[typus]
+        if callback not in callback_list:
+            callback_list.append(callback)
+
+    def remove_callback(self, typus: Literal["ALL", "DEBUG", "INFO", "WARNING", "CRITICAL", "ERROR"], callback: Callable[["LOG_RECORD_TYPES"], None]):
+        try:
+            self._callbacks[typus].remove(callback)
+        except ValueError:
+            pass
 
     def set_max_storage_size(self, max_storage_size: int = None):
         for store in self.table.values():
             store.maxlen = max_storage_size
 
     def emit(self, record: "LOG_RECORD_TYPES") -> None:
+        with self.emit_lock:
+            target = self.table.get(record.levelname, self.other_messages)
+
+            target.append(record)
+
+            self._all_messages.append(record)
+
+            for callback in self._callbacks.get("ALL", []):
+                callback(record)
+
+            typus = record.levelname.upper()
+            if typus == "WARN":
+                typus = "WARNING"
 
-        target = self.table.get(record.levelname, self.other_messages)
+            if typus == "FATAL":
+                typus = "CRITICAL"
 
-        target.append(record)
+            for callback in self._callbacks.get(typus, []):
+                callback(record)
 
     def get_stored_messages(self) -> dict[str, tuple["LOG_RECORD_TYPES"]]:
-        _out = {}
-        for level, store in self.table.items():
-            _out[level] = tuple(store)
 
-        return _out
+        return {k: tuple(v) for k, v in self.table.items() if k not in {"FATAL", "WARN"}}
+        # _out = {}
+        # for level, store in self.table.items():
+        #     if level == "FATAL":
+        #         level = "CRITICAL"
+        #     elif level == "WARN":
+        #         level = "WARNING"
+        #     _out[level] = tuple(store)
+
+        # return _out
+
+    def get_all_messages(self, formatted: bool = False) -> tuple["LOG_RECORD_TYPES"]:
+        with self.emit_lock:
+            all_messages = tuple(self._all_messages)
+            if formatted is True:
+                list(self.format(r) for r in all_messages)
+
+            return all_messages
 
     def get_formated_messages(self) -> dict[str, tuple[str]]:
         _out = {}
         for level, store in self.table.items():
+            if level == "FATAL":
+                level = "CRITICAL"
+            elif level == "WARN":
+                level = "WARNING"
             _out[level] = tuple(self.format(r) for r in store)
         return _out
 
     def __len__(self) -> int:
-        _out = 0
-        for store in self.table.values():
-            _out += len(store)
-        return _out
+        with self.emit_lock:
+            return len(self._all_messages)
+
+    def clear(self, typus: None | Literal["debug", "info", "warning", "critical", "error", "other"] = None):
+        if typus is not None:
+            _deque: "LOG_DEQUE_TYPE" = getattr(self, f"{typus.casefold()}_messages")
+            _deque.clear()
+
+        else:
+            for _deque in (self.debug_messages, self.info_messages, self.warning_messages, self.critical_messages, self.error_messages, self.other_messages, self._all_messages):
+                _deque.clear()
 # region [Main_Exec]
 
 
 if __name__ == '__main__':
     pass
 # endregion [Main_Exec]
```

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/logger.py` & `gidapptools-0.5.2/gidapptools/gid_logger/logger.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/misc.py` & `gidapptools-0.5.2/gidapptools/gid_logger/misc.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_logger/records.py` & `gidapptools-0.5.2/gidapptools/gid_logger/records.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_parsing/py_log_parsing.py` & `gidapptools-0.5.2/gidapptools/gid_parsing/py_log_parsing.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_parsing/tokens/base_tokens.py` & `gidapptools-0.5.2/gidapptools/gid_parsing/tokens/base_tokens.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_parsing/universal/character_elements.py` & `gidapptools-0.5.2/gidapptools/gid_parsing/universal/character_elements.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_parsing/universal/datetime_elements.py` & `gidapptools-0.5.2/gidapptools/gid_parsing/universal/datetime_elements.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_signal/interface.py` & `gidapptools-0.5.2/gidapptools/gid_signal/interface.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_signal/signal_registry.py` & `gidapptools-0.5.2/gidapptools/gid_signal/signal_registry.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_signal/signals/abstract_signal.py` & `gidapptools-0.5.2/gidapptools/gid_signal/signals/abstract_signal.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_signal/signals/basic_signal.py` & `gidapptools-0.5.2/gidapptools/gid_signal/signals/basic_signal.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_utility/version_item.py` & `gidapptools-0.5.2/gidapptools/gid_utility/version_item.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_warning/deprecation.py` & `gidapptools-0.5.2/gidapptools/gid_warning/deprecation.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gid_warning/experimental.py` & `gidapptools-0.5.2/gidapptools/gid_warning/experimental.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/__init__.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/__init__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/debugging_icon.png` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/debugging_icon.png`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/default_app_icon.png` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/default_app_icon.png`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/images/placeholder.png` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/images/placeholder.png`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/about_template.jinja_html`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/_data/templates/arg_doc_html_template.jinja_html`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/abc/abstract_syntax_highlighting_rule.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/abc/abstract_syntax_highlighting_rule.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/application.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/application.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/application_info.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/application_info.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/application_new.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/application_new.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/main_window.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/main_window.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/menu_bar.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/menu_bar.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/status_bar.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/status_bar.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/basics/sys_tray.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/basics/sys_tray.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_value_widgets/__init__.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_value_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_value_widgets/_checks.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_value_widgets/_checks.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_value_widgets/standard_types.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_value_widgets/standard_types.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/debug_widget.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/debug_widget.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/debug/event_analyzer.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/debug/event_analyzer.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/dialogs/app_info_dialog.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/command_line_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/misc.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/misc.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/object_name.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/object_name.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/syntax_highlighting/rules.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/syntax_highlighting/rules.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/window_geometry_helper.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/window_geometry_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/helper/window_reference_keeper.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/helper/window_reference_keeper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/layouts/sorted_layout.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/layouts/sorted_layout.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/layouts/vertical_form_layout.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/models/basic_model.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/models/basic_model.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/resources/placeholder.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/resources/placeholder.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/resources/resources_helper.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/resources/resources_helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/sub_typing.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/sub_typing.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/category_select_widget.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/category_select_widget.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/collapsible_widget.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/hyperlink_label.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/hyperlink_label.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/icon_text_button.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/icon_text_button.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/json_editor.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/json_editor.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/scrollable_widget.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/scrollable_widget.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/separator_lines.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/separator_lines.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/spinner_widget.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/spinner_widget.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidapptools_qt/widgets/std_stream_widget.py` & `gidapptools-0.5.2/gidapptools/gidapptools_qt/widgets/std_stream_widget.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/color.py` & `gidapptools-0.5.2/gidapptools/gidcolor/color.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/color_item.py` & `gidapptools-0.5.2/gidapptools/gidcolor/color_item.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/color_string_formatter.py` & `gidapptools-0.5.2/gidapptools/gidcolor/color_string_formatter.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/coversion.py` & `gidapptools-0.5.2/gidapptools/gidcolor/coversion.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/misc_calculations.py` & `gidapptools-0.5.2/gidapptools/gidcolor/misc_calculations.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/palette.py` & `gidapptools-0.5.2/gidapptools/gidcolor/palette.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/gidcolor/preset_colors/web_colors.py` & `gidapptools-0.5.2/gidapptools/gidcolor/preset_colors/web_colors.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/config_kwargs.py` & `gidapptools-0.5.2/gidapptools/meta_data/config_kwargs.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/interface.py` & `gidapptools-0.5.2/gidapptools/meta_data/interface.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/meta_info/meta_info_factory.py` & `gidapptools-0.5.2/gidapptools/meta_data/meta_info/meta_info_factory.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/meta_info/meta_info_item.py` & `gidapptools-0.5.2/gidapptools/meta_data/meta_info/meta_info_item.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/meta_paths/appdirs_implementations.py` & `gidapptools-0.5.2/gidapptools/meta_data/meta_paths/appdirs_implementations.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/meta_paths/meta_paths_factory.py` & `gidapptools-0.5.2/gidapptools/meta_data/meta_paths/meta_paths_factory.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/meta_data/meta_paths/meta_paths_item.py` & `gidapptools-0.5.2/gidapptools/meta_data/meta_paths/meta_paths_item.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/utility/enums.py` & `gidapptools-0.5.2/gidapptools/utility/enums.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/utility/helper.py` & `gidapptools-0.5.2/gidapptools/utility/helper.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/utility/kwarg_dict.py` & `gidapptools-0.5.2/gidapptools/utility/kwarg_dict.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/vendored/atomic_writes.py` & `gidapptools-0.5.2/gidapptools/vendored/atomic_writes.py`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/gidapptools/vendored/atomic_writes_LICENSE` & `gidapptools-0.5.2/gidapptools/vendored/atomic_writes_LICENSE`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/pyproject.toml` & `gidapptools-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gidapptools-0.5.1/PKG-INFO` & `gidapptools-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gidapptools
-Version: 0.5.1
+Version: 0.5.2
 Summary: WiP
 Author: brocaprogs
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: attrs>=22.1
 Requires-Dist: frozendict>=2.3
```

