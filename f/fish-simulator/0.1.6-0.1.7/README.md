# Comparing `tmp/fish_simulator-0.1.6.tar.gz` & `tmp/fish_simulator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_simulator-0.1.6.tar", last modified: Fri May 31 19:52:16 2024, max compression
+gzip compressed data, was "fish_simulator-0.1.7.tar", last modified: Fri May 31 20:03:16 2024, max compression
```

## Comparing `fish_simulator-0.1.6.tar` & `fish_simulator-0.1.7.tar`

### file list

```diff
@@ -1,88 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.291526 fish_simulator-0.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   195592 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/examples/demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.295526 fish_simulator-0.1.6/examples/demo_vid/
--rw-r--r--   0 runner    (1001) docker     (127)   238867 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/examples/demo_vid/run_ani_swim01.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    40841 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/examples/demo_vid/run_img_swim01.mp4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.295526 fish_simulator-0.1.6/fish_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/image_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.291526 fish_simulator-0.1.6/fish_simulator/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.295526 fish_simulator-0.1.6/fish_simulator/templates/template_img/
--rw-r--r--   0 runner    (1001) docker     (127)    70542 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img/head.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.295526 fish_simulator-0.1.6/fish_simulator/templates/template_img/segs/
--rw-r--r--   0 runner    (1001) docker     (127)    46534 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img/segs/tail.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.295526 fish_simulator-0.1.6/fish_simulator/templates/template_img2/
--rw-r--r--   0 runner    (1001) docker     (127)    55963 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/fish_head.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/00.png
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/01.png
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/02.png
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/03.png
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/04.png
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/05.png
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/06.png
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/07.png
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/08.png
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/09.png
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/10.png
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/11.png
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/12.png
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/13.png
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/14.png
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/15.png
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/17.png
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/18.png
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/20.png
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/21.png
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/22.png
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/23.png
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/25.png
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/26.png
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/27.png
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/28.png
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/29.png
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/30.png
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/31.png
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/33.png
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/34.png
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/35.png
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/36.png
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/37.png
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/38.png
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/39.png
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/40.png
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/41.png
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/42.png
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/43.png
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/44.png
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/45.png
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/46.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/47.png
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/fish_simulator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/fish_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-31 19:52:16.000000 fish_simulator-0.1.6/fish_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-31 19:52:16.000000 fish_simulator-0.1.6/fish_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:52:16.000000 fish_simulator-0.1.6/fish_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 19:52:16.000000 fish_simulator-0.1.6/fish_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 19:52:16.000000 fish_simulator-0.1.6/fish_simulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:16.307526 fish_simulator-0.1.6/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-31 19:52:11.000000 fish_simulator-0.1.6/test/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.377535 fish_simulator-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-31 20:03:16.377535 fish_simulator-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.361535 fish_simulator-0.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   195592 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/examples/demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.361535 fish_simulator-0.1.7/examples/demo_vid/
+-rw-r--r--   0 runner    (1001) docker     (127)   238867 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/examples/demo_vid/run_ani_swim01.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    40841 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/examples/demo_vid/run_img_swim01.mp4
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.365535 fish_simulator-0.1.7/fish_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.361535 fish_simulator-0.1.7/fish_simulator/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.365535 fish_simulator-0.1.7/fish_simulator/templates/template_img/
+-rw-r--r--   0 runner    (1001) docker     (127)    70542 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img/head.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.365535 fish_simulator-0.1.7/fish_simulator/templates/template_img/segs/
+-rw-r--r--   0 runner    (1001) docker     (127)    46534 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img/segs/tail.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.365535 fish_simulator-0.1.7/fish_simulator/templates/template_img2/
+-rw-r--r--   0 runner    (1001) docker     (127)    55963 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/fish_head.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.373535 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/00.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/01.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/02.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/03.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/04.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/05.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/06.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/07.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/08.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/09.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/10.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/11.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/12.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/13.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/14.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/15.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/17.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/18.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/20.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/21.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/22.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/23.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/25.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/26.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/27.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/28.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/29.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/30.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/31.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/33.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/34.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/35.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/36.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/37.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/39.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/40.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/41.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/42.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/43.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/44.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/45.png
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/46.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/47.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/fish_simulator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.377535 fish_simulator-0.1.7/fish_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-31 20:03:16.000000 fish_simulator-0.1.7/fish_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-31 20:03:16.000000 fish_simulator-0.1.7/fish_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:03:16.000000 fish_simulator-0.1.7/fish_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 20:03:16.000000 fish_simulator-0.1.7/fish_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 20:03:16.000000 fish_simulator-0.1.7/fish_simulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:03:16.377535 fish_simulator-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:03:16.373535 fish_simulator-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-31 20:03:11.000000 fish_simulator-0.1.7/test/test_methods.py
```

### Comparing `fish_simulator-0.1.6/LICENSE` & `fish_simulator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/MANIFEST.in` & `fish_simulator-0.1.7/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 recursive-include fish_simulator *.pyx *.pxd *.pxi *.py *.pyi *.h *.ini *.npy *.txt *.in *.md
 recursive-include fish_simulator/templates *
 recursive-include fish_simulator/templates/template_img *
 recursive-include fish_simulator/templates/template_img/segs *
 recursive-include fish_simulator/templates/template_img2 *
 recursive-include fish_simulator/templates/template_img2/segs *
 recursive-include examples/ *
-recursive-include tests/ *
+recursive-include tests/ *
+recursive-include tests/fixtures/ *
```

### Comparing `fish_simulator-0.1.6/PKG-INFO` & `fish_simulator-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish_simulator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simulate zebrafish swim from tail angle tracking data
 Author-email: Thomas Soares Mullen <thomasmullen96@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Soares Mullen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fish_simulator-0.1.6/README.md` & `fish_simulator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/examples/demo.ipynb` & `fish_simulator-0.1.7/examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/examples/demo_vid/run_ani_swim01.mp4` & `fish_simulator-0.1.7/examples/demo_vid/run_ani_swim01.mp4`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/examples/demo_vid/run_img_swim01.mp4` & `fish_simulator-0.1.7/examples/demo_vid/run_img_swim01.mp4`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/image_loader.py` & `fish_simulator-0.1.7/fish_simulator/image_loader.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/simulator.py` & `fish_simulator-0.1.7/fish_simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img/head.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img/head.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img/segs/tail.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img/segs/tail.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/fish_head.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/fish_head.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/00.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/00.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/01.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/01.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/02.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/02.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/03.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/03.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/04.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/04.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/05.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/05.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/06.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/06.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/07.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/07.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/08.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/08.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/09.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/09.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/10.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/10.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/11.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/11.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/12.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/12.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/13.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/13.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/14.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/14.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/15.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/15.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/16.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/16.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/17.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/17.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/18.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/18.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/19.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/19.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/20.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/20.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/21.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/21.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/22.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/22.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/23.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/23.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/24.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/24.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/25.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/25.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/26.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/26.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/27.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/27.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/28.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/28.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/29.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/29.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/30.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/30.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/31.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/31.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/32.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/32.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/33.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/33.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/34.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/34.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/35.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/35.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/36.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/36.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/37.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/37.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/38.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/38.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/39.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/39.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/40.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/40.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/41.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/41.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/42.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/42.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/43.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/43.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/44.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/44.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/45.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/45.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/46.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/46.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/templates/template_img2/segs/47.png` & `fish_simulator-0.1.7/fish_simulator/templates/template_img2/segs/47.png`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/transforms.py` & `fish_simulator-0.1.7/fish_simulator/transforms.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator/utils.py` & `fish_simulator-0.1.7/fish_simulator/utils.py`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/fish_simulator.egg-info/PKG-INFO` & `fish_simulator-0.1.7/fish_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish_simulator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simulate zebrafish swim from tail angle tracking data
 Author-email: Thomas Soares Mullen <thomasmullen96@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Thomas Soares Mullen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fish_simulator-0.1.6/fish_simulator.egg-info/SOURCES.txt` & `fish_simulator-0.1.7/fish_simulator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
-examples/__init__.py
 examples/demo.ipynb
 examples/demo_vid/run_ani_swim01.mp4
 examples/demo_vid/run_img_swim01.mp4
 fish_simulator/VERSION
 fish_simulator/__init__.py
 fish_simulator/image_loader.py
 fish_simulator/simulator.py
@@ -65,10 +64,8 @@
 fish_simulator/templates/template_img2/segs/41.png
 fish_simulator/templates/template_img2/segs/42.png
 fish_simulator/templates/template_img2/segs/43.png
 fish_simulator/templates/template_img2/segs/44.png
 fish_simulator/templates/template_img2/segs/45.png
 fish_simulator/templates/template_img2/segs/46.png
 fish_simulator/templates/template_img2/segs/47.png
-test/__init__.py
-test/test_methods.py
-test/fixtures/__init__.py
+test/test_methods.py
```

### Comparing `fish_simulator-0.1.6/pyproject.toml` & `fish_simulator-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.1.6/test/test_methods.py` & `fish_simulator-0.1.7/test/test_methods.py`

 * *Files identical despite different names*

