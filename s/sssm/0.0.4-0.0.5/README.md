# Comparing `tmp/sssm-0.0.4.tar.gz` & `tmp/sssm-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssm-0.0.4.tar", last modified: Mon May 13 01:33:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

## Comparing `sssm-0.0.4.tar` & `sssm/saved_models/model.pt`

 * *Files 10% similar despite different names*

### file list

```diff
@@ -1,17 +1,90 @@
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-13 01:33:19.356510 sssm-0.0.4/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       31 2024-05-12 15:27:39.000000 sssm-0.0.4/MANIFEST.in
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-13 01:33:19.356510 sssm-0.0.4/PKG-INFO
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       38 2024-05-13 01:33:19.356510 sssm-0.0.4/setup.cfg
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      429 2024-05-13 01:33:05.000000 sssm-0.0.4/setup.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-13 01:33:19.353176 sssm-0.0.4/sssm/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 09:14:40.000000 sssm-0.0.4/sssm/__init__.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-13 01:33:19.356510 sssm-0.0.4/sssm/saved_models/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-04-20 07:45:12.000000 sssm-0.0.4/sssm/saved_models/__init__.py
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)  2186030 2024-05-12 15:00:16.000000 sssm-0.0.4/sssm/saved_models/model.pt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)     9596 2024-05-13 01:29:38.000000 sssm-0.0.4/sssm/ssm.py
-drwxr-xr-x   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        0 2024-05-13 01:33:19.356510 sssm-0.0.4/sssm.egg-info/
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      262 2024-05-13 01:33:19.000000 sssm-0.0.4/sssm.egg-info/PKG-INFO
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)      310 2024-05-13 01:33:19.000000 sssm-0.0.4/sssm.egg-info/SOURCES.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        1 2024-05-13 01:33:19.000000 sssm-0.0.4/sssm.egg-info/dependency_links.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)       79 2024-05-13 01:33:19.000000 sssm-0.0.4/sssm.egg-info/requires.txt
--rw-r--r--   0 bkxcyu_arch  (1000) bkxcyu_arch  (1000)        5 2024-05-13 01:33:19.000000 sssm-0.0.4/sssm.egg-info/top_level.txt
+-rw-rw-r--   0        0        0    17444 1979-11-30 00:00:00.000000 ckp_last/data.pkl
+-rw-rw-r--   0        0        0        6 1979-11-30 00:00:00.000000 ckp_last/byteorder
+-rw-rw-r--   0        0        0     3200 1979-11-30 00:00:00.000000 ckp_last/data/0
+-rw-rw-r--   0        0        0      128 1979-11-30 00:00:00.000000 ckp_last/data/1
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/10
+-rw-rw-r--   0        0        0        8 1979-11-30 00:00:00.000000 ckp_last/data/11
+-rw-rw-r--   0        0        0   262144 1979-11-30 00:00:00.000000 ckp_last/data/12
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/13
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/14
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/15
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/16
+-rw-rw-r--   0        0        0        8 1979-11-30 00:00:00.000000 ckp_last/data/17
+-rw-rw-r--   0        0        0    53760 1979-11-30 00:00:00.000000 ckp_last/data/18
+-rw-rw-r--   0        0        0       28 1979-11-30 00:00:00.000000 ckp_last/data/19
+-rw-rw-r--   0        0        0      128 1979-11-30 00:00:00.000000 ckp_last/data/2
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/20
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/21
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/22
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/23
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/24
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/25
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/26
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/27
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/28
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/29
+-rw-rw-r--   0        0        0      128 1979-11-30 00:00:00.000000 ckp_last/data/3
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/30
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/31
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/32
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/33
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/34
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/35
+-rw-rw-r--   0        0        0        8 1979-11-30 00:00:00.000000 ckp_last/data/36
+-rw-rw-r--   0        0        0     8192 1979-11-30 00:00:00.000000 ckp_last/data/37
+-rw-rw-r--   0        0        0      128 1979-11-30 00:00:00.000000 ckp_last/data/38
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/39
+-rw-rw-r--   0        0        0      128 1979-11-30 00:00:00.000000 ckp_last/data/4
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/40
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/41
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/42
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/43
+-rw-rw-r--   0        0        0   196608 1979-11-30 00:00:00.000000 ckp_last/data/44
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/45
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/46
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/47
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/48
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/49
+-rw-rw-r--   0        0        0        8 1979-11-30 00:00:00.000000 ckp_last/data/5
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/50
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/51
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/52
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/53
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/54
+-rw-rw-r--   0        0        0   196608 1979-11-30 00:00:00.000000 ckp_last/data/55
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/56
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/57
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/58
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/59
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/6
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/60
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/61
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/62
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/63
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/64
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/65
+-rw-rw-r--   0        0        0   196608 1979-11-30 00:00:00.000000 ckp_last/data/66
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/67
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/68
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/69
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/7
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/70
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/71
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/72
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/73
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/74
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/75
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/76
+-rw-rw-r--   0        0        0   196608 1979-11-30 00:00:00.000000 ckp_last/data/77
+-rw-rw-r--   0        0        0    65536 1979-11-30 00:00:00.000000 ckp_last/data/78
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/79
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/8
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/80
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/81
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/82
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/83
+-rw-rw-r--   0        0        0    32768 1979-11-30 00:00:00.000000 ckp_last/data/84
+-rw-rw-r--   0        0        0      512 1979-11-30 00:00:00.000000 ckp_last/data/85
+-rw-rw-r--   0        0        0      256 1979-11-30 00:00:00.000000 ckp_last/data/9
+-rw-rw-r--   0        0        0        2 1979-11-30 00:00:00.000000 ckp_last/version
+-rw-rw-r--   0        0        0       40 1979-11-30 00:00:00.000000 ckp_last/.data/serialization_id
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+Zip archive data, at least v0.0 to extract, compression method=store
```

### filetype from diffoscope

```diff
@@ -1 +1 @@
-TarFile
+ZipFile
```

