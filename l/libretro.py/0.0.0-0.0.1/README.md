# Comparing `tmp/libretro_py-0.0.0.tar.gz` & `tmp/libretro_py-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_py-0.0.0.tar", last modified: Sun Apr 21 21:30:19 2024, max compression
+gzip compressed data, was "libretro_py-0.0.1.tar", last modified: Fri May 31 17:45:43 2024, max compression
```

## Comparing `libretro_py-0.0.0.tar` & `libretro_py-0.0.1.tar`

### file list

```diff
@@ -1,170 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.940329 libretro_py-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-21 21:29:29.000000 libretro_py-0.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 21:29:29.000000 libretro_py-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 21:29:29.000000 libretro_py-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-21 21:30:19.940329 libretro_py-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-21 21:29:29.000000 libretro_py-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-21 21:29:29.000000 libretro_py-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:30:19.940329 libretro_py-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-21 21:29:29.000000 libretro_py-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.916329 libretro_py-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.920329 libretro_py-0.0.0/src/libretro/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.924329 libretro_py-0.0.0/src/libretro/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/av.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.924329 libretro_py-0.0.0/src/libretro/api/input/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/analog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/joypad.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/lightgun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/input/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/midi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/netpacket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/perf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/rumble.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/savestate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/vfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/api/video/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/video/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/video/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/video/negotiate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/api/video/render.py
--rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    24705 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/audio/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/audio/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/audio/wave.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/camera/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/camera/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/camera/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/content/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/content/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/content/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/disk/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/disk/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47527 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/environment/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/environment/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/environment/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/environment/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.928329 libretro_py-0.0.0/src/libretro/drivers/input/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/input/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    21413 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/input/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/led/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/led/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/led/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/location/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/location/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/location/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/log/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/log/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/log/unformatted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/message/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/message/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/message/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/microphone/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/microphone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/microphone/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/microphone/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/midi/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/midi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/midi/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/midi/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/netpacket/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/netpacket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/netpacket/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/netpacket/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/options/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/options/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/options/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.932329 libretro_py-0.0.0/src/libretro/drivers/path/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/path/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/path/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/perf/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/perf/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/perf/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/power/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/power/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/rumble/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/rumble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/rumble/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/rumble/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/sensor/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/sensor/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/timing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/timing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/timing/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/timing/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/user/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/user/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/user/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/vfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/vfs/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/vfs/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18395 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/vfs/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/video/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.936329 libretro_py-0.0.0/src/libretro/drivers/video/opengl/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/opengl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/opengl/moderngl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.940329 libretro_py-0.0.0/src/libretro/drivers/video/software/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/software/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/software/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/drivers/video/software/pillow.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/h.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-04-21 21:29:29.000000 libretro_py-0.0.0/src/libretro/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:19.940329 libretro_py-0.0.0/src/libretro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-21 21:30:19.000000 libretro_py-0.0.0/src/libretro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-21 21:30:19.000000 libretro_py-0.0.0/src/libretro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:30:19.000000 libretro_py-0.0.0/src/libretro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-21 21:30:19.000000 libretro_py-0.0.0/src/libretro.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 21:30:19.000000 libretro_py-0.0.0/src/libretro.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.734617 libretro_py-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-31 17:44:51.000000 libretro_py-0.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 17:44:51.000000 libretro_py-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 17:44:51.000000 libretro_py-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-31 17:45:43.734617 libretro_py-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-31 17:44:51.000000 libretro_py-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-31 17:44:51.000000 libretro_py-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:45:43.734617 libretro_py-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-31 17:44:51.000000 libretro_py-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.702614 libretro_py-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.706614 libretro_py-0.0.1/src/libretro/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.714615 libretro_py-0.0.1/src/libretro/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/av.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.714615 libretro_py-0.0.1/src/libretro/api/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/analog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/joypad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/lightgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/input/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/midi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/netpacket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/rumble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/savestate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/vfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.714615 libretro_py-0.0.1/src/libretro/api/video/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/video/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/video/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/video/negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/api/video/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29812 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25401 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.714615 libretro_py-0.0.1/src/libretro/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/audio/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/audio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/audio/wave.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/camera/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/camera/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/content/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/content/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/disk/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/environment/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/environment/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/environment/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/environment/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/input/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21421 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/input/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.718615 libretro_py-0.0.1/src/libretro/drivers/led/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/led/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/led/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/location/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/location/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/location/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/log/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/log/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/log/unformatted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/message/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/message/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/message/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/microphone/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/microphone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/microphone/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/microphone/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/midi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/midi/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/midi/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/netpacket/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/netpacket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/netpacket/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/netpacket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.722616 libretro_py-0.0.1/src/libretro/drivers/options/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/options/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/options/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/path/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/path/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/perf/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/perf/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/power/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/power/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/rumble/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/rumble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/rumble/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/rumble/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/sensor/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/sensor/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/timing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/timing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/timing/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/timing/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/user/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/user/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.726616 libretro_py-0.0.1/src/libretro/drivers/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/vfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/vfs/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/vfs/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/vfs/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.730617 libretro_py-0.0.1/src/libretro/drivers/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.730617 libretro_py-0.0.1/src/libretro/drivers/video/opengl/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/opengl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/opengl/moderngl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.730617 libretro_py-0.0.1/src/libretro/drivers/video/software/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/software/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/drivers/video/software/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/h.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-05-31 17:44:51.000000 libretro_py-0.0.1/src/libretro/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:43.730617 libretro_py-0.0.1/src/libretro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-31 17:45:43.000000 libretro_py-0.0.1/src/libretro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-31 17:45:43.000000 libretro_py-0.0.1/src/libretro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:45:43.000000 libretro_py-0.0.1/src/libretro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-31 17:45:43.000000 libretro_py-0.0.1/src/libretro.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 17:45:43.000000 libretro_py-0.0.1/src/libretro.py.egg-info/top_level.txt
```

### Comparing `libretro_py-0.0.0/LICENSE` & `libretro_py-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/PKG-INFO` & `libretro_py-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretro.py
-Version: 0.0.0
+Version: 0.0.1
 Summary: A libretro frontend for Python intended for testing cores.
 Author-email: Jesse Talavera <jesse@jesse.tg>
 Maintainer-email: Jesse Talavera <jesse@jesse.tg>
 License: MIT License
 Project-URL: Homepage, https://github.com/JesseTG/libretro.py
 Project-URL: Issues, https://github.com/JesseTG/libretro.py/issues
 Project-URL: Repository, https://github.com/JesseTG/libretro.py
@@ -31,45 +31,44 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions==4.*; python_version == "3.10"
 Provides-Extra: build
 Requires-Dist: build==1.2.1; extra == "build"
 Requires-Dist: setuptools>=69.1.1; extra == "build"
 Requires-Dist: twine==5.0.0; extra == "build"
+Requires-Dist: pre-commit==3.7.*; extra == "build"
 Provides-Extra: dev
 Requires-Dist: bandit==1.7.*; extra == "dev"
-Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: black==24.*; extra == "dev"
 Requires-Dist: flake8==6.*; extra == "dev"
 Requires-Dist: isort==5.*; extra == "dev"
 Requires-Dist: mypy==1.5.*; extra == "dev"
 Requires-Dist: libretro.py[build]; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: Sphinx==7.*; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.*; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: doc
 Requires-Dist: libretro.py[docs]; extra == "doc"
 Provides-Extra: opengl
 Requires-Dist: moderngl==5.10.*; extra == "opengl"
-Provides-Extra: pillow
-Requires-Dist: pillow==10.2.*; extra == "pillow"
-Requires-Dist: types-Pillow; extra == "pillow"
+Requires-Dist: PyOpenGL==3.1.*; extra == "opengl"
 Provides-Extra: all
-Requires-Dist: libretro.py[build,dev,docs,opengl,pillow]; extra == "all"
+Requires-Dist: libretro.py[build,dev,docs,opengl]; extra == "all"
 
 # libretro.py
 
 A Python binding for [libretro][libretro] intended for testing cores,
 but suitable for any purpose.
 Ease of use, flexibility, and complete API support are top priorities.
 
 <div align="center">
 
-[![Build Status](https://github.com/JesseTG/libretro.py/workflows/build/badge.svg)](https://github.com/JesseTG/libretro.py/actions)
-[![PyPi](https://img.shields.io/pypi/v/PROJECT_NAME_URL)](https://pypi.org/project/PROJECT_NAME_URL)
+[![Workflow Status](https://github.com/JesseTG/libretro.py/actions/workflows/release.yml/badge.svg)](https://github.com/JesseTG/libretro.py/actions/workflows/release.yml)
+[![PyPi](https://img.shields.io/pypi/v/libretro.py)](https://pypi.org/project/libretro.py)
 [![License](https://img.shields.io/github/license/JesseTG/libretro.py)](LICENSE)
 
 </div>
 
 # Supported Environments
 
 libretro.py has the following requirements:
@@ -123,28 +122,23 @@
 To install additional features,
 add one or more of the following extras to the `install` command:
 
 - **`dev`:** Assorted tools used to help develop libretro.py.
   Required if contributing to libretro.py.
 - **`opengl`:** Support for the built-in OpenGL video driver.
   Required if testing a core's OpenGL support.
-- **`pillow`:** Support for the built-in software-only video driver
-  powered by the [Pillow][pillow] image processing library.
-  Not required for any particular feature,
-  but it simplifies tests that inspect the core's video output.
 
-For example, if you want to submit an improvement to the Pillow video driver,
+For example, if you want to submit an improvement to the OpenGL video driver,
 you would install libretro.py like so:
 
 ```bash
-pip install libretro.py[pillow,dev]
+pip install libretro.py[opengl,dev]
 ```
 
 And if you just want to test your libretro core's OpenGL support:
 
 ```bash
 pip install libretro.py[opengl]
 ```
 
 [just]: https://just.systems
 [libretro]: https://www.libretro.com
-[pillow]: https://python-pillow.org
```

### Comparing `libretro_py-0.0.0/README.md` & `libretro_py-0.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 A Python binding for [libretro][libretro] intended for testing cores,
 but suitable for any purpose.
 Ease of use, flexibility, and complete API support are top priorities.
 
 <div align="center">
 
-[![Build Status](https://github.com/JesseTG/libretro.py/workflows/build/badge.svg)](https://github.com/JesseTG/libretro.py/actions)
-[![PyPi](https://img.shields.io/pypi/v/PROJECT_NAME_URL)](https://pypi.org/project/PROJECT_NAME_URL)
+[![Workflow Status](https://github.com/JesseTG/libretro.py/actions/workflows/release.yml/badge.svg)](https://github.com/JesseTG/libretro.py/actions/workflows/release.yml)
+[![PyPi](https://img.shields.io/pypi/v/libretro.py)](https://pypi.org/project/libretro.py)
 [![License](https://img.shields.io/github/license/JesseTG/libretro.py)](LICENSE)
 
 </div>
 
 # Supported Environments
 
 libretro.py has the following requirements:
@@ -65,28 +65,23 @@
 To install additional features,
 add one or more of the following extras to the `install` command:
 
 - **`dev`:** Assorted tools used to help develop libretro.py.
   Required if contributing to libretro.py.
 - **`opengl`:** Support for the built-in OpenGL video driver.
   Required if testing a core's OpenGL support.
-- **`pillow`:** Support for the built-in software-only video driver
-  powered by the [Pillow][pillow] image processing library.
-  Not required for any particular feature,
-  but it simplifies tests that inspect the core's video output.
 
-For example, if you want to submit an improvement to the Pillow video driver,
+For example, if you want to submit an improvement to the OpenGL video driver,
 you would install libretro.py like so:
 
 ```bash
-pip install libretro.py[pillow,dev]
+pip install libretro.py[opengl,dev]
 ```
 
 And if you just want to test your libretro core's OpenGL support:
 
 ```bash
 pip install libretro.py[opengl]
 ```
 
 [just]: https://just.systems
 [libretro]: https://www.libretro.com
-[pillow]: https://python-pillow.org
```

### Comparing `libretro_py-0.0.0/pyproject.toml` & `libretro_py-0.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -36,37 +36,35 @@
 ]
 
 [project.optional-dependencies]
 build = [
     'build == 1.2.1',
     'setuptools>=69.1.1',
     'twine == 5.0.0',
+    'pre-commit == 3.7.*',
 ]
 dev = [
     'bandit == 1.7.*',
-    'black == 23.*',
+    'black == 24.*',
     'flake8 == 6.*',
     'isort == 5.*',
     'mypy == 1.5.*',
     "libretro.py[build]"
 ]
 docs = [
     'Sphinx == 7.*',
     'sphinx-autobuild == 2024.*',
     'furo',
 ]
 doc = ["libretro.py[docs]"] # Alias for the docs extra
 opengl = [
     'moderngl == 5.10.*',
+    'PyOpenGL == 3.1.*',
 ]
-pillow = [
-    'pillow == 10.2.*',
-    'types-Pillow',
-]
-all = ["libretro.py[build,dev,docs,opengl,pillow]"]
+all = ["libretro.py[build,dev,docs,opengl]"]
 
 [project.urls]
 Homepage = "https://github.com/JesseTG/libretro.py"
 Issues = "https://github.com/JesseTG/libretro.py/issues"
 Repository = "https://github.com/JesseTG/libretro.py"
 Changelog = "https://github.com/JesseTG/libretro.py/blob/master/CHANGELOG.md"
```

### Comparing `libretro_py-0.0.0/setup.py` & `libretro_py-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/_utils.py` & `libretro_py-0.0.1/src/libretro/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,9 +380,8 @@
     """
     return ord(value) if (isinstance(value, bytes) or isinstance(value, str)) else value
 
 
 @runtime_checkable
 class Pollable(Protocol):
     @abstractmethod
-    def poll(self) -> None:
-        ...
+    def poll(self) -> None: ...
```

### Comparing `libretro_py-0.0.0/src/libretro/api/__init__.py` & `libretro_py-0.0.1/src/libretro/api/__init__.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/_utils.py` & `libretro_py-0.0.1/src/libretro/api/_utils.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/audio.py` & `libretro_py-0.0.1/src/libretro/api/audio.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 retro_audio_sample_t = CFUNCTYPE(None, c_int16, c_int16)
 retro_audio_sample_batch_t = CFUNCTYPE(c_size_t, POINTER(c_int16), c_size_t)
 retro_audio_callback_t = CFUNCTYPE(None)
 retro_audio_set_state_callback_t = CFUNCTYPE(None, c_bool)
 retro_audio_buffer_status_callback_t = CFUNCTYPE(None, c_bool, c_uint, c_bool)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_audio_callback(Structure, metaclass=FieldsFromTypeHints):
     callback: retro_audio_callback_t
     set_state: retro_audio_set_state_callback_t
 
     def __deepcopy__(self, _):
         return retro_audio_callback(callback=self.callback, set_state=self.set_state)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_audio_buffer_status_callback(Structure, metaclass=FieldsFromTypeHints):
     callback: retro_audio_buffer_status_callback_t
 
     def __call__(self, active: bool, occupancy: int, underrun_likely: bool) -> None:
         if self.callback:
             self.callback(active, occupancy, underrun_likely)
```

### Comparing `libretro_py-0.0.0/src/libretro/api/av.py` & `libretro_py-0.0.1/src/libretro/api/av.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     AUDIO = RETRO_AV_ENABLE_AUDIO
     FAST_SAVESTATES = RETRO_AV_ENABLE_FAST_SAVESTATES
     HARD_DISABLE_AUDIO = RETRO_AV_ENABLE_HARD_DISABLE_AUDIO
 
     ALL = VIDEO | AUDIO | FAST_SAVESTATES | HARD_DISABLE_AUDIO
 
 
-@dataclass
+@dataclass(init=False)
 class retro_game_geometry(Structure, metaclass=FieldsFromTypeHints):
     base_width: c_uint
     base_height: c_uint
     max_width: c_uint
     max_height: c_uint
     aspect_ratio: c_float
 
@@ -45,25 +45,33 @@
             base_width=self.base_width,
             base_height=self.base_height,
             max_width=self.max_width,
             max_height=self.max_height,
             aspect_ratio=self.aspect_ratio,
         )
 
+    @property
+    def base_size(self) -> tuple[int, int]:
+        return self.base_width, self.base_height
 
-@dataclass
+    @property
+    def max_size(self) -> tuple[int, int]:
+        return self.max_width, self.max_height
+
+
+@dataclass(init=False)
 class retro_system_timing(Structure, metaclass=FieldsFromTypeHints):
     fps: c_double
     sample_rate: c_double
 
     def __deepcopy__(self, _):
         return retro_system_timing(self.fps, self.sample_rate)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_system_av_info(Structure, metaclass=FieldsFromTypeHints):
     geometry: retro_game_geometry
     timing: retro_system_timing
 
     def __deepcopy__(self, _):
         return retro_system_av_info(self.geometry, self.timing)
```

### Comparing `libretro_py-0.0.0/src/libretro/api/camera.py` & `libretro_py-0.0.1/src/libretro/api/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class CameraCapabilityFlags(IntFlag):
     OPENGL_TEXTURE = 1 << CameraCapabilities.OPENGL_TEXTURE
     RAW_FRAMEBUFFER = 1 << CameraCapabilities.RAW_FRAMEBUFFER
 
 
-@dataclass
+@dataclass(init=False)
 class retro_camera_callback(Structure, metaclass=FieldsFromTypeHints):
     caps: c_uint64
     width: c_uint
     height: c_uint
     start: retro_camera_start_t
     stop: retro_camera_stop_t
     frame_raw_framebuffer: retro_camera_frame_raw_framebuffer_t
```

### Comparing `libretro_py-0.0.0/src/libretro/api/content.py` & `libretro_py-0.0.1/src/libretro/api/content.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     as_bytes,
     deepcopy_array,
     deepcopy_buffer,
     mmap_file,
 )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_system_info(Structure, metaclass=FieldsFromTypeHints):
     library_name: c_char_p
     library_version: c_char_p
     valid_extensions: c_char_p
     need_fullpath: c_bool
     block_extract: c_bool
 
@@ -47,15 +47,15 @@
 
     @property
     def extensions(self) -> Iterator[bytes]:
         if self.valid_extensions:
             yield from self.valid_extensions.split(b"|")
 
 
-@dataclass
+@dataclass(init=False)
 class retro_game_info(Structure, metaclass=FieldsFromTypeHints):
     path: c_char_p
     data: c_void_p
     size: c_size_t
     meta: c_char_p
 
     def __deepcopy__(self, _):
@@ -73,43 +73,41 @@
 
 
 class SubsystemContent(NamedTuple):
     game_type: int | str | bytes
     info: Sequence[Content]
 
 
-@dataclass
+@dataclass(init=False)
 class retro_subsystem_memory_info(Structure, metaclass=FieldsFromTypeHints):
     extension: c_char_p
     type: c_uint
 
     def __deepcopy__(self, _):
         return retro_subsystem_memory_info(self.extension, self.type)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_subsystem_rom_info(Structure, metaclass=FieldsFromTypeHints):
     desc: c_char_p
     valid_extensions: c_char_p
     need_fullpath: c_bool
     block_extract: c_bool
     required: c_bool
     memory: POINTER(retro_subsystem_memory_info)
     num_memory: c_uint
 
     def __len__(self):
         return int(self.num_memory)
 
     @overload
-    def __getitem__(self, index: int) -> retro_subsystem_memory_info:
-        ...
+    def __getitem__(self, index: int) -> retro_subsystem_memory_info: ...
 
     @overload
-    def __getitem__(self, index: slice) -> Sequence[retro_subsystem_memory_info]:
-        ...
+    def __getitem__(self, index: slice) -> Sequence[retro_subsystem_memory_info]: ...
 
     def __getitem__(self, index):
         if not self.memory:
             raise ValueError("No subsystem ROM memory types available")
 
         match index:
             case int(i):
@@ -137,32 +135,30 @@
 
     @property
     def extensions(self) -> Iterator[bytes]:
         if self.valid_extensions:
             yield from self.valid_extensions.split(b"|")
 
 
-@dataclass
+@dataclass(init=False)
 class retro_subsystem_info(Structure, metaclass=FieldsFromTypeHints):
     desc: c_char_p
     ident: c_char_p
     roms: POINTER(retro_subsystem_rom_info)
     num_roms: c_uint
     id: c_uint
 
     def __len__(self):
         return int(self.num_roms)
 
     @overload
-    def __getitem__(self, index: int) -> retro_subsystem_rom_info:
-        ...
+    def __getitem__(self, index: int) -> retro_subsystem_rom_info: ...
 
     @overload
-    def __getitem__(self, index: slice) -> Sequence[retro_subsystem_rom_info]:
-        ...
+    def __getitem__(self, index: slice) -> Sequence[retro_subsystem_rom_info]: ...
 
     def __getitem__(self, index):
         if not self.roms:
             raise ValueError("No subsystem ROM types available")
 
         match index:
             case int(i):
@@ -249,15 +245,15 @@
     def __iter__(self):
         return iter(self._subsystems)
 
     def __len__(self):
         return len(self._subsystems)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_system_content_info_override(Structure, metaclass=FieldsFromTypeHints):
     extensions: c_char_p
     need_fullpath: c_bool
     persistent_data: c_bool
 
     def __deepcopy__(self, _):
         return retro_system_content_info_override(
@@ -340,15 +336,15 @@
         return len(self._overrides)
 
     @property
     def by_extension(self) -> Mapping[bytes, retro_system_content_info_override]:
         return self._overrides_by_ext
 
 
-@dataclass
+@dataclass(init=False)
 class retro_game_info_ext(Structure, metaclass=FieldsFromTypeHints):
     full_path: c_char_p
     archive_path: c_char_p
     archive_file: c_char_p
     dir: c_char_p
     name: c_char_p
     ext: c_char_p
```

### Comparing `libretro_py-0.0.0/src/libretro/api/disk.py` & `libretro_py-0.0.1/src/libretro/api/disk.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 retro_replace_image_index_t = CFUNCTYPE(c_bool, c_uint, POINTER(retro_game_info))
 retro_add_image_index_t = CFUNCTYPE(c_bool)
 retro_set_initial_image_t = CFUNCTYPE(c_bool, c_uint, c_char_p)
 retro_get_image_path_t = CFUNCTYPE(c_bool, c_uint, c_char_p, c_size_t)
 retro_get_image_label_t = CFUNCTYPE(c_bool, c_uint, c_char_p, c_size_t)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_disk_control_callback(Structure, metaclass=FieldsFromTypeHints):
     set_eject_state: retro_set_eject_state_t
     get_eject_state: retro_get_eject_state_t
     get_image_index: retro_get_image_index_t
     set_image_index: retro_set_image_index_t
     get_num_images: retro_get_num_images_t
     replace_image_index: retro_replace_image_index_t
@@ -34,15 +34,15 @@
             set_image_index=self.set_image_index,
             get_num_images=self.get_num_images,
             replace_image_index=self.replace_image_index,
             add_image_index=self.add_image_index,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_disk_control_ext_callback(retro_disk_control_callback, metaclass=FieldsFromTypeHints):
     set_initial_image: retro_set_initial_image_t
     get_image_path: retro_get_image_path_t
     get_image_label: retro_get_image_label_t
 
     def __deepcopy__(self, _):
         return retro_disk_control_ext_callback(
```

### Comparing `libretro_py-0.0.0/src/libretro/api/environment.py` & `libretro_py-0.0.1/src/libretro/api/environment.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/input/analog.py` & `libretro_py-0.0.1/src/libretro/api/input/analog.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
     def left_y(self) -> int:
         return self.lstick[1]
 
     @property
     def right_x(self) -> int:
         return self.rstick[0]
 
+    @property
+    def right_y(self) -> int:
+        return self.rstick[1]
+
     def __getitem__(self, item) -> int:
         match item:
             case DeviceIdJoypad.B:
                 return self.b
             case DeviceIdJoypad.Y:
                 return self.y
             case DeviceIdJoypad.SELECT:
```

### Comparing `libretro_py-0.0.0/src/libretro/api/input/device.py` & `libretro_py-0.0.1/src/libretro/api/input/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self._type_ = "H"
 
     @property
     def flag(self) -> InputDeviceFlag:
         return InputDeviceFlag(1 << self.value)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_input_descriptor(Structure, metaclass=FieldsFromTypeHints):
     port: c_uint
     device: c_uint
     index: c_uint
     id: c_uint
     description: c_char_p
 
@@ -70,41 +70,39 @@
             device=self.device,
             index=self.index,
             id=self.id,
             description=self.description,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_controller_description(Structure, metaclass=FieldsFromTypeHints):
     desc: c_char_p
     id: c_uint
 
     def __deepcopy__(self, _):
         return retro_controller_description(self.desc, self.id)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_controller_info(Structure, metaclass=FieldsFromTypeHints):
     types: POINTER(retro_controller_description)
     num_types: c_uint
 
     def __deepcopy__(self, memo):
         return retro_controller_info(
             types=(deepcopy_array(self.types, self.num_types, memo) if self.types else None),
             num_types=self.num_types,
         )
 
     @overload
-    def __getitem__(self, index: int) -> retro_controller_description:
-        ...
+    def __getitem__(self, index: int) -> retro_controller_description: ...
 
     @overload
-    def __getitem__(self, index: slice) -> Sequence[retro_controller_description]:
-        ...
+    def __getitem__(self, index: slice) -> Sequence[retro_controller_description]: ...
 
     def __getitem__(self, index):
         if not self.types:
             raise ValueError("No controller types available")
 
         match index:
             case int(i):
```

### Comparing `libretro_py-0.0.0/src/libretro/api/input/joypad.py` & `libretro_py-0.0.1/src/libretro/api/input/joypad.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/input/keyboard.py` & `libretro_py-0.0.1/src/libretro/api/input/keyboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
         else:
             return False
 
 
 retro_keyboard_event_t = CFUNCTYPE(None, c_bool, c_uint, c_uint32, c_uint16)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_keyboard_callback(Structure, metaclass=FieldsFromTypeHints):
     callback: retro_keyboard_event_t
 
     def __deepcopy__(self, _):
         return retro_keyboard_callback(callback=self.callback)
 
     def __call__(
```

### Comparing `libretro_py-0.0.0/src/libretro/api/input/lightgun.py` & `libretro_py-0.0.1/src/libretro/api/input/lightgun.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/input/mouse.py` & `libretro_py-0.0.1/src/libretro/api/input/mouse.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/input/pointer.py` & `libretro_py-0.0.1/src/libretro/api/input/pointer.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/location.py` & `libretro_py-0.0.1/src/libretro/api/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 retro_location_set_interval_t = CFUNCTYPE(None, c_uint, c_uint)
 retro_location_start_t = CFUNCTYPE(c_bool)
 retro_location_stop_t = CFUNCTYPE(None)
 retro_location_get_position_t = CFUNCTYPE(c_bool, c_double_p, c_double_p, c_double_p, c_double_p)
 retro_location_lifetime_status_t = CFUNCTYPE(None)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_location_callback(Structure, metaclass=FieldsFromTypeHints):
     start: retro_location_start_t
     stop: retro_location_stop_t
     get_position: retro_location_get_position_t
     set_interval: retro_location_set_interval_t
     initialized: retro_location_lifetime_status_t
     deinitialized: retro_location_lifetime_status_t
```

### Comparing `libretro_py-0.0.0/src/libretro/api/log.py` & `libretro_py-0.0.1/src/libretro/api/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 return logging.INFO
             case self.WARNING:
                 return logging.WARN
             case self.ERROR:
                 return logging.ERROR
 
 
-@dataclass
+@dataclass(init=False)
 class retro_log_callback(Structure, metaclass=FieldsFromTypeHints):
     log: retro_log_printf_t
 
     def __call__(self, level: LogLevel, message: bytes) -> None:
         if self.log:
             self.log(level, message)
```

### Comparing `libretro_py-0.0.0/src/libretro/api/memory.py` & `libretro_py-0.0.1/src/libretro/api/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ALIGN_4 = RETRO_MEMDESC_ALIGN_4
     ALIGN_8 = RETRO_MEMDESC_ALIGN_8
     MINSIZE_2 = RETRO_MEMDESC_MINSIZE_2
     MINSIZE_4 = RETRO_MEMDESC_MINSIZE_4
     MINSIZE_8 = RETRO_MEMDESC_MINSIZE_8
 
 
-@dataclass
+@dataclass(init=False)
 class retro_memory_descriptor(Structure, metaclass=FieldsFromTypeHints):
     flags: c_uint64
     ptr: c_void_p
     offset: c_size_t
     start: c_size_t
     select: c_size_t
     disconnect: c_size_t
@@ -54,15 +54,15 @@
             addrspace=self.addrspace,
         )
 
     # TODO: Implement __getitem__, __setitem__
     # TODO: Implement a buffer property (not __buffer__ because Structure provides that)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_memory_map(Structure, metaclass=FieldsFromTypeHints):
     descriptors: POINTER(retro_memory_descriptor)
     num_descriptors: c_uint
 
     def __len__(self):
         return self.num_descriptors
```

### Comparing `libretro_py-0.0.0/src/libretro/api/message.py` & `libretro_py-0.0.1/src/libretro/api/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
     STATUS = RETRO_MESSAGE_TYPE_STATUS
     PROGRESS = RETRO_MESSAGE_TYPE_PROGRESS
 
     def __init__(self, value: int):
         self._type_ = "I"
 
 
-@dataclass
+@dataclass(init=False)
 class retro_message(Structure, metaclass=FieldsFromTypeHints):
     msg: c_char_p
     frames: c_uint
 
     def __deepcopy__(self, memodict):
         return retro_message(msg=self.msg, frames=self.frames)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_message_ext(Structure, metaclass=FieldsFromTypeHints):
     msg: c_char_p
     duration: c_uint
     priority: c_uint
     level: retro_log_level
     target: retro_message_target
     type: retro_message_type
```

### Comparing `libretro_py-0.0.0/src/libretro/api/microphone.py` & `libretro_py-0.0.1/src/libretro/api/microphone.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 # This one has no fields, it doesn't need the weight of a metaclass
 class retro_microphone(Structure):
     pass
 
 
-@dataclass
+@dataclass(init=False)
 class retro_microphone_params(Structure, metaclass=FieldsFromTypeHints):
     rate: c_uint
 
     def __deepcopy__(self, _):
         return retro_microphone_params(self.rate)
 
 
@@ -37,15 +37,15 @@
     c_bool, POINTER(retro_microphone), POINTER(retro_microphone_params)
 )
 retro_set_mic_state_t = CFUNCTYPE(c_bool, POINTER(retro_microphone), c_bool)
 retro_get_mic_state_t = CFUNCTYPE(c_bool, POINTER(retro_microphone))
 retro_read_mic_t = CFUNCTYPE(c_int, POINTER(retro_microphone), POINTER(c_int16), c_size_t)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_microphone_interface(Structure, metaclass=FieldsFromTypeHints):
     interface_version: c_uint
     open_mic: retro_open_mic_t
     close_mic: retro_close_mic_t
     get_params: retro_get_mic_params_t
     set_mic_state: retro_set_mic_state_t
     get_mic_state: retro_get_mic_state_t
```

### Comparing `libretro_py-0.0.0/src/libretro/api/midi.py` & `libretro_py-0.0.1/src/libretro/api/midi.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 retro_midi_input_enabled_t = CFUNCTYPE(c_bool)
 retro_midi_output_enabled_t = CFUNCTYPE(c_bool)
 retro_midi_read_t = CFUNCTYPE(c_bool, POINTER(c_uint8))
 retro_midi_write_t = CFUNCTYPE(c_bool, c_uint8, c_uint32)
 retro_midi_flush_t = CFUNCTYPE(c_bool)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_midi_interface(Structure, metaclass=FieldsFromTypeHints):
     input_enabled: retro_midi_input_enabled_t
     output_enabled: retro_midi_output_enabled_t
     read: retro_midi_read_t
     write: retro_midi_write_t
     flush: retro_midi_flush_t
```

### Comparing `libretro_py-0.0.0/src/libretro/api/netpacket.py` & `libretro_py-0.0.1/src/libretro/api/netpacket.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     UNSEQUENCED = RETRO_NETPACKET_UNSEQUENCED
     FLUSH_HINT = RETRO_NETPACKET_FLUSH_HINT
 
 
 BROADCAST = RETRO_NETPACKET_BROADCAST
 
 
-@dataclass
+@dataclass(init=False)
 class retro_netpacket_callback(Structure, metaclass=FieldsFromTypeHints):
     start: retro_netpacket_start_t
     receive: retro_netpacket_receive_t
     stop: retro_netpacket_stop_t
     poll: retro_netpacket_poll_t
     connected: retro_netpacket_connected_t
     disconnected: retro_netpacket_disconnected_t
```

### Comparing `libretro_py-0.0.0/src/libretro/api/options.py` & `libretro_py-0.0.1/src/libretro/api/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,46 +5,46 @@
 from libretro.api._utils import FieldsFromTypeHints, deepcopy_array
 
 RETRO_NUM_CORE_OPTION_VALUES_MAX = 128
 
 retro_core_options_update_display_callback_t = CFUNCTYPE(c_bool)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_variable(Structure, metaclass=FieldsFromTypeHints):
     key: c_char_p
     value: c_char_p
 
     def __deepcopy__(self, _):
         return retro_variable(self.key, self.value)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_option_display(Structure, metaclass=FieldsFromTypeHints):
     key: c_char_p
     visible: c_bool
 
     def __deepcopy__(self, _):
         return retro_core_option_display(self.key, self.visible)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_option_value(Structure, metaclass=FieldsFromTypeHints):
     value: c_char_p
     label: c_char_p
 
     def __deepcopy__(self, _):
         return retro_core_option_value(self.value, self.label)
 
 
 NUM_CORE_OPTION_VALUES_MAX = RETRO_NUM_CORE_OPTION_VALUES_MAX
 CoreOptionArray: type[Array] = retro_core_option_value * RETRO_NUM_CORE_OPTION_VALUES_MAX
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_option_definition(Structure, metaclass=FieldsFromTypeHints):
     key: c_char_p
     desc: c_char_p
     info: c_char_p
     values: CoreOptionArray
     default_value: c_char_p
 
@@ -54,37 +54,37 @@
             self.desc,
             self.info,
             deepcopy_array(self.values, NUM_CORE_OPTION_VALUES_MAX, memo),
             self.default_value,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_options_intl(Structure, metaclass=FieldsFromTypeHints):
     us: POINTER(retro_core_option_definition)
     local: POINTER(retro_core_option_definition)
 
     def __deepcopy__(self, memo):
         return retro_core_options_intl(
             pointer(deepcopy(self.us[0], memo)) if self.us else None,
             pointer(deepcopy(self.local[0], memo)) if self.local else None,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_option_v2_category(Structure, metaclass=FieldsFromTypeHints):
     key: c_char_p
     desc: c_char_p
     info: c_char_p
 
     def __deepcopy__(self, _):
         return retro_core_option_v2_category(self.key, self.desc, self.info)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_option_v2_definition(Structure, metaclass=FieldsFromTypeHints):
     key: c_char_p
     desc: c_char_p
     desc_categorized: c_char_p
     info: c_char_p
     info_categorized: c_char_p
     category_key: c_char_p
@@ -100,39 +100,39 @@
             self.info_categorized,
             self.category_key,
             deepcopy_array(self.values, NUM_CORE_OPTION_VALUES_MAX, memo),
             self.default_value,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_options_v2(Structure, metaclass=FieldsFromTypeHints):
     categories: POINTER(retro_core_option_v2_category)
     definitions: POINTER(retro_core_option_v2_definition)
 
     def __deepcopy__(self, memo):
         return retro_core_options_v2(
             pointer(deepcopy(self.categories[0], memo)) if self.categories else None,
             pointer(deepcopy(self.definitions[0], memo)) if self.definitions else None,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_options_v2_intl(Structure, metaclass=FieldsFromTypeHints):
     us: POINTER(retro_core_options_v2)
     local: POINTER(retro_core_options_v2)
 
     def __deepcopy__(self, memo):
         return retro_core_options_v2_intl(
             pointer(deepcopy(self.us[0], memo)) if self.us else None,
             pointer(deepcopy(self.local[0], memo)) if self.local else None,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_core_options_update_display_callback(Structure, metaclass=FieldsFromTypeHints):
     callback: retro_core_options_update_display_callback_t
 
     def __call__(self) -> bool:
         if not self.callback:
             raise ValueError("No callback has been set")
```

### Comparing `libretro_py-0.0.0/src/libretro/api/perf.py` & `libretro_py-0.0.1/src/libretro/api/perf.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     VFPV4 = RETRO_SIMD_VFPV4
     POPCNT = RETRO_SIMD_POPCNT
     MOVBE = RETRO_SIMD_MOVBE
     CMOV = RETRO_SIMD_CMOV
     ASIMD = RETRO_SIMD_ASIMD
 
 
-@dataclass
+@dataclass(init=False)
 class retro_perf_counter(Structure, metaclass=FieldsFromTypeHints):
     ident: c_char_p
     start: retro_perf_tick_t
     total: retro_perf_tick_t
     call_cnt: retro_perf_tick_t
     registered: c_bool
 
@@ -80,15 +80,15 @@
 retro_get_cpu_features_t = CFUNCTYPE(c_uint64)
 retro_perf_log_t = CFUNCTYPE(None)
 retro_perf_register_t = CFUNCTYPE(None, POINTER(retro_perf_counter))
 retro_perf_start_t = CFUNCTYPE(None, POINTER(retro_perf_counter))
 retro_perf_stop_t = CFUNCTYPE(None, POINTER(retro_perf_counter))
 
 
-@dataclass
+@dataclass(init=False)
 class retro_perf_callback(Structure, metaclass=FieldsFromTypeHints):
     get_time_usec: retro_perf_get_time_usec_t
     get_cpu_features: retro_get_cpu_features_t
     get_perf_counter: retro_perf_get_counter_t
     perf_register: retro_perf_register_t
     perf_start: retro_perf_start_t
     perf_stop: retro_perf_stop_t
```

### Comparing `libretro_py-0.0.0/src/libretro/api/power.py` & `libretro_py-0.0.1/src/libretro/api/power.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     CHARGED = RETRO_POWERSTATE_CHARGED
     PLUGGED_IN = RETRO_POWERSTATE_PLUGGED_IN
 
     def __init__(self, value: int):
         self._type_ = "I"
 
 
-@dataclass
+@dataclass(init=False)
 class retro_device_power(Structure, metaclass=FieldsFromTypeHints):
     state: retro_power_state
     seconds: c_int
     percent: c_int8
 
     def __deepcopy__(self, _):
         return retro_device_power(state=self.state, seconds=self.seconds, percent=self.percent)
```

### Comparing `libretro_py-0.0.0/src/libretro/api/proc.py` & `libretro_py-0.0.1/src/libretro/api/proc.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from libretro.api._utils import UNCHECKED, FieldsFromTypeHints
 
 retro_proc_address_t = CFUNCTYPE(None)
 retro_get_proc_address_t = CFUNCTYPE(UNCHECKED(retro_proc_address_t), c_char_p)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_get_proc_address_interface(Structure, metaclass=FieldsFromTypeHints):
     get_proc_address: retro_get_proc_address_t
 
     def __call__(self, sym: AnyStr) -> retro_proc_address_t:
         if not self.get_proc_address:
             raise ValueError("get_proc_address is NULL")
```

### Comparing `libretro_py-0.0.0/src/libretro/api/rumble.py` & `libretro_py-0.0.1/src/libretro/api/rumble.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class RumbleEffect(IntEnum):
     STRONG = RETRO_RUMBLE_STRONG
     WEAK = RETRO_RUMBLE_WEAK
 
 
-@dataclass
+@dataclass(init=False)
 class retro_rumble_interface(Structure, metaclass=FieldsFromTypeHints):
     set_rumble_state: retro_set_rumble_state_t
 
     def __deepcopy__(self, _):
         return retro_rumble_interface(self.set_rumble_state)
```

### Comparing `libretro_py-0.0.0/src/libretro/api/savestate.py` & `libretro_py-0.0.1/src/libretro/api/savestate.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/sensor.py` & `libretro_py-0.0.1/src/libretro/api/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RETRO_SENSOR_GYROSCOPE_Z = 5
 RETRO_SENSOR_ILLUMINANCE = 6
 
 retro_set_sensor_state_t = CFUNCTYPE(c_bool, c_uint, retro_sensor_action, c_uint)
 retro_sensor_get_input_t = CFUNCTYPE(c_float, c_uint, c_uint)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_sensor_interface(Structure, metaclass=FieldsFromTypeHints):
     set_sensor_state: retro_set_sensor_state_t
     get_sensor_input: retro_sensor_get_input_t
 
     def __deepcopy__(self, _):
         return retro_sensor_interface(self.set_sensor_state, self.get_sensor_input)
 
@@ -93,15 +93,15 @@
 
     def __init__(self, value):
         self._type_ = "i"
 
     @property
     def type(self) -> SensorType:
         match self:
-            case (Sensor.ACCELEROMETER_X | Sensor.ACCELEROMETER_Y | Sensor.ACCELEROMETER_Z):
+            case Sensor.ACCELEROMETER_X | Sensor.ACCELEROMETER_Y | Sensor.ACCELEROMETER_Z:
                 return SensorType.ACCELEROMETER
             case Sensor.GYROSCOPE_X | Sensor.GYROSCOPE_Y | Sensor.GYROSCOPE_Z:
                 return SensorType.GYROSCOPE
             case Sensor.ILLUMINANCE:
                 return SensorType.ILLUMINANCE
             case _:
                 raise ValueError(f"Invalid sensor: {self}")
```

### Comparing `libretro_py-0.0.0/src/libretro/api/timing.py` & `libretro_py-0.0.1/src/libretro/api/timing.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 RETRO_THROTTLE_UNBLOCKED = 6
 
 
 retro_usec_t = c_int64
 retro_frame_time_callback_t = CFUNCTYPE(None, retro_usec_t)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_frame_time_callback(Structure, metaclass=FieldsFromTypeHints):
     callback: retro_frame_time_callback_t
     reference: retro_usec_t
 
     def __call__(self, time: int | None = None):
         if not isinstance(time, int) and time is not None:
             raise TypeError(f"time must be an int or None, not {type(time).__name__}")
@@ -45,28 +45,28 @@
     VSYNC = RETRO_THROTTLE_VSYNC
     UNBLOCKED = RETRO_THROTTLE_UNBLOCKED
 
     def __init__(self, value: int):
         self._type_ = "I"
 
 
-@dataclass
+@dataclass(init=False)
 class retro_fastforwarding_override(Structure, metaclass=FieldsFromTypeHints):
     ratio: c_float
     fastforward: c_bool
     notification: c_bool
     inhibit_toggle: c_bool
 
     def __deepcopy__(self, _):
         return retro_fastforwarding_override(
             self.ratio, self.fastforward, self.notification, self.inhibit_toggle
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_throttle_state(Structure, metaclass=FieldsFromTypeHints):
     mode: c_uint
     rate: c_float
 
     def __deepcopy__(self, _):
         return retro_throttle_state(self.mode, self.rate)
```

### Comparing `libretro_py-0.0.0/src/libretro/api/user.py` & `libretro_py-0.0.1/src/libretro/api/user.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/vfs.py` & `libretro_py-0.0.1/src/libretro/api/vfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 retro_vfs_opendir_t = CFUNCTYPE(c_void_p, c_char_p, c_bool)
 retro_vfs_readdir_t = CFUNCTYPE(c_bool, POINTER(retro_vfs_dir_handle))
 retro_vfs_dirent_get_name_t = CFUNCTYPE(c_char_p, POINTER(retro_vfs_dir_handle))
 retro_vfs_dirent_is_dir_t = CFUNCTYPE(c_bool, POINTER(retro_vfs_dir_handle))
 retro_vfs_closedir_t = CFUNCTYPE(c_int, POINTER(retro_vfs_dir_handle))
 
 
-@dataclass
+@dataclass(init=False)
 class retro_vfs_interface(Structure, metaclass=FieldsFromTypeHints):
     get_path: retro_vfs_get_path_t
     open: retro_vfs_open_t
     close: retro_vfs_close_t
     size: retro_vfs_size_t
     tell: retro_vfs_tell_t
     seek: retro_vfs_seek_t
@@ -134,15 +134,15 @@
             self.readdir,
             self.dirent_get_name,
             self.dirent_is_dir,
             self.closedir,
         )
 
 
-@dataclass
+@dataclass(init=False)
 class retro_vfs_interface_info(Structure, metaclass=FieldsFromTypeHints):
     required_interface_version: c_uint32
     iface: POINTER(retro_vfs_interface)
 
     def __deepcopy__(self, memo):
         return retro_vfs_interface_info(
             self.required_interface_version,
```

### Comparing `libretro_py-0.0.0/src/libretro/api/video/context.py` & `libretro_py-0.0.1/src/libretro/api/video/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 retro_hw_context_reset_t = CFUNCTYPE(None)
 retro_hw_get_current_framebuffer_t = CFUNCTYPE(c_uintptr)
 retro_hw_get_proc_address_t = CFUNCTYPE(UNCHECKED(retro_proc_address_t), c_char_p)
 
 
-@dataclass
+@dataclass(init=False)
 class retro_hw_render_callback(Structure, metaclass=FieldsFromTypeHints):
     context_type: retro_hw_context_type
     context_reset: retro_hw_context_reset_t
     get_current_framebuffer: retro_hw_get_current_framebuffer_t
     get_proc_address: retro_hw_get_proc_address_t
     depth: c_bool
     stencil: c_bool
```

### Comparing `libretro_py-0.0.0/src/libretro/api/video/frame.py` & `libretro_py-0.0.1/src/libretro/api/video/frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 
 class MemoryType(IntFlag):
     NONE = 0
     CACHED = RETRO_MEMORY_TYPE_CACHED
 
 
-@dataclass
+@dataclass(init=False)
 class retro_framebuffer(Structure, metaclass=FieldsFromTypeHints):
     data: c_void_p
     width: c_uint
     height: c_uint
     pitch: c_size_t
     format: retro_pixel_format
     access_flags: c_uint
```

### Comparing `libretro_py-0.0.0/src/libretro/api/video/negotiate.py` & `libretro_py-0.0.1/src/libretro/api/video/negotiate.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/api/video/render.py` & `libretro_py-0.0.1/src/libretro/api/video/render.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/builder.py` & `libretro_py-0.0.1/src/libretro/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     HardwareContext,
     PowerState,
     SavestateContext,
     SubsystemContent,
     ThrottleMode,
     retro_device_power,
     retro_game_info,
+    retro_hw_render_callback,
     retro_throttle_state,
 )
 from libretro.core import Core
 from libretro.drivers import (
     ArrayAudioDriver,
     ArrayVideoDriver,
     AudioDriver,
@@ -45,27 +46,34 @@
     LocationDriver,
     LocationInputGenerator,
     LogDriver,
     LoggerMessageInterface,
     MessageInterface,
     MicrophoneDriver,
     MidiDriver,
+    MultiVideoDriver,
     OptionDriver,
     PathDriver,
     PerfDriver,
     PowerDriver,
     StandardContentDriver,
     StandardFileSystemInterface,
     TimingDriver,
     UnformattedLogDriver,
     UserDriver,
     VideoDriver,
+    VideoDriverInitArgs,
 )
 from libretro.session import Session
 
+try:
+    from libretro.drivers.video import ModernGlVideoDriver
+except ImportError:
+    ModernGlVideoDriver = None
+
 type _RequiredFactory[T] = Callable[[], T]
 type _OptionalFactory[T] = Callable[[], T | None]
 
 type _RequiredArg[T] = T | _RequiredFactory[T]
 type _OptionalArg[T] = T | _OptionalFactory[T] | Default | None
 
 
@@ -292,34 +300,61 @@
                         case err:
                             raise TypeError(
                                 f"Expected a generator, an iterable, an iterator, or an InputDriver from the callable, got {type(err).__name__}"
                             )
 
                 self._args["input"] = _generate
             case _DefaultType.DEFAULT:
-                self._args[
-                    "input"
-                ] = GeneratorInputDriver  # TODO: Set the rumble and sensor interfaces
+                self._args["input"] = (
+                    GeneratorInputDriver  # TODO: Set the rumble and sensor interfaces
+                )
             case None:
                 raise ValueError("An input driver is required")
             case _:
                 raise TypeError(
                     f"Expected InputDriver or a callable that returns one, a callable or iterator that yields InputState, or DEFAULT; got {type(input).__name__}"
                 )
 
         return self
 
     def with_video(self, video: VideoDriverArg) -> Self:
+        """
+        Sets the video driver for this session.
+
+        The default video driver is a ``MultiVideoDriver`` that supports the following contexts:
+
+        - ``HardwareContext.NONE``: An ``ArrayVideoDriver``.
+        - ``HardwareContext.OPENGL``: A ``ModernGlVideoDriver`` if the ``moderngl`` package is installed,
+          absent if not.
+
+        :param video: One of the following:
+
+            - A ``VideoDriver`` that will be used as-is.
+            - A ``Callable`` that returns a ``VideoDriver``.
+            - A :class:`Callable` that returns a :class:`VideoDriver`.
+            - :py:const:`DEFAULT` to use the default video driver.
+            - :py:const:`None` to raise an error.
+        :return: This builder object.
+        """
+
         match video:
             case Callable() as func:
                 self._args["video"] = func
             case VideoDriver():
                 self._args["video"] = lambda: video
             case _DefaultType.DEFAULT:
-                self._args["video"] = ArrayVideoDriver
+                drivers: dict[HardwareContext, Callable[[], VideoDriver]] = dict()
+                drivers[HardwareContext.NONE] = ArrayVideoDriver
+
+                if ModernGlVideoDriver:
+                    # If moderngl is installed...
+                    drivers[HardwareContext.OPENGL] = ModernGlVideoDriver
+                    drivers[HardwareContext.OPENGL_CORE] = ModernGlVideoDriver
+
+                self._args["video"] = lambda: MultiVideoDriver(drivers)
             case None:
                 raise ValueError("A video driver is required")
             case _:
                 raise TypeError(
                     f"Expected a VideoDriver, a callable that returns one, or DEFAULT; got {type(video).__name__}"
                 )
```

### Comparing `libretro_py-0.0.0/src/libretro/core.py` & `libretro_py-0.0.1/src/libretro/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod
-from collections.abc import Buffer, Sequence
+from collections.abc import Buffer, Callable, Sequence
 from copy import deepcopy
 from ctypes import (
     CDLL,
     POINTER,
     Array,
     byref,
     c_bool,
@@ -40,112 +40,87 @@
 
 class CoreInterface(Protocol):
     """
     An interface for a libretro core.
     """
 
     @abstractmethod
-    def set_environment(self, env: retro_environment_t) -> None:
-        ...
+    def set_environment(self, env: retro_environment_t) -> None: ...
 
     @abstractmethod
-    def set_video_refresh(self, video: retro_video_refresh_t) -> None:
-        ...
+    def set_video_refresh(self, video: retro_video_refresh_t) -> None: ...
 
     @abstractmethod
-    def set_audio_sample(self, audio: retro_audio_sample_t) -> None:
-        ...
+    def set_audio_sample(self, audio: retro_audio_sample_t) -> None: ...
 
     @abstractmethod
-    def set_audio_sample_batch(self, audio: retro_audio_sample_batch_t) -> None:
-        ...
+    def set_audio_sample_batch(self, audio: retro_audio_sample_batch_t) -> None: ...
 
     @abstractmethod
-    def set_input_poll(self, poll: retro_input_poll_t) -> None:
-        ...
+    def set_input_poll(self, poll: retro_input_poll_t) -> None: ...
 
     @abstractmethod
-    def set_input_state(self, state: retro_input_state_t) -> None:
-        ...
+    def set_input_state(self, state: retro_input_state_t) -> None: ...
 
     @abstractmethod
-    def init(self) -> None:
-        ...
+    def init(self) -> None: ...
 
     @abstractmethod
-    def deinit(self) -> None:
-        ...
+    def deinit(self) -> None: ...
 
     @abstractmethod
-    def api_version(self) -> int:
-        ...
+    def api_version(self) -> int: ...
 
     @abstractmethod
-    def get_system_info(self) -> retro_system_info:
-        ...
+    def get_system_info(self) -> retro_system_info: ...
 
     @abstractmethod
-    def get_system_av_info(self) -> retro_system_av_info:
-        ...
+    def get_system_av_info(self) -> retro_system_av_info: ...
 
     @abstractmethod
-    def set_controller_port_device(self, port: int, device: int) -> None:
-        ...
+    def set_controller_port_device(self, port: int, device: int) -> None: ...
 
     @abstractmethod
-    def reset(self) -> None:
-        ...
+    def reset(self) -> None: ...
 
     @abstractmethod
-    def run(self) -> None:
-        ...
+    def run(self) -> None: ...
 
     @abstractmethod
-    def serialize_size(self) -> int:
-        ...
+    def serialize_size(self) -> int: ...
 
     @abstractmethod
-    def serialize(self, data: bytearray | memoryview) -> bool:
-        ...
+    def serialize(self, data: bytearray | memoryview) -> bool: ...
 
     @abstractmethod
-    def unserialize(self, data: bytes | bytearray | memoryview) -> bool:
-        ...
+    def unserialize(self, data: bytes | bytearray | memoryview) -> bool: ...
 
     @abstractmethod
-    def cheat_reset(self) -> None:
-        ...
+    def cheat_reset(self) -> None: ...
 
     @abstractmethod
-    def cheat_set(self, index: int, enabled: bool, code: bytes | bytearray | memoryview) -> None:
-        ...
+    def cheat_set(self, index: int, enabled: bool, code: bytes | bytearray | str) -> None: ...
 
     @abstractmethod
-    def load_game(self, game: retro_game_info | None) -> bool:
-        ...
+    def load_game(self, game: retro_game_info | None) -> bool: ...
 
     @abstractmethod
-    def load_game_special(self, game_type: int, info: Sequence[retro_game_info]) -> bool:
-        ...
+    def load_game_special(self, game_type: int, info: Sequence[retro_game_info]) -> bool: ...
 
     @abstractmethod
-    def unload_game(self) -> None:
-        ...
+    def unload_game(self) -> None: ...
 
     @abstractmethod
-    def get_region(self) -> Region:
-        ...
+    def get_region(self) -> Region: ...
 
     @abstractmethod
-    def get_memory_data(self, id: int) -> c_void_p | None:
-        ...
+    def get_memory_data(self, id: int) -> c_void_p | None: ...
 
     @abstractmethod
-    def get_memory_size(self, id: int) -> int:
-        ...
+    def get_memory_size(self, id: int) -> int: ...
 
     def get_memory(self, id: int) -> memoryview | None:
         """
         Convenience method that returns a writable ``memoryview``
         of the memory region given by ``id``.
 
         :param id: The ID of the memory region to access.
@@ -293,83 +268,119 @@
     def set_environment(self, env: retro_environment_t) -> None:
         """
         Calls the core's ``retro_set_environment`` function with the given callback.
 
         :param env: The function that the core should use for environment calls.
         :raises TypeError: If ``env`` is not a ``retro_environment_t``.
         """
-        if not isinstance(env, retro_environment_t):
-            raise TypeError(f"Expected a retro_environment_t, got {type(env).__name__}")
+        match env:
+            case retro_environment_t():
+                self._environment = env
+            case Callable():
+                self._environment = retro_environment_t(env)
+            case _:
+                raise TypeError(
+                    f"Expected a retro_environment_t or an equivalent callable, got {type(env).__name__}"
+                )
 
-        self._environment = retro_environment_t(env)
         self._core.retro_set_environment(self._environment)
 
     def set_video_refresh(self, video: retro_video_refresh_t) -> None:
         """
         Calls the core's ``retro_set_video_refresh`` function with the given callback.
 
         :param video: The function that the core should call to update its video output.
         :raises TypeError: If ``video`` is not a ``retro_video_refresh_t``.
         """
-        if not isinstance(video, retro_video_refresh_t):
-            raise TypeError(f"Expected a retro_video_refresh_t, got {type(video).__name__}")
+        match video:
+            case retro_video_refresh_t():
+                self._video_refresh = video
+            case Callable():
+                self._video_refresh = retro_video_refresh_t(video)
+            case _:
+                raise TypeError(
+                    f"Expected a retro_video_refresh_t or an equivalent callable, got {type(video).__name__}"
+                )
 
-        self._video_refresh = retro_video_refresh_t(video)
         self._core.retro_set_video_refresh(self._video_refresh)
 
     def set_audio_sample(self, audio: retro_audio_sample_t) -> None:
         """
         Calls the core's ``retro_set_audio_sample`` function with the given callback.
 
         :param audio: The function that the core should call to render a single audio frame.
         :raises TypeError: If ``audio`` is not a ``retro_audio_sample_t``.
         """
-        if not isinstance(audio, retro_audio_sample_t):
-            raise TypeError(f"Expected a retro_audio_sample_t, got {type(audio).__name__}")
+        match audio:
+            case retro_audio_sample_t():
+                self._audio_sample = audio
+            case Callable():
+                self._audio_sample = retro_audio_sample_t(audio)
+            case _:
+                raise TypeError(
+                    f"Expected a retro_audio_sample_t or an equivalent callable, got {type(audio).__name__}"
+                )
 
-        self._audio_sample = retro_audio_sample_t(audio)
         self._core.retro_set_audio_sample(self._audio_sample)
 
     def set_audio_sample_batch(self, audio: retro_audio_sample_batch_t) -> None:
         """
         Calls the core's ``retro_set_audio_sample_batch`` function with the given callback.
 
         :param audio: The function that the core should call to render a batch of audio frames.
         :raises TypeError: If ``audio`` is not a ``retro_audio_sample_batch_t``.
         """
-        if not isinstance(audio, retro_audio_sample_batch_t):
-            raise TypeError(f"Expected a retro_audio_sample_batch_t, got {type(audio).__name__}")
+        match audio:
+            case retro_audio_sample_batch_t():
+                self._audio_sample_batch = audio
+            case Callable():
+                self._audio_sample_batch = retro_audio_sample_batch_t(audio)
+            case _:
+                raise TypeError(
+                    f"Expected a retro_audio_sample_batch_t or an equivalent callable, got {type(audio).__name__}"
+                )
 
-        self._audio_sample_batch = retro_audio_sample_batch_t(audio)
         self._core.retro_set_audio_sample_batch(self._audio_sample_batch)
 
     def set_input_poll(self, poll: retro_input_poll_t) -> None:
         """
         Calls the core's ``retro_set_input_poll`` function with the given callback.
 
         :param poll: The function that the core should call to poll for updated input state.
         :raises TypeError: If ``poll`` is not a ``retro_input_poll_t``.
         """
-        if not isinstance(poll, retro_input_poll_t):
-            raise TypeError(f"Expected a retro_input_poll_t, got {type(poll).__name__}")
+        match poll:
+            case retro_input_poll_t():
+                self._input_poll = poll
+            case Callable():
+                self._input_poll = retro_input_poll_t(poll)
+            case _:
+                raise TypeError(
+                    f"Expected a retro_input_poll_t or an equivalent callable, got {type(poll).__name__}"
+                )
 
-        self._input_poll = retro_input_poll_t(poll)
         self._core.retro_set_input_poll(self._input_poll)
 
     def set_input_state(self, state: retro_input_state_t) -> None:
         """
         Calls the core's ``retro_set_input_state`` function with the given callback.
 
         :param state: The function that the core should call to request part of the input state.
         :raises TypeError: If ``state`` is not a ``retro_input_state_t``.
         """
-        if not isinstance(state, retro_input_state_t):
-            raise TypeError(f"Expected a retro_input_state_t, got {type(state).__name__}")
+        match state:
+            case retro_input_state_t():
+                self._input_state = state
+            case Callable():
+                self._input_state = retro_input_state_t(state)
+            case _:
+                raise TypeError(
+                    f"Expected a retro_input_state_t or an equivalent callable, got {type(state).__name__}"
+                )
 
-        self._input_state = retro_input_state_t(state)
         self._core.retro_set_input_state(self._input_state)
 
     def init(self):
         """
         Calls the core's ``retro_init`` function.
 
         :note: This method does not check if the core has already been initialized.
@@ -515,15 +526,15 @@
 
     def cheat_reset(self):
         """
         Calls the core's ``retro_cheat_reset`` function.
         """
         self._core.retro_cheat_reset()
 
-    def cheat_set(self, index: int, enabled: bool, code: bytes | bytearray | memoryview | Buffer):
+    def cheat_set(self, index: int, enabled: bool, code: bytes | bytearray | str):
         """
         Calls the core's ``retro_cheat_set`` function with the given arguments.
 
         :param index: The number of the cheat code to toggle.
         :param enabled: Whether the cheat code should be enabled or disabled.
         :param code: A buffer containing a zero-terminated byte string.
         :raise TypeError: If any parameter's value is inconsistent with its documented type.
@@ -531,27 +542,24 @@
         """
         if not isinstance(index, int):
             raise TypeError(f"Expected int, got {type(index).__name__}")
 
         if not isinstance(enabled, bool):
             raise TypeError(f"Expected bool, got {type(enabled).__name__}")
 
-        buf: memoryview
+        buf: bytes
         match code:
-            case bytes() | bytearray() | Buffer():
-                buf = memoryview(code)
-            case memoryview():
+            case bytes():
                 buf = code
+            case bytearray():
+                buf = bytes(code)
+            case str():
+                buf = code.encode()
             case _:
-                raise TypeError(
-                    f"Expected bytes, bytearray, memoryview, or Buffer; got {type(code).__name__}"
-                )
-
-        if 0 not in buf:
-            raise ValueError("code must contain a zero-terminated byte string")
+                raise TypeError(f"Expected bytes, bytearray, or str; got {type(code).__name__}")
 
         self._core.retro_cheat_set(index, enabled, buf)
 
     def load_game(self, game: retro_game_info | None) -> bool:
         """
         Calls the core's ``retro_load_game`` function with the given game info.
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/__init__.py` & `libretro_py-0.0.1/src/libretro/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/audio/array.py` & `libretro_py-0.0.1/src/libretro/drivers/audio/array.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/audio/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/audio/driver.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,73 +7,63 @@
     retro_system_av_info,
 )
 
 
 @runtime_checkable
 class AudioDriver(Protocol):
     @abstractmethod
-    def sample(self, left: int, right: int) -> None:
-        ...
+    def sample(self, left: int, right: int) -> None: ...
 
     @abstractmethod
-    def sample_batch(self, frames: memoryview) -> int:
-        ...
+    def sample_batch(self, frames: memoryview) -> int: ...
 
     @property
     @abstractmethod
-    def callbacks(self) -> retro_audio_callback | None:
-        ...
+    def callbacks(self) -> retro_audio_callback | None: ...
 
     @callbacks.setter
     @abstractmethod
-    def callbacks(self, callback: retro_audio_callback | None) -> None:
-        ...
+    def callbacks(self, callback: retro_audio_callback | None) -> None: ...
 
     def set_state(self, enabled: bool) -> None:
         callbacks = self.callbacks
         if callbacks and callbacks.callback:
             callbacks.callback(enabled)
 
     def callback(self) -> None:
         callbacks = self.callbacks
         if callbacks and callbacks.callback:
             callbacks.callback()
 
     @property
     @abstractmethod
-    def buffer_status(self) -> retro_audio_buffer_status_callback | None:
-        ...
+    def buffer_status(self) -> retro_audio_buffer_status_callback | None: ...
 
     @buffer_status.setter
     @abstractmethod
-    def buffer_status(self, callback: retro_audio_buffer_status_callback) -> None:
-        ...
+    def buffer_status(self, callback: retro_audio_buffer_status_callback) -> None: ...
 
     def report_buffer_status(self, active: bool, occupancy: int, underrun_likely: bool) -> None:
         callback = self.buffer_status
         if callback:
             callback(active, occupancy, underrun_likely)
 
     @property
     @abstractmethod
-    def minimum_latency(self) -> int | None:
-        ...
+    def minimum_latency(self) -> int | None: ...
 
     @minimum_latency.setter
     @abstractmethod
-    def minimum_latency(self, latency: int | None) -> None:
-        ...
+    def minimum_latency(self, latency: int | None) -> None: ...
 
     @property
     @abstractmethod
-    def system_av_info(self) -> retro_system_av_info | None:
-        ...
+    def system_av_info(self) -> retro_system_av_info | None: ...
 
     @system_av_info.setter
     @abstractmethod
-    def system_av_info(self, info: retro_system_av_info) -> None:
-        ...
+    def system_av_info(self, info: retro_system_av_info) -> None: ...
 
 
 __all__ = [
     "AudioDriver",
 ]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/audio/wave.py` & `libretro_py-0.0.1/src/libretro/drivers/audio/wave.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/camera/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/camera/driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,89 +18,72 @@
     def __init__(self):
         self._as_parameter_: retro_camera_callback = retro_camera_callback()
         self._as_parameter_.start = retro_camera_start_t(self.start)
         self._as_parameter_.stop = retro_camera_stop_t(self.stop)
 
     @property
     @abstractmethod
-    def caps(self) -> CameraCapabilityFlags:
-        ...
+    def caps(self) -> CameraCapabilityFlags: ...
 
     @caps.setter
     @abstractmethod
-    def caps(self, value: CameraCapabilityFlags) -> None:
-        ...
+    def caps(self, value: CameraCapabilityFlags) -> None: ...
 
     @abstractmethod
-    def start(self) -> bool:
-        ...
+    def start(self) -> bool: ...
 
     @abstractmethod
-    def stop(self) -> None:
-        ...
+    def stop(self) -> None: ...
 
     @abstractmethod
-    def poll(self) -> None:
-        ...
+    def poll(self) -> None: ...
 
     @property
     @abstractmethod
-    def width(self) -> int:
-        ...
+    def width(self) -> int: ...
 
     @width.setter
     @abstractmethod
-    def width(self, value: int) -> None:
-        ...
+    def width(self, value: int) -> None: ...
 
     @property
     @abstractmethod
-    def height(self) -> int:
-        ...
+    def height(self) -> int: ...
 
     @height.setter
     @abstractmethod
-    def height(self, value: int) -> None:
-        ...
+    def height(self, value: int) -> None: ...
 
     @property
     @abstractmethod
-    def frame_raw_framebuffer(self) -> retro_camera_frame_raw_framebuffer_t | None:
-        ...
+    def frame_raw_framebuffer(self) -> retro_camera_frame_raw_framebuffer_t | None: ...
 
     @frame_raw_framebuffer.setter
     @abstractmethod
-    def frame_raw_framebuffer(self, value: retro_camera_frame_raw_framebuffer_t) -> None:
-        ...
+    def frame_raw_framebuffer(self, value: retro_camera_frame_raw_framebuffer_t) -> None: ...
 
     @property
     @abstractmethod
-    def frame_opengl_texture(self) -> retro_camera_frame_opengl_texture_t | None:
-        ...
+    def frame_opengl_texture(self) -> retro_camera_frame_opengl_texture_t | None: ...
 
     @frame_opengl_texture.setter
     @abstractmethod
-    def frame_opengl_texture(self, value: retro_camera_frame_opengl_texture_t) -> None:
-        ...
+    def frame_opengl_texture(self, value: retro_camera_frame_opengl_texture_t) -> None: ...
 
     @property
     @abstractmethod
-    def initialized(self) -> retro_camera_lifetime_status_t | None:
-        ...
+    def initialized(self) -> retro_camera_lifetime_status_t | None: ...
 
     @initialized.setter
     @abstractmethod
-    def initialized(self, value: retro_camera_lifetime_status_t) -> None:
-        ...
+    def initialized(self, value: retro_camera_lifetime_status_t) -> None: ...
 
     @property
     @abstractmethod
-    def deinitialized(self) -> retro_camera_lifetime_status_t | None:
-        ...
+    def deinitialized(self) -> retro_camera_lifetime_status_t | None: ...
 
     @deinitialized.setter
     @abstractmethod
-    def deinitialized(self, value: retro_camera_lifetime_status_t) -> None:
-        ...
+    def deinitialized(self, value: retro_camera_lifetime_status_t) -> None: ...
 
 
 __all__ = ["CameraDriver"]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/camera/generator.py` & `libretro_py-0.0.1/src/libretro/drivers/camera/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/content/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/content/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,61 +91,51 @@
             All files not marked as persistent will be closed when the context manager exits.
             The ones that are persistent will be closed when the driver is destroyed.
         """
         ...
 
     @property
     @abstractmethod
-    def enable_extended_info(self) -> bool:
-        ...
+    def enable_extended_info(self) -> bool: ...
 
     @property
     @abstractmethod
-    def game_info_ext(self) -> Array[retro_game_info_ext] | None:
-        ...
+    def game_info_ext(self) -> Array[retro_game_info_ext] | None: ...
 
     @property
     @abstractmethod
-    def system_info(self) -> retro_system_info | None:
-        ...
+    def system_info(self) -> retro_system_info | None: ...
 
     @system_info.setter
     @abstractmethod
-    def system_info(self, info: retro_system_info) -> None:
-        ...
+    def system_info(self, info: retro_system_info) -> None: ...
 
     @property
     @abstractmethod
-    def overrides(self) -> Sequence[retro_system_content_info_override] | None:
-        ...
+    def overrides(self) -> Sequence[retro_system_content_info_override] | None: ...
 
     @overrides.setter
     @abstractmethod
-    def overrides(self, overrides: Sequence[retro_system_content_info_override]) -> None:
-        ...
+    def overrides(self, overrides: Sequence[retro_system_content_info_override]) -> None: ...
 
     @property
     @abstractmethod
-    def subsystem_info(self) -> Subsystems | None:
-        ...
+    def subsystem_info(self) -> Subsystems | None: ...
 
     @subsystem_info.setter
     @abstractmethod
-    def subsystem_info(self, subsystems: Sequence[retro_subsystem_info]) -> None:
-        ...
+    def subsystem_info(self, subsystems: Sequence[retro_subsystem_info]) -> None: ...
 
     @property
     @abstractmethod
-    def support_no_game(self) -> bool | None:
-        ...
+    def support_no_game(self) -> bool | None: ...
 
     @support_no_game.setter
     @abstractmethod
-    def support_no_game(self, support: bool) -> None:
-        ...
+    def support_no_game(self, support: bool) -> None: ...
 
 
 __all__ = [
     "ContentDriver",
     "ContentAttributes",
     "LoadedContentFile",
     "LoadedContent",
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/content/standard.py` & `libretro_py-0.0.1/src/libretro/drivers/content/standard.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/disk/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/disk/driver.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,43 +7,37 @@
 )
 
 
 @runtime_checkable
 class DiskDriver(Protocol):
     @property
     @abstractmethod
-    def version(self) -> int:
-        ...
+    def version(self) -> int: ...
 
     @property
     @abstractmethod
     def callback(
         self,
-    ) -> retro_disk_control_callback | retro_disk_control_ext_callback | None:
-        ...
+    ) -> retro_disk_control_callback | retro_disk_control_ext_callback | None: ...
 
     @callback.setter
     @abstractmethod
     def callback(
         self, value: retro_disk_control_callback | retro_disk_control_ext_callback
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @callback.deleter
     @abstractmethod
-    def callback(self) -> None:
-        ...
+    def callback(self) -> None: ...
 
     @property
     @abstractmethod
-    def eject_state(self) -> bool:
-        ...
+    def eject_state(self) -> bool: ...
 
     @eject_state.setter
     @abstractmethod
-    def eject_state(self, value: bool) -> None:
-        ...
+    def eject_state(self, value: bool) -> None: ...
 
 
 __all__ = [
     "DiskDriver",
 ]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/environment/composite.py` & `libretro_py-0.0.1/src/libretro/drivers/environment/composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     c_bool,
     c_char_p,
     c_float,
     c_int16,
     c_uint,
     c_uint64,
     c_void_p,
-    cast,
     memmove,
     pointer,
     sizeof,
     string_at,
 )
 from typing import AnyStr, Required, TypedDict, override
 
@@ -104,15 +103,15 @@
 from libretro.drivers.options import OptionDriver
 from libretro.drivers.path import PathDriver
 from libretro.drivers.perf import PerfDriver
 from libretro.drivers.power import PowerDriver
 from libretro.drivers.timing import TimingDriver
 from libretro.drivers.user import UserDriver
 from libretro.drivers.vfs import FileSystemInterface
-from libretro.drivers.video import VideoDriver
+from libretro.drivers.video import FrameBufferSpecial, VideoDriver
 
 from .default import DefaultEnvironmentDriver
 
 # TODO: Match envcalls even if the experimental flag is unset (but still consider it for ABI differences)
 
 
 class CompositeEnvironmentDriver(DefaultEnvironmentDriver):
@@ -314,22 +313,30 @@
 
     @property
     def timing(self) -> TimingDriver | None:
         return self._timing
 
     @override
     def video_refresh(self, data: c_void_p, width: int, height: int, pitch: int) -> None:
-        if data:
-            view = memoryview_at(data, pitch * height, readonly=True)
-            assert (
-                len(view) == pitch * height
-            ), f"Expected view to have {pitch * height} bytes, got {len(view)} bytes"
-            self._video.refresh(view, width, height, pitch)
-        else:
-            self._video.refresh(None, width, height, pitch)
+        # Handle the constants and their equivalent ints, just to be safe
+        match data:
+            case FrameBufferSpecial.DUPE | 0 | None:
+                self._video.refresh(FrameBufferSpecial.DUPE, width, height, pitch)
+            case FrameBufferSpecial.HARDWARE | -1 | 18446744073709551615:
+                self._video.refresh(FrameBufferSpecial.HARDWARE, width, height, pitch)
+            case int() | c_void_p():
+                view = memoryview_at(data, pitch * height, readonly=True)
+                assert (
+                    len(view) == pitch * height
+                ), f"Expected view to have {pitch * height} bytes, got {len(view)} bytes"
+                self._video.refresh(view, width, height, pitch)
+            case _:
+                raise TypeError(
+                    f"Expected FrameBufferSpecial, int, or c_void_p, got {type(data).__name__}"
+                )
 
     @override
     def audio_sample(self, left: int, right: int) -> None:
         self._audio.sample(left, right)
 
     @override
     def audio_sample_batch(self, data: POINTER(c_int16), frames: int) -> int:
@@ -495,17 +502,16 @@
             raise ValueError("RETRO_ENVIRONMENT_SET_HW_RENDER doesn't accept NULL")
 
         context = self._video.set_context(hw_render_ptr[0])
         if context is None:
             return False
 
         hw_render_ptr[0] = context
+        # Give the core the callbacks that the video driver defines
 
-        # TODO: Call the provided context_reset at the start of the next frame, not immediately
-        # TODO: Save the context
         return True
 
     @property
     def options(self) -> OptionDriver | None:
         return self._options
 
     @override
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/environment/default.py` & `libretro_py-0.0.1/src/libretro/drivers/environment/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/environment/dict.py` & `libretro_py-0.0.1/src/libretro/drivers/environment/dict.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/environment/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/environment/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,36 +62,30 @@
 )
 
 
 # noinspection PyMethodMayBeStatic,PyUnusedLocal,PyShadowingNames
 @runtime_checkable
 class EnvironmentDriver(Protocol):
     @abstractmethod
-    def environment(self, cmd: int, data: c_void_p) -> bool:
-        ...
+    def environment(self, cmd: int, data: c_void_p) -> bool: ...
 
     @abstractmethod
-    def video_refresh(self, data: c_void_p, width: int, height: int, pitch: int) -> None:
-        ...
+    def video_refresh(self, data: c_void_p, width: int, height: int, pitch: int) -> None: ...
 
     @abstractmethod
-    def audio_sample(self, left: int, right: int) -> None:
-        ...
+    def audio_sample(self, left: int, right: int) -> None: ...
 
     @abstractmethod
-    def audio_sample_batch(self, data: POINTER(c_int16), frames: int) -> int:
-        ...
+    def audio_sample_batch(self, data: POINTER(c_int16), frames: int) -> int: ...
 
     @abstractmethod
-    def input_poll(self) -> None:
-        ...
+    def input_poll(self) -> None: ...
 
     @abstractmethod
-    def input_state(self, port: int, device: int, index: int, id: int) -> int:
-        ...
+    def input_state(self, port: int, device: int, index: int, id: int) -> int: ...
 
     def _set_rotation(self, rotation: POINTER(c_uint)) -> bool:
         return False
 
     def _get_overscan(self, overscan: POINTER(c_bool)) -> bool:
         return False
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/input/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/input/driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,108 +15,89 @@
 from libretro.drivers.rumble import RumbleInterface
 from libretro.drivers.sensor import SensorInterface
 
 
 @runtime_checkable
 class InputDriver(Protocol):
     @abstractmethod
-    def poll(self) -> None:
-        ...
+    def poll(self) -> None: ...
 
     @abstractmethod
-    def state(self, port: Port, device: InputDevice, index: int, _id: int) -> int:
-        ...
+    def state(self, port: Port, device: InputDevice, index: int, _id: int) -> int: ...
 
     @property
     @abstractmethod
-    def descriptors(self) -> Sequence[retro_input_descriptor] | None:
-        ...
+    def descriptors(self) -> Sequence[retro_input_descriptor] | None: ...
 
     @descriptors.setter
     @abstractmethod
-    def descriptors(self, descriptors: Sequence[retro_input_descriptor]) -> None:
-        ...
+    def descriptors(self, descriptors: Sequence[retro_input_descriptor]) -> None: ...
 
     @property
     @abstractmethod
-    def keyboard_callback(self) -> retro_keyboard_callback | None:
-        ...
+    def keyboard_callback(self) -> retro_keyboard_callback | None: ...
 
     @keyboard_callback.setter
     @abstractmethod
-    def keyboard_callback(self, callback: retro_keyboard_callback) -> None:
-        ...
+    def keyboard_callback(self, callback: retro_keyboard_callback) -> None: ...
 
     def keyboard_event(
         self, down: bool, keycode: Key, character: int, modifiers: KeyModifier
     ) -> None:
         callback = self.keyboard_callback
         if callback:
             callback.callback(down, keycode, character, modifiers)
 
     @property
     @abstractmethod
-    def rumble(self) -> RumbleInterface | None:
-        ...
+    def rumble(self) -> RumbleInterface | None: ...
 
     @property
     @abstractmethod
-    def sensor(self) -> SensorInterface | None:
-        ...
+    def sensor(self) -> SensorInterface | None: ...
 
     @property
     @abstractmethod
-    def device_capabilities(self) -> InputDeviceFlag | None:
-        ...
+    def device_capabilities(self) -> InputDeviceFlag | None: ...
 
     @device_capabilities.setter
     @abstractmethod
-    def device_capabilities(self, capabilities: InputDeviceFlag) -> None:
-        ...
+    def device_capabilities(self, capabilities: InputDeviceFlag) -> None: ...
 
     @device_capabilities.deleter
     @abstractmethod
-    def device_capabilities(self) -> None:
-        ...
+    def device_capabilities(self) -> None: ...
 
     @property
     @abstractmethod
-    def controller_info(self) -> Sequence[retro_controller_info] | None:
-        ...
+    def controller_info(self) -> Sequence[retro_controller_info] | None: ...
 
     @controller_info.setter
     @abstractmethod
-    def controller_info(self, info: Sequence[retro_controller_info]) -> None:
-        ...
+    def controller_info(self, info: Sequence[retro_controller_info]) -> None: ...
 
     @property
     @abstractmethod
-    def bitmasks_supported(self) -> bool | None:
-        ...
+    def bitmasks_supported(self) -> bool | None: ...
 
     @bitmasks_supported.setter
     @abstractmethod
-    def bitmasks_supported(self, bitmask_supported: bool) -> None:
-        ...
+    def bitmasks_supported(self, bitmask_supported: bool) -> None: ...
 
     @bitmasks_supported.deleter
     @abstractmethod
-    def bitmasks_supported(self) -> None:
-        ...
+    def bitmasks_supported(self) -> None: ...
 
     @property
     @abstractmethod
-    def max_users(self) -> int | None:
-        ...
+    def max_users(self) -> int | None: ...
 
     @max_users.setter
     @abstractmethod
-    def max_users(self, max_users: int) -> None:
-        ...
+    def max_users(self, max_users: int) -> None: ...
 
     @max_users.deleter
     @abstractmethod
-    def max_users(self) -> None:
-        ...
+    def max_users(self) -> None: ...
 
 
 __all__ = ["InputDriver"]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/input/generator.py` & `libretro_py-0.0.1/src/libretro/drivers/input/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Callable, Generator, Iterable, Iterator, Sequence
 from dataclasses import dataclass
-from enum import IntEnum
+from enum import Enum, auto
 from typing import override
 
 from libretro._utils import Pollable
 from libretro.api.input import (
     AnalogState,
     DeviceIdAnalog,
     DeviceIdJoypad,
@@ -37,19 +37,19 @@
     x: int = 0
     y: int = 0
 
 
 DeviceState = JoypadState | MouseState | KeyboardState | LightGunState | AnalogState | PointerState
 
 
-class Direction(IntEnum):
-    RIGHT = (0,)
-    UP = (1,)
-    LEFT = (2,)
-    DOWN = (3,)
+class Direction(Enum):
+    RIGHT = auto()
+    UP = auto()
+    LEFT = auto()
+    DOWN = auto()
 
     def matches_direction(self, other: DeviceIdJoypad | Key | DeviceIdLightgun) -> bool:
         match (self, other):
             case (
                 Direction.RIGHT,
                 DeviceIdJoypad.RIGHT | Key.RIGHT | DeviceIdLightgun.DPAD_RIGHT,
             ):
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/led/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/led/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,20 @@
         self._as_parameter_ = retro_led_interface()
         self._as_parameter_.set_led_state = retro_set_led_state_t(self.__set_led_state)
 
     def __set_led_state(self, led: int, state: int) -> None:
         self.set_led_state(led, state)
 
     @abstractmethod
-    def set_led_state(self, led: int, state: int) -> None:
-        ...
+    def set_led_state(self, led: int, state: int) -> None: ...
 
     def __setitem__(self, key: int, value: int):
         self.set_led_state(int(key), int(value))
 
     @abstractmethod
-    def get_led_state(self, led: int) -> int:
-        ...
+    def get_led_state(self, led: int) -> int: ...
 
     def __getitem__(self, key: int) -> int:
         return self.get_led_state(int(key))
 
 
 __all__ = ["LedDriver"]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/location/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/location/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,24 @@
         self._as_parameter_ = retro_location_callback()
         self._as_parameter_.start = retro_location_start_t(self.start)
         self._as_parameter_.stop = retro_location_stop_t(self.stop)
         self._as_parameter_.get_position = retro_location_get_position_t(self.__get_position)
         self._as_parameter_.set_interval = retro_location_set_interval_t(self.set_interval)
 
     @abstractmethod
-    def start(self) -> bool:
-        ...
+    def start(self) -> bool: ...
 
     @abstractmethod
-    def stop(self) -> None:
-        ...
+    def stop(self) -> None: ...
 
     @abstractmethod
-    def get_position(self) -> Position | None:
-        ...
+    def get_position(self) -> Position | None: ...
 
     @abstractmethod
-    def set_interval(self, interval: int, distance: int) -> None:
-        ...
+    def set_interval(self, interval: int, distance: int) -> None: ...
 
     @property
     def initialized(self) -> retro_location_lifetime_status_t:
         return self._as_parameter_.initialized
 
     @initialized.setter
     def initialized(self, value: retro_location_lifetime_status_t) -> None:
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/location/generator.py` & `libretro_py-0.0.1/src/libretro/drivers/location/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/log/unformatted.py` & `libretro_py-0.0.1/src/libretro/drivers/log/unformatted.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/message/logger.py` & `libretro_py-0.0.1/src/libretro/drivers/message/logger.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/microphone/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/microphone/driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,35 +24,30 @@
     def __init__(self, params: retro_microphone_params | None):
         self._as_parameter_ = id(self)
 
     def __del__(self) -> None:
         self.close()
 
     @abstractmethod
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
     @property
     @abstractmethod
-    def params(self) -> retro_microphone_params | None:
-        ...
+    def params(self) -> retro_microphone_params | None: ...
 
     @abstractmethod
-    def read(self, frames: int) -> Sequence[int]:
-        ...
+    def read(self, frames: int) -> Sequence[int]: ...
 
     @property
     @abstractmethod
-    def state(self) -> bool:
-        ...
+    def state(self) -> bool: ...
 
     @state.setter
     @abstractmethod
-    def state(self, value: bool) -> None:
-        ...
+    def state(self, value: bool) -> None: ...
 
 
 @runtime_checkable
 class MicrophoneDriver(Protocol):
     # We want to keep the samples in a queue so that generators
     # don't have to be mindful of yielding the exact right amount of samples
     class __MicHandle(NamedTuple):
@@ -70,20 +65,18 @@
         interface.get_mic_state = retro_get_mic_state_t(self.__get_state)
         interface.read_mic = retro_read_mic_t(self.__read_mic)
         self.__microphones: dict[int, MicrophoneDriver.__MicHandle] = {}
         self._as_parameter_ = interface
 
     @property
     @abstractmethod
-    def version(self) -> int:
-        ...
+    def version(self) -> int: ...
 
     @abstractmethod
-    def open_mic(self, params: retro_microphone_params | None) -> Microphone:
-        ...
+    def open_mic(self, params: retro_microphone_params | None) -> Microphone: ...
 
     def __open_mic(self, params: POINTER(retro_microphone_params)) -> POINTER(retro_microphone):
         mic_params: retro_microphone_params | None = params[0] if params else None
 
         mic = self.open_mic(mic_params)
         if not mic:
             return None
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/microphone/generator.py` & `libretro_py-0.0.1/src/libretro/drivers/microphone/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/midi/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/midi/driver.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,33 +20,28 @@
         self._as_parameter_.output_enabled = retro_midi_output_enabled_t(self.__output_enabled)
         self._as_parameter_.read = retro_midi_read_t(self.__read)
         self._as_parameter_.write = retro_midi_write_t(self.__write)
         self._as_parameter_.flush = retro_midi_flush_t(self.__flush)
 
     @property
     @abstractmethod
-    def input_enabled(self) -> bool:
-        ...
+    def input_enabled(self) -> bool: ...
 
     @property
     @abstractmethod
-    def output_enabled(self) -> bool:
-        ...
+    def output_enabled(self) -> bool: ...
 
     @abstractmethod
-    def read(self) -> int | None:
-        ...
+    def read(self) -> int | None: ...
 
     @abstractmethod
-    def write(self, byte: int, delta_time: int) -> bool:
-        ...
+    def write(self, byte: int, delta_time: int) -> bool: ...
 
     @abstractmethod
-    def flush(self) -> bool:
-        ...
+    def flush(self) -> bool: ...
 
     def __input_enabled(self) -> bool:
         return self.input_enabled
 
     def __output_enabled(self) -> bool:
         return self.output_enabled
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/midi/generator.py` & `libretro_py-0.0.1/src/libretro/drivers/midi/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/netpacket/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/netpacket/driver.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,69 +10,55 @@
 BROADCAST = ClientID(libretro.api.netpacket.BROADCAST)
 
 
 @runtime_checkable
 class NetpacketDriver(Protocol):
     @property
     @abstractmethod
-    def callback(self) -> retro_netpacket_callback | None:
-        ...
+    def callback(self) -> retro_netpacket_callback | None: ...
 
     @callback.setter
     @abstractmethod
-    def callback(self, value: retro_netpacket_callback) -> None:
-        ...
+    def callback(self, value: retro_netpacket_callback) -> None: ...
 
     @callback.deleter
     @abstractmethod
-    def callback(self) -> None:
-        ...
+    def callback(self) -> None: ...
 
     @property
     @abstractmethod
-    def version(self) -> bytes | None:
-        ...
+    def version(self) -> bytes | None: ...
 
     @version.setter
     @abstractmethod
-    def version(self, value: bytes) -> None:
-        ...
+    def version(self, value: bytes) -> None: ...
 
     @version.deleter
     @abstractmethod
-    def version(self) -> None:
-        ...
+    def version(self) -> None: ...
 
     @abstractmethod
-    def start(self, client_id: ClientID) -> None:
-        ...
+    def start(self, client_id: ClientID) -> None: ...
 
     @abstractmethod
-    def receive(self, buf: memoryview, client_id: ClientID) -> None:
-        ...
+    def receive(self, buf: memoryview, client_id: ClientID) -> None: ...
 
     @abstractmethod
-    def stop(self, client_id: ClientID) -> None:
-        ...
+    def stop(self, client_id: ClientID) -> None: ...
 
     @abstractmethod
-    def poll(self) -> None:
-        ...
+    def poll(self) -> None: ...
 
     @abstractmethod
-    def connected(self, client_id: ClientID) -> bool:
-        ...
+    def connected(self, client_id: ClientID) -> bool: ...
 
     @abstractmethod
-    def disconnected(self, client_id: ClientID) -> None:
-        ...
+    def disconnected(self, client_id: ClientID) -> None: ...
 
     @abstractmethod
-    def _send(self, flags: NetpacketFlags, buf: memoryview, client_id: ClientID) -> None:
-        ...
+    def _send(self, flags: NetpacketFlags, buf: memoryview, client_id: ClientID) -> None: ...
 
     @abstractmethod
-    def _poll_receive(self) -> None:
-        ...
+    def _poll_receive(self) -> None: ...
 
 
 __all__ = ["NetpacketDriver"]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/netpacket/socket.py` & `libretro_py-0.0.1/src/libretro/drivers/netpacket/socket.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,41 +14,35 @@
 
     def __del__(self):
         self._socket.close()
         del self._socket
 
     @property
     @override
-    def callback(self) -> retro_netpacket_callback | None:
-        ...
+    def callback(self) -> retro_netpacket_callback | None: ...
 
     @callback.setter
     @override
-    def callback(self, value: retro_netpacket_callback) -> None:
-        ...
+    def callback(self, value: retro_netpacket_callback) -> None: ...
 
     @callback.deleter
     @override
-    def callback(self) -> None:
-        ...
+    def callback(self) -> None: ...
 
     @property
     @override
-    def version(self) -> bytes | None:
-        ...
+    def version(self) -> bytes | None: ...
 
     @version.setter
     @override
-    def version(self, value: bytes) -> None:
-        ...
+    def version(self, value: bytes) -> None: ...
 
     @version.deleter
     @override
-    def version(self) -> None:
-        ...
+    def version(self) -> None: ...
 
     def start(self, client_id: ClientID) -> None:
         pass
 
     def receive(self, buf: memoryview, client_id: ClientID) -> None:
         pass
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/options/dict.py` & `libretro_py-0.0.1/src/libretro/drivers/options/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             {as_bytes(k): as_bytes(v) for k, v in variables.items()} if variables else {}
         )
 
         self._visibility: dict[bytes, bool] = (
             {as_bytes(k): True for k in variables} if variables else {}
         )
 
-        self._update_display_callback: (retro_core_options_update_display_callback | None) = None
+        self._update_display_callback: retro_core_options_update_display_callback | None = None
         self._categories_us: dict[bytes, retro_core_option_v2_category] = {}
         self._options_us: dict[bytes, retro_core_option_v2_definition] = {}
         self._categories_intl: dict[bytes, retro_core_option_v2_category] = {}
         self._options_intl: dict[bytes, retro_core_option_v2_definition] = {}
 
     def get_variable(self, item: bytes) -> bytes | None:
         if not self._options_us or not item:
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/options/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/options/driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,83 +25,69 @@
             Otherwise, return the default value.
 
         :note: Corresponds to ``EnvironmentCall.GET_VARIABLE``.
         """
         ...
 
     @abstractmethod
-    def set_variables(self, variables: Sequence[retro_variable] | None):
-        ...
+    def set_variables(self, variables: Sequence[retro_variable] | None): ...
 
     @property
     @abstractmethod
-    def variable_updated(self) -> bool:
-        ...
+    def variable_updated(self) -> bool: ...
 
     @property
     @abstractmethod
-    def version(self) -> int:
-        ...
+    def version(self) -> int: ...
 
     @abstractmethod
-    def set_options(self, options: Sequence[retro_core_option_definition] | None):
-        ...
+    def set_options(self, options: Sequence[retro_core_option_definition] | None): ...
 
     @abstractmethod
-    def set_options_intl(self, options: retro_core_options_intl | None):
-        ...
+    def set_options_intl(self, options: retro_core_options_intl | None): ...
 
     @abstractmethod
-    def set_display(self, var: bytes, visible: bool):
-        ...
+    def set_display(self, var: bytes, visible: bool): ...
 
     @abstractmethod
-    def set_options_v2(self, options: retro_core_options_v2 | None):
-        ...
+    def set_options_v2(self, options: retro_core_options_v2 | None): ...
 
     @abstractmethod
-    def set_options_v2_intl(self, options: retro_core_options_v2_intl | None):
-        ...
+    def set_options_v2_intl(self, options: retro_core_options_v2_intl | None): ...
 
     @property
     @abstractmethod
-    def update_display_callback(self) -> retro_core_options_update_display_callback:
-        ...
+    def update_display_callback(self) -> retro_core_options_update_display_callback: ...
 
     @update_display_callback.setter
     @abstractmethod
-    def update_display_callback(self, callback: retro_core_options_update_display_callback | None):
-        ...
+    def update_display_callback(
+        self, callback: retro_core_options_update_display_callback | None
+    ): ...
 
     @abstractmethod
-    def set_variable(self, var: bytes, value: bytes) -> bool:
-        ...
+    def set_variable(self, var: bytes, value: bytes) -> bool: ...
 
     @property
     @abstractmethod
-    def supports_categories(self) -> bool:
-        ...
+    def supports_categories(self) -> bool: ...
 
     @property
     @abstractmethod
-    def variables(self) -> MutableMapping[AnyStr, bytes]:
-        ...
+    def variables(self) -> MutableMapping[AnyStr, bytes]: ...
 
     @property
     @abstractmethod
-    def visibility(self) -> Mapping[AnyStr, bool]:
-        ...
+    def visibility(self) -> Mapping[AnyStr, bool]: ...
 
     @property
     @abstractmethod
-    def categories(self) -> Mapping[bytes, retro_core_option_v2_category] | None:
-        ...
+    def categories(self) -> Mapping[bytes, retro_core_option_v2_category] | None: ...
 
     @property
     @abstractmethod
-    def definitions(self) -> Mapping[bytes, retro_core_option_v2_definition] | None:
-        ...
+    def definitions(self) -> Mapping[bytes, retro_core_option_v2_definition] | None: ...
 
 
 __all__ = [
     "OptionDriver",
 ]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/path/default.py` & `libretro_py-0.0.1/src/libretro/drivers/path/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/path/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/path/driver.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,29 +14,25 @@
         """
         Corresponds to ``EnvironmentCall.GET_SYSTEM_DIRECTORY``.
         """
         ...
 
     @property
     @abstractmethod
-    def libretro_path(self) -> bytes | None:
-        ...
+    def libretro_path(self) -> bytes | None: ...
 
     @property
     @abstractmethod
-    def core_assets_dir(self) -> bytes | None:
-        ...
+    def core_assets_dir(self) -> bytes | None: ...
 
     @property
     @abstractmethod
-    def save_dir(self) -> bytes | None:
-        ...
+    def save_dir(self) -> bytes | None: ...
 
     @property
     @abstractmethod
-    def playlist_dir(self) -> bytes | None:
-        ...
+    def playlist_dir(self) -> bytes | None: ...
 
 
 __all__ = [
     "PathDriver",
 ]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/perf/default.py` & `libretro_py-0.0.1/src/libretro/drivers/perf/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/perf/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/perf/driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,40 +26,33 @@
         self._as_parameter_.get_perf_counter = retro_perf_get_counter_t(self.get_perf_counter)
         self._as_parameter_.perf_register = retro_perf_register_t(self.__perf_register)
         self._as_parameter_.perf_start = retro_perf_start_t(self.__perf_start)
         self._as_parameter_.perf_stop = retro_perf_stop_t(self.__perf_stop)
         self._as_parameter_.perf_log = retro_perf_log_t(self.perf_log)
 
     @abstractmethod
-    def get_time_usec(self) -> int:
-        ...
+    def get_time_usec(self) -> int: ...
 
     @abstractmethod
-    def get_cpu_features(self) -> CpuFeatures:
-        ...
+    def get_cpu_features(self) -> CpuFeatures: ...
 
     @abstractmethod
-    def get_perf_counter(self) -> int:
-        ...
+    def get_perf_counter(self) -> int: ...
 
     @abstractmethod
-    def perf_register(self, counter: retro_perf_counter) -> None:
-        ...
+    def perf_register(self, counter: retro_perf_counter) -> None: ...
 
     @abstractmethod
-    def perf_start(self, counter: retro_perf_counter) -> None:
-        ...
+    def perf_start(self, counter: retro_perf_counter) -> None: ...
 
     @abstractmethod
-    def perf_stop(self, counter: retro_perf_counter) -> None:
-        ...
+    def perf_stop(self, counter: retro_perf_counter) -> None: ...
 
     @abstractmethod
-    def perf_log(self) -> None:
-        ...
+    def perf_log(self) -> None: ...
 
     def __perf_register(self, counter: POINTER(retro_perf_counter)) -> None:
         if not counter:
             raise ValueError("counter must not be NULL")
 
         perf_counter = counter[0]
         try:
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/power/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/power/driver.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from libretro.api.power import retro_device_power
 
 
 @runtime_checkable
 class PowerDriver(Protocol):
     @property
     @abstractmethod
-    def device_power(self) -> retro_device_power:
-        ...
+    def device_power(self) -> retro_device_power: ...
 
 
 class ConstantPowerDriver(PowerDriver):
     def __init__(self, device_power: retro_device_power):
         self._device_power: retro_device_power
         self.device_power = device_power
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/rumble/default.py` & `libretro_py-0.0.1/src/libretro/drivers/rumble/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/rumble/interface.py` & `libretro_py-0.0.1/src/libretro/drivers/rumble/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 class RumbleInterface(Protocol):
     @abstractmethod
     def __init__(self):
         self._as_parameter_ = retro_rumble_interface()
         self._as_parameter_.set_rumble_state = retro_set_rumble_state_t(self.__set_rumble_state)
 
     @abstractmethod
-    def _set_rumble_state(self, port: int, effect: RumbleEffect, strength: int) -> bool:
-        ...
+    def _set_rumble_state(self, port: int, effect: RumbleEffect, strength: int) -> bool: ...
 
     def set_rumble_state(self, port: int, effect: RumbleEffect | int, strength: int) -> bool:
         """
         Set the rumble state of a controller port.
 
         Validates the input and calls the implementation of _set_rumble_state.
         """
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/sensor/generator.py` & `libretro_py-0.0.1/src/libretro/drivers/sensor/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,18 @@
 @dataclass(slots=True)
 class PortSensorState:
     accelerometer: SensorState = field(default_factory=SensorState)
     gyroscope: SensorState = field(default_factory=SensorState)
     illuminance: SensorState = field(default_factory=SensorState)
 
     @overload
-    def __getitem__(self, item: SensorType) -> SensorState:
-        ...
+    def __getitem__(self, item: SensorType) -> SensorState: ...
 
     @overload
-    def __getitem__(self, item: SensorAction) -> bool:
-        ...
+    def __getitem__(self, item: SensorAction) -> bool: ...
 
     def __getitem__(self, item: SensorType | SensorAction) -> SensorState | bool:
         match item:
             case SensorType.ACCELEROMETER:
                 return self.accelerometer
             case SensorType.GYROSCOPE:
                 return self.gyroscope
@@ -57,20 +55,18 @@
                 return not self.illuminance.enabled
             case _:
                 raise TypeError(
                     f"Expected a SensorType or SensorAction, got {type(item).__name__}"
                 )
 
     @overload
-    def __setitem__(self, key: SensorType, value: SensorState):
-        ...
+    def __setitem__(self, key: SensorType, value: SensorState): ...
 
     @overload
-    def __setitem__(self, key: SensorAction, value: bool):
-        ...
+    def __setitem__(self, key: SensorAction, value: bool): ...
 
     def __setitem__(self, key: SensorType | SensorAction, value: SensorState | bool):
         match key, value:
             case SensorType.ACCELEROMETER, SensorState(s):
                 self.accelerometer = SensorState(s.enabled, s.rate)
             case SensorType.GYROSCOPE, SensorState(s):
                 self.gyroscope = SensorState(s.enabled, s.rate)
@@ -97,20 +93,18 @@
 @dataclass(slots=True)
 class PortState:
     accelerometer: SensorState = field(default_factory=SensorState)
     gyroscope: SensorState = field(default_factory=SensorState)
     illuminance: SensorState = field(default_factory=SensorState)
 
     @overload
-    def __getitem__(self, item: SensorType) -> SensorState:
-        ...
+    def __getitem__(self, item: SensorType) -> SensorState: ...
 
     @overload
-    def __getitem__(self, item: SensorAction) -> bool:
-        ...
+    def __getitem__(self, item: SensorAction) -> bool: ...
 
     def __getitem__(self, item: SensorType | SensorAction) -> SensorState | bool:
         match item:
             case SensorType.ACCELEROMETER:
                 return self.accelerometer
             case SensorType.GYROSCOPE:
                 return self.gyroscope
@@ -130,20 +124,18 @@
                 return not self.illuminance.enabled
             case _:
                 raise TypeError(
                     f"Expected a SensorType or SensorAction, got {type(item).__name__}"
                 )
 
     @overload
-    def __setitem__(self, key: SensorType, value: SensorState):
-        ...
+    def __setitem__(self, key: SensorType, value: SensorState): ...
 
     @overload
-    def __setitem__(self, key: SensorAction, value: bool):
-        ...
+    def __setitem__(self, key: SensorAction, value: bool): ...
 
     def __setitem__(self, key: SensorType | SensorAction, value: SensorState | bool):
         match key, value:
             case SensorType.ACCELEROMETER, SensorState(s):
                 self.accelerometer = SensorState(s.enabled, s.rate)
             case SensorType.GYROSCOPE, SensorState(s):
                 self.gyroscope = SensorState(s.enabled, s.rate)
@@ -193,32 +185,27 @@
 @dataclass(slots=True)
 class PortInput:
     accelerometer: AccelerometerInput = field(default_factory=AccelerometerInput)
     gyroscope: GyroscopeInput = field(default_factory=GyroscopeInput)
     illuminance: IlluminanceInput = field(default_factory=IlluminanceInput)
 
     @overload
-    def __getitem__(self, item: Sensor) -> float:
-        ...
+    def __getitem__(self, item: Sensor) -> float: ...
 
     @overload
-    def __getitem__(self, item: Literal[SensorType.ACCELEROMETER]) -> AccelerometerInput:
-        ...
+    def __getitem__(self, item: Literal[SensorType.ACCELEROMETER]) -> AccelerometerInput: ...
 
     @overload
-    def __getitem__(self, item: Literal[SensorType.GYROSCOPE]) -> GyroscopeInput:
-        ...
+    def __getitem__(self, item: Literal[SensorType.GYROSCOPE]) -> GyroscopeInput: ...
 
     @overload
-    def __getitem__(self, item: Literal[SensorType.ILLUMINANCE]) -> IlluminanceInput:
-        ...
+    def __getitem__(self, item: Literal[SensorType.ILLUMINANCE]) -> IlluminanceInput: ...
 
     @overload
-    def __getitem__(self, item: SensorType) -> SensorInput:
-        ...
+    def __getitem__(self, item: SensorType) -> SensorInput: ...
 
     def __getitem__(self, item: Sensor | SensorType) -> float | SensorInput:
         match item:
             case Sensor.ACCELEROMETER_X:
                 return self.accelerometer.x
             case Sensor.ACCELEROMETER_Y:
                 return self.accelerometer.y
@@ -238,32 +225,27 @@
                 return self.gyroscope
             case SensorType.ILLUMINANCE:
                 return self.illuminance
             case _:
                 raise TypeError(f"Expected a Sensor or SensorType, got {type(item).__name__}")
 
     @overload
-    def __setitem__(self, key: Sensor, value: float):
-        ...
+    def __setitem__(self, key: Sensor, value: float): ...
 
     @overload
-    def __setitem__(self, key: Literal[SensorType.ACCELEROMETER], value: AccelerometerInput):
-        ...
+    def __setitem__(self, key: Literal[SensorType.ACCELEROMETER], value: AccelerometerInput): ...
 
     @overload
-    def __setitem__(self, key: Literal[SensorType.GYROSCOPE], value: GyroscopeInput):
-        ...
+    def __setitem__(self, key: Literal[SensorType.GYROSCOPE], value: GyroscopeInput): ...
 
     @overload
-    def __setitem__(self, key: Literal[SensorType.ILLUMINANCE], value: IlluminanceInput):
-        ...
+    def __setitem__(self, key: Literal[SensorType.ILLUMINANCE], value: IlluminanceInput): ...
 
     @overload
-    def __setitem__(self, key: SensorType, value: SensorState):
-        ...
+    def __setitem__(self, key: SensorType, value: SensorState): ...
 
     def __setitem__(self, key: Sensor | SensorType, value: float | SensorInput):
         match key, value:
             case Sensor.ACCELEROMETER_X, Real(x):
                 self.accelerometer.x = x
             case Sensor.ACCELEROMETER_Y, Real(y):
                 self.accelerometer.y = y
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/sensor/interface.py` & `libretro_py-0.0.1/src/libretro/drivers/sensor/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 
         if not (0 <= rate < ((2**32) - 1)):
             raise ValueError(f"Expected 0 <= rate < 2**32 - 1, got {rate}")
 
         return bool(self._set_sensor_state(port, SensorAction(action), rate))
 
     @abstractmethod
-    def _set_sensor_state(self, port: int, action: SensorAction, rate: int) -> bool:
-        ...
+    def _set_sensor_state(self, port: int, action: SensorAction, rate: int) -> bool: ...
 
     def __set_sensor_state(self, port: int, action: int, rate: int) -> bool:
         return self.set_sensor_state(port, SensorAction(action), rate)
 
     def get_sensor_input(self, port: int, sensor: Sensor) -> float:
         if not isinstance(port, int):
             raise TypeError(f"port must be an int, not {type(port).__name__}")
@@ -58,16 +57,15 @@
                 return float(f)
             case e:
                 raise TypeError(
                     f"Expected _get_sensor_input to return a float, got {type(e).__name__}"
                 )
 
     @abstractmethod
-    def _get_sensor_input(self, port: int, sensor: Sensor) -> float:
-        ...
+    def _get_sensor_input(self, port: int, sensor: Sensor) -> float: ...
 
     def __get_sensor_input(self, port: int, sensor: int) -> float:
         return self.get_sensor_input(port, Sensor(sensor))
 
 
 __all__ = [
     "SensorInterface",
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/timing/default.py` & `libretro_py-0.0.1/src/libretro/drivers/timing/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/timing/driver.py` & `libretro_py-0.0.1/src/libretro/drivers/timing/driver.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,62 +8,52 @@
 )
 
 
 @runtime_checkable
 class TimingDriver(Protocol):
     @property
     @abstractmethod
-    def frame_time_callback(self) -> retro_frame_time_callback | None:
-        ...
+    def frame_time_callback(self) -> retro_frame_time_callback | None: ...
 
     @frame_time_callback.setter
     @abstractmethod
-    def frame_time_callback(self, value: retro_frame_time_callback) -> None:
-        ...
+    def frame_time_callback(self, value: retro_frame_time_callback) -> None: ...
 
     def frame_time(self, time: int | None) -> None:
         callback = self.frame_time_callback
         if callback:
             callback(time if time is not None else callback.reference)
 
     @property
     @abstractmethod
-    def fastforwarding_override(self) -> retro_fastforwarding_override | None:
-        ...
+    def fastforwarding_override(self) -> retro_fastforwarding_override | None: ...
 
     @fastforwarding_override.setter
     @abstractmethod
-    def fastforwarding_override(self, value: retro_fastforwarding_override) -> None:
-        ...
+    def fastforwarding_override(self, value: retro_fastforwarding_override) -> None: ...
 
     @property
     @abstractmethod
-    def throttle_state(self) -> retro_throttle_state | None:
-        ...
+    def throttle_state(self) -> retro_throttle_state | None: ...
 
     @throttle_state.setter
     @abstractmethod
-    def throttle_state(self, value: retro_throttle_state) -> None:
-        ...
+    def throttle_state(self, value: retro_throttle_state) -> None: ...
 
     @throttle_state.deleter
     @abstractmethod
-    def throttle_state(self) -> None:
-        ...
+    def throttle_state(self) -> None: ...
 
     @property
     @abstractmethod
-    def target_refresh_rate(self) -> float | None:
-        ...
+    def target_refresh_rate(self) -> float | None: ...
 
     @target_refresh_rate.setter
     @abstractmethod
-    def target_refresh_rate(self, value: float) -> None:
-        ...
+    def target_refresh_rate(self, value: float) -> None: ...
 
     @target_refresh_rate.deleter
     @abstractmethod
-    def target_refresh_rate(self) -> None:
-        ...
+    def target_refresh_rate(self) -> None: ...
 
 
 __all__ = ["TimingDriver"]
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/user/default.py` & `libretro_py-0.0.1/src/libretro/drivers/user/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/vfs/default.py` & `libretro_py-0.0.1/src/libretro/drivers/vfs/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/vfs/history.py` & `libretro_py-0.0.1/src/libretro/drivers/vfs/history.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.0.0/src/libretro/drivers/vfs/interface.py` & `libretro_py-0.0.1/src/libretro/drivers/vfs/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,50 +39,41 @@
 @runtime_checkable
 class FileHandle(Protocol):
     @abstractmethod
     def __init__(self, path: VfsPath, mode: VfsFileAccess, hints: VfsFileAccessHint):
         self._as_parameter_ = id(self)
 
     @abstractmethod
-    def close(self) -> bool:
-        ...
+    def close(self) -> bool: ...
 
     @property
     @abstractmethod
-    def path(self) -> bytes:
-        ...
+    def path(self) -> bytes: ...
 
     @property
     @abstractmethod
-    def size(self) -> int:
-        ...
+    def size(self) -> int: ...
 
     @abstractmethod
-    def tell(self) -> int:
-        ...
+    def tell(self) -> int: ...
 
     @abstractmethod
-    def seek(self, offset: int, whence: VfsSeekPosition) -> int:
-        ...
+    def seek(self, offset: int, whence: VfsSeekPosition) -> int: ...
 
     @abstractmethod
-    def read(self, buffer: bytearray | memoryview) -> int:
-        ...
+    def read(self, buffer: bytearray | memoryview) -> int: ...
 
     @abstractmethod
-    def write(self, buffer: bytes | bytearray | memoryview) -> int:
-        ...
+    def write(self, buffer: bytes | bytearray | memoryview) -> int: ...
 
     @abstractmethod
-    def flush(self) -> bool:
-        ...
+    def flush(self) -> bool: ...
 
     @abstractmethod
-    def truncate(self, length: int) -> int:
-        ...
+    def truncate(self, length: int) -> int: ...
 
 
 class DirEntry(NamedTuple):
     name: bytes
     is_dir: bool
 
 
@@ -90,30 +81,28 @@
 class DirectoryHandle(Protocol):
     @abstractmethod
     def __init__(self, dir: bytes, include_hidden: bool):
         self._as_parameter_ = id(self)
         self._current_dirent: DirEntry | None = None
 
     @abstractmethod
-    def close(self) -> bool:
-        ...  # Corresponds to closedir
+    def close(self) -> bool: ...  # Corresponds to closedir
 
     def __iter__(self):
         return self
 
     def __next__(self) -> DirEntry:
         self._current_dirent = self.readdir()
         if self._current_dirent is None:
             raise StopIteration
 
         return self._current_dirent
 
     @abstractmethod
-    def readdir(self) -> DirEntry | None:
-        ...
+    def readdir(self) -> DirEntry | None: ...
 
     def dirent_name(self) -> bytes | None:
         """
         Returns the most recent directory entry returned by readdir
         """
         return self._current_dirent and self._current_dirent.name
 
@@ -136,42 +125,35 @@
             )
 
         self._logger = logger
         self.__interface: retro_vfs_interface | None = None
 
     @property
     @abstractmethod
-    def version(self) -> int:
-        ...
+    def version(self) -> int: ...
 
     @abstractmethod
     def open(
         self, path: bytes, mode: VfsFileAccess, hints: VfsFileAccessHint
-    ) -> FileHandle | None:
-        ...
+    ) -> FileHandle | None: ...
 
     @abstractmethod
-    def remove(self, path: bytes) -> bool:
-        ...
+    def remove(self, path: bytes) -> bool: ...
 
     @abstractmethod
-    def rename(self, old_path: bytes, new_path: bytes) -> bool:
-        ...
+    def rename(self, old_path: bytes, new_path: bytes) -> bool: ...
 
     @abstractmethod
-    def stat(self, path: bytes) -> tuple[VfsStat, int] | None:
-        ...
+    def stat(self, path: bytes) -> tuple[VfsStat, int] | None: ...
 
     @abstractmethod
-    def mkdir(self, path: bytes) -> VfsMkdirResult:
-        ...
+    def mkdir(self, path: bytes) -> VfsMkdirResult: ...
 
     @abstractmethod
-    def opendir(self, path: bytes, include_hidden: bool) -> DirectoryHandle | None:
-        ...
+    def opendir(self, path: bytes, include_hidden: bool) -> DirectoryHandle | None: ...
 
     @property
     def _as_parameter_(self) -> retro_vfs_interface:
         if not self.__interface:
             self.__interface: retro_vfs_interface = retro_vfs_interface()
             if self.version >= 1:
                 self.__interface.get_path = retro_vfs_get_path_t(self.__get_path)
```

### Comparing `libretro_py-0.0.0/src/libretro/drivers/video/opengl/moderngl.py` & `libretro_py-0.0.1/src/libretro/drivers/video/software/array.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,195 +1,159 @@
+import itertools
 from array import array
-from collections.abc import Set
 from copy import deepcopy
-from ctypes import c_char_p
-from typing import override
-
-import moderngl
-from glcontext.empty import GLContext
+from typing import final, override
+from warnings import warn
 
 from libretro.api.av import retro_game_geometry, retro_system_av_info
-from libretro.api.proc import retro_proc_address_t
-from libretro.api.video import (
-    HardwareContext,
-    MemoryAccess,
-    PixelFormat,
-    Rotation,
-    retro_framebuffer,
-    retro_hw_get_current_framebuffer_t,
-    retro_hw_get_proc_address_t,
-    retro_hw_render_callback,
-    retro_hw_render_interface,
-)
-
-from ..driver import VideoDriver
-
-
-class ModernGlVideoDriver(VideoDriver):
-    def __init__(self, callback: retro_hw_render_callback | None = None):
-        self._context: GLContext | None = None
-        self._pixel_format: PixelFormat = PixelFormat.RGB1555
-        self._system_av_info: retro_system_av_info | None = None
-        self._hw_render_callback = callback
-        self._use_shared_context = False
-        self._needs_recreate = True
+from libretro.api.video import MemoryAccess, PixelFormat, Rotation, retro_framebuffer
 
-    def __del__(self):
-        if self._context:
-            self._context.release()
+from ..driver import FrameBufferSpecial, Screenshot
+from .base import SoftwareVideoDriver
 
-            del self._context
 
-    def refresh(self, data: memoryview | None, width: int, height: int, pitch: int) -> None:
-        # TODO: Recreate the frame buffer based on the pixel format and system AV info
-        pass  # TODO: Implement
+@final
+class ArrayVideoDriver(SoftwareVideoDriver):
+    def __init__(self):
+        self._frame: array | None = None
+        self._pixel_format: PixelFormat = PixelFormat.RGB1555
+        self._system_av_info: retro_system_av_info | None = None
+        self._rotation: Rotation = Rotation.NONE
+        self._last_width: int | None = None
+        self._last_height: int | None = None
 
-    def supported_contexts(self) -> Set[HardwareContext]:
-        pass
+    @override
+    def refresh(
+        self, data: memoryview | FrameBufferSpecial, width: int, height: int, pitch: int
+    ) -> None:
+        match data:
+            case memoryview():
+                frameview = memoryview(self._frame)
+                frameview[: len(data)] = data
 
-    @property
-    def preferred_context(self) -> HardwareContext | None:
-        pass
+            case FrameBufferSpecial.DUPE:
+                pass  # Do nothing
 
-    def active_context(self) -> HardwareContext | None:
-        if self._context:
-            return HardwareContext.OPENGL
+            case FrameBufferSpecial.HARDWARE:
+                warn("RETRO_HW_FRAME_BUFFER_VALID passed to software-only video refresh callback")
 
-        return HardwareContext.NONE
+            case _:
+                raise TypeError(
+                    f"Expected a memoryview or a FrameBufferSpecial, got {type(data).__name__}"
+                )
 
-    @override
-    def set_context(self, callback: retro_hw_render_callback) -> retro_hw_render_callback | None:
-        if not isinstance(callback, retro_hw_render_callback):
-            raise TypeError(f"Expected a retro_hw_render_callback, got {type(callback).__name__}")
+        self._last_width = width
+        self._last_height = height
 
-        self._hw_render_callback = deepcopy(callback)
-        self._hw_render_callback.get_current_framebuffer = retro_hw_get_current_framebuffer_t(
-            self.get_hw_framebuffer
-        )
-        self._hw_render_callback.get_proc_address = retro_hw_get_proc_address_t(
-            self.__get_proc_address
-        )
+    @override
+    @property
+    def needs_reinit(self) -> bool:
+        return self._frame is None
 
-        return self._hw_render_callback
+    @override
+    def reinit(self) -> None:
+        geometry = self._system_av_info.geometry
+        bufsize = geometry.max_width * geometry.max_height * self._pixel_format.bytes_per_pixel
+        self._frame = array("B", itertools.repeat(0, bufsize))
 
     @property
     @override
-    def geometry(self) -> retro_game_geometry:
-        if not self._system_av_info:
-            raise RuntimeError("No system AV info has been set")
-
-        return deepcopy(self._system_av_info.geometry)
+    def rotation(self) -> Rotation:
+        return self._rotation
 
-    @geometry.setter
+    @rotation.setter
     @override
-    def geometry(self, geometry: retro_game_geometry) -> None:
-        if not isinstance(geometry, retro_game_geometry):
-            raise TypeError(f"Expected a retro_game_geometry, got {type(geometry).__name__}")
+    def rotation(self, rotation: Rotation) -> None:
+        if not isinstance(rotation, Rotation):
+            raise TypeError(f"Expected a Rotation, got {type(rotation).__name__}")
+
+        if rotation not in Rotation:
+            raise ValueError(f"Invalid rotation: {rotation}")
 
-        self._system_av_info.geometry = geometry
-        # TODO: Crop the OpenGL texture if necessary
+        self._rotation = rotation
 
     @property
     @override
     def pixel_format(self) -> PixelFormat:
         return self._pixel_format
 
     @pixel_format.setter
     @override
     def pixel_format(self, format: PixelFormat) -> None:
-        if not isinstance(format, PixelFormat):
-            raise TypeError(f"Expected a PixelFormat, got {type(format).__name__}")
-
         if format not in PixelFormat:
             raise ValueError(f"Invalid pixel format: {format}")
 
+        if not isinstance(format, PixelFormat):
+            raise TypeError(f"Expected a PixelFormat, got {type(format).__name__}")
+
         if self._pixel_format != format:
-            self._pixel_format = format
-            self._needs_recreate = True
+            # If the pixel format has changed, recreate the frame buffer
+            self._frame = None
 
-    @property
-    @override
-    def rotation(self) -> Rotation:
-        pass
+        self._pixel_format = format
 
-    @rotation.setter
     @override
-    def rotation(self, rotation: Rotation) -> None:
-        pass  # TODO: Implement
+    def screenshot(self) -> Screenshot | None:
+        if not self._frame:
+            return None
+
+        last_frame_length = (
+            self._last_width * self._last_height * self._pixel_format.bytes_per_pixel
+        )
+        screen = self._frame[:last_frame_length]
+        for i in range(0, last_frame_length, self._pixel_format.bytes_per_pixel):
+            r, g, b, a = screen[i : i + self._pixel_format.bytes_per_pixel]
+            screen[i : i + self._pixel_format.bytes_per_pixel] = array("B", (b, g, r, a))
+            # the lower 8 bits of the pixel are the red channel;
+            # we need to swap them so images don't look wrong
+            # in common Python imaging libraries
+
+        # TODO: support RGB565 and RGB555
+        # TODO: support rotation
+
+        return Screenshot(
+            memoryview(screen),
+            self._last_width,
+            self._last_height,
+            self._rotation,
+            self._pixel_format,
+        )
+
+    def get_software_framebuffer(
+        self, width: int, height: int, flags: MemoryAccess
+    ) -> retro_framebuffer | None:
+        pass
 
     @property
     @override
     def system_av_info(self) -> retro_system_av_info | None:
         return deepcopy(self._system_av_info) if self._system_av_info else None
 
     @system_av_info.setter
     @override
     def system_av_info(self, av_info: retro_system_av_info) -> None:
         if not isinstance(av_info, retro_system_av_info):
             raise TypeError(f"Expected a retro_system_av_info, got {type(av_info).__name__}")
 
-        self._system_av_info = av_info
-        self._needs_recreate = True
-
-    @property
-    def frame(self):
-        pass
-
-    @property
-    def frame_max(self):
-        pass
+        self._system_av_info = deepcopy(av_info)
+        self.reinit()
 
     @property
     @override
-    def shared_context(self) -> bool:
-        return self._use_shared_context
-
-    @shared_context.setter
-    @override
-    def shared_context(self, shared: bool) -> None:
-        self._use_shared_context = bool(shared)
-
-    def set_rotation(self, rotation: Rotation) -> bool:
-        raise NotImplementedError()  # TODO: Implement
-
-    @property
-    def can_dupe(self) -> bool:
-        return True
-
-    def get_hw_framebuffer(self) -> int:
-        raise NotImplementedError()  # TODO: Implement
-
-    def __get_proc_address(self, sym: c_char_p) -> retro_proc_address_t:
-        return self.get_proc_address(bytes(sym))
-
-    def get_proc_address(self, sym: bytes) -> retro_proc_address_t | None:
-        if not sym:
+    def geometry(self) -> retro_game_geometry | None:
+        if not self._system_av_info:
             return None
 
-        if not self._context:
-            raise RuntimeError("No OpenGL context has been initialized")
-
-        return retro_proc_address_t(self._context.load_opengl_function(sym))
-
-    def get_software_framebuffer(
-        self, width: int, size: int, flags: MemoryAccess
-    ) -> retro_framebuffer | None:
-        # TODO: Map the OpenGL texture to a software framebuffer
-        pass
-
-    @property
-    def hw_render_interface(self) -> retro_hw_render_interface | None:
-        # libretro doesn't define one of these for OpenGL, so no need
-        return None
-
-    def context_reset(self) -> None:
-        pass  # TODO: Implement
+        return deepcopy(self._system_av_info.geometry)
 
-    def context_destroy(self) -> None:
-        if not self._context:
-            raise RuntimeError("No OpenGL context has been initialized")
+    @geometry.setter
+    @override
+    def geometry(self, geometry: retro_game_geometry) -> None:
+        if not isinstance(geometry, retro_game_geometry):
+            raise TypeError(f"Expected a retro_game_geometry, got {type(geometry).__name__}")
 
-        if self._hw_render_callback.context_destroy:
-            self._hw_render_callback.context_destroy()
+        self._system_av_info.geometry.base_width = geometry.base_width
+        self._system_av_info.geometry.base_height = geometry.base_height
+        self._system_av_info.geometry.aspect_ratio = geometry.aspect_ratio
 
 
-__all__ = ["ModernGlVideoDriver"]
+__all__ = ["ArrayVideoDriver"]
```

### Comparing `libretro_py-0.0.0/src/libretro/session.py` & `libretro_py-0.0.1/src/libretro/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,17 @@
     ) -> Sequence[retro_system_content_info_override] | None:
         return self._environment.content.overrides
 
     def run(self) -> None:
         if self._is_exited or self._environment.is_shutdown:
             raise CoreShutDownException()
 
+        if self._environment.video.needs_reinit:
+            self._environment.video.reinit()
+
         # TODO: In RetroArch, retro_audio_callback.set_state is called on the main thread,
         # just before starting the audio thread and just after stopping it.
         # TODO: In RetroArch, retro_audio_callback.callback is called on the audio thread.
         # TODO: In RetroArch, an audio thread is started if the core registers an audio callback
 
         if isinstance(self._environment.microphones, Pollable):
             self._environment.microphones.poll()
```

### Comparing `libretro_py-0.0.0/src/libretro.py.egg-info/PKG-INFO` & `libretro_py-0.0.1/src/libretro.py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretro.py
-Version: 0.0.0
+Version: 0.0.1
 Summary: A libretro frontend for Python intended for testing cores.
 Author-email: Jesse Talavera <jesse@jesse.tg>
 Maintainer-email: Jesse Talavera <jesse@jesse.tg>
 License: MIT License
 Project-URL: Homepage, https://github.com/JesseTG/libretro.py
 Project-URL: Issues, https://github.com/JesseTG/libretro.py/issues
 Project-URL: Repository, https://github.com/JesseTG/libretro.py
@@ -31,45 +31,44 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions==4.*; python_version == "3.10"
 Provides-Extra: build
 Requires-Dist: build==1.2.1; extra == "build"
 Requires-Dist: setuptools>=69.1.1; extra == "build"
 Requires-Dist: twine==5.0.0; extra == "build"
+Requires-Dist: pre-commit==3.7.*; extra == "build"
 Provides-Extra: dev
 Requires-Dist: bandit==1.7.*; extra == "dev"
-Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: black==24.*; extra == "dev"
 Requires-Dist: flake8==6.*; extra == "dev"
 Requires-Dist: isort==5.*; extra == "dev"
 Requires-Dist: mypy==1.5.*; extra == "dev"
 Requires-Dist: libretro.py[build]; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: Sphinx==7.*; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.*; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: doc
 Requires-Dist: libretro.py[docs]; extra == "doc"
 Provides-Extra: opengl
 Requires-Dist: moderngl==5.10.*; extra == "opengl"
-Provides-Extra: pillow
-Requires-Dist: pillow==10.2.*; extra == "pillow"
-Requires-Dist: types-Pillow; extra == "pillow"
+Requires-Dist: PyOpenGL==3.1.*; extra == "opengl"
 Provides-Extra: all
-Requires-Dist: libretro.py[build,dev,docs,opengl,pillow]; extra == "all"
+Requires-Dist: libretro.py[build,dev,docs,opengl]; extra == "all"
 
 # libretro.py
 
 A Python binding for [libretro][libretro] intended for testing cores,
 but suitable for any purpose.
 Ease of use, flexibility, and complete API support are top priorities.
 
 <div align="center">
 
-[![Build Status](https://github.com/JesseTG/libretro.py/workflows/build/badge.svg)](https://github.com/JesseTG/libretro.py/actions)
-[![PyPi](https://img.shields.io/pypi/v/PROJECT_NAME_URL)](https://pypi.org/project/PROJECT_NAME_URL)
+[![Workflow Status](https://github.com/JesseTG/libretro.py/actions/workflows/release.yml/badge.svg)](https://github.com/JesseTG/libretro.py/actions/workflows/release.yml)
+[![PyPi](https://img.shields.io/pypi/v/libretro.py)](https://pypi.org/project/libretro.py)
 [![License](https://img.shields.io/github/license/JesseTG/libretro.py)](LICENSE)
 
 </div>
 
 # Supported Environments
 
 libretro.py has the following requirements:
@@ -123,28 +122,23 @@
 To install additional features,
 add one or more of the following extras to the `install` command:
 
 - **`dev`:** Assorted tools used to help develop libretro.py.
   Required if contributing to libretro.py.
 - **`opengl`:** Support for the built-in OpenGL video driver.
   Required if testing a core's OpenGL support.
-- **`pillow`:** Support for the built-in software-only video driver
-  powered by the [Pillow][pillow] image processing library.
-  Not required for any particular feature,
-  but it simplifies tests that inspect the core's video output.
 
-For example, if you want to submit an improvement to the Pillow video driver,
+For example, if you want to submit an improvement to the OpenGL video driver,
 you would install libretro.py like so:
 
 ```bash
-pip install libretro.py[pillow,dev]
+pip install libretro.py[opengl,dev]
 ```
 
 And if you just want to test your libretro core's OpenGL support:
 
 ```bash
 pip install libretro.py[opengl]
 ```
 
 [just]: https://just.systems
 [libretro]: https://www.libretro.com
-[pillow]: https://python-pillow.org
```

### Comparing `libretro_py-0.0.0/src/libretro.py.egg-info/SOURCES.txt` & `libretro_py-0.0.1/src/libretro.py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -127,9 +127,8 @@
 src/libretro/drivers/video/__init__.py
 src/libretro/drivers/video/driver.py
 src/libretro/drivers/video/multi.py
 src/libretro/drivers/video/opengl/__init__.py
 src/libretro/drivers/video/opengl/moderngl.py
 src/libretro/drivers/video/software/__init__.py
 src/libretro/drivers/video/software/array.py
-src/libretro/drivers/video/software/base.py
-src/libretro/drivers/video/software/pillow.py
+src/libretro/drivers/video/software/base.py
```

