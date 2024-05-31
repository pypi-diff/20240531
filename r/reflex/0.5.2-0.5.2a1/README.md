# Comparing `tmp/reflex-0.5.2.tar.gz` & `tmp/reflex-0.5.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.5.2.tar", max compression
+gzip compressed data, was "reflex-0.5.2a1.tar", max compression
```

## Comparing `reflex-0.5.2.tar` & `reflex-0.5.2a1.tar`

### file list

```diff
@@ -1,522 +1,522 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.2/LICENSE
--rw-r--r--   0        0        0     9838 2024-05-23 22:07:24.004599 reflex-0.5.2/README.md
--rw-r--r--   0        0        0     2972 2024-05-31 00:00:20.587062 reflex-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.2/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.2/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      926 2024-05-23 22:07:24.026702 reflex-0.5.2/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.2/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.2/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.2/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.2/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.2/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.2/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.2/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2927 2024-05-23 22:07:24.026869 reflex-0.5.2/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.2/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-05-23 22:07:24.027050 reflex-0.5.2/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10906 2024-05-23 22:07:24.027242 reflex-0.5.2/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8381 2024-05-23 22:07:24.027471 reflex-0.5.2/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-05-23 22:07:24.027876 reflex-0.5.2/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-05-23 22:07:24.028048 reflex-0.5.2/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-05-23 22:07:24.028210 reflex-0.5.2/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.2/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.2/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.2/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-05-23 22:07:24.028477 reflex-0.5.2/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-05-23 22:07:24.028657 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-05-23 22:07:24.028787 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-05-23 22:07:24.035433 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-05-23 22:07:24.035615 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-05-23 22:07:24.035773 reflex-0.5.2/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.2/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-05-23 22:07:24.036845 reflex-0.5.2/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-05-23 22:07:24.036930 reflex-0.5.2/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-05-23 22:07:24.037352 reflex-0.5.2/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-05-23 22:07:24.037689 reflex-0.5.2/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-05-23 22:07:24.037946 reflex-0.5.2/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.2/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-05-23 22:07:24.038352 reflex-0.5.2/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.2/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-05-23 22:07:24.038521 reflex-0.5.2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.2/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.2/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-05-23 22:07:24.038697 reflex-0.5.2/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.2/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-05-23 22:07:24.038822 reflex-0.5.2/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.2/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      761 2024-05-23 22:07:24.039110 reflex-0.5.2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-05-23 22:07:24.039386 reflex-0.5.2/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.2/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.2/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.2/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-05-23 22:07:24.039706 reflex-0.5.2/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.2/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.2/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2024-05-24 16:47:17.136778 reflex-0.5.2/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2024-05-24 16:47:17.136946 reflex-0.5.2/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.2/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-05-23 22:07:24.039831 reflex-0.5.2/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0      528 2024-05-23 22:07:24.039893 reflex-0.5.2/reflex/.templates/web/utils/helpers/debounce.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.2/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0      566 2024-05-23 22:07:24.039949 reflex-0.5.2/reflex/.templates/web/utils/helpers/throttle.js
--rw-r--r--   0        0        0    22617 2024-05-23 22:07:24.040119 reflex-0.5.2/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5831 2024-05-23 22:07:24.040585 reflex-0.5.2/reflex/__init__.py
--rw-r--r--   0        0        0     7791 2024-05-26 21:36:23.014634 reflex-0.5.2/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.2/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.2/reflex/admin.py
--rw-r--r--   0        0        0    48956 2024-05-24 16:47:17.137462 reflex-0.5.2/reflex/app.py
--rw-r--r--   0        0        0     1227 2024-05-23 22:07:24.041327 reflex-0.5.2/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4274 2024-05-23 22:07:24.041585 reflex-0.5.2/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.2/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17455 2024-05-23 22:07:24.041899 reflex-0.5.2/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-05-23 22:07:24.042172 reflex-0.5.2/reflex/compiler/templates.py
--rw-r--r--   0        0        0    13274 2024-05-23 22:07:24.042547 reflex-0.5.2/reflex/compiler/utils.py
--rw-r--r--   0        0        0      552 2024-05-23 22:07:24.042676 reflex-0.5.2/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-05-23 22:07:24.042785 reflex-0.5.2/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-05-23 22:07:24.042894 reflex-0.5.2/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-05-24 18:17:26.775810 reflex-0.5.2/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-05-23 22:07:24.043424 reflex-0.5.2/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.2/reflex/components/base/body.py
--rw-r--r--   0        0        0     3206 2024-05-24 18:17:28.445017 reflex-0.5.2/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-05-23 22:07:24.043906 reflex-0.5.2/reflex/components/base/document.py
--rw-r--r--   0        0        0    14232 2024-05-24 18:17:26.993081 reflex-0.5.2/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-05-23 22:07:24.044107 reflex-0.5.2/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3218 2024-05-24 18:17:26.730059 reflex-0.5.2/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2024-05-23 22:07:24.044322 reflex-0.5.2/reflex/components/base/head.py
--rw-r--r--   0        0        0     6002 2024-05-24 18:17:27.212239 reflex-0.5.2/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.2/reflex/components/base/link.py
--rw-r--r--   0        0        0     6990 2024-05-24 18:17:28.411498 reflex-0.5.2/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.2/reflex/components/base/meta.py
--rw-r--r--   0        0        0    12804 2024-05-24 18:17:27.232380 reflex-0.5.2/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.2/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-05-24 18:17:27.261455 reflex-0.5.2/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-05-23 22:07:24.045051 reflex-0.5.2/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-05-23 22:07:24.045134 reflex-0.5.2/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    10917 2024-05-24 18:17:24.861757 reflex-0.5.2/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-05-23 22:07:24.045326 reflex-0.5.2/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-05-23 22:07:24.045398 reflex-0.5.2/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3654 2024-05-24 18:17:23.594412 reflex-0.5.2/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-05-23 22:07:24.045575 reflex-0.5.2/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3229 2024-05-24 18:17:23.555248 reflex-0.5.2/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-05-23 22:07:24.045714 reflex-0.5.2/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     3934 2024-05-24 18:17:23.503426 reflex-0.5.2/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-05-23 22:07:24.045852 reflex-0.5.2/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3251 2024-05-24 18:17:24.668110 reflex-0.5.2/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.046229 reflex-0.5.2/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    12991 2024-05-24 18:17:24.625763 reflex-0.5.2/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-05-23 22:07:24.046512 reflex-0.5.2/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.921677 reflex-0.5.2/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-05-23 22:07:24.046775 reflex-0.5.2/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27252 2024-05-24 18:17:24.570212 reflex-0.5.2/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-05-23 22:07:24.046980 reflex-0.5.2/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    15734 2024-05-24 18:17:23.854192 reflex-0.5.2/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-05-23 22:07:24.047198 reflex-0.5.2/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3510 2024-05-23 22:07:24.047299 reflex-0.5.2/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    15803 2024-05-24 18:17:24.269813 reflex-0.5.2/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-05-23 22:07:24.047512 reflex-0.5.2/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18525 2024-05-24 18:17:23.577560 reflex-0.5.2/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-05-23 22:07:24.047752 reflex-0.5.2/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20003 2024-05-24 18:17:23.981249 reflex-0.5.2/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-05-23 22:07:24.047917 reflex-0.5.2/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3258 2024-05-24 18:17:23.263087 reflex-0.5.2/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-05-23 22:07:24.048055 reflex-0.5.2/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-05-23 22:07:24.048128 reflex-0.5.2/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12381 2024-05-24 18:17:24.114056 reflex-0.5.2/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-05-23 22:07:24.048304 reflex-0.5.2/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7637 2024-05-24 18:17:24.157731 reflex-0.5.2/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-05-23 22:07:24.048486 reflex-0.5.2/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4278 2024-05-24 18:17:24.226071 reflex-0.5.2/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-05-23 22:07:24.048623 reflex-0.5.2/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10690 2024-05-24 18:17:24.080524 reflex-0.5.2/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-05-23 22:07:24.048760 reflex-0.5.2/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4107 2024-05-24 18:17:24.399345 reflex-0.5.2/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-05-23 22:07:24.048929 reflex-0.5.2/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-05-23 22:07:24.049012 reflex-0.5.2/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10545 2024-05-24 18:17:24.063143 reflex-0.5.2/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-05-23 22:07:24.049323 reflex-0.5.2/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10301 2024-05-24 18:17:23.972016 reflex-0.5.2/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-05-23 22:07:24.049528 reflex-0.5.2/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18459 2024-05-24 18:17:23.734040 reflex-0.5.2/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-05-23 22:07:24.049762 reflex-0.5.2/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.844965 reflex-0.5.2/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-05-23 22:07:24.049973 reflex-0.5.2/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-05-24 18:17:23.355983 reflex-0.5.2/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-05-23 22:07:24.050115 reflex-0.5.2/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13339 2024-05-24 18:17:24.448401 reflex-0.5.2/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-05-23 22:07:24.050281 reflex-0.5.2/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-05-24 18:17:23.790638 reflex-0.5.2/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-05-23 22:07:24.050478 reflex-0.5.2/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20619 2024-05-24 18:17:23.741717 reflex-0.5.2/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-05-23 22:07:24.050744 reflex-0.5.2/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4668 2024-05-24 18:17:23.790245 reflex-0.5.2/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-05-23 22:07:24.050915 reflex-0.5.2/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21514 2024-05-24 18:17:24.148687 reflex-0.5.2/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-05-23 22:07:24.051118 reflex-0.5.2/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-05-23 22:07:24.051235 reflex-0.5.2/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18093 2024-05-24 18:17:24.503442 reflex-0.5.2/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-05-23 22:07:24.051441 reflex-0.5.2/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-05-24 18:17:23.849665 reflex-0.5.2/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6503 2024-05-23 22:07:24.051630 reflex-0.5.2/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9369 2024-05-24 18:17:23.634451 reflex-0.5.2/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3172 2024-05-23 22:07:24.051792 reflex-0.5.2/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8410 2024-05-24 18:17:24.617235 reflex-0.5.2/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4543 2024-05-23 22:07:24.051994 reflex-0.5.2/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    13939 2024-05-24 18:17:23.752785 reflex-0.5.2/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-05-23 22:07:24.052210 reflex-0.5.2/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-05-24 18:17:23.466505 reflex-0.5.2/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-05-23 22:07:24.052410 reflex-0.5.2/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.839820 reflex-0.5.2/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-05-23 22:07:24.052576 reflex-0.5.2/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6531 2024-05-24 18:17:23.439877 reflex-0.5.2/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-05-23 22:07:24.052732 reflex-0.5.2/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-05-24 18:17:23.406701 reflex-0.5.2/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-05-23 22:07:24.052879 reflex-0.5.2/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.338287 reflex-0.5.2/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-05-23 22:07:24.053058 reflex-0.5.2/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-05-23 22:07:24.053146 reflex-0.5.2/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3379 2024-05-24 18:17:24.134750 reflex-0.5.2/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-05-23 22:07:24.053303 reflex-0.5.2/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3662 2024-05-24 18:17:23.684534 reflex-0.5.2/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-05-23 22:07:24.053447 reflex-0.5.2/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    13850 2024-05-24 18:17:23.661739 reflex-0.5.2/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-05-23 22:07:24.053601 reflex-0.5.2/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8692 2024-05-24 18:17:23.861262 reflex-0.5.2/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-05-23 22:07:24.053774 reflex-0.5.2/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3431 2024-05-24 18:17:23.906150 reflex-0.5.2/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-05-23 22:07:24.053931 reflex-0.5.2/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4138 2024-05-24 18:17:23.856235 reflex-0.5.2/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-05-23 22:07:24.054108 reflex-0.5.2/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    13853 2024-05-24 18:17:23.508048 reflex-0.5.2/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-05-23 22:07:24.054265 reflex-0.5.2/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3230 2024-05-24 18:17:23.753119 reflex-0.5.2/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-05-23 22:07:24.054391 reflex-0.5.2/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12219 2024-05-24 18:17:23.812312 reflex-0.5.2/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-05-23 22:07:24.054557 reflex-0.5.2/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     6943 2024-05-24 18:17:24.095832 reflex-0.5.2/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-05-23 22:07:24.054738 reflex-0.5.2/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-05-23 22:07:24.054834 reflex-0.5.2/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10445 2024-05-24 18:17:25.119256 reflex-0.5.2/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2462 2024-05-23 22:07:24.054978 reflex-0.5.2/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6271 2024-05-24 18:17:24.970682 reflex-0.5.2/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-05-23 22:07:24.055112 reflex-0.5.2/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-05-24 18:17:25.284214 reflex-0.5.2/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-05-23 22:07:24.055273 reflex-0.5.2/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-05-23 22:07:24.055368 reflex-0.5.2/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13575 2024-05-24 18:17:24.223760 reflex-0.5.2/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-05-23 22:07:24.055559 reflex-0.5.2/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-05-24 18:17:24.135785 reflex-0.5.2/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-05-23 22:07:24.055765 reflex-0.5.2/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6233 2024-05-24 18:17:24.315782 reflex-0.5.2/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-05-23 22:07:24.055929 reflex-0.5.2/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    27922 2024-05-24 18:17:23.937771 reflex-0.5.2/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-05-23 22:07:24.056145 reflex-0.5.2/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-05-23 22:07:24.056257 reflex-0.5.2/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    23985 2024-05-24 18:17:25.493171 reflex-0.5.2/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-05-23 22:07:24.056468 reflex-0.5.2/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25406 2024-05-24 18:17:24.311417 reflex-0.5.2/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-05-23 22:07:24.056645 reflex-0.5.2/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    28682 2024-05-24 18:17:25.078723 reflex-0.5.2/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-05-23 22:07:24.056817 reflex-0.5.2/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23549 2024-05-24 18:17:25.909264 reflex-0.5.2/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-05-23 22:07:24.057050 reflex-0.5.2/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    29893 2024-05-24 18:17:24.574288 reflex-0.5.2/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-05-23 22:07:24.057260 reflex-0.5.2/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6060 2024-05-24 18:17:24.470002 reflex-0.5.2/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-05-23 22:07:24.057423 reflex-0.5.2/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-05-23 22:07:24.057495 reflex-0.5.2/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3706 2024-05-24 18:17:24.173439 reflex-0.5.2/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-05-23 22:07:24.057873 reflex-0.5.2/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3645 2024-05-24 18:17:24.260699 reflex-0.5.2/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-05-23 22:07:24.058053 reflex-0.5.2/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3372 2024-05-24 18:17:24.311205 reflex-0.5.2/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-05-23 22:07:24.058204 reflex-0.5.2/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3596 2024-05-24 18:17:24.218016 reflex-0.5.2/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    77001 2024-05-23 22:07:24.058552 reflex-0.5.2/reflex/components/component.py
--rw-r--r--   0        0        0      943 2024-05-23 22:07:24.058811 reflex-0.5.2/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     8043 2024-05-23 22:07:24.058914 reflex-0.5.2/reflex/components/core/banner.py
--rw-r--r--   0        0        0    22528 2024-05-24 18:17:25.155664 reflex-0.5.2/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-05-23 22:07:24.059088 reflex-0.5.2/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6264 2024-05-24 18:17:24.651237 reflex-0.5.2/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-05-23 22:07:24.059236 reflex-0.5.2/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6163 2024-05-23 22:07:24.059313 reflex-0.5.2/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4820 2024-05-23 22:07:24.059567 reflex-0.5.2/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4216 2024-05-24 18:17:24.719439 reflex-0.5.2/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4732 2024-05-23 22:07:24.060166 reflex-0.5.2/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1284 2024-05-23 22:07:24.060230 reflex-0.5.2/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-05-24 18:17:24.552128 reflex-0.5.2/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-05-23 22:07:24.060774 reflex-0.5.2/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9484 2024-05-23 22:07:24.060867 reflex-0.5.2/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-05-23 22:07:24.061035 reflex-0.5.2/reflex/components/core/responsive.py
--rw-r--r--   0        0        0    10146 2024-05-23 22:07:24.061115 reflex-0.5.2/reflex/components/core/upload.py
--rw-r--r--   0        0        0    17147 2024-05-24 18:17:24.472841 reflex-0.5.2/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-05-23 22:07:24.061822 reflex-0.5.2/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11347 2024-05-24 16:47:17.137792 reflex-0.5.2/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31197 2024-05-24 18:17:25.129041 reflex-0.5.2/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-05-23 22:07:24.062397 reflex-0.5.2/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-05-24 18:17:24.719094 reflex-0.5.2/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-05-23 22:07:24.062734 reflex-0.5.2/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.2/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.2/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.2/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.2/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.2/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.2/reflex/components/el/element.py
--rw-r--r--   0        0        0     3213 2024-05-24 18:17:24.504591 reflex-0.5.2/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-05-23 22:07:24.063280 reflex-0.5.2/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-05-23 22:07:24.063391 reflex-0.5.2/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6340 2024-05-24 18:17:25.763640 reflex-0.5.2/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20167 2024-05-23 22:07:24.063679 reflex-0.5.2/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0    99555 2024-05-24 18:17:29.297573 reflex-0.5.2/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-05-23 22:07:24.064187 reflex-0.5.2/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   164607 2024-05-24 18:17:28.121848 reflex-0.5.2/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     8467 2024-05-23 22:07:24.064879 reflex-0.5.2/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    93669 2024-05-24 18:17:25.809803 reflex-0.5.2/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.2/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28031 2024-05-24 18:17:26.420859 reflex-0.5.2/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.2/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42033 2024-05-24 18:17:28.117892 reflex-0.5.2/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-05-23 22:07:24.065615 reflex-0.5.2/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19615 2024-05-24 18:17:25.678066 reflex-0.5.2/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-05-23 22:07:24.065964 reflex-0.5.2/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    87242 2024-05-24 18:17:27.638168 reflex-0.5.2/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-05-23 22:07:24.066552 reflex-0.5.2/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    61849 2024-05-24 18:17:25.354377 reflex-0.5.2/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-05-23 22:07:24.067050 reflex-0.5.2/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    89115 2024-05-24 18:17:25.804750 reflex-0.5.2/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-05-23 22:07:24.067621 reflex-0.5.2/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4304 2024-05-23 22:07:24.067706 reflex-0.5.2/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7053 2024-05-24 18:17:23.290206 reflex-0.5.2/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-05-23 22:07:24.067888 reflex-0.5.2/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-05-23 22:07:24.067968 reflex-0.5.2/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34077 2024-05-23 22:07:24.068288 reflex-0.5.2/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    37918 2024-05-24 18:17:27.204674 reflex-0.5.2/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-05-23 22:07:24.068931 reflex-0.5.2/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    10867 2024-05-23 22:07:24.069105 reflex-0.5.2/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5100 2024-05-24 18:17:24.542827 reflex-0.5.2/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-05-23 22:07:24.069399 reflex-0.5.2/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-05-23 22:07:24.069584 reflex-0.5.2/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-05-23 22:07:24.069684 reflex-0.5.2/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-05-23 22:07:24.069782 reflex-0.5.2/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-05-24 18:17:24.208012 reflex-0.5.2/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-05-23 22:07:24.069942 reflex-0.5.2/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-05-23 22:07:24.070005 reflex-0.5.2/reflex/components/next/base.py
--rw-r--r--   0        0        0     3233 2024-05-24 18:17:23.601458 reflex-0.5.2/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-05-23 22:07:24.070176 reflex-0.5.2/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-05-24 18:17:23.566367 reflex-0.5.2/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-05-23 22:07:24.070408 reflex-0.5.2/reflex/components/next/link.py
--rw-r--r--   0        0        0     3461 2024-05-24 18:17:23.327764 reflex-0.5.2/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-05-23 22:07:24.070545 reflex-0.5.2/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-05-24 18:17:23.378778 reflex-0.5.2/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-05-23 22:07:24.070725 reflex-0.5.2/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-05-23 22:07:24.070795 reflex-0.5.2/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     6865 2024-05-24 18:17:24.804257 reflex-0.5.2/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      906 2024-05-23 22:07:24.071050 reflex-0.5.2/reflex/components/props.py
--rw-r--r--   0        0        0      112 2024-05-23 22:07:24.071248 reflex-0.5.2/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-05-23 22:07:24.071337 reflex-0.5.2/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    15801 2024-05-24 16:47:17.138407 reflex-0.5.2/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    38019 2024-05-24 18:17:25.203694 reflex-0.5.2/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-05-23 22:07:24.071818 reflex-0.5.2/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6478 2024-05-24 18:17:25.726505 reflex-0.5.2/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-05-23 22:07:24.071992 reflex-0.5.2/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34484 2024-05-24 18:17:25.412916 reflex-0.5.2/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4941 2024-05-24 16:47:17.138863 reflex-0.5.2/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48143 2024-05-24 18:17:26.612449 reflex-0.5.2/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     4022 2024-05-24 16:47:17.139254 reflex-0.5.2/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22866 2024-05-24 18:17:25.528909 reflex-0.5.2/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     4931 2024-05-24 16:47:17.139573 reflex-0.5.2/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    16882 2024-05-24 18:17:25.761516 reflex-0.5.2/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-05-23 22:07:24.072888 reflex-0.5.2/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8294 2024-05-24 16:47:17.140143 reflex-0.5.2/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    26971 2024-05-24 18:17:26.902500 reflex-0.5.2/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     5543 2024-05-23 22:07:24.073463 reflex-0.5.2/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    22145 2024-05-24 18:17:26.852778 reflex-0.5.2/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     2440 2024-05-23 22:07:24.073836 reflex-0.5.2/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-05-23 22:07:24.073912 reflex-0.5.2/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-05-24 18:17:26.331761 reflex-0.5.2/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0      400 2024-05-23 22:07:24.074131 reflex-0.5.2/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-05-24 18:17:25.739485 reflex-0.5.2/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0      989 2024-05-23 22:07:24.074476 reflex-0.5.2/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-05-24 18:17:26.067405 reflex-0.5.2/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      821 2024-05-23 22:07:24.074712 reflex-0.5.2/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9347 2024-05-24 18:17:26.688767 reflex-0.5.2/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1125 2024-05-23 22:07:24.074970 reflex-0.5.2/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11939 2024-05-24 18:17:26.426242 reflex-0.5.2/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-05-23 22:07:24.075116 reflex-0.5.2/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-05-24 18:17:27.786118 reflex-0.5.2/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-05-23 22:07:24.075348 reflex-0.5.2/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-05-24 18:17:25.927754 reflex-0.5.2/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-05-23 22:07:24.075767 reflex-0.5.2/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-05-24 18:17:26.537814 reflex-0.5.2/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     1301 2024-05-23 22:07:24.075944 reflex-0.5.2/reflex/components/radix/themes/components/checkbox_cards.py
--rw-r--r--   0        0        0     9591 2024-05-24 18:17:26.071013 reflex-0.5.2/reflex/components/radix/themes/components/checkbox_cards.pyi
--rw-r--r--   0        0        0     1024 2024-05-23 22:07:24.076147 reflex-0.5.2/reflex/components/radix/themes/components/checkbox_group.py
--rw-r--r--   0        0        0     9012 2024-05-24 18:17:26.465537 reflex-0.5.2/reflex/components/radix/themes/components/checkbox_group.pyi
--rw-r--r--   0        0        0     5049 2024-05-23 22:07:24.076463 reflex-0.5.2/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-05-24 18:17:25.791725 reflex-0.5.2/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0     1508 2024-05-23 22:07:24.076861 reflex-0.5.2/reflex/components/radix/themes/components/data_list.py
--rw-r--r--   0        0        0    15403 2024-05-24 18:17:25.949327 reflex-0.5.2/reflex/components/radix/themes/components/data_list.pyi
--rw-r--r--   0        0        0     2600 2024-05-23 22:07:24.077463 reflex-0.5.2/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-05-24 18:17:26.907873 reflex-0.5.2/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-05-23 22:07:24.077898 reflex-0.5.2/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-05-24 18:17:25.758638 reflex-0.5.2/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0     2405 2024-05-23 22:07:24.078310 reflex-0.5.2/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-05-24 18:17:26.245730 reflex-0.5.2/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0     2940 2024-05-23 22:07:24.078537 reflex-0.5.2/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    12126 2024-05-24 18:17:25.994520 reflex-0.5.2/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0     1015 2024-05-23 22:07:24.078815 reflex-0.5.2/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-05-24 18:17:25.880962 reflex-0.5.2/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-05-23 22:07:24.078952 reflex-0.5.2/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-05-24 18:17:27.220650 reflex-0.5.2/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     1598 2024-05-23 22:07:24.079284 reflex-0.5.2/reflex/components/radix/themes/components/progress.py
--rw-r--r--   0        0        0     6676 2024-05-24 18:17:27.120916 reflex-0.5.2/reflex/components/radix/themes/components/progress.pyi
--rw-r--r--   0        0        0      762 2024-05-23 22:07:24.079594 reflex-0.5.2/reflex/components/radix/themes/components/radio.py
--rw-r--r--   0        0        0     5924 2024-05-24 18:17:26.105142 reflex-0.5.2/reflex/components/radix/themes/components/radio.pyi
--rw-r--r--   0        0        0     1250 2024-05-23 22:07:24.079896 reflex-0.5.2/reflex/components/radix/themes/components/radio_cards.py
--rw-r--r--   0        0        0     9561 2024-05-24 18:17:26.020173 reflex-0.5.2/reflex/components/radix/themes/components/radio_cards.pyi
--rw-r--r--   0        0        0     6233 2024-05-23 22:07:24.080200 reflex-0.5.2/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-05-24 18:17:27.243752 reflex-0.5.2/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0      920 2024-05-23 22:07:24.080634 reflex-0.5.2/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-05-24 18:17:25.967210 reflex-0.5.2/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     1292 2024-05-23 22:07:24.080814 reflex-0.5.2/reflex/components/radix/themes/components/segmented_control.py
--rw-r--r--   0        0        0     9507 2024-05-24 18:17:27.306298 reflex-0.5.2/reflex/components/radix/themes/components/segmented_control.pyi
--rw-r--r--   0        0        0     8028 2024-05-23 22:07:24.081113 reflex-0.5.2/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-05-24 18:17:26.898165 reflex-0.5.2/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-05-23 22:07:24.081415 reflex-0.5.2/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-05-24 18:17:25.687922 reflex-0.5.2/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0      643 2024-05-23 22:07:24.081575 reflex-0.5.2/reflex/components/radix/themes/components/skeleton.py
--rw-r--r--   0        0        0     4289 2024-05-24 18:17:25.850463 reflex-0.5.2/reflex/components/radix/themes/components/skeleton.pyi
--rw-r--r--   0        0        0     3234 2024-05-23 22:07:24.081922 reflex-0.5.2/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-05-24 18:17:26.148774 reflex-0.5.2/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0      431 2024-05-23 22:07:24.082079 reflex-0.5.2/reflex/components/radix/themes/components/spinner.py
--rw-r--r--   0        0        0     3845 2024-05-24 18:17:26.082297 reflex-0.5.2/reflex/components/radix/themes/components/spinner.pyi
--rw-r--r--   0        0        0     1976 2024-05-23 22:07:24.082258 reflex-0.5.2/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-05-24 18:17:26.168928 reflex-0.5.2/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-05-23 22:07:24.082419 reflex-0.5.2/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-05-24 18:17:26.938839 reflex-0.5.2/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     4150 2024-05-24 16:47:17.140632 reflex-0.5.2/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    19419 2024-05-24 18:17:26.410383 reflex-0.5.2/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-05-23 22:07:24.082757 reflex-0.5.2/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-05-24 18:17:27.057578 reflex-0.5.2/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     6527 2024-05-26 21:37:39.077690 reflex-0.5.2/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    26637 2024-05-26 21:37:39.077958 reflex-0.5.2/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0     4465 2024-05-23 22:07:24.083240 reflex-0.5.2/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-05-24 18:17:25.698313 reflex-0.5.2/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-05-23 22:07:24.083683 reflex-0.5.2/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-23 22:07:24.083755 reflex-0.5.2/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7663 2024-05-24 18:17:25.624770 reflex-0.5.2/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-05-23 22:07:24.083913 reflex-0.5.2/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-05-24 18:17:25.882224 reflex-0.5.2/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      465 2024-05-24 16:47:17.140943 reflex-0.5.2/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8272 2024-05-24 18:17:25.473218 reflex-0.5.2/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0     1405 2024-05-23 22:07:24.084328 reflex-0.5.2/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     5247 2024-05-24 18:17:25.624749 reflex-0.5.2/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-05-23 22:07:24.084951 reflex-0.5.2/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-05-24 18:17:25.530022 reflex-0.5.2/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-05-23 22:07:24.085255 reflex-0.5.2/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-05-24 18:17:25.811757 reflex-0.5.2/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4933 2024-05-24 16:47:17.141260 reflex-0.5.2/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    28910 2024-05-24 18:17:25.170181 reflex-0.5.2/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-05-23 22:07:24.085674 reflex-0.5.2/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-05-24 18:17:25.552977 reflex-0.5.2/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      448 2024-05-24 16:47:17.141536 reflex-0.5.2/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8272 2024-05-24 18:17:25.268878 reflex-0.5.2/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1522 2024-05-23 22:07:24.086073 reflex-0.5.2/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-05-24 18:17:25.348075 reflex-0.5.2/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-05-23 22:07:24.086549 reflex-0.5.2/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-05-23 22:07:24.086650 reflex-0.5.2/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-05-23 22:07:24.086739 reflex-0.5.2/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-05-24 18:17:27.346449 reflex-0.5.2/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-05-23 22:07:24.086897 reflex-0.5.2/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-05-24 18:17:26.430780 reflex-0.5.2/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     1324 2024-05-23 22:07:24.087027 reflex-0.5.2/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-05-24 18:17:26.529375 reflex-0.5.2/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     3291 2024-05-23 22:07:24.087167 reflex-0.5.2/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12144 2024-05-24 18:17:26.965637 reflex-0.5.2/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     2604 2024-05-23 22:07:24.089032 reflex-0.5.2/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-05-24 18:17:27.176095 reflex-0.5.2/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-05-23 22:07:24.089192 reflex-0.5.2/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089247 reflex-0.5.2/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.599273 reflex-0.5.2/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-05-23 22:07:24.089413 reflex-0.5.2/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4354 2024-05-24 18:17:28.170716 reflex-0.5.2/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089570 reflex-0.5.2/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.664099 reflex-0.5.2/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-05-23 22:07:24.089736 reflex-0.5.2/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-05-23 22:07:24.089831 reflex-0.5.2/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    84151 2024-05-24 18:17:27.836727 reflex-0.5.2/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-05-23 22:07:24.090297 reflex-0.5.2/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-05-24 18:17:28.679664 reflex-0.5.2/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-05-23 22:07:24.090528 reflex-0.5.2/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    22787 2024-05-24 18:17:28.255295 reflex-0.5.2/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-05-23 22:07:24.090691 reflex-0.5.2/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24326 2024-05-24 18:17:27.711371 reflex-0.5.2/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-05-23 22:07:24.090842 reflex-0.5.2/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8535 2024-05-24 18:17:27.949443 reflex-0.5.2/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0       68 2024-05-23 22:07:24.092435 reflex-0.5.2/reflex/components/sonner/__init__.py
--rw-r--r--   0        0        0     9822 2024-05-23 22:07:24.092539 reflex-0.5.2/reflex/components/sonner/toast.py
--rw-r--r--   0        0        0     8164 2024-05-24 18:17:24.719075 reflex-0.5.2/reflex/components/sonner/toast.pyi
--rw-r--r--   0        0        0      109 2024-05-23 22:07:24.092719 reflex-0.5.2/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-05-23 22:07:24.092808 reflex-0.5.2/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-05-24 18:17:24.308668 reflex-0.5.2/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-05-23 22:07:24.093075 reflex-0.5.2/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.2/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3927 2024-05-23 22:07:24.093403 reflex-0.5.2/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-05-23 22:07:24.093478 reflex-0.5.2/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-05-23 22:07:24.093780 reflex-0.5.2/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.2/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    10859 2024-05-24 16:47:17.142090 reflex-0.5.2/reflex/config.py
--rw-r--r--   0        0        0     3402 2024-05-24 16:47:17.142369 reflex-0.5.2/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-05-23 22:07:24.094524 reflex-0.5.2/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5640 2024-05-23 22:07:24.094682 reflex-0.5.2/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-05-23 22:07:24.094912 reflex-0.5.2/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1625 2024-05-23 22:07:24.094987 reflex-0.5.2/reflex/constants/colors.py
--rw-r--r--   0        0        0     4207 2024-05-23 22:07:24.095289 reflex-0.5.2/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-05-23 22:07:24.095442 reflex-0.5.2/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-05-23 22:07:24.095535 reflex-0.5.2/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-05-23 22:07:24.095664 reflex-0.5.2/reflex/constants/event.py
--rw-r--r--   0        0        0     3419 2024-05-24 16:47:17.142506 reflex-0.5.2/reflex/constants/installer.py
--rw-r--r--   0        0        0     2144 2024-05-23 22:07:24.096361 reflex-0.5.2/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-05-23 22:07:24.096532 reflex-0.5.2/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-05-23 22:07:24.096625 reflex-0.5.2/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    33067 2024-05-24 16:47:17.143111 reflex-0.5.2/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    28087 2024-05-26 21:37:48.497700 reflex-0.5.2/reflex/event.py
--rw-r--r--   0        0        0      778 2024-05-23 22:07:24.097229 reflex-0.5.2/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     6597 2024-05-23 22:07:24.097324 reflex-0.5.2/reflex/experimental/client_state.py
--rw-r--r--   0        0        0     2196 2024-05-23 22:07:24.097529 reflex-0.5.2/reflex/experimental/hooks.py
--rw-r--r--   0        0        0     7267 2024-05-24 16:47:17.143287 reflex-0.5.2/reflex/experimental/layout.py
--rw-r--r--   0        0        0      281 2024-05-23 22:07:24.097664 reflex-0.5.2/reflex/experimental/misc.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.2/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.097791 reflex-0.5.2/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.2/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13227 2024-05-23 22:07:24.098145 reflex-0.5.2/reflex/model.py
--rw-r--r--   0        0        0     2077 2024-05-23 22:07:24.098419 reflex-0.5.2/reflex/page.py
--rw-r--r--   0        0        0    17826 2024-05-23 22:07:24.098559 reflex-0.5.2/reflex/reflex.py
--rw-r--r--   0        0        0     4198 2024-05-23 22:07:24.098696 reflex-0.5.2/reflex/route.py
--rw-r--r--   0        0        0   107026 2024-05-26 21:35:54.556468 reflex-0.5.2/reflex/state.py
--rw-r--r--   0        0        0     9542 2024-05-26 21:37:48.498428 reflex-0.5.2/reflex/style.py
--rw-r--r--   0        0        0    31567 2024-05-24 18:15:31.927241 reflex-0.5.2/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.2/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-05-23 22:07:24.099525 reflex-0.5.2/reflex/utils/build.py
--rw-r--r--   0        0        0     1255 2024-05-23 22:07:24.099853 reflex-0.5.2/reflex/utils/compat.py
--rw-r--r--   0        0        0     5182 2024-05-23 22:07:24.100141 reflex-0.5.2/reflex/utils/console.py
--rw-r--r--   0        0        0     2163 2024-05-23 22:07:24.100417 reflex-0.5.2/reflex/utils/exceptions.py
--rw-r--r--   0        0        0    10498 2024-05-24 16:47:17.144439 reflex-0.5.2/reflex/utils/exec.py
--rw-r--r--   0        0        0     2270 2024-05-23 22:07:24.100962 reflex-0.5.2/reflex/utils/export.py
--rw-r--r--   0        0        0    25149 2024-05-23 22:07:24.101499 reflex-0.5.2/reflex/utils/format.py
--rw-r--r--   0        0        0     2309 2024-05-23 22:07:24.101709 reflex-0.5.2/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-05-23 22:07:24.101899 reflex-0.5.2/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    52824 2024-05-23 22:07:24.102428 reflex-0.5.2/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0    11972 2024-05-23 22:07:24.102655 reflex-0.5.2/reflex/utils/processes.py
--rw-r--r--   0        0        0    30637 2024-05-23 22:07:24.102877 reflex-0.5.2/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     9037 2024-05-23 22:07:24.103180 reflex-0.5.2/reflex/utils/serializers.py
--rw-r--r--   0        0        0     5568 2024-05-24 16:47:17.144759 reflex-0.5.2/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    15152 2024-05-23 22:07:24.103627 reflex-0.5.2/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.2/reflex/utils/watch.py
--rw-r--r--   0        0        0    69637 2024-05-26 21:37:48.498752 reflex-0.5.2/reflex/vars.py
--rw-r--r--   0        0        0     5753 2024-05-23 22:07:24.104898 reflex-0.5.2/reflex/vars.pyi
--rw-r--r--   0        0        0    12083 1970-01-01 00:00:00.000000 reflex-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.2a1/LICENSE
+-rw-r--r--   0        0        0     9838 2024-05-23 22:07:24.004599 reflex-0.5.2a1/README.md
+-rw-r--r--   0        0        0     2974 2024-05-26 21:38:07.551506 reflex-0.5.2a1/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.2a1/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.2a1/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-23 22:07:24.026702 reflex-0.5.2a1/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.2a1/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.2a1/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-23 22:07:24.026869 reflex-0.5.2a1/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-05-23 22:07:24.027050 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10906 2024-05-23 22:07:24.027242 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8381 2024-05-23 22:07:24.027471 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-05-23 22:07:24.027876 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-05-23 22:07:24.028048 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-05-23 22:07:24.028210 reflex-0.5.2a1/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.2a1/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-05-23 22:07:24.028477 reflex-0.5.2a1/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-05-23 22:07:24.028657 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-05-23 22:07:24.028787 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-05-23 22:07:24.035433 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-05-23 22:07:24.035615 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-05-23 22:07:24.035773 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.2a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-05-23 22:07:24.036845 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-05-23 22:07:24.036930 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-05-23 22:07:24.037352 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-05-23 22:07:24.037689 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-05-23 22:07:24.037946 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.2a1/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-05-23 22:07:24.038352 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-05-23 22:07:24.038521 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-05-23 22:07:24.038697 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-05-23 22:07:24.038822 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.2a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      761 2024-05-23 22:07:24.039110 reflex-0.5.2a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-05-23 22:07:24.039386 reflex-0.5.2a1/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.2a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.2a1/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.2a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-05-23 22:07:24.039706 reflex-0.5.2a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.2a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.2a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0       82 2024-05-24 16:47:17.136778 reflex-0.5.2a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0       59 2024-05-24 16:47:17.136946 reflex-0.5.2a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.2a1/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-05-23 22:07:24.039831 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0      528 2024-05-23 22:07:24.039893 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/debounce.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0      566 2024-05-23 22:07:24.039949 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/throttle.js
+-rw-r--r--   0        0        0    22617 2024-05-23 22:07:24.040119 reflex-0.5.2a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     5831 2024-05-23 22:07:24.040585 reflex-0.5.2a1/reflex/__init__.py
+-rw-r--r--   0        0        0     7791 2024-05-26 21:36:23.014634 reflex-0.5.2a1/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.2a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.2a1/reflex/admin.py
+-rw-r--r--   0        0        0    48956 2024-05-24 16:47:17.137462 reflex-0.5.2a1/reflex/app.py
+-rw-r--r--   0        0        0     1227 2024-05-23 22:07:24.041327 reflex-0.5.2a1/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4274 2024-05-23 22:07:24.041585 reflex-0.5.2a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.2a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17455 2024-05-23 22:07:24.041899 reflex-0.5.2a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-05-23 22:07:24.042172 reflex-0.5.2a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    13274 2024-05-23 22:07:24.042547 reflex-0.5.2a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      552 2024-05-23 22:07:24.042676 reflex-0.5.2a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-23 22:07:24.042785 reflex-0.5.2a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-23 22:07:24.042894 reflex-0.5.2a1/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-05-24 18:17:26.775810 reflex-0.5.2a1/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-05-23 22:07:24.043424 reflex-0.5.2a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.2a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-05-24 18:17:28.445017 reflex-0.5.2a1/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-05-23 22:07:24.043906 reflex-0.5.2a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-05-24 18:17:26.993081 reflex-0.5.2a1/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      312 2024-05-23 22:07:24.044107 reflex-0.5.2a1/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3218 2024-05-24 18:17:26.730059 reflex-0.5.2a1/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      297 2024-05-23 22:07:24.044322 reflex-0.5.2a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6002 2024-05-24 18:17:27.212239 reflex-0.5.2a1/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.2a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-05-24 18:17:28.411498 reflex-0.5.2a1/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.2a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-05-24 18:17:27.232380 reflex-0.5.2a1/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.2a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4500 2024-05-24 18:17:27.261455 reflex-0.5.2a1/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-05-23 22:07:24.045051 reflex-0.5.2a1/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-23 22:07:24.045134 reflex-0.5.2a1/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-05-24 18:17:24.861757 reflex-0.5.2a1/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-05-23 22:07:24.045326 reflex-0.5.2a1/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-05-23 22:07:24.045398 reflex-0.5.2a1/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-05-24 18:17:23.594412 reflex-0.5.2a1/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-05-23 22:07:24.045575 reflex-0.5.2a1/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-05-24 18:17:23.555248 reflex-0.5.2a1/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-05-23 22:07:24.045714 reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-05-24 18:17:23.503426 reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-05-23 22:07:24.045852 reflex-0.5.2a1/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-05-24 18:17:24.668110 reflex-0.5.2a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.046229 reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12991 2024-05-24 18:17:24.625763 reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-05-23 22:07:24.046512 reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.921677 reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-05-23 22:07:24.046775 reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-05-24 18:17:24.570212 reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-05-23 22:07:24.046980 reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-05-24 18:17:23.854192 reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-05-23 22:07:24.047198 reflex-0.5.2a1/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3510 2024-05-23 22:07:24.047299 reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-05-24 18:17:24.269813 reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-05-23 22:07:24.047512 reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-05-24 18:17:23.577560 reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-05-23 22:07:24.047752 reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-05-24 18:17:23.981249 reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-05-23 22:07:24.047917 reflex-0.5.2a1/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-05-24 18:17:23.263087 reflex-0.5.2a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-05-23 22:07:24.048055 reflex-0.5.2a1/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-05-23 22:07:24.048128 reflex-0.5.2a1/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-05-24 18:17:24.114056 reflex-0.5.2a1/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-05-23 22:07:24.048304 reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-05-24 18:17:24.157731 reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-05-23 22:07:24.048486 reflex-0.5.2a1/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-05-24 18:17:24.226071 reflex-0.5.2a1/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-05-23 22:07:24.048623 reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-05-24 18:17:24.080524 reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-05-23 22:07:24.048760 reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-05-24 18:17:24.399345 reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-05-23 22:07:24.048929 reflex-0.5.2a1/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-05-23 22:07:24.049012 reflex-0.5.2a1/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-05-24 18:17:24.063143 reflex-0.5.2a1/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-05-23 22:07:24.049323 reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-05-24 18:17:23.972016 reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-05-23 22:07:24.049528 reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-05-24 18:17:23.734040 reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-05-23 22:07:24.049762 reflex-0.5.2a1/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.844965 reflex-0.5.2a1/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-05-23 22:07:24.049973 reflex-0.5.2a1/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-05-24 18:17:23.355983 reflex-0.5.2a1/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-05-23 22:07:24.050115 reflex-0.5.2a1/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-05-24 18:17:24.448401 reflex-0.5.2a1/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-05-23 22:07:24.050281 reflex-0.5.2a1/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-05-24 18:17:23.790638 reflex-0.5.2a1/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-05-23 22:07:24.050478 reflex-0.5.2a1/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-05-24 18:17:23.741717 reflex-0.5.2a1/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-05-23 22:07:24.050744 reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-05-24 18:17:23.790245 reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-05-23 22:07:24.050915 reflex-0.5.2a1/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-05-24 18:17:24.148687 reflex-0.5.2a1/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-05-23 22:07:24.051118 reflex-0.5.2a1/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-05-23 22:07:24.051235 reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-05-24 18:17:24.503442 reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-05-23 22:07:24.051441 reflex-0.5.2a1/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-05-24 18:17:23.849665 reflex-0.5.2a1/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-05-23 22:07:24.051630 reflex-0.5.2a1/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9369 2024-05-24 18:17:23.634451 reflex-0.5.2a1/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-05-23 22:07:24.051792 reflex-0.5.2a1/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-05-24 18:17:24.617235 reflex-0.5.2a1/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-05-23 22:07:24.051994 reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-05-24 18:17:23.752785 reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-05-23 22:07:24.052210 reflex-0.5.2a1/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-05-24 18:17:23.466505 reflex-0.5.2a1/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-05-23 22:07:24.052410 reflex-0.5.2a1/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.839820 reflex-0.5.2a1/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-05-23 22:07:24.052576 reflex-0.5.2a1/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-05-24 18:17:23.439877 reflex-0.5.2a1/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-05-23 22:07:24.052732 reflex-0.5.2a1/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-05-24 18:17:23.406701 reflex-0.5.2a1/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-05-23 22:07:24.052879 reflex-0.5.2a1/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.338287 reflex-0.5.2a1/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-05-23 22:07:24.053058 reflex-0.5.2a1/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-23 22:07:24.053146 reflex-0.5.2a1/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-05-24 18:17:24.134750 reflex-0.5.2a1/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-05-23 22:07:24.053303 reflex-0.5.2a1/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-05-24 18:17:23.684534 reflex-0.5.2a1/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-05-23 22:07:24.053447 reflex-0.5.2a1/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-05-24 18:17:23.661739 reflex-0.5.2a1/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-05-23 22:07:24.053601 reflex-0.5.2a1/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-05-24 18:17:23.861262 reflex-0.5.2a1/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-05-23 22:07:24.053774 reflex-0.5.2a1/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-05-24 18:17:23.906150 reflex-0.5.2a1/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-05-23 22:07:24.053931 reflex-0.5.2a1/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-05-24 18:17:23.856235 reflex-0.5.2a1/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-05-23 22:07:24.054108 reflex-0.5.2a1/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-05-24 18:17:23.508048 reflex-0.5.2a1/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-05-23 22:07:24.054265 reflex-0.5.2a1/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-05-24 18:17:23.753119 reflex-0.5.2a1/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-05-23 22:07:24.054391 reflex-0.5.2a1/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-05-24 18:17:23.812312 reflex-0.5.2a1/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-05-23 22:07:24.054557 reflex-0.5.2a1/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-05-24 18:17:24.095832 reflex-0.5.2a1/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-05-23 22:07:24.054738 reflex-0.5.2a1/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-05-23 22:07:24.054834 reflex-0.5.2a1/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-05-24 18:17:25.119256 reflex-0.5.2a1/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2462 2024-05-23 22:07:24.054978 reflex-0.5.2a1/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-05-24 18:17:24.970682 reflex-0.5.2a1/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-05-23 22:07:24.055112 reflex-0.5.2a1/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-05-24 18:17:25.284214 reflex-0.5.2a1/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-05-23 22:07:24.055273 reflex-0.5.2a1/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-05-23 22:07:24.055368 reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-05-24 18:17:24.223760 reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-05-23 22:07:24.055559 reflex-0.5.2a1/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-05-24 18:17:24.135785 reflex-0.5.2a1/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-05-23 22:07:24.055765 reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-05-24 18:17:24.315782 reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-05-23 22:07:24.055929 reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-05-24 18:17:23.937771 reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-05-23 22:07:24.056145 reflex-0.5.2a1/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-05-23 22:07:24.056257 reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-05-24 18:17:25.493171 reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-05-23 22:07:24.056468 reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-05-24 18:17:24.311417 reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-05-23 22:07:24.056645 reflex-0.5.2a1/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-05-24 18:17:25.078723 reflex-0.5.2a1/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-05-23 22:07:24.056817 reflex-0.5.2a1/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-05-24 18:17:25.909264 reflex-0.5.2a1/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-05-23 22:07:24.057050 reflex-0.5.2a1/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-05-24 18:17:24.574288 reflex-0.5.2a1/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-05-23 22:07:24.057260 reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-05-24 18:17:24.470002 reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-05-23 22:07:24.057423 reflex-0.5.2a1/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-05-23 22:07:24.057495 reflex-0.5.2a1/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-05-24 18:17:24.173439 reflex-0.5.2a1/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-05-23 22:07:24.057873 reflex-0.5.2a1/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-05-24 18:17:24.260699 reflex-0.5.2a1/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-05-23 22:07:24.058053 reflex-0.5.2a1/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-05-24 18:17:24.311205 reflex-0.5.2a1/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-05-23 22:07:24.058204 reflex-0.5.2a1/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-05-24 18:17:24.218016 reflex-0.5.2a1/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    77001 2024-05-23 22:07:24.058552 reflex-0.5.2a1/reflex/components/component.py
+-rw-r--r--   0        0        0      943 2024-05-23 22:07:24.058811 reflex-0.5.2a1/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     8043 2024-05-23 22:07:24.058914 reflex-0.5.2a1/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    22528 2024-05-24 18:17:25.155664 reflex-0.5.2a1/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-05-23 22:07:24.059088 reflex-0.5.2a1/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-05-24 18:17:24.651237 reflex-0.5.2a1/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-05-23 22:07:24.059236 reflex-0.5.2a1/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6163 2024-05-23 22:07:24.059313 reflex-0.5.2a1/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4820 2024-05-23 22:07:24.059567 reflex-0.5.2a1/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4216 2024-05-24 18:17:24.719439 reflex-0.5.2a1/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4732 2024-05-23 22:07:24.060166 reflex-0.5.2a1/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1284 2024-05-23 22:07:24.060230 reflex-0.5.2a1/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6616 2024-05-24 18:17:24.552128 reflex-0.5.2a1/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-05-23 22:07:24.060774 reflex-0.5.2a1/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9484 2024-05-23 22:07:24.060867 reflex-0.5.2a1/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1907 2024-05-23 22:07:24.061035 reflex-0.5.2a1/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0    10146 2024-05-23 22:07:24.061115 reflex-0.5.2a1/reflex/components/core/upload.py
+-rw-r--r--   0        0        0    17147 2024-05-24 18:17:24.472841 reflex-0.5.2a1/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      357 2024-05-23 22:07:24.061822 reflex-0.5.2a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0    11347 2024-05-24 16:47:17.137792 reflex-0.5.2a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31197 2024-05-24 18:17:25.129041 reflex-0.5.2a1/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12632 2024-05-23 22:07:24.062397 reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10485 2024-05-24 18:17:24.719094 reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-05-23 22:07:24.062734 reflex-0.5.2a1/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.2a1/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.2a1/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.2a1/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.2a1/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.2a1/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.2a1/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-05-24 18:17:24.504591 reflex-0.5.2a1/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     3529 2024-05-23 22:07:24.063280 reflex-0.5.2a1/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     1982 2024-05-23 22:07:24.063391 reflex-0.5.2a1/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-05-24 18:17:25.763640 reflex-0.5.2a1/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20167 2024-05-23 22:07:24.063679 reflex-0.5.2a1/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99555 2024-05-24 18:17:29.297573 reflex-0.5.2a1/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     3610 2024-05-23 22:07:24.064187 reflex-0.5.2a1/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   164607 2024-05-24 18:17:28.121848 reflex-0.5.2a1/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     8467 2024-05-23 22:07:24.064879 reflex-0.5.2a1/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93669 2024-05-24 18:17:25.809803 reflex-0.5.2a1/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.2a1/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28031 2024-05-24 18:17:26.420859 reflex-0.5.2a1/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.2a1/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42033 2024-05-24 18:17:28.117892 reflex-0.5.2a1/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1406 2024-05-23 22:07:24.065615 reflex-0.5.2a1/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19615 2024-05-24 18:17:25.678066 reflex-0.5.2a1/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1535 2024-05-23 22:07:24.065964 reflex-0.5.2a1/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87242 2024-05-24 18:17:27.638168 reflex-0.5.2a1/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2767 2024-05-23 22:07:24.066552 reflex-0.5.2a1/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    61849 2024-05-24 18:17:25.354377 reflex-0.5.2a1/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2432 2024-05-23 22:07:24.067050 reflex-0.5.2a1/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89115 2024-05-24 18:17:25.804750 reflex-0.5.2a1/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-05-23 22:07:24.067621 reflex-0.5.2a1/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4304 2024-05-23 22:07:24.067706 reflex-0.5.2a1/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-05-24 18:17:23.290206 reflex-0.5.2a1/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-05-23 22:07:24.067888 reflex-0.5.2a1/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-05-23 22:07:24.067968 reflex-0.5.2a1/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34077 2024-05-23 22:07:24.068288 reflex-0.5.2a1/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37918 2024-05-24 18:17:27.204674 reflex-0.5.2a1/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-05-23 22:07:24.068931 reflex-0.5.2a1/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    10867 2024-05-23 22:07:24.069105 reflex-0.5.2a1/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5100 2024-05-24 18:17:24.542827 reflex-0.5.2a1/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-05-23 22:07:24.069399 reflex-0.5.2a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-05-23 22:07:24.069584 reflex-0.5.2a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       79 2024-05-23 22:07:24.069684 reflex-0.5.2a1/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-05-23 22:07:24.069782 reflex-0.5.2a1/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-05-24 18:17:24.208012 reflex-0.5.2a1/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-05-23 22:07:24.069942 reflex-0.5.2a1/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-23 22:07:24.070005 reflex-0.5.2a1/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-05-24 18:17:23.601458 reflex-0.5.2a1/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-05-23 22:07:24.070176 reflex-0.5.2a1/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-05-24 18:17:23.566367 reflex-0.5.2a1/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-05-23 22:07:24.070408 reflex-0.5.2a1/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-05-24 18:17:23.327764 reflex-0.5.2a1/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-05-23 22:07:24.070545 reflex-0.5.2a1/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-05-24 18:17:23.378778 reflex-0.5.2a1/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-05-23 22:07:24.070725 reflex-0.5.2a1/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0      964 2024-05-23 22:07:24.070795 reflex-0.5.2a1/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     6865 2024-05-24 18:17:24.804257 reflex-0.5.2a1/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      906 2024-05-23 22:07:24.071050 reflex-0.5.2a1/reflex/components/props.py
+-rw-r--r--   0        0        0      112 2024-05-23 22:07:24.071248 reflex-0.5.2a1/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-23 22:07:24.071337 reflex-0.5.2a1/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0    15801 2024-05-24 16:47:17.138407 reflex-0.5.2a1/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    38019 2024-05-24 18:17:25.203694 reflex-0.5.2a1/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-05-23 22:07:24.071818 reflex-0.5.2a1/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-05-24 18:17:25.726505 reflex-0.5.2a1/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-05-23 22:07:24.071992 reflex-0.5.2a1/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-05-24 18:17:25.412916 reflex-0.5.2a1/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4941 2024-05-24 16:47:17.138863 reflex-0.5.2a1/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    48143 2024-05-24 18:17:26.612449 reflex-0.5.2a1/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     4022 2024-05-24 16:47:17.139254 reflex-0.5.2a1/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22866 2024-05-24 18:17:25.528909 reflex-0.5.2a1/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     4931 2024-05-24 16:47:17.139573 reflex-0.5.2a1/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16882 2024-05-24 18:17:25.761516 reflex-0.5.2a1/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      292 2024-05-23 22:07:24.072888 reflex-0.5.2a1/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0     8294 2024-05-24 16:47:17.140143 reflex-0.5.2a1/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    26971 2024-05-24 18:17:26.902500 reflex-0.5.2a1/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     5543 2024-05-23 22:07:24.073463 reflex-0.5.2a1/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    22145 2024-05-24 18:17:26.852778 reflex-0.5.2a1/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0     2440 2024-05-23 22:07:24.073836 reflex-0.5.2a1/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     3267 2024-05-23 22:07:24.073912 reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24434 2024-05-24 18:17:26.331761 reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0      400 2024-05-23 22:07:24.074131 reflex-0.5.2a1/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-05-24 18:17:25.739485 reflex-0.5.2a1/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0      989 2024-05-23 22:07:24.074476 reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-05-24 18:17:26.067405 reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      821 2024-05-23 22:07:24.074712 reflex-0.5.2a1/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9347 2024-05-24 18:17:26.688767 reflex-0.5.2a1/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1125 2024-05-23 22:07:24.074970 reflex-0.5.2a1/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11939 2024-05-24 18:17:26.426242 reflex-0.5.2a1/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2378 2024-05-23 22:07:24.075116 reflex-0.5.2a1/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38710 2024-05-24 18:17:27.786118 reflex-0.5.2a1/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      659 2024-05-23 22:07:24.075348 reflex-0.5.2a1/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7200 2024-05-24 18:17:25.927754 reflex-0.5.2a1/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-05-23 22:07:24.075767 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-05-24 18:17:26.537814 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     1301 2024-05-23 22:07:24.075944 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.py
+-rw-r--r--   0        0        0     9591 2024-05-24 18:17:26.071013 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.pyi
+-rw-r--r--   0        0        0     1024 2024-05-23 22:07:24.076147 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.py
+-rw-r--r--   0        0        0     9012 2024-05-24 18:17:26.465537 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.pyi
+-rw-r--r--   0        0        0     5049 2024-05-23 22:07:24.076463 reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-05-24 18:17:25.791725 reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0     1508 2024-05-23 22:07:24.076861 reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.py
+-rw-r--r--   0        0        0    15403 2024-05-24 18:17:25.949327 reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.pyi
+-rw-r--r--   0        0        0     2600 2024-05-23 22:07:24.077463 reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24895 2024-05-24 18:17:26.907873 reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-05-23 22:07:24.077898 reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-05-24 18:17:25.758638 reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0     2405 2024-05-23 22:07:24.078310 reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17744 2024-05-24 18:17:26.245730 reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0     2940 2024-05-23 22:07:24.078537 reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    12126 2024-05-24 18:17:25.994520 reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0     1015 2024-05-23 22:07:24.078815 reflex-0.5.2a1/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7889 2024-05-24 18:17:25.880962 reflex-0.5.2a1/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3177 2024-05-23 22:07:24.078952 reflex-0.5.2a1/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17404 2024-05-24 18:17:27.220650 reflex-0.5.2a1/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     1598 2024-05-23 22:07:24.079284 reflex-0.5.2a1/reflex/components/radix/themes/components/progress.py
+-rw-r--r--   0        0        0     6676 2024-05-24 18:17:27.120916 reflex-0.5.2a1/reflex/components/radix/themes/components/progress.pyi
+-rw-r--r--   0        0        0      762 2024-05-23 22:07:24.079594 reflex-0.5.2a1/reflex/components/radix/themes/components/radio.py
+-rw-r--r--   0        0        0     5924 2024-05-24 18:17:26.105142 reflex-0.5.2a1/reflex/components/radix/themes/components/radio.pyi
+-rw-r--r--   0        0        0     1250 2024-05-23 22:07:24.079896 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.py
+-rw-r--r--   0        0        0     9561 2024-05-24 18:17:26.020173 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.pyi
+-rw-r--r--   0        0        0     6233 2024-05-23 22:07:24.080200 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-05-24 18:17:27.243752 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0      920 2024-05-23 22:07:24.080634 reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-05-24 18:17:25.967210 reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     1292 2024-05-23 22:07:24.080814 reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.py
+-rw-r--r--   0        0        0     9507 2024-05-24 18:17:27.306298 reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.pyi
+-rw-r--r--   0        0        0     8028 2024-05-23 22:07:24.081113 reflex-0.5.2a1/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-05-24 18:17:26.898165 reflex-0.5.2a1/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-05-23 22:07:24.081415 reflex-0.5.2a1/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-05-24 18:17:25.687922 reflex-0.5.2a1/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0      643 2024-05-23 22:07:24.081575 reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.py
+-rw-r--r--   0        0        0     4289 2024-05-24 18:17:25.850463 reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.pyi
+-rw-r--r--   0        0        0     3234 2024-05-23 22:07:24.081922 reflex-0.5.2a1/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-05-24 18:17:26.148774 reflex-0.5.2a1/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0      431 2024-05-23 22:07:24.082079 reflex-0.5.2a1/reflex/components/radix/themes/components/spinner.py
+-rw-r--r--   0        0        0     3845 2024-05-24 18:17:26.082297 reflex-0.5.2a1/reflex/components/radix/themes/components/spinner.pyi
+-rw-r--r--   0        0        0     1976 2024-05-23 22:07:24.082258 reflex-0.5.2a1/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-05-24 18:17:26.168928 reflex-0.5.2a1/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3111 2024-05-23 22:07:24.082419 reflex-0.5.2a1/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47387 2024-05-24 18:17:26.938839 reflex-0.5.2a1/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     4150 2024-05-24 16:47:17.140632 reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    19419 2024-05-24 18:17:26.410383 reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3233 2024-05-23 22:07:24.082757 reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    11711 2024-05-24 18:17:27.057578 reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     6527 2024-05-26 21:37:39.077690 reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    26637 2024-05-26 21:37:39.077958 reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0     4465 2024-05-23 22:07:24.083240 reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-05-24 18:17:25.698313 reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      811 2024-05-23 22:07:24.083683 reflex-0.5.2a1/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-23 22:07:24.083755 reflex-0.5.2a1/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7663 2024-05-24 18:17:25.624770 reflex-0.5.2a1/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      281 2024-05-23 22:07:24.083913 reflex-0.5.2a1/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6462 2024-05-24 18:17:25.882224 reflex-0.5.2a1/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      465 2024-05-24 16:47:17.140943 reflex-0.5.2a1/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8272 2024-05-24 18:17:25.473218 reflex-0.5.2a1/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0     1405 2024-05-23 22:07:24.084328 reflex-0.5.2a1/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     5247 2024-05-24 18:17:25.624749 reflex-0.5.2a1/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1374 2024-05-23 22:07:24.084951 reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8501 2024-05-24 18:17:25.530022 reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1498 2024-05-23 22:07:24.085255 reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8907 2024-05-24 18:17:25.811757 reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     4933 2024-05-24 16:47:17.141260 reflex-0.5.2a1/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    28910 2024-05-24 18:17:25.170181 reflex-0.5.2a1/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      458 2024-05-23 22:07:24.085674 reflex-0.5.2a1/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6758 2024-05-24 18:17:25.552977 reflex-0.5.2a1/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      448 2024-05-24 16:47:17.141536 reflex-0.5.2a1/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8272 2024-05-24 18:17:25.268878 reflex-0.5.2a1/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1522 2024-05-23 22:07:24.086073 reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22132 2024-05-24 18:17:25.348075 reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      343 2024-05-23 22:07:24.086549 reflex-0.5.2a1/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-23 22:07:24.086650 reflex-0.5.2a1/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      799 2024-05-23 22:07:24.086739 reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9316 2024-05-24 18:17:27.346449 reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      909 2024-05-23 22:07:24.086897 reflex-0.5.2a1/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9513 2024-05-24 18:17:26.430780 reflex-0.5.2a1/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     1324 2024-05-23 22:07:24.087027 reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10106 2024-05-24 18:17:26.529375 reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     3291 2024-05-23 22:07:24.087167 reflex-0.5.2a1/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12144 2024-05-24 18:17:26.965637 reflex-0.5.2a1/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     2604 2024-05-23 22:07:24.089032 reflex-0.5.2a1/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57238 2024-05-24 18:17:27.176095 reflex-0.5.2a1/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-05-23 22:07:24.089192 reflex-0.5.2a1/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089247 reflex-0.5.2a1/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.599273 reflex-0.5.2a1/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-05-23 22:07:24.089413 reflex-0.5.2a1/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-05-24 18:17:28.170716 reflex-0.5.2a1/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089570 reflex-0.5.2a1/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.664099 reflex-0.5.2a1/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2373 2024-05-23 22:07:24.089736 reflex-0.5.2a1/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0    19595 2024-05-23 22:07:24.089831 reflex-0.5.2a1/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84151 2024-05-24 18:17:27.836727 reflex-0.5.2a1/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18493 2024-05-23 22:07:24.090297 reflex-0.5.2a1/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    48757 2024-05-24 18:17:28.679664 reflex-0.5.2a1/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5624 2024-05-23 22:07:24.090528 reflex-0.5.2a1/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22787 2024-05-24 18:17:28.255295 reflex-0.5.2a1/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10410 2024-05-23 22:07:24.090691 reflex-0.5.2a1/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24326 2024-05-24 18:17:27.711371 reflex-0.5.2a1/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-05-23 22:07:24.090842 reflex-0.5.2a1/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-05-24 18:17:27.949443 reflex-0.5.2a1/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0       68 2024-05-23 22:07:24.092435 reflex-0.5.2a1/reflex/components/sonner/__init__.py
+-rw-r--r--   0        0        0     9822 2024-05-23 22:07:24.092539 reflex-0.5.2a1/reflex/components/sonner/toast.py
+-rw-r--r--   0        0        0     8164 2024-05-24 18:17:24.719075 reflex-0.5.2a1/reflex/components/sonner/toast.pyi
+-rw-r--r--   0        0        0      109 2024-05-23 22:07:24.092719 reflex-0.5.2a1/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-05-23 22:07:24.092808 reflex-0.5.2a1/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-05-24 18:17:24.308668 reflex-0.5.2a1/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-05-23 22:07:24.093075 reflex-0.5.2a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.2a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3927 2024-05-23 22:07:24.093403 reflex-0.5.2a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-05-23 22:07:24.093478 reflex-0.5.2a1/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-05-23 22:07:24.093780 reflex-0.5.2a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.2a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    10859 2024-05-24 16:47:17.142090 reflex-0.5.2a1/reflex/config.py
+-rw-r--r--   0        0        0     3402 2024-05-24 16:47:17.142369 reflex-0.5.2a1/reflex/config.pyi
+-rw-r--r--   0        0        0     2036 2024-05-23 22:07:24.094524 reflex-0.5.2a1/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5640 2024-05-23 22:07:24.094682 reflex-0.5.2a1/reflex/constants/base.py
+-rw-r--r--   0        0        0     2980 2024-05-23 22:07:24.094912 reflex-0.5.2a1/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1625 2024-05-23 22:07:24.094987 reflex-0.5.2a1/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-05-23 22:07:24.095289 reflex-0.5.2a1/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-05-23 22:07:24.095442 reflex-0.5.2a1/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-05-23 22:07:24.095535 reflex-0.5.2a1/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-05-23 22:07:24.095664 reflex-0.5.2a1/reflex/constants/event.py
+-rw-r--r--   0        0        0     3419 2024-05-24 16:47:17.142506 reflex-0.5.2a1/reflex/constants/installer.py
+-rw-r--r--   0        0        0     2144 2024-05-23 22:07:24.096361 reflex-0.5.2a1/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-05-23 22:07:24.096532 reflex-0.5.2a1/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-05-23 22:07:24.096625 reflex-0.5.2a1/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    33067 2024-05-24 16:47:17.143111 reflex-0.5.2a1/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    28087 2024-05-26 21:37:48.497700 reflex-0.5.2a1/reflex/event.py
+-rw-r--r--   0        0        0      778 2024-05-23 22:07:24.097229 reflex-0.5.2a1/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     6597 2024-05-23 22:07:24.097324 reflex-0.5.2a1/reflex/experimental/client_state.py
+-rw-r--r--   0        0        0     2196 2024-05-23 22:07:24.097529 reflex-0.5.2a1/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0     7267 2024-05-24 16:47:17.143287 reflex-0.5.2a1/reflex/experimental/layout.py
+-rw-r--r--   0        0        0      281 2024-05-23 22:07:24.097664 reflex-0.5.2a1/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.2a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.097791 reflex-0.5.2a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.2a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13227 2024-05-23 22:07:24.098145 reflex-0.5.2a1/reflex/model.py
+-rw-r--r--   0        0        0     2077 2024-05-23 22:07:24.098419 reflex-0.5.2a1/reflex/page.py
+-rw-r--r--   0        0        0    17826 2024-05-23 22:07:24.098559 reflex-0.5.2a1/reflex/reflex.py
+-rw-r--r--   0        0        0     4198 2024-05-23 22:07:24.098696 reflex-0.5.2a1/reflex/route.py
+-rw-r--r--   0        0        0   107026 2024-05-26 21:35:54.556468 reflex-0.5.2a1/reflex/state.py
+-rw-r--r--   0        0        0     9542 2024-05-26 21:37:48.498428 reflex-0.5.2a1/reflex/style.py
+-rw-r--r--   0        0        0    31567 2024-05-24 18:15:31.927241 reflex-0.5.2a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.2a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-05-23 22:07:24.099525 reflex-0.5.2a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-05-23 22:07:24.099853 reflex-0.5.2a1/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5182 2024-05-23 22:07:24.100141 reflex-0.5.2a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     2163 2024-05-23 22:07:24.100417 reflex-0.5.2a1/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0    10498 2024-05-24 16:47:17.144439 reflex-0.5.2a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-05-23 22:07:24.100962 reflex-0.5.2a1/reflex/utils/export.py
+-rw-r--r--   0        0        0    25149 2024-05-23 22:07:24.101499 reflex-0.5.2a1/reflex/utils/format.py
+-rw-r--r--   0        0        0     2309 2024-05-23 22:07:24.101709 reflex-0.5.2a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     4737 2024-05-23 22:07:24.101899 reflex-0.5.2a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    52824 2024-05-23 22:07:24.102428 reflex-0.5.2a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    11972 2024-05-23 22:07:24.102655 reflex-0.5.2a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0    30637 2024-05-23 22:07:24.102877 reflex-0.5.2a1/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     9037 2024-05-23 22:07:24.103180 reflex-0.5.2a1/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     5568 2024-05-24 16:47:17.144759 reflex-0.5.2a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    15152 2024-05-23 22:07:24.103627 reflex-0.5.2a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.2a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    69637 2024-05-26 21:37:48.498752 reflex-0.5.2a1/reflex/vars.py
+-rw-r--r--   0        0        0     5753 2024-05-23 22:07:24.104898 reflex-0.5.2a1/reflex/vars.pyi
+-rw-r--r--   0        0        0    12085 1970-01-01 00:00:00.000000 reflex-0.5.2a1/PKG-INFO
```

### Comparing `reflex-0.5.2/LICENSE` & `reflex-0.5.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/README.md` & `reflex-0.5.2a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/pyproject.toml` & `reflex-0.5.2a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.5.2"
+version = "0.5.2a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
```

### Comparing `reflex-0.5.2/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.5.2a1/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.5.2a1/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/web/tailwind.config.js.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.5.2a1/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.5.2a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.5.2a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.5.2a1/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/utils/helpers/debounce.js` & `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/debounce.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/utils/helpers/throttle.js` & `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/throttle.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/.templates/web/utils/state.js` & `reflex-0.5.2a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/__init__.py` & `reflex-0.5.2a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/__init__.pyi` & `reflex-0.5.2a1/reflex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/app.py` & `reflex-0.5.2a1/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/app_module_for_backend.py` & `reflex-0.5.2a1/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/base.py` & `reflex-0.5.2a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/compiler/compiler.py` & `reflex-0.5.2a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/compiler/templates.py` & `reflex-0.5.2a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/compiler/utils.py` & `reflex-0.5.2a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/__init__.py` & `reflex-0.5.2a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/app_wrap.py` & `reflex-0.5.2a1/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/app_wrap.pyi` & `reflex-0.5.2a1/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/bare.py` & `reflex-0.5.2a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/body.pyi` & `reflex-0.5.2a1/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/document.py` & `reflex-0.5.2a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/document.pyi` & `reflex-0.5.2a1/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/fragment.pyi` & `reflex-0.5.2a1/reflex/components/base/fragment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/head.pyi` & `reflex-0.5.2a1/reflex/components/base/head.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/link.py` & `reflex-0.5.2a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/link.pyi` & `reflex-0.5.2a1/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/meta.py` & `reflex-0.5.2a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/meta.pyi` & `reflex-0.5.2a1/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/script.py` & `reflex-0.5.2a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/base/script.pyi` & `reflex-0.5.2a1/reflex/components/base/script.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/__init__.py` & `reflex-0.5.2a1/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/base.py` & `reflex-0.5.2a1/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/base.pyi` & `reflex-0.5.2a1/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/list.py` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/table.py` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/transition.py` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.5.2a1/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/alert.py` & `reflex-0.5.2a1/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.5.2a1/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/progress.py` & `reflex-0.5.2a1/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.5.2a1/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/spinner.py` & `reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/__init__.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/button.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/button.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/checkbox.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/editable.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/editable.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/email.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/form.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/form.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/input.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/input.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/multiselect.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/numberinput.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/password.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/pininput.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/radio.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/radio.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/select.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/select.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/slider.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/slider.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/switch.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/switch.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/textarea.py` & `reflex-0.5.2a1/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.5.2a1/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/box.py` & `reflex-0.5.2a1/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/box.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/card.py` & `reflex-0.5.2a1/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/card.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/center.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/container.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/flex.py` & `reflex-0.5.2a1/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/flex.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/grid.py` & `reflex-0.5.2a1/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/grid.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/stack.py` & `reflex-0.5.2a1/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/stack.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/wrap.py` & `reflex-0.5.2a1/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.5.2a1/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/media/avatar.py` & `reflex-0.5.2a1/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/media/avatar.pyi` & `reflex-0.5.2a1/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/media/icon.py` & `reflex-0.5.2a1/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/media/icon.pyi` & `reflex-0.5.2a1/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/media/image.py` & `reflex-0.5.2a1/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/media/image.pyi` & `reflex-0.5.2a1/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/link.py` & `reflex-0.5.2a1/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/link.pyi` & `reflex-0.5.2a1/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/stepper.py` & `reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/__init__.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/drawer.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/menu.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.5.2a1/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/modal.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.5.2a1/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/popover.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.5.2a1/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/typography/heading.pyi` & `reflex-0.5.2a1/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/typography/highlight.py` & `reflex-0.5.2a1/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.5.2a1/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/typography/span.pyi` & `reflex-0.5.2a1/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/chakra/typography/text.pyi` & `reflex-0.5.2a1/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/component.py` & `reflex-0.5.2a1/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/__init__.py` & `reflex-0.5.2a1/reflex/components/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/banner.py` & `reflex-0.5.2a1/reflex/components/core/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/banner.pyi` & `reflex-0.5.2a1/reflex/components/core/banner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/client_side_routing.py` & `reflex-0.5.2a1/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/client_side_routing.pyi` & `reflex-0.5.2a1/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/colors.py` & `reflex-0.5.2a1/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/cond.py` & `reflex-0.5.2a1/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/debounce.py` & `reflex-0.5.2a1/reflex/components/core/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/debounce.pyi` & `reflex-0.5.2a1/reflex/components/core/debounce.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/foreach.py` & `reflex-0.5.2a1/reflex/components/core/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/html.py` & `reflex-0.5.2a1/reflex/components/core/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/html.pyi` & `reflex-0.5.2a1/reflex/components/core/html.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/match.py` & `reflex-0.5.2a1/reflex/components/core/match.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/responsive.py` & `reflex-0.5.2a1/reflex/components/core/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/upload.py` & `reflex-0.5.2a1/reflex/components/core/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/core/upload.pyi` & `reflex-0.5.2a1/reflex/components/core/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/datadisplay/code.py` & `reflex-0.5.2a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/datadisplay/code.pyi` & `reflex-0.5.2a1/reflex/components/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/datadisplay/dataeditor.py` & `reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/datadisplay/logo.py` & `reflex-0.5.2a1/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/constants/html.py` & `reflex-0.5.2a1/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/constants/react.py` & `reflex-0.5.2a1/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/constants/reflex.py` & `reflex-0.5.2a1/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/element.pyi` & `reflex-0.5.2a1/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/__init__.py` & `reflex-0.5.2a1/reflex/components/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/base.py` & `reflex-0.5.2a1/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/base.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/forms.py` & `reflex-0.5.2a1/reflex/components/el/elements/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/forms.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/forms.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/inline.py` & `reflex-0.5.2a1/reflex/components/el/elements/inline.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/inline.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/inline.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/media.py` & `reflex-0.5.2a1/reflex/components/el/elements/media.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/media.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/media.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/metadata.py` & `reflex-0.5.2a1/reflex/components/el/elements/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/metadata.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/metadata.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/other.py` & `reflex-0.5.2a1/reflex/components/el/elements/other.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/other.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/other.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/scripts.py` & `reflex-0.5.2a1/reflex/components/el/elements/scripts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/scripts.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/scripts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/sectioning.py` & `reflex-0.5.2a1/reflex/components/el/elements/sectioning.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/sectioning.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/sectioning.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/tables.py` & `reflex-0.5.2a1/reflex/components/el/elements/tables.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/tables.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/tables.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/typography.py` & `reflex-0.5.2a1/reflex/components/el/elements/typography.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/el/elements/typography.pyi` & `reflex-0.5.2a1/reflex/components/el/elements/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/gridjs/datatable.py` & `reflex-0.5.2a1/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/gridjs/datatable.pyi` & `reflex-0.5.2a1/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/lucide/icon.py` & `reflex-0.5.2a1/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/lucide/icon.pyi` & `reflex-0.5.2a1/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/markdown/markdown.py` & `reflex-0.5.2a1/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/markdown/markdown.pyi` & `reflex-0.5.2a1/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/moment/moment.py` & `reflex-0.5.2a1/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/moment/moment.pyi` & `reflex-0.5.2a1/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/next/base.pyi` & `reflex-0.5.2a1/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/next/image.py` & `reflex-0.5.2a1/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/next/image.pyi` & `reflex-0.5.2a1/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/next/link.pyi` & `reflex-0.5.2a1/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/next/video.py` & `reflex-0.5.2a1/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/next/video.pyi` & `reflex-0.5.2a1/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/plotly/plotly.py` & `reflex-0.5.2a1/reflex/components/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/plotly/plotly.pyi` & `reflex-0.5.2a1/reflex/components/plotly/plotly.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/props.py` & `reflex-0.5.2a1/reflex/components/props.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/accordion.py` & `reflex-0.5.2a1/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.5.2a1/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/base.py` & `reflex-0.5.2a1/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/base.pyi` & `reflex-0.5.2a1/reflex/components/radix/primitives/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/drawer.py` & `reflex-0.5.2a1/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.5.2a1/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/form.py` & `reflex-0.5.2a1/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/form.pyi` & `reflex-0.5.2a1/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/progress.py` & `reflex-0.5.2a1/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/progress.pyi` & `reflex-0.5.2a1/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/slider.py` & `reflex-0.5.2a1/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/primitives/slider.pyi` & `reflex-0.5.2a1/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/base.py` & `reflex-0.5.2a1/reflex/components/radix/themes/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/base.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/color_mode.py` & `reflex-0.5.2a1/reflex/components/radix/themes/color_mode.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/color_mode.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/__init__.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/avatar.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/badge.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/badge.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/button.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/button.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/callout.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/callout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/callout.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/card.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/card.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/checkbox_cards.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/checkbox_cards.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/checkbox_group.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/checkbox_group.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/data_list.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/data_list.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/dialog.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/inset.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/inset.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/inset.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/popover.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/progress.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/progress.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/radio.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/radio.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/radio_cards.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/radio_cards.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/segmented_control.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/segmented_control.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/select.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/select.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/separator.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/skeleton.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/skeleton.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/slider.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/spinner.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/switch.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/table.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/table.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/tabs.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/text_area.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/text_field.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/__init__.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/base.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/container.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/container.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/flex.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/grid.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/list.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/section.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/stack.py` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/code.py` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/heading.py` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/link.py` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/text.py` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/text.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.5.2a1/reflex/components/radix/themes/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/react_player/audio.pyi` & `reflex-0.5.2a1/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/react_player/react_player.py` & `reflex-0.5.2a1/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/react_player/react_player.pyi` & `reflex-0.5.2a1/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/react_player/video.pyi` & `reflex-0.5.2a1/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/__init__.py` & `reflex-0.5.2a1/reflex/components/recharts/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/cartesian.py` & `reflex-0.5.2a1/reflex/components/recharts/cartesian.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/cartesian.pyi` & `reflex-0.5.2a1/reflex/components/recharts/cartesian.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/charts.py` & `reflex-0.5.2a1/reflex/components/recharts/charts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/charts.pyi` & `reflex-0.5.2a1/reflex/components/recharts/charts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/general.py` & `reflex-0.5.2a1/reflex/components/recharts/general.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/general.pyi` & `reflex-0.5.2a1/reflex/components/recharts/general.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/polar.py` & `reflex-0.5.2a1/reflex/components/recharts/polar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/polar.pyi` & `reflex-0.5.2a1/reflex/components/recharts/polar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/recharts.py` & `reflex-0.5.2a1/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/recharts/recharts.pyi` & `reflex-0.5.2a1/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/sonner/toast.py` & `reflex-0.5.2a1/reflex/components/sonner/toast.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/sonner/toast.pyi` & `reflex-0.5.2a1/reflex/components/sonner/toast.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/suneditor/editor.py` & `reflex-0.5.2a1/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/suneditor/editor.pyi` & `reflex-0.5.2a1/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/tags/iter_tag.py` & `reflex-0.5.2a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/tags/tag.py` & `reflex-0.5.2a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/components/tags/tagless.py` & `reflex-0.5.2a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/config.py` & `reflex-0.5.2a1/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/config.pyi` & `reflex-0.5.2a1/reflex/config.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/__init__.py` & `reflex-0.5.2a1/reflex/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/base.py` & `reflex-0.5.2a1/reflex/constants/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/base.pyi` & `reflex-0.5.2a1/reflex/constants/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/colors.py` & `reflex-0.5.2a1/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/compiler.py` & `reflex-0.5.2a1/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/config.py` & `reflex-0.5.2a1/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/custom_components.py` & `reflex-0.5.2a1/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/event.py` & `reflex-0.5.2a1/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/installer.py` & `reflex-0.5.2a1/reflex/constants/installer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/route.py` & `reflex-0.5.2a1/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/constants/style.py` & `reflex-0.5.2a1/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/custom_components/custom_components.py` & `reflex-0.5.2a1/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/event.py` & `reflex-0.5.2a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/experimental/__init__.py` & `reflex-0.5.2a1/reflex/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/experimental/client_state.py` & `reflex-0.5.2a1/reflex/experimental/client_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/experimental/hooks.py` & `reflex-0.5.2a1/reflex/experimental/hooks.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/experimental/layout.py` & `reflex-0.5.2a1/reflex/experimental/layout.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/middleware/hydrate_middleware.py` & `reflex-0.5.2a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/middleware/middleware.py` & `reflex-0.5.2a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/model.py` & `reflex-0.5.2a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/page.py` & `reflex-0.5.2a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/reflex.py` & `reflex-0.5.2a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/route.py` & `reflex-0.5.2a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/state.py` & `reflex-0.5.2a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/style.py` & `reflex-0.5.2a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/testing.py` & `reflex-0.5.2a1/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/build.py` & `reflex-0.5.2a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/compat.py` & `reflex-0.5.2a1/reflex/utils/compat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/console.py` & `reflex-0.5.2a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/exceptions.py` & `reflex-0.5.2a1/reflex/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/exec.py` & `reflex-0.5.2a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/export.py` & `reflex-0.5.2a1/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/format.py` & `reflex-0.5.2a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/imports.py` & `reflex-0.5.2a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/path_ops.py` & `reflex-0.5.2a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/prerequisites.py` & `reflex-0.5.2a1/reflex/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/processes.py` & `reflex-0.5.2a1/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/pyi_generator.py` & `reflex-0.5.2a1/reflex/utils/pyi_generator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/serializers.py` & `reflex-0.5.2a1/reflex/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/telemetry.py` & `reflex-0.5.2a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/types.py` & `reflex-0.5.2a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/utils/watch.py` & `reflex-0.5.2a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/vars.py` & `reflex-0.5.2a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/reflex/vars.pyi` & `reflex-0.5.2a1/reflex/vars.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2/PKG-INFO` & `reflex-0.5.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.5.2
+Version: 0.5.2a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
```

