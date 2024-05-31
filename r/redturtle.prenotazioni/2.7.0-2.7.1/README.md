# Comparing `tmp/redturtle.prenotazioni-2.7.0.tar.gz` & `tmp/redturtle.prenotazioni-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.7.0.tar", last modified: Wed May 29 09:53:33 2024, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.7.1.tar", last modified: Fri May 31 09:49:42 2024, max compression
```

## Comparing `redturtle.prenotazioni-2.7.0.tar` & `redturtle.prenotazioni-2.7.1.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.621829 redturtle.prenotazioni-2.7.0/
--rw-r--r--   0 lucabel    (501) staff       (20)      748 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/APP_IO.txt
--rw-r--r--   0 lucabel    (501) staff       (20)    18210 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      152 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      586 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      667 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      110 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    47127 2024-05-29 09:53:33.621964 redturtle.prenotazioni-2.7.0/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    27508 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      164 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/TODO.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/constraints-5.2.x.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/constraints.txt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.542757 redturtle.prenotazioni-2.7.0/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7984 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       89 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      476 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/requirements-6.0.x.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       48 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-05-29 09:53:33.622430 redturtle.prenotazioni-2.7.0/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3420 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.524665 redturtle.prenotazioni-2.7.0/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.543047 redturtle.prenotazioni-2.7.0/src/redturtle/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.548627 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/
--rw-r--r--   0 lucabel    (501) staff       (20)     4638 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.549482 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      226 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3333 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/mail.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.552142 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    15296 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booker.py
--rw-r--r--   0 lucabel    (501) staff       (20)      729 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booking_code.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5974 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     4988 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/conflict.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5035 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/ical.py
--rw-r--r--   0 lucabel    (501) staff       (20)      273 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9662 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8771 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.552442 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.553285 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      563 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1766 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.553882 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
--rw-r--r--   0 lucabel    (501) staff       (20)     2362 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.555673 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
--rw-r--r--   0 lucabel    (501) staff       (20)    11754 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4255 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2364 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3445 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4807 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1151 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
--rw-r--r--   0 lucabel    (501) staff       (20)      423 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.557173 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
--rw-r--r--   0 lucabel    (501) staff       (20)    11125 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1791 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2284 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     4353 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13947 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.558662 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
--rw-r--r--   0 lucabel    (501) staff       (20)     6521 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1495 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1689 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3775 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3877 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
--rw-r--r--   0 lucabel    (501) staff       (20)      284 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.563909 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1817 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/base.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7331 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      655 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5709 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-r--r--   0 lucabel    (501) staff       (20)      673 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-r--r--   0 lucabel    (501) staff       (20)      155 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.564180 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/overrides/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10057 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5252 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2721 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-r--r--   0 lucabel    (501) staff       (20)    38319 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1735 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13788 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.565890 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-r--r--   0 lucabel    (501) staff       (20)      364 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-r--r--   0 lucabel    (501) staff       (20)      266 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-r--r--   0 lucabel    (501) staff       (20)     9794 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-r--r--   0 lucabel    (501) staff       (20)     1600 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-r--r--   0 lucabel    (501) staff       (20)      922 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.527995 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.527785 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.567298 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-r--r--   0 lucabel    (501) staff       (20)     3239 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-r--r--   0 lucabel    (501) staff       (20)     3808 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-r--r--   0 lucabel    (501) staff       (20)   349785 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-r--r--   0 lucabel    (501) staff       (20)      148 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.567558 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.567814 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-r--r--   0 lucabel    (501) staff       (20)     5095 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.568335 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-r--r--   0 lucabel    (501) staff       (20)     4705 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-r--r--   0 lucabel    (501) staff       (20)     1059 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.570926 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-r--r--   0 lucabel    (501) staff       (20)     3010 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      204 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     2874 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      401 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     1888 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     4187 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      337 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     1745 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      961 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-r--r--   0 lucabel    (501) staff       (20)     1261 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.571445 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-r--r--   0 lucabel    (501) staff       (20)      941 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-r--r--   0 lucabel    (501) staff       (20)      298 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.572462 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      698 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3863 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-r--r--   0 lucabel    (501) staff       (20)      575 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.575857 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     2836 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     1518 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     4828 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     2417 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-r--r--   0 lucabel    (501) staff       (20)       48 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     7714 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     9592 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-r--r--   0 lucabel    (501) staff       (20)    16384 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     2227 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5299 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5241 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     1858 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      362 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.576563 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      494 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1873 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8087 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/vacations.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1524 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/viewlets.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10861 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/week.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1193 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/widget.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6304 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-r--r--   0 lucabel    (501) staff       (20)      485 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/config.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2049 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.579140 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      111 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/booking_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1537 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/pause.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7504 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1251 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)      367 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-r--r--   0 lucabel    (501) staff       (20)    19857 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-r--r--   0 lucabel    (501) staff       (20)      371 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-r--r--   0 lucabel    (501) staff       (20)      371 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8518 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/validators.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.580489 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/
--rw-r--r--   0 lucabel    (501) staff       (20)       77 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1088 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      227 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.530438 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.581107 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.581370 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      133 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      630 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1347 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/smsdemo.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.582615 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/
--rw-r--r--   0 lucabel    (501) staff       (20)      270 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1615 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2101 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/events_logger.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1907 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.583110 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/
--rw-r--r--   0 lucabel    (501) staff       (20)      129 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/booker.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.583856 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      476 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1410 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1445 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.586769 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/
--rw-r--r--   0 lucabel    (501) staff       (20)     5302 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/README.md
--rw-r--r--   0 lucabel    (501) staff       (20)      207 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9443 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1035 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/cli.py
--rw-r--r--   0 lucabel    (501) staff       (20)    16384 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/io.db
--rw-r--r--   0 lucabel    (501) staff       (20)       45 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/io_tools.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1945 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/monkey.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2833 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/rdbms.py
--rw-r--r--   0 lucabel    (501) staff       (20)    27521 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/spec.yaml
--rw-r--r--   0 lucabel    (501) staff       (20)      961 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/storage.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.588083 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.531763 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.588372 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    62535 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.532106 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.589041 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)      804 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)    80885 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-r--r--   0 lucabel    (501) staff       (20)     1012 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/manual.pot
--rw-r--r--   0 lucabel    (501) staff       (20)    62826 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1618 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      521 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.sh
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.589588 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/monkeypatcher/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      499 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1565 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/permissions.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      507 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/prenotazione_event.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.534731 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.592378 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)     2656 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      185 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      349 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       71 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      196 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      325 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.593145 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)     5140 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2015 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      251 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3421 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      277 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/sharing.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.594665 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     3565 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2983 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3861 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3257 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3845 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3846 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      713 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.533509 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.594926 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)    12711 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.595273 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)     8877 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      613 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.595547 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1402/
--rw-r--r--   0 lucabel    (501) staff       (20)     1508 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.595812 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1500/
--rw-r--r--   0 lucabel    (501) staff       (20)      226 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.596330 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/
--rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      638 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.596950 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/
--rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.534549 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.597204 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)    12711 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.597466 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      125 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.598172 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)      431 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      152 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.598627 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      199 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.599120 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.600828 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      468 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     7769 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)      973 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)      925 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1721 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)      162 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.601081 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.601797 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      352 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3734 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.603742 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6553 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1641 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1209 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1166 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1328 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/move.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1152 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
--rw-r--r--   0 lucabel    (501) staff       (20)      966 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.604515 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5395 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.605376 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      548 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     4137 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-r--r--   0 lucabel    (501) staff       (20)      336 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.606123 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      365 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6732 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/day.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.606821 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      216 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      915 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.607264 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      525 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1062 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3443 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.616875 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1223 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/helpers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3222 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_block.py
--rw-r--r--   0 lucabel    (501) staff       (20)    25000 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1980 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)    17450 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_available_slots.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2011 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_base_slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4387 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6402 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6901 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_notify.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8748 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8696 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6036 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3088 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6317 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_day.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10871 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10361 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4000 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_gates_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8161 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_move_booking_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5216 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3591 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notify_the_message_failure.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14545 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5029 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
--rw-r--r--   0 lucabel    (501) staff       (20)    15081 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4861 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7049 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
--rw-r--r--   0 lucabel    (501) staff       (20)      740 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
--rw-r--r--   0 lucabel    (501) staff       (20)    19833 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2485 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9722 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_send_ical.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4180 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3046 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_stringinterp.py
--rw-r--r--   0 lucabel    (501) staff       (20)      905 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_utils.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6486 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vacation_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1198 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2349 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)    23517 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)    16971 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10649 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.618296 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/
--rw-r--r--   0 lucabel    (501) staff       (20)       94 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2900 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-r--r--   0 lucabel    (501) staff       (20)      489 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/email.py
--rw-r--r--   0 lucabel    (501) staff       (20)      549 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/log_errors.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1118 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/urls.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.618836 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/
--rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      597 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.621628 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1444 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      607 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1011 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-r--r--   0 lucabel    (501) staff       (20)      598 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1814 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-r--r--   0 lucabel    (501) staff       (20)      776 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1128 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2549 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1367 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      440 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.545560 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    47127 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    17737 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      267 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       10 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      425 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       10 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.252486 redturtle.prenotazioni-2.7.1/
+-rw-r--r--   0 roman      (502) staff       (20)      748 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/APP_IO.txt
+-rw-r--r--   0 roman      (502) staff       (20)    18293 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/CHANGES.rst
+-rw-r--r--   0 roman      (502) staff       (20)      152 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/CONTRIBUTORS.rst
+-rw-r--r--   0 roman      (502) staff       (20)      586 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/DEVELOP.rst
+-rw-r--r--   0 roman      (502) staff       (20)    18092 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/LICENSE.GPL
+-rw-r--r--   0 roman      (502) staff       (20)      667 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/LICENSE.rst
+-rw-r--r--   0 roman      (502) staff       (20)      110 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/MANIFEST.in
+-rw-r--r--   0 roman      (502) staff       (20)    61925 2024-05-31 09:49:42.253068 redturtle.prenotazioni-2.7.1/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)    27508 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/README.rst
+-rw-r--r--   0 roman      (502) staff       (20)      164 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/TODO.txt
+-rw-r--r--   0 roman      (502) staff       (20)      105 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/constraints-5.2.x.txt
+-rw-r--r--   0 roman      (502) staff       (20)      105 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/constraints.txt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.182513 redturtle.prenotazioni-2.7.1/docs/
+-rw-r--r--   0 roman      (502) staff       (20)     7984 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/docs/conf.py
+-rw-r--r--   0 roman      (502) staff       (20)       89 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/docs/index.rst
+-rw-r--r--   0 roman      (502) staff       (20)      476 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/requirements-6.0.x.txt
+-rw-r--r--   0 roman      (502) staff       (20)       48 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/requirements.txt
+-rw-r--r--   0 roman      (502) staff       (20)      344 2024-05-31 09:49:42.253569 redturtle.prenotazioni-2.7.1/setup.cfg
+-rw-r--r--   0 roman      (502) staff       (20)     3420 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/setup.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.169778 redturtle.prenotazioni-2.7.1/src/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.182736 redturtle.prenotazioni-2.7.1/src/redturtle/
+-rw-r--r--   0 roman      (502) staff       (20)       80 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.187109 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/
+-rw-r--r--   0 roman      (502) staff       (20)     4638 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.187866 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/actions/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/actions/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      226 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3333 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/actions/mail.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.190039 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)    15296 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/booker.py
+-rw-r--r--   0 roman      (502) staff       (20)      729 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/booking_code.py
+-rw-r--r--   0 roman      (502) staff       (20)     5974 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     4988 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-r--r--   0 roman      (502) staff       (20)     5035 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/ical.py
+-rw-r--r--   0 roman      (502) staff       (20)      273 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-r--r--   0 roman      (502) staff       (20)     9662 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/slot.py
+-rw-r--r--   0 roman      (502) staff       (20)     8771 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.190318 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.190976 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      563 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1766 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.191532 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
+-rw-r--r--   0 roman      (502) staff       (20)     2362 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.193029 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
+-rw-r--r--   0 roman      (502) staff       (20)    11754 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     4255 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     2364 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3445 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
+-rw-r--r--   0 roman      (502) staff       (20)     4807 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
+-rw-r--r--   0 roman      (502) staff       (20)     1151 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
+-rw-r--r--   0 roman      (502) staff       (20)      423 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.194203 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
+-rw-r--r--   0 roman      (502) staff       (20)    11125 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1791 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     2284 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     4353 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
+-rw-r--r--   0 roman      (502) staff       (20)    13947 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.195475 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
+-rw-r--r--   0 roman      (502) staff       (20)     6521 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1495 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
+-rw-r--r--   0 roman      (502) staff       (20)     1689 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3775 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
+-rw-r--r--   0 roman      (502) staff       (20)     3877 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
+-rw-r--r--   0 roman      (502) staff       (20)      284 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.199934 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1817 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/base.py
+-rw-r--r--   0 roman      (502) staff       (20)     7331 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      655 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-r--r--   0 roman      (502) staff       (20)     5709 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-r--r--   0 roman      (502) staff       (20)      673 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-r--r--   0 roman      (502) staff       (20)      155 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.200162 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/overrides/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-r--r--   0 roman      (502) staff       (20)     3169 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)    10057 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-r--r--   0 roman      (502) staff       (20)     5252 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-r--r--   0 roman      (502) staff       (20)     2721 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-r--r--   0 roman      (502) staff       (20)    38319 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-r--r--   0 roman      (502) staff       (20)     1735 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-r--r--   0 roman      (502) staff       (20)    13788 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.201697 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-r--r--   0 roman      (502) staff       (20)      364 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-r--r--   0 roman      (502) staff       (20)      503 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-r--r--   0 roman      (502) staff       (20)      266 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-r--r--   0 roman      (502) staff       (20)     9794 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-r--r--   0 roman      (502) staff       (20)     1600 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-r--r--   0 roman      (502) staff       (20)      922 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.171863 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.171733 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.203415 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-r--r--   0 roman      (502) staff       (20)     3239 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-r--r--   0 roman      (502) staff       (20)     3808 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-r--r--   0 roman      (502) staff       (20)   349785 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-r--r--   0 roman      (502) staff       (20)      148 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.203687 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.203972 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-r--r--   0 roman      (502) staff       (20)     5095 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.204565 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-r--r--   0 roman      (502) staff       (20)     4705 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-r--r--   0 roman      (502) staff       (20)     1059 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.207042 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-r--r--   0 roman      (502) staff       (20)     3010 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-r--r--   0 roman      (502) staff       (20)      204 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-r--r--   0 roman      (502) staff       (20)     2874 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
+-rw-r--r--   0 roman      (502) staff       (20)      401 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
+-rw-r--r--   0 roman      (502) staff       (20)     1888 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-r--r--   0 roman      (502) staff       (20)      314 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-r--r--   0 roman      (502) staff       (20)     4187 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
+-rw-r--r--   0 roman      (502) staff       (20)      337 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
+-rw-r--r--   0 roman      (502) staff       (20)     1745 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-r--r--   0 roman      (502) staff       (20)      961 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-r--r--   0 roman      (502) staff       (20)     1261 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.207560 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-r--r--   0 roman      (502) staff       (20)      941 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-r--r--   0 roman      (502) staff       (20)      298 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.208498 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      698 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-r--r--   0 roman      (502) staff       (20)     3863 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-r--r--   0 roman      (502) staff       (20)      575 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.211784 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/
+-rw-r--r--   0 roman      (502) staff       (20)     2836 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-r--r--   0 roman      (502) staff       (20)     1518 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-r--r--   0 roman      (502) staff       (20)     4828 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-r--r--   0 roman      (502) staff       (20)     2417 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-r--r--   0 roman      (502) staff       (20)       48 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-r--r--   0 roman      (502) staff       (20)     7714 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-r--r--   0 roman      (502) staff       (20)     9592 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-r--r--   0 roman      (502) staff       (20)    16384 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-r--r--   0 roman      (502) staff       (20)     2227 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-r--r--   0 roman      (502) staff       (20)     5299 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-r--r--   0 roman      (502) staff       (20)     5241 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-r--r--   0 roman      (502) staff       (20)     1858 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-r--r--   0 roman      (502) staff       (20)      362 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.212431 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/utilities/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/utilities/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      494 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/utilities/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1873 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
+-rw-r--r--   0 roman      (502) staff       (20)     8087 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/vacations.py
+-rw-r--r--   0 roman      (502) staff       (20)     1524 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-r--r--   0 roman      (502) staff       (20)    10861 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/week.py
+-rw-r--r--   0 roman      (502) staff       (20)     1193 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/widget.py
+-rw-r--r--   0 roman      (502) staff       (20)     6304 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-r--r--   0 roman      (502) staff       (20)      485 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/config.py
+-rw-r--r--   0 roman      (502) staff       (20)     2049 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.214805 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      111 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/booking_type.py
+-rw-r--r--   0 roman      (502) staff       (20)     1537 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/pause.py
+-rw-r--r--   0 roman      (502) staff       (20)     7504 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)     1251 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazione_type.py
+-rw-r--r--   0 roman      (502) staff       (20)      367 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-r--r--   0 roman      (502) staff       (20)    19857 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-r--r--   0 roman      (502) staff       (20)      371 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-r--r--   0 roman      (502) staff       (20)      371 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-r--r--   0 roman      (502) staff       (20)     8518 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/validators.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.216198 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/
+-rw-r--r--   0 roman      (502) staff       (20)       77 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1088 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      227 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.173337 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/profiles/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.216908 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/profiles/default/
+-rw-r--r--   0 roman      (502) staff       (20)      208 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)       88 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.217185 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/profiles/uninstall/
+-rw-r--r--   0 roman      (502) staff       (20)      133 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      630 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/setuphandlers.py
+-rw-r--r--   0 roman      (502) staff       (20)     1347 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/smsdemo.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.218341 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/
+-rw-r--r--   0 roman      (502) staff       (20)      270 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1615 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     2101 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/events_logger.py
+-rw-r--r--   0 roman      (502) staff       (20)     1907 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)     1189 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.218791 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/exceptions/
+-rw-r--r--   0 roman      (502) staff       (20)      129 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/exceptions/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      712 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/exceptions/booker.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.219479 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/indexers/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      476 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1410 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/indexers/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)     1445 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/interfaces.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.221905 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/
+-rw-r--r--   0 roman      (502) staff       (20)     5302 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/README.md
+-rw-r--r--   0 roman      (502) staff       (20)      207 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     9443 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/api.py
+-rw-r--r--   0 roman      (502) staff       (20)     1035 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/cli.py
+-rw-r--r--   0 roman      (502) staff       (20)    16384 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/io.db
+-rw-r--r--   0 roman      (502) staff       (20)       45 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/io_tools.py
+-rw-r--r--   0 roman      (502) staff       (20)     1945 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/monkey.py
+-rw-r--r--   0 roman      (502) staff       (20)     2833 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/rdbms.py
+-rw-r--r--   0 roman      (502) staff       (20)    27521 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/spec.yaml
+-rw-r--r--   0 roman      (502) staff       (20)      961 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/storage.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.222942 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.174181 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/en/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.223181 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)    62535 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.174392 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/it/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.223734 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-r--r--   0 roman      (502) staff       (20)      804 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 roman      (502) staff       (20)    80885 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-r--r--   0 roman      (502) staff       (20)     1012 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/manual.pot
+-rw-r--r--   0 roman      (502) staff       (20)    62826 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-r--r--   0 roman      (502) staff       (20)     1618 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/update.py
+-rwxr-xr-x   0 roman      (502) staff       (20)      521 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/update.sh
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.224248 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/monkeypatcher/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      499 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1565 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/permissions.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      507 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/prenotazione_event.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.176173 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.226733 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/
+-rw-r--r--   0 roman      (502) staff       (20)     2656 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-r--r--   0 roman      (502) staff       (20)      185 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-r--r--   0 roman      (502) staff       (20)      349 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-r--r--   0 roman      (502) staff       (20)       71 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-r--r--   0 roman      (502) staff       (20)      196 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/diff_tool.xml
+-rw-r--r--   0 roman      (502) staff       (20)      325 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.227407 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-r--r--   0 roman      (502) staff       (20)     5140 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-r--r--   0 roman      (502) staff       (20)     2015 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-r--r--   0 roman      (502) staff       (20)     1001 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-r--r--   0 roman      (502) staff       (20)      251 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/repositorytool.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3421 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+-rw-r--r--   0 roman      (502) staff       (20)      277 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/sharing.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.228762 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/
+-rw-r--r--   0 roman      (502) staff       (20)     3565 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-r--r--   0 roman      (502) staff       (20)     2983 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3861 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3257 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3845 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-r--r--   0 roman      (502) staff       (20)     3846 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-r--r--   0 roman      (502) staff       (20)      713 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.175313 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.228989 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-r--r--   0 roman      (502) staff       (20)    12711 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.229220 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-r--r--   0 roman      (502) staff       (20)     8877 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-r--r--   0 roman      (502) staff       (20)      613 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.229448 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-r--r--   0 roman      (502) staff       (20)     1508 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.229668 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-r--r--   0 roman      (502) staff       (20)      226 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.230112 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2005/
+-rw-r--r--   0 roman      (502) staff       (20)       88 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
+-rw-r--r--   0 roman      (502) staff       (20)      638 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.230554 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/
+-rw-r--r--   0 roman      (502) staff       (20)       88 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.176051 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.230792 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
+-rw-r--r--   0 roman      (502) staff       (20)    12711 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
+-rw-r--r--   0 roman      (502) staff       (20)      279 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.231032 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-r--r--   0 roman      (502) staff       (20)      125 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.231498 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-r--r--   0 roman      (502) staff       (20)      431 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-r--r--   0 roman      (502) staff       (20)      152 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.231901 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      199 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.232298 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.233687 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      468 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     7769 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-r--r--   0 roman      (502) staff       (20)      973 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
+-rw-r--r--   0 roman      (502) staff       (20)      925 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
+-rw-r--r--   0 roman      (502) staff       (20)     1721 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-r--r--   0 roman      (502) staff       (20)      162 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.233953 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.234593 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/available_slots/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      352 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     3734 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.236409 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     6553 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-r--r--   0 roman      (502) staff       (20)     1641 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     1209 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-r--r--   0 roman      (502) staff       (20)     1166 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/get.py
+-rw-r--r--   0 roman      (502) staff       (20)     1328 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/move.py
+-rw-r--r--   0 roman      (502) staff       (20)     1152 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
+-rw-r--r--   0 roman      (502) staff       (20)      966 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.237074 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      404 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     5395 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.237698 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      548 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     4137 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-r--r--   0 roman      (502) staff       (20)      336 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.238330 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/day/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/day/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      365 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)     6732 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/day/day.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.238952 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/types/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/types/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      216 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      915 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/types/get.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.239351 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/scripts/
+-rw-r--r--   0 roman      (502) staff       (20)        0 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      525 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
+-rw-r--r--   0 roman      (502) staff       (20)     1062 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/setuphandlers.py
+-rw-r--r--   0 roman      (502) staff       (20)     3443 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/testing.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.248118 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/
+-rw-r--r--   0 roman      (502) staff       (20)      105 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1223 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/helpers.py
+-rw-r--r--   0 roman      (502) staff       (20)     3222 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_add_block.py
+-rw-r--r--   0 roman      (502) staff       (20)    25000 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_add_booking.py
+-rw-r--r--   0 roman      (502) staff       (20)     1980 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_add_booking_type.py
+-rw-r--r--   0 roman      (502) staff       (20)    17450 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_available_slots.py
+-rw-r--r--   0 roman      (502) staff       (20)     2011 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_base_slot.py
+-rw-r--r--   0 roman      (502) staff       (20)     4387 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
+-rw-r--r--   0 roman      (502) staff       (20)     6402 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-r--r--   0 roman      (502) staff       (20)     6901 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booking_notify.py
+-rw-r--r--   0 roman      (502) staff       (20)     8748 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-r--r--   0 roman      (502) staff       (20)     8696 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
+-rw-r--r--   0 roman      (502) staff       (20)     6036 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
+-rw-r--r--   0 roman      (502) staff       (20)     3088 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
+-rw-r--r--   0 roman      (502) staff       (20)     6317 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_day.py
+-rw-r--r--   0 roman      (502) staff       (20)    10871 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-r--r--   0 roman      (502) staff       (20)    10361 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-r--r--   0 roman      (502) staff       (20)     4000 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_gates_overrides.py
+-rw-r--r--   0 roman      (502) staff       (20)     8161 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_move_booking_api.py
+-rw-r--r--   0 roman      (502) staff       (20)     5216 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
+-rw-r--r--   0 roman      (502) staff       (20)     3591 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_notify_the_message_failure.py
+-rw-r--r--   0 roman      (502) staff       (20)    14545 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
+-rw-r--r--   0 roman      (502) staff       (20)     5029 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
+-rw-r--r--   0 roman      (502) staff       (20)    15081 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
+-rw-r--r--   0 roman      (502) staff       (20)     4861 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-r--r--   0 roman      (502) staff       (20)     7049 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
+-rw-r--r--   0 roman      (502) staff       (20)      740 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
+-rw-r--r--   0 roman      (502) staff       (20)    19833 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-r--r--   0 roman      (502) staff       (20)     2485 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
+-rw-r--r--   0 roman      (502) staff       (20)     9722 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_send_ical.py
+-rw-r--r--   0 roman      (502) staff       (20)     4180 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-r--r--   0 roman      (502) staff       (20)     3046 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_stringinterp.py
+-rw-r--r--   0 roman      (502) staff       (20)      905 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_utils.py
+-rw-r--r--   0 roman      (502) staff       (20)     6486 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_vacation_api.py
+-rw-r--r--   0 roman      (502) staff       (20)     1198 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py
+-rw-r--r--   0 roman      (502) staff       (20)     2349 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_vocabularies.py
+-rw-r--r--   0 roman      (502) staff       (20)    23517 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-r--r--   0 roman      (502) staff       (20)    17023 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/upgrades.py
+-rw-r--r--   0 roman      (502) staff       (20)    10917 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/upgrades.zcml
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.249324 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/
+-rw-r--r--   0 roman      (502) staff       (20)       94 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     2900 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-r--r--   0 roman      (502) staff       (20)      489 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/email.py
+-rw-r--r--   0 roman      (502) staff       (20)      549 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/log_errors.py
+-rw-r--r--   0 roman      (502) staff       (20)     1118 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/urls.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.249787 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utils/
+-rw-r--r--   0 roman      (502) staff       (20)       67 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utils/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)      597 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.252286 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/
+-rw-r--r--   0 roman      (502) staff       (20)       24 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-r--r--   0 roman      (502) staff       (20)     1444 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-r--r--   0 roman      (502) staff       (20)      607 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-r--r--   0 roman      (502) staff       (20)     1011 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-r--r--   0 roman      (502) staff       (20)      598 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-r--r--   0 roman      (502) staff       (20)     1814 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-r--r--   0 roman      (502) staff       (20)      776 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
+-rw-r--r--   0 roman      (502) staff       (20)     1128 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-r--r--   0 roman      (502) staff       (20)     2549 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-r--r--   0 roman      (502) staff       (20)     1367 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+-rw-r--r--   0 roman      (502) staff       (20)      440 2024-05-31 09:49:41.000000 redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
+drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-05-31 09:49:42.184769 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/
+-rw-r--r--   0 roman      (502) staff       (20)    61925 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (502) staff       (20)    17737 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (502) staff       (20)      295 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-r--r--   0 roman      (502) staff       (20)       10 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-r--r--   0 roman      (502) staff       (20)        1 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-r--r--   0 roman      (502) staff       (20)      425 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-r--r--   0 roman      (502) staff       (20)       10 2024-05-31 09:49:42.000000 redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.7.0/APP_IO.txt` & `redturtle.prenotazioni-2.7.1/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/CHANGES.rst` & `redturtle.prenotazioni-2.7.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+2.7.1 (2024-05-31)
+------------------
+
+- Hotfix missing permission.
+  [folix-01]
+
+
 2.7.0 (2024-05-29)
 ------------------
 
 - Workarounds for external integration: search with tinit- prefixed user,
   schema with some fields with only spaces
   [mamico]
```

### Comparing `redturtle.prenotazioni-2.7.0/DEVELOP.rst` & `redturtle.prenotazioni-2.7.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/LICENSE.GPL` & `redturtle.prenotazioni-2.7.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/LICENSE.rst` & `redturtle.prenotazioni-2.7.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/README.rst` & `redturtle.prenotazioni-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/docs/conf.py` & `redturtle.prenotazioni-2.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/setup.py` & `redturtle.prenotazioni-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.7.0",
+    version="2.7.1",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booking_code.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/booking_code.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/ical.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione_type.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/setuphandlers.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/smsdemo.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/demo/smsdemo.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/booker.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/exceptions/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/prenotazione.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/indexers/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/README.md` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/api.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/cli.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/io.db` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/monkey.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/rdbms.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/spec.yaml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/storage.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.sh` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/get.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/available_slots/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/move.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/vacation.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking/vacation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/day.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/day/day.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/get.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/helpers.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_block.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_add_block.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_add_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking_type.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_add_booking_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_available_slots.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_available_slots.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_base_slot.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_base_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_notify.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booking_notify.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_day.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_day.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_gates_overrides.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_gates_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_move_booking_api.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_move_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notify_the_message_failure.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_notify_the_message_failure.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_pauses_overrides.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_pauses_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_events.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazione_events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_restapi_types_override.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_restapi_types_override.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_send_ical.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_send_ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_stringinterp.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_utils.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vacation_api.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_vacation_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vocabularies.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/upgrades.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,7 +512,11 @@
     update_profile(context, "repositorytool")
 
     portal_types = api.portal.get_tool(name="portal_types")
     modulo_behaviors = [x for x in portal_types["Prenotazione"].behaviors]
     if "plone.versioning" not in modulo_behaviors:
         modulo_behaviors.append("plone.versioning")
     portal_types["Prenotazione"].behaviors = tuple(modulo_behaviors)
+
+
+def to_2010(context):
+    update_rolemap(context)
```

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -361,9 +361,19 @@
       destination="2009"
       >
     <genericsetup:upgradeStep
         title="Add versioning to Prenotazione c.t."
         handler=".upgrades.to_2009"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="redturtle.prenotazioni:default"
+      source="2009"
+      destination="2010"
+      >
+    <genericsetup:upgradeStep
+        title="Update rolemap"
+        handler=".upgrades.to_2010"
+        />
+  </genericsetup:upgradeSteps>
 
 </configure>
```

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/log_errors.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/log_errors.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.7.1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.7.1/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

