# Comparing `tmp/detroit-1.1.0.tar.gz` & `tmp/detroit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detroit-1.1.0.tar", last modified: Wed Mar 13 18:15:16 2024, max compression
+gzip compressed data, was "detroit-1.2.0.tar", last modified: Fri May 31 13:48:14 2024, max compression
```

## Comparing `detroit-1.1.0.tar` & `detroit-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,182 @@
-drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-03-13 18:15:16.717074 detroit-1.1.0/
--rw-rw-r--   0 nut       (1000) nut       (1000)     1503 2023-11-25 15:13:50.000000 detroit-1.1.0/LICENSE
--rw-rw-r--   0 nut       (1000) nut       (1000)       71 2024-01-06 13:38:00.000000 detroit-1.1.0/MANIFEST.in
--rw-r--r--   0 nut       (1000) nut       (1000)     5226 2024-03-13 18:15:16.717074 detroit-1.1.0/PKG-INFO
--rw-rw-r--   0 nut       (1000) nut       (1000)     2419 2023-12-23 21:47:04.000000 detroit-1.1.0/README.md
-drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-03-13 18:15:16.713074 detroit-1.1.0/detroit/
--rw-rw-r--   0 nut       (1000) nut       (1000)      277 2024-03-13 18:07:48.000000 detroit-1.1.0/detroit/__init__.py
--rw-rw-r--   0 nut       (1000) nut       (1000)    21682 2024-03-13 18:07:48.000000 detroit-1.1.0/detroit/d3.py
--rw-rw-r--   0 nut       (1000) nut       (1000)     4140 2023-12-23 20:33:36.000000 detroit-1.1.0/detroit/plot.py
-drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-03-13 18:15:16.713074 detroit-1.1.0/detroit/static/
--rw-rw-r--   0 nut       (1000) nut       (1000)      493 2023-12-20 17:40:42.000000 detroit-1.1.0/detroit/static/serialize.js
--rw-rw-r--   0 nut       (1000) nut       (1000)     7620 2023-12-23 20:33:36.000000 detroit-1.1.0/detroit/static/svg.js
--rw-rw-r--   0 nut       (1000) nut       (1000)      579 2023-12-20 17:40:42.000000 detroit-1.1.0/detroit/static/wait.js
--rw-rw-r--   0 nut       (1000) nut       (1000)     5212 2024-03-13 18:07:48.000000 detroit-1.1.0/detroit/style.py
-drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-03-13 18:15:16.713074 detroit-1.1.0/detroit/templates/
--rw-rw-r--   0 nut       (1000) nut       (1000)      371 2023-12-20 17:40:42.000000 detroit-1.1.0/detroit/templates/base.html
--rw-rw-r--   0 nut       (1000) nut       (1000)     1149 2024-03-02 21:38:16.000000 detroit-1.1.0/detroit/templates/d3.html
--rw-rw-r--   0 nut       (1000) nut       (1000)     1452 2024-03-02 21:38:16.000000 detroit-1.1.0/detroit/templates/plot.html
--rw-rw-r--   0 nut       (1000) nut       (1000)      458 2024-03-13 18:07:48.000000 detroit-1.1.0/detroit/templates/websocket.html
--rw-rw-r--   0 nut       (1000) nut       (1000)    15895 2024-03-13 18:07:48.000000 detroit-1.1.0/detroit/ui.py
--rw-rw-r--   0 nut       (1000) nut       (1000)     6270 2024-03-13 18:07:48.000000 detroit-1.1.0/detroit/utils.py
-drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-03-13 18:15:16.717074 detroit-1.1.0/detroit.egg-info/
--rw-r--r--   0 nut       (1000) nut       (1000)     5226 2024-03-13 18:15:16.000000 detroit-1.1.0/detroit.egg-info/PKG-INFO
--rw-rw-r--   0 nut       (1000) nut       (1000)      484 2024-03-13 18:15:16.000000 detroit-1.1.0/detroit.egg-info/SOURCES.txt
--rw-rw-r--   0 nut       (1000) nut       (1000)        1 2024-03-13 18:15:16.000000 detroit-1.1.0/detroit.egg-info/dependency_links.txt
--rw-rw-r--   0 nut       (1000) nut       (1000)       68 2024-03-13 18:15:16.000000 detroit-1.1.0/detroit.egg-info/requires.txt
--rw-rw-r--   0 nut       (1000) nut       (1000)        8 2024-03-13 18:15:16.000000 detroit-1.1.0/detroit.egg-info/top_level.txt
--rw-rw-r--   0 nut       (1000) nut       (1000)      962 2024-03-13 18:08:33.000000 detroit-1.1.0/pyproject.toml
--rw-rw-r--   0 nut       (1000) nut       (1000)       38 2024-03-13 18:15:16.717074 detroit-1.1.0/setup.cfg
+drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-05-31 13:48:14.988519 detroit-1.2.0/
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1503 2023-11-25 15:13:50.000000 detroit-1.2.0/LICENSE
+-rw-rw-r--   0 nut       (1000) nut       (1000)       92 2024-05-31 13:48:11.000000 detroit-1.2.0/MANIFEST.in
+-rw-r--r--   0 nut       (1000) nut       (1000)     5226 2024-05-31 13:48:14.984518 detroit-1.2.0/PKG-INFO
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2419 2023-12-23 21:47:04.000000 detroit-1.2.0/README.md
+drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-05-31 13:48:14.972518 detroit-1.2.0/detroit/
+-rw-rw-r--   0 nut       (1000) nut       (1000)      298 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/__init__.py
+drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-05-31 13:48:14.984518 detroit-1.2.0/detroit/d3/
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1327 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/Adder.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    17782 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/Delaunay.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)   410721 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/__init__.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    52395 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/_select.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    52509 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/_selectAll.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    52509 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/_selection.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    12493 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/arc.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    12663 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/area.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     7224 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/areaRadial.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10609 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/axisBottom.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10585 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/axisLeft.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10597 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/axisRight.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10573 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/axisTop.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     5637 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/bin.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2605 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/bisector.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     8517 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/brush.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     8527 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/brushX.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     8527 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/brushY.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3210 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/chord.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3089 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/cluster.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6590 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/color.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      859 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/conic.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6377 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/contourDensity.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3849 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/contours.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2814 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveBasis.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2856 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveBasisClosed.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2842 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveBasisOpen.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2814 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveBumpX.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2814 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveBumpY.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3536 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveBundle.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3588 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveCardinal.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3636 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveCardinalClosed.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3620 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveCardinalOpen.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3699 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveCatmullRom.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3747 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveCatmullRomClosed.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3731 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveCatmullRomOpen.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2821 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveLinear.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2863 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveLinearClosed.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2842 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveMonotoneX.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2842 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveMonotoneY.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2828 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveNatural.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2807 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveStep.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2842 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveStepAfter.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2849 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/curveStepBefore.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3793 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/dispatch.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10225 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/drag.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    12175 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/dsvFormat.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      845 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeBack.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      851 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeBackIn.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      860 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeBackInOut.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      854 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeBackOut.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1386 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeElastic.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1394 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeElasticIn.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1406 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeElasticInOut.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1398 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easeElasticOut.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1113 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easePoly.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1119 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easePolyIn.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1128 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easePolyInOut.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1122 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/easePolyOut.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1628 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/event.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2133 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceCenter.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3351 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceCollide.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6765 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceLink.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     5871 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceManyBody.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3985 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceRadial.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    13950 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceSimulation.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2994 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceX.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2994 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/forceY.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3244 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/geoCircle.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4835 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/geoGraticule.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    14172 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/geoIdentity.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     8705 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/geoPath.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3599 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/geoStream.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      908 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/hsl.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1192 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/interpolateColor.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1139 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/interpolateZoom.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6996 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/line.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3166 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/lineRadial.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     5384 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/link.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     5464 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/linkHorizontal.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1333 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/linkRadial.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     5448 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/linkVertical.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3121 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/local.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10322 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/node.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3003 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/pack.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2182 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/partition.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6405 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/path.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10175 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/pie.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      795 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/project.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    14152 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/projection.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    13087 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/quadtree.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1426 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomBates.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1438 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomBernoulli.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1423 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomBeta.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1435 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomBinomial.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1429 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomCauchy.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1444 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomExponential.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1426 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomGamma.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1438 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomGeometric.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1420 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomInt.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1438 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomIrwinHall.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1438 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomLogNormal.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1435 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomLogistic.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1429 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomNormal.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1429 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomPareto.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1432 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomPoisson.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1432 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomUniform.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1432 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/randomWeibull.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      954 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/rgb.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     7655 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/ribbon.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1143 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/ribbonArrow.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     8506 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleBand.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2743 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleDiverging.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      874 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleDivergingLog.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      874 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleDivergingPow.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      878 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleDivergingSqrt.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      886 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleDivergingSymlog.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      858 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleIdentity.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      858 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleImplicit.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    11609 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleLinear.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4284 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleLog.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3157 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleOrdinal.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6448 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scalePoint.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1617 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scalePow.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4016 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleQuantile.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3681 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleQuantize.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      850 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleRadial.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     2748 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSequential.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      878 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSequentialLog.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      878 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSequentialPow.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1713 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSequentialQuantile.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      882 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSequentialSqrt.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      890 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSequentialSymlog.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      842 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSqrt.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1582 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleSymlog.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3518 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleThreshold.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4983 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleTime.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)      838 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/scaleUtc.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4789 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/stack.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4199 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/stratify.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4819 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/symbol.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1047 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/symbolType.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    10098 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/timeInterval.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1371 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/timer.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    32939 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/transition.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3316 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/tree.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     7149 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/treemap.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1657 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/treemapResquarify.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1651 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/treemapSquarify.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     9153 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/voronoi.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)    20724 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/zoom.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6761 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3/zoomTransform.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     3128 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/d3_utils.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)   103402 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/plot.py
+drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-05-31 13:48:14.984518 detroit-1.2.0/detroit/static/
+-rw-rw-r--   0 nut       (1000) nut       (1000)      493 2023-12-20 17:40:42.000000 detroit-1.2.0/detroit/static/serialize.js
+-rw-rw-r--   0 nut       (1000) nut       (1000)     7620 2023-12-23 20:33:36.000000 detroit-1.2.0/detroit/static/svg.js
+-rw-rw-r--   0 nut       (1000) nut       (1000)      579 2023-12-20 17:40:42.000000 detroit-1.2.0/detroit/static/wait.js
+-rw-rw-r--   0 nut       (1000) nut       (1000)     5212 2024-05-12 16:10:24.000000 detroit-1.2.0/detroit/style.py
+drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-05-31 13:48:14.984518 detroit-1.2.0/detroit/templates/
+-rw-rw-r--   0 nut       (1000) nut       (1000)      371 2024-05-19 16:54:15.000000 detroit-1.2.0/detroit/templates/base.html
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1149 2024-03-02 21:38:16.000000 detroit-1.2.0/detroit/templates/d3.html
+-rw-rw-r--   0 nut       (1000) nut       (1000)     1452 2024-04-04 21:01:20.000000 detroit-1.2.0/detroit/templates/plot.html
+-rw-rw-r--   0 nut       (1000) nut       (1000)      458 2024-03-13 18:07:48.000000 detroit-1.2.0/detroit/templates/websocket.html
+-rw-rw-r--   0 nut       (1000) nut       (1000)    15906 2024-05-31 13:39:53.000000 detroit-1.2.0/detroit/ui.py
+-rw-rw-r--   0 nut       (1000) nut       (1000)     6270 2024-05-04 15:36:51.000000 detroit-1.2.0/detroit/utils.py
+drwxrwxr-x   0 nut       (1000) nut       (1000)        0 2024-05-31 13:48:14.984518 detroit-1.2.0/detroit.egg-info/
+-rw-r--r--   0 nut       (1000) nut       (1000)     5226 2024-05-31 13:48:14.000000 detroit-1.2.0/detroit.egg-info/PKG-INFO
+-rw-rw-r--   0 nut       (1000) nut       (1000)     4395 2024-05-31 13:48:14.000000 detroit-1.2.0/detroit.egg-info/SOURCES.txt
+-rw-rw-r--   0 nut       (1000) nut       (1000)        1 2024-05-31 13:48:14.000000 detroit-1.2.0/detroit.egg-info/dependency_links.txt
+-rw-rw-r--   0 nut       (1000) nut       (1000)       68 2024-05-31 13:48:14.000000 detroit-1.2.0/detroit.egg-info/requires.txt
+-rw-rw-r--   0 nut       (1000) nut       (1000)        1 2024-05-31 13:48:14.000000 detroit-1.2.0/detroit.egg-info/top_level.txt
+-rw-rw-r--   0 nut       (1000) nut       (1000)      997 2024-05-31 13:47:20.000000 detroit-1.2.0/pyproject.toml
+-rw-rw-r--   0 nut       (1000) nut       (1000)       38 2024-05-31 13:48:14.988519 detroit-1.2.0/setup.cfg
```

### Comparing `detroit-1.1.0/LICENSE` & `detroit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/PKG-INFO` & `detroit-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detroit
-Version: 1.1.0
+Version: 1.2.0
 Summary: detroit is wrapper for Python of d3js and Observable Plot.
 Author-email: Benjamin BOURBON <ben.bourbon06@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Benjamin Bourbon
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: detroit Version: 1.1.0 Summary: detroit is wrapper
+Metadata-Version: 2.1 Name: detroit Version: 1.2.0 Summary: detroit is wrapper
 for Python of d3js and Observable Plot. Author-email: Benjamin BOURBON
 gmail.com> License: BSD 3-Clause License Copyright (c) 2023, Benjamin Bourbon
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `detroit-1.1.0/README.md` & `detroit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit/static/svg.js` & `detroit-1.2.0/detroit/static/svg.js`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit/static/wait.js` & `detroit-1.2.0/detroit/static/wait.js`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit/style.py` & `detroit-1.2.0/detroit/style.py`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit/templates/d3.html` & `detroit-1.2.0/detroit/templates/d3.html`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit/templates/plot.html` & `detroit-1.2.0/detroit/templates/plot.html`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit/ui.py` & `detroit-1.2.0/detroit/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 from enum import Enum, auto
 from pathlib import Path
 from typing import Dict, Generator, List, Optional, Union
 
 from markupsafe import Markup
 
-from .d3 import Script
-from .plot import Plot
+from .d3_utils import Script
+from .plot import Plot_
 from .style import CSS, GRID
 from .utils import Data, DataInput, arrange
 
-JSCode = Union[Plot, Script]
+JSCode = Union[Plot_, Script]
 JSInput = Union[Dict[str, JSCode], List[JSCode]]
 
 class PlotType(Enum):
     SINGLE_PLOT = auto()
     MULTIPLE_PLOTS = auto()
     SINGLE_D3 = auto()
     MULTIPLE_D3 = auto()
@@ -40,26 +40,26 @@
         plot javascript code
 
     Returns
     -------
     PlotType
         type of the plot
     """
-    if isinstance(plot, Plot):
+    if isinstance(plot, Plot_):
         return PlotType.SINGLE_PLOT
     elif isinstance(plot, Script):
         return PlotType.SINGLE_D3
     elif isinstance(plot, dict):
         objs = plot.values()
-        if all(map(lambda obj: isinstance(obj, Plot), objs)):
+        if all(map(lambda obj: isinstance(obj, Plot_), objs)):
             return PlotType.MULTIPLE_PLOTS
         elif all(map(lambda obj: isinstance(obj, Script), objs)):
             return PlotType.MULTIPLE_D3
     elif isinstance(plot, list):
-        if all(map(lambda obj: isinstance(obj, Plot), plot)):
+        if all(map(lambda obj: isinstance(obj, Plot_), plot)):
             return PlotType.MULTIPLE_PLOTS
         elif all(map(lambda obj: isinstance(obj, Script), plot)):
             return PlotType.MULTIPLE_D3
     return PlotType.UNIDENTIFIED
 
 async def html(data: dict, plot: JSInput, style:Union[Path, str, dict]=None, svg:bool=False, grid:int=1, event:Optional[str] = None) -> str:
     """
```

### Comparing `detroit-1.1.0/detroit/utils.py` & `detroit-1.2.0/detroit/utils.py`

 * *Files identical despite different names*

### Comparing `detroit-1.1.0/detroit.egg-info/PKG-INFO` & `detroit-1.2.0/detroit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detroit
-Version: 1.1.0
+Version: 1.2.0
 Summary: detroit is wrapper for Python of d3js and Observable Plot.
 Author-email: Benjamin BOURBON <ben.bourbon06@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Benjamin Bourbon
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: detroit Version: 1.1.0 Summary: detroit is wrapper
+Metadata-Version: 2.1 Name: detroit Version: 1.2.0 Summary: detroit is wrapper
 for Python of d3js and Observable Plot. Author-email: Benjamin BOURBON
 gmail.com> License: BSD 3-Clause License Copyright (c) 2023, Benjamin Bourbon
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `detroit-1.1.0/pyproject.toml` & `detroit-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "detroit"
 description = "detroit is wrapper for Python of d3js and Observable Plot."
-version = "1.1.0"
+version = "1.2.0"
 readme = "README.md"
 authors = [
   { name = "Benjamin BOURBON", email = "ben.bourbon06@gmail.com"},
 ]
 requires-python = ">=3.9"
 dependencies = [
   "jinja2",
@@ -28,7 +28,10 @@
 [project.urls]
 Homepage="https://github.com/bourbonut/detroit"
 Repository="https://github.com/bourbonut/detroit"
 Documentation="https://detroit.readthedocs.io/en/latest/"
 
 [project.optional-dependencies]
 jupyter = ["notebook", "nest_asyncio"]
+
+[tool.setuptools]
+py-modules = []
```

