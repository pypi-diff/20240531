# Comparing `tmp/cdnmon-0.5.5.tar.gz` & `tmp/cdnmon-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.5.5.tar", max compression
+gzip compressed data, was "cdnmon-0.5.6.tar", max compression
```

## Comparing `cdnmon-0.5.5.tar` & `cdnmon-0.5.6.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0      636 2024-05-27 12:28:59.593274 cdnmon-0.5.5/README.md
--rw-r--r--   0        0        0      609 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/__init__.py
--rw-r--r--   0        0        0     9924 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/__init__.py
--rw-r--r--   0        0        0      401 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/advancedhosting.py
--rw-r--r--   0        0        0     1870 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/akamai.py
--rw-r--r--   0        0        0    14636 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/alibaba_cdn.py
--rw-r--r--   0        0        0     2630 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/alibaba_dcdn.py
--rw-r--r--   0        0        0     1607 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/alibaba_waf.py
--rw-r--r--   0        0        0      335 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/asia_isp.py
--rw-r--r--   0        0        0      435 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/azion.py
--rw-r--r--   0        0        0     1554 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/baidu.py
--rw-r--r--   0        0        0      919 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/baishan.py
--rw-r--r--   0        0        0      427 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/bunny.py
--rw-r--r--   0        0        0      449 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/cachefly.py
--rw-r--r--   0        0        0      335 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/cdn77.py
--rw-r--r--   0        0        0      312 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/cdnetworks.py
--rw-r--r--   0        0        0      308 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/chinacache.py
--rw-r--r--   0        0        0      365 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/chinanet.py
--rw-r--r--   0        0        0     1869 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/cloudflare.py
--rw-r--r--   0        0        0     1330 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/cloudfront.py
--rw-r--r--   0        0        0     1235 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/ctyun.py
--rw-r--r--   0        0        0      515 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/douyin.py
--rw-r--r--   0        0        0      307 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/edgecast.py
--rw-r--r--   0        0        0      277 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/edgio.py
--rw-r--r--   0        0        0     2765 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/fastly.py
--rw-r--r--   0        0        0      309 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/fastly_edge_compute.py
--rw-r--r--   0        0        0     1190 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/frontdoor.py
--rw-r--r--   0        0        0     1627 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/gcore.py
--rw-r--r--   0        0        0    12774 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/huawei.py
--rw-r--r--   0        0        0      303 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/imperva.py
--rw-r--r--   0        0        0      307 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/incapsula.py
--rw-r--r--   0        0        0     5903 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/jingdong.py
--rw-r--r--   0        0        0      395 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/keycdn.py
--rw-r--r--   0        0        0     1363 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/kingsoft.py
--rw-r--r--   0        0        0      538 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/leaseweb.py
--rw-r--r--   0        0        0      406 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/limelight.py
--rw-r--r--   0        0        0      396 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/netease.py
--rw-r--r--   0        0        0     1193 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/qihoo.py
--rw-r--r--   0        0        0     3222 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/qiniu.py
--rw-r--r--   0        0        0     2233 2024-05-27 12:28:59.597274 cdnmon-0.5.5/cdnmon/model/cdn/tencent.py
--rw-r--r--   0        0        0       15 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/afx.py
--rw-r--r--   0        0        0       21 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/agile.py
--rw-r--r--   0        0        0       21 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/ananke.py
--rw-r--r--   0        0        0       61 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/aodianyun.py
--rw-r--r--   0        0        0       40 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/arvancloud.py
--rw-r--r--   0        0        0       16 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/att.py
--rw-r--r--   0        0        0      299 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/beluga.py
--rw-r--r--   0        0        0       14 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/cdnify.py
--rw-r--r--   0        0        0       29 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/cdnsun.py
--rw-r--r--   0        0        0      211 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/cdnvideo.py
--rw-r--r--   0        0        0       15 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/cotendo.py
--rw-r--r--   0        0        0       16 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/cube.py
--rw-r--r--   0        0        0       16 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/digitalink.py
--rw-r--r--   0        0        0      202 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/dnion.py
--rw-r--r--   0        0        0      211 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/edgenext.py
--rw-r--r--   0        0        0       20 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/eschoolview.py
--rw-r--r--   0        0        0       20 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/gocache.py
--rw-r--r--   0        0        0     1620 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/google.py
--rw-r--r--   0        0        0       31 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/instartlogic.py
--rw-r--r--   0        0        0       20 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/internap.py
--rw-r--r--   0        0        0       24 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/invisionpower.py
--rw-r--r--   0        0        0       41 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/jiasule.py
--rw-r--r--   0        0        0       21 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/jsdelivr.py
--rw-r--r--   0        0        0      218 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/lumen.py
--rw-r--r--   0        0        0       14 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/manmanyun.py
--rw-r--r--   0        0        0     1438 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/maxcdn.py
--rw-r--r--   0        0        0       20 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/mediacloud.py
--rw-r--r--   0        0        0      272 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/medianova.py
--rw-r--r--   0        0        0       58 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/mirrorimage.py
--rw-r--r--   0        0        0       53 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/netdna.py
--rw-r--r--   0        0        0       57 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/netlify.py
--rw-r--r--   0        0        0       15 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/ngenix.py
--rw-r--r--   0        0        0       30 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/nyiftw.py
--rw-r--r--   0        0        0       38 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/onapp.py
--rw-r--r--   0        0        0       17 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/pagerain.py
--rw-r--r--   0        0        0       17 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/presscdn.py
--rw-r--r--   0        0        0       19 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/qinglanyun.py
--rw-r--r--   0        0        0      127 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/stackpath.py
--rw-r--r--   0        0        0      215 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/tata.py
--rw-r--r--   0        0        0       38 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/thunderbird.py
--rw-r--r--   0        0        0      224 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/todo/verizon.py
--rw-r--r--   0        0        0     1366 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/ucloud.py
--rw-r--r--   0        0        0     2894 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/upyun.py
--rw-r--r--   0        0        0      432 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/volc.py
--rw-r--r--   0        0        0    15882 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/wangsu.py
--rw-r--r--   0        0        0      327 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/model/cdn/xiaomi.py
--rw-r--r--   0        0        0      691 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/util/aws.py
--rw-r--r--   0        0        0     1051 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/util/bgpview.py
--rw-r--r--   0        0        0      389 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/util/cidr.py
--rw-r--r--   0        0        0      258 2024-05-27 12:28:59.601274 cdnmon-0.5.5/cdnmon/util/db.py
--rw-r--r--   0        0        0      531 2024-05-27 12:28:59.601274 cdnmon-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 cdnmon-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      761 2024-05-31 11:15:58.479292 cdnmon-0.5.6/README.md
+-rw-r--r--   0        0        0      609 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/__init__.py
+-rw-r--r--   0        0        0     9924 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/advancedhosting.py
+-rw-r--r--   0        0        0     1870 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/akamai.py
+-rw-r--r--   0        0        0    14636 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/alibaba_cdn.py
+-rw-r--r--   0        0        0     2630 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/alibaba_dcdn.py
+-rw-r--r--   0        0        0     1607 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/alibaba_waf.py
+-rw-r--r--   0        0        0      335 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/asia_isp.py
+-rw-r--r--   0        0        0      435 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/azion.py
+-rw-r--r--   0        0        0     1554 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/baidu.py
+-rw-r--r--   0        0        0      919 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/baishan.py
+-rw-r--r--   0        0        0      427 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/bunny.py
+-rw-r--r--   0        0        0      712 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/byteplus.py
+-rw-r--r--   0        0        0      449 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/cachefly.py
+-rw-r--r--   0        0        0      335 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/cdn77.py
+-rw-r--r--   0        0        0      312 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/cdnetworks.py
+-rw-r--r--   0        0        0      308 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/chinacache.py
+-rw-r--r--   0        0        0      365 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/chinanet.py
+-rw-r--r--   0        0        0     1869 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/cloudflare.py
+-rw-r--r--   0        0        0     1358 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/cloudfront.py
+-rw-r--r--   0        0        0     1235 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/ctyun.py
+-rw-r--r--   0        0        0      515 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/douyin.py
+-rw-r--r--   0        0        0      307 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/edgecast.py
+-rw-r--r--   0        0        0      277 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/edgio.py
+-rw-r--r--   0        0        0     2765 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/fastly.py
+-rw-r--r--   0        0        0      309 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/fastly_edge_compute.py
+-rw-r--r--   0        0        0     1190 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/frontdoor.py
+-rw-r--r--   0        0        0     1627 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/gcore.py
+-rw-r--r--   0        0        0    12774 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/huawei.py
+-rw-r--r--   0        0        0      303 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/imperva.py
+-rw-r--r--   0        0        0      307 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/incapsula.py
+-rw-r--r--   0        0        0     5903 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/jingdong.py
+-rw-r--r--   0        0        0      395 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/keycdn.py
+-rw-r--r--   0        0        0     1363 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/kingsoft.py
+-rw-r--r--   0        0        0      538 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/leaseweb.py
+-rw-r--r--   0        0        0      406 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/limelight.py
+-rw-r--r--   0        0        0      396 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/netease.py
+-rw-r--r--   0        0        0     1193 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/qihoo.py
+-rw-r--r--   0        0        0     3222 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/qiniu.py
+-rw-r--r--   0        0        0     2233 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/tencent.py
+-rw-r--r--   0        0        0       15 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/afx.py
+-rw-r--r--   0        0        0       21 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/agile.py
+-rw-r--r--   0        0        0       21 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/ananke.py
+-rw-r--r--   0        0        0       61 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/aodianyun.py
+-rw-r--r--   0        0        0       40 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/arvancloud.py
+-rw-r--r--   0        0        0       16 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/att.py
+-rw-r--r--   0        0        0      299 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/beluga.py
+-rw-r--r--   0        0        0       14 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/cdnify.py
+-rw-r--r--   0        0        0       29 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/cdnsun.py
+-rw-r--r--   0        0        0      211 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/cdnvideo.py
+-rw-r--r--   0        0        0       15 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/cotendo.py
+-rw-r--r--   0        0        0       16 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/cube.py
+-rw-r--r--   0        0        0       16 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/digitalink.py
+-rw-r--r--   0        0        0      202 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/dnion.py
+-rw-r--r--   0        0        0      211 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/edgenext.py
+-rw-r--r--   0        0        0       20 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/eschoolview.py
+-rw-r--r--   0        0        0       20 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/gocache.py
+-rw-r--r--   0        0        0     1620 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/google.py
+-rw-r--r--   0        0        0       31 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/instartlogic.py
+-rw-r--r--   0        0        0       20 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/internap.py
+-rw-r--r--   0        0        0       24 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/invisionpower.py
+-rw-r--r--   0        0        0       41 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/jiasule.py
+-rw-r--r--   0        0        0       21 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/jsdelivr.py
+-rw-r--r--   0        0        0      218 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/lumen.py
+-rw-r--r--   0        0        0       14 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/manmanyun.py
+-rw-r--r--   0        0        0     1438 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/maxcdn.py
+-rw-r--r--   0        0        0       20 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/mediacloud.py
+-rw-r--r--   0        0        0      272 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/medianova.py
+-rw-r--r--   0        0        0       58 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/mirrorimage.py
+-rw-r--r--   0        0        0       53 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/netdna.py
+-rw-r--r--   0        0        0       57 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/netlify.py
+-rw-r--r--   0        0        0       15 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/ngenix.py
+-rw-r--r--   0        0        0       30 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/nyiftw.py
+-rw-r--r--   0        0        0       38 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/onapp.py
+-rw-r--r--   0        0        0       17 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/pagerain.py
+-rw-r--r--   0        0        0       17 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/presscdn.py
+-rw-r--r--   0        0        0       19 2024-05-31 11:15:58.483292 cdnmon-0.5.6/cdnmon/model/cdn/todo/qinglanyun.py
+-rw-r--r--   0        0        0      127 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/todo/stackpath.py
+-rw-r--r--   0        0        0      215 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/todo/tata.py
+-rw-r--r--   0        0        0       38 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/todo/thunderbird.py
+-rw-r--r--   0        0        0      224 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/todo/verizon.py
+-rw-r--r--   0        0        0     1366 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/ucloud.py
+-rw-r--r--   0        0        0     2894 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/upyun.py
+-rw-r--r--   0        0        0      432 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/volc.py
+-rw-r--r--   0        0        0    15882 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/wangsu.py
+-rw-r--r--   0        0        0      327 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/model/cdn/xiaomi.py
+-rw-r--r--   0        0        0      691 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/util/aws.py
+-rw-r--r--   0        0        0     1051 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/util/bgpview.py
+-rw-r--r--   0        0        0      389 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/util/cidr.py
+-rw-r--r--   0        0        0      258 2024-05-31 11:15:58.487292 cdnmon-0.5.6/cdnmon/util/db.py
+-rw-r--r--   0        0        0      531 2024-05-31 11:15:58.487292 cdnmon-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 cdnmon-0.5.6/PKG-INFO
```

### Comparing `cdnmon-0.5.5/README.md` & `cdnmon-0.5.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 # Get an example subscriber domain of the given CDN
 cloudflare.subscribers()
 ```
 
 ## TODO
 
 - [ ] Support downloading ingress / egress nodes list
+- [ ] Add `unchanged_since` in `index.html`
+- [ ] Change `updated_at` in `index.html`
+- [ ] Add example code in `index.html`
 - [x] Add type annotations
 
 ## FAQ
 
 ### How to obtain an access token?
 
 Please contact <wangyihanger@gmail.com>.
```

### Comparing `cdnmon-0.5.5/cdnmon/__init__.py` & `cdnmon-0.5.6/cdnmon/__init__.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/__init__.py` & `cdnmon-0.5.6/cdnmon/model/cdn/__init__.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/akamai.py` & `cdnmon-0.5.6/cdnmon/model/cdn/akamai.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/alibaba_cdn.py` & `cdnmon-0.5.6/cdnmon/model/cdn/alibaba_cdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/alibaba_dcdn.py` & `cdnmon-0.5.6/cdnmon/model/cdn/alibaba_dcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/alibaba_waf.py` & `cdnmon-0.5.6/cdnmon/model/cdn/alibaba_waf.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/baidu.py` & `cdnmon-0.5.6/cdnmon/model/cdn/baidu.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/baishan.py` & `cdnmon-0.5.6/cdnmon/model/cdn/baishan.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/cloudflare.py` & `cdnmon-0.5.6/cdnmon/model/cdn/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/cloudfront.py` & `cdnmon-0.5.6/cdnmon/model/cdn/cloudfront.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,12 +28,12 @@
         }
 
 
 CDN = CommonCDN(
     name="cloudfront",
     asn_patterns=["cloudfront", "amazon"],
     cname_suffixes=[
-        CNAMEPattern(suffix=".cloudfront.net"),
+        CNAMEPattern(suffix=".cloudfront.net", is_root=True, is_leaf=True),
         CNAMEPattern(suffix=".cloudfront.cn"),
     ],
     cidr=CloudFrontCIDR(),
 )
```

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/ctyun.py` & `cdnmon-0.5.6/cdnmon/model/cdn/ctyun.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/douyin.py` & `cdnmon-0.5.6/cdnmon/model/cdn/douyin.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/fastly.py` & `cdnmon-0.5.6/cdnmon/model/cdn/fastly.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/frontdoor.py` & `cdnmon-0.5.6/cdnmon/model/cdn/frontdoor.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/gcore.py` & `cdnmon-0.5.6/cdnmon/model/cdn/gcore.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/huawei.py` & `cdnmon-0.5.6/cdnmon/model/cdn/huawei.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/jingdong.py` & `cdnmon-0.5.6/cdnmon/model/cdn/jingdong.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/kingsoft.py` & `cdnmon-0.5.6/cdnmon/model/cdn/kingsoft.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/leaseweb.py` & `cdnmon-0.5.6/cdnmon/model/cdn/leaseweb.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/qihoo.py` & `cdnmon-0.5.6/cdnmon/model/cdn/qihoo.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/qiniu.py` & `cdnmon-0.5.6/cdnmon/model/cdn/qiniu.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/tencent.py` & `cdnmon-0.5.6/cdnmon/model/cdn/tencent.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/todo/google.py` & `cdnmon-0.5.6/cdnmon/model/cdn/todo/google.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/todo/maxcdn.py` & `cdnmon-0.5.6/cdnmon/model/cdn/todo/maxcdn.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/ucloud.py` & `cdnmon-0.5.6/cdnmon/model/cdn/ucloud.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/upyun.py` & `cdnmon-0.5.6/cdnmon/model/cdn/upyun.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/model/cdn/wangsu.py` & `cdnmon-0.5.6/cdnmon/model/cdn/wangsu.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/util/aws.py` & `cdnmon-0.5.6/cdnmon/util/aws.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/cdnmon/util/bgpview.py` & `cdnmon-0.5.6/cdnmon/util/bgpview.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.5.5/pyproject.toml` & `cdnmon-0.5.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdnmon"
-version = "0.5.5"
+version = "0.5.6"
 description = ""
 authors = ["Yihang Wang <wangyihanger@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `cdnmon-0.5.5/PKG-INFO` & `cdnmon-0.5.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.5.5
+Version: 0.5.6
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -46,14 +46,17 @@
 # Get an example subscriber domain of the given CDN
 cloudflare.subscribers()
 ```
 
 ## TODO
 
 - [ ] Support downloading ingress / egress nodes list
+- [ ] Add `unchanged_since` in `index.html`
+- [ ] Change `updated_at` in `index.html`
+- [ ] Add example code in `index.html`
 - [x] Add type annotations
 
 ## FAQ
 
 ### How to obtain an access token?
 
 Please contact <wangyihanger@gmail.com>.
```

