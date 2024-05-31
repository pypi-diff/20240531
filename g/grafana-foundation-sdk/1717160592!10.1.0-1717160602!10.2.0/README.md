# Comparing `tmp/grafana_foundation_sdk-1717160592!10.1.0.tar.gz` & `tmp/grafana_foundation_sdk-1717160602!10.2.0.tar.gz`

## Comparing `grafana_foundation_sdk-1717160592!10.1.0.tar` & `grafana_foundation_sdk-1717160602!10.2.0.tar`

### file list

```diff
@@ -1,109 +1,107 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    18535 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/alertgroups.py
--rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/alerting.py
--rw-r--r--   0        0        0    20414 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    37625 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    20170 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    47608 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    48574 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    76202 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    20296 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    63438 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0    50546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/expr.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/folder.py
--rw-r--r--   0        0        0    19181 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    19072 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    31190 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/playlist.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    23046 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    22763 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    19916 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    18178 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    45683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    45406 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    35041 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/alertgroups.py
--rw-r--r--   0        0        0    27377 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/alerting.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    13569 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    84497 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    88204 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    91769 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0    66523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/expr.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/folder.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    32298 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    20031 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/playlist.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    20860 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160592!10.1.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    19134 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/alerting.py
+-rw-r--r--   0        0        0    21013 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    39082 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    21782 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    49071 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    19196 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    49221 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    71606 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    21328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    18505 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    63438 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    50546 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/expr.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/folder.py
+-rw-r--r--   0        0        0    20746 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    19671 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    19922 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    29259 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    32649 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    20580 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    18581 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    18530 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    20698 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    23645 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    28284 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    12358 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    18777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    47144 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    46857 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    36496 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0    27221 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/alerting.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    13660 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    86153 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    85474 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    91769 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0    66523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/expr.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/folder.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    27647 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    20787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0    10653 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    21201 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    17916 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1717160602!10.2.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/alertgroups.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/alertgroups.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/alerting.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/alerting.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,18 @@
         if not len(title) <= 190:
             raise ValueError("len(title) must be <= 190")
         self._internal.title = title
     
         return self
     
     def uid(self, uid: str) -> typing.Self:        
+        if not len(uid) >= 1:
+            raise ValueError("len(uid) must be >= 1")
+        if not len(uid) <= 40:
+            raise ValueError("len(uid) must be <= 40")
         self._internal.uid = uid
     
         return self
     
     def updated(self, updated: str) -> typing.Self:        
         self._internal.updated = updated
     
@@ -431,14 +435,18 @@
     
     def uid(self, uid: str) -> typing.Self:    
         """
         EmbeddedContactPoint is the contact point type that is used
         by grafanas embedded alertmanager implementation.
         """
             
+        if not len(uid) >= 1:
+            raise ValueError("len(uid) must be >= 1")
+        if not len(uid) <= 40:
+            raise ValueError("len(uid) must be <= 40")
         self._internal.uid = uid
     
         return self
     
 
 class NotificationPolicy(cogbuilder.Builder[alerting.NotificationPolicy]):    
     """
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,26 +367,35 @@
         Array of resource URIs to be queried.
         """
             
         self._internal.resources = resources
     
         return self
     
-    def intersect_time(self, intersect_time: bool) -> typing.Self:    
+    def dashboard_time(self, dashboard_time: bool) -> typing.Self:    
         """
-        If set to true the intersection of time ranges specified in the query and Grafana will be used. Otherwise the query time ranges will be used. Defaults to false
+        If set to true the dashboard time range will be used as a filter for the query. Otherwise the query time ranges will be used. Defaults to false.
         """
             
-        self._internal.intersect_time = intersect_time
+        self._internal.dashboard_time = dashboard_time
+    
+        return self
+    
+    def time_column(self, time_column: str) -> typing.Self:    
+        """
+        If dashboardTime is set to true this value dictates which column the time filter will be applied to. Defaults to the first tables timeSpan column, the first datetime column found, or TimeGenerated
+        """
+            
+        self._internal.time_column = time_column
     
         return self
     
     def workspace(self, workspace: str) -> typing.Self:    
         """
-        Workspace ID. This was removed in Grafana 8, but remains for backwards compat
+        Workspace ID. This was removed in Grafana 8, but remains for backwards compat.
         """
             
         self._internal.workspace = workspace
     
         return self
     
     def resource(self, resource: str) -> typing.Self:    
@@ -394,14 +403,23 @@
         @deprecated Use resources instead
         """
             
         self._internal.resource = resource
     
         return self
     
+    def intersect_time(self, intersect_time: bool) -> typing.Self:    
+        """
+        @deprecated Use dashboardTime instead
+        """
+            
+        self._internal.intersect_time = intersect_time
+    
+        return self
+    
 
 class AzureTracesQuery(cogbuilder.Builder[azuremonitor.AzureTracesQuery]):    
     """
     Application Insights Traces sub-query properties
     """
     
     _internal: azuremonitor.AzureTracesQuery
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -780,14 +799,28 @@
             self._internal.field_config.defaults.custom = barchart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = barchart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -814,21 +847,21 @@
             self._internal.field_config.defaults.custom = barchart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
         thresholds_style_resource = thresholds_style.build()
         self._internal.field_config.defaults.custom.thresholds_style = thresholds_style_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = barchart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, barchart.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/gauge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
+from ..models import gauge
 from ..models import common
-from ..models import bargauge
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "bargauge"
+        self._internal.type_val = "gauge"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -417,73 +436,73 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def display_mode(self, display_mode: common.BarGaugeDisplayMode) -> typing.Self:        
+    def show_threshold_labels(self, show_threshold_labels: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.display_mode = display_mode
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
+        self._internal.options.show_threshold_labels = show_threshold_labels
     
         return self
     
-    def value_mode(self, value_mode: common.BarGaugeValueMode) -> typing.Self:        
+    def show_threshold_markers(self, show_threshold_markers: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.value_mode = value_mode
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
+        self._internal.options.show_threshold_markers = show_threshold_markers
     
         return self
     
-    def show_unfilled(self, show_unfilled: bool) -> typing.Self:        
+    def sizing(self, sizing: common.BarGaugeSizing) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
-        self._internal.options.show_unfilled = show_unfilled
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
+        self._internal.options.sizing = sizing
     
         return self
     
     def min_viz_width(self, min_viz_width: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
         self._internal.options.min_viz_width = min_viz_width
     
         return self
     
     def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
         reduce_options_resource = reduce_options.build()
         self._internal.options.reduce_options = reduce_options_resource
     
         return self
     
     def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
         text_resource = text.build()
         self._internal.options.text = text_resource
     
         return self
     
     def min_viz_height(self, min_viz_height: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
         self._internal.options.min_viz_height = min_viz_height
     
         return self
     
     def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = bargauge.Options()
-        assert isinstance(self._internal.options, bargauge.Options)
+            self._internal.options = gauge.Options()
+        assert isinstance(self._internal.options, gauge.Options)
         self._internal.options.orientation = orientation
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -781,14 +800,28 @@
             self._internal.field_config.defaults.custom = candlestick.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = candlestick.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -901,25 +934,25 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = candlestick.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = candlestick.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, candlestick.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,14 +618,19 @@
         return self
     
     def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
         self._internal.axis_centered_zero = axis_centered_zero
     
         return self
     
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+        self._internal.axis_border_show = axis_border_show
+    
+        return self
+    
 
 class HideSeriesConfig(cogbuilder.Builder[common.HideSeriesConfig]):    
     """
     TODO docs
     """
     
     _internal: common.HideSeriesConfig
@@ -1039,14 +1044,19 @@
     
     def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
         scale_distribution_resource = scale_distribution.build()
         self._internal.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        self._internal.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         self._internal.bar_alignment = bar_alignment
     
         return self
     
     def bar_width_factor(self, bar_width_factor: float) -> typing.Self:        
         self._internal.bar_width_factor = bar_width_factor
@@ -1087,16 +1097,16 @@
         return self
     
     def point_symbol(self, point_symbol: str) -> typing.Self:        
         self._internal.point_symbol = point_symbol
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        self._internal.axis_centered_zero = axis_centered_zero
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+        self._internal.axis_border_show = axis_border_show
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         self._internal.bar_max_width = bar_max_width
     
         return self
@@ -1403,14 +1413,19 @@
     
     def scale_distribution(self, scale_distribution: cogbuilder.Builder[common.ScaleDistributionConfig]) -> typing.Self:        
         scale_distribution_resource = scale_distribution.build()
         self._internal.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        self._internal.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         self._internal.bar_alignment = bar_alignment
     
         return self
     
     def bar_width_factor(self, bar_width_factor: float) -> typing.Self:        
         self._internal.bar_width_factor = bar_width_factor
@@ -1425,14 +1440,19 @@
     
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         hide_from_resource = hide_from.build()
         self._internal.hide_from = hide_from_resource
     
         return self
     
+    def hide_value(self, hide_value: bool) -> typing.Self:        
+        self._internal.hide_value = hide_value
+    
+        return self
+    
     def transform(self, transform: common.GraphTransform) -> typing.Self:        
         self._internal.transform = transform
     
         return self
     
     def span_nulls(self, span_nulls: typing.Union[bool, float]) -> typing.Self:    
         """
@@ -1451,16 +1471,16 @@
         return self
     
     def point_symbol(self, point_symbol: str) -> typing.Self:        
         self._internal.point_symbol = point_symbol
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
-        self._internal.axis_centered_zero = axis_centered_zero
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
+        self._internal.axis_border_show = axis_border_show
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         self._internal.bar_max_width = bar_max_width
     
         return self
@@ -1690,14 +1710,14 @@
     def filterable(self, filterable: bool) -> typing.Self:        
         self._internal.filterable = filterable
     
         return self
     
     def hide_header(self, hide_header: bool) -> typing.Self:    
         """
-        Hides any header for a column, usefull for columns that show some static content or buttons.
+        Hides any header for a column, useful for columns that show some static content or buttons.
         """
             
         self._internal.hide_header = hide_header
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,24 +80,14 @@
         Tags associated with dashboard.
         """
             
         self._internal.tags = tags
     
         return self
     
-    def style(self, style: typing.Literal["light", "dark"]) -> typing.Self:    
-        """
-        Theme of dashboard.
-        Default value: dark.
-        """
-            
-        self._internal.style = style
-    
-        return self
-    
     def timezone(self, timezone: str) -> typing.Self:    
         """
         Timezone of dashboard. Accepted values are IANA TZDB zone ID or "browser" or "utc".
         """
             
         self._internal.timezone = timezone
     
@@ -144,15 +134,15 @@
         if self._internal.time is None:
             self._internal.time = dashboard.DashboardDashboardTime()
         assert isinstance(self._internal.time, dashboard.DashboardDashboardTime)
         self._internal.time.to = to
     
         return self
     
-    def timepicker(self, timepicker: cogbuilder.Builder[dashboard.TimePicker]) -> typing.Self:    
+    def timepicker(self, timepicker: cogbuilder.Builder[dashboard.TimePickerConfig]) -> typing.Self:    
         """
         Configuration of the time picker shown at the top of a dashboard.
         """
             
         timepicker_resource = timepicker.build()
         self._internal.timepicker = timepicker_resource
     
@@ -546,14 +536,23 @@
         TODO -- this should not exist here, it is based on the --grafana-- datasource
         """
             
         self._internal.type_val = type_val
     
         return self
     
+    def built_in(self, built_in: float) -> typing.Self:    
+        """
+        Set to 1 for the standard annotation query all dashboards have by default.
+        """
+            
+        self._internal.built_in = built_in
+    
+        return self
+    
 
 class DashboardLink(cogbuilder.Builder[dashboard.DashboardLink]):    
     """
     Links with references to other dashboards or external resources
     """
     
     _internal: dashboard.DashboardLink
@@ -825,14 +824,56 @@
     def options(self, options: cogbuilder.Builder[dashboard.DashboardSpecialValueMapOptions]) -> typing.Self:        
         options_resource = options.build()
         self._internal.options = options_resource
     
         return self
     
 
+class TimePicker(cogbuilder.Builder[dashboard.TimePickerConfig]):    
+    """
+    Time picker configuration
+    It defines the default config for the time picker and the refresh picker for the specific dashboard.
+    """
+    
+    _internal: dashboard.TimePickerConfig
+
+    def __init__(self):
+        self._internal = dashboard.TimePickerConfig()
+
+    def build(self) -> dashboard.TimePickerConfig:
+        return self._internal    
+    
+    def hidden(self, hidden: bool) -> typing.Self:    
+        """
+        Whether timepicker is visible or not.
+        """
+            
+        self._internal.hidden = hidden
+    
+        return self
+    
+    def refresh_intervals(self, refresh_intervals: list[str]) -> typing.Self:    
+        """
+        Interval options available in the refresh picker dropdown.
+        """
+            
+        self._internal.refresh_intervals = refresh_intervals
+    
+        return self
+    
+    def time_options(self, time_options: list[str]) -> typing.Self:    
+        """
+        Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
+        """
+            
+        self._internal.time_options = time_options
+    
+        return self
+    
+
 class Snapshot(cogbuilder.Builder[dashboard.Snapshot]):    
     """
     A dashboard snapshot shares an interactive dashboard publicly.
     It is a read-only version of a dashboard, and is not editable.
     It is possible to create a snapshot of a snapshot.
     Grafana strips away all sensitive information from the dashboard.
     Sensitive information stripped: queries (metric, template,annotation) and panel links.
@@ -1081,14 +1122,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -1155,14 +1206,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -1428,95 +1488,14 @@
         """
             
         self._internal.repeat = repeat
     
         return self
     
 
-class GraphPanel(cogbuilder.Builder[dashboard.GraphPanel]):    
-    """
-    Support for legacy graph panel.
-    @deprecated this a deprecated panel type
-    """
-    
-    _internal: dashboard.GraphPanel
-
-    def __init__(self):
-        self._internal = dashboard.GraphPanel()        
-        self._internal.type_val = "graph"
-
-    def build(self) -> dashboard.GraphPanel:
-        return self._internal    
-    
-    def legend(self, legend: cogbuilder.Builder[dashboard.DashboardGraphPanelLegend]) -> typing.Self:    
-        """
-        @deprecated this is part of deprecated graph panel
-        """
-            
-        legend_resource = legend.build()
-        self._internal.legend = legend_resource
-    
-        return self
-    
-
-class TimePicker(cogbuilder.Builder[dashboard.TimePicker]):    
-    _internal: dashboard.TimePicker
-
-    def __init__(self):
-        self._internal = dashboard.TimePicker()
-
-    def build(self) -> dashboard.TimePicker:
-        return self._internal    
-    
-    def hidden(self, hidden: bool) -> typing.Self:    
-        """
-        Whether timepicker is visible or not.
-        """
-            
-        self._internal.hidden = hidden
-    
-        return self
-    
-    def refresh_intervals(self, refresh_intervals: list[str]) -> typing.Self:    
-        """
-        Interval options available in the refresh picker dropdown.
-        """
-            
-        self._internal.refresh_intervals = refresh_intervals
-    
-        return self
-    
-    def collapse(self, collapse: bool) -> typing.Self:    
-        """
-        Whether timepicker is collapsed or not. Has no effect on provisioned dashboard.
-        """
-            
-        self._internal.collapse = collapse
-    
-        return self
-    
-    def enable(self, enable: bool) -> typing.Self:    
-        """
-        Whether timepicker is enabled or not. Has no effect on provisioned dashboard.
-        """
-            
-        self._internal.enable = enable
-    
-        return self
-    
-    def time_options(self, time_options: list[str]) -> typing.Self:    
-        """
-        Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
-        """
-            
-        self._internal.time_options = time_options
-    
-        return self
-    
-
 class DashboardDashboardTemplating(cogbuilder.Builder[dashboard.DashboardDashboardTemplating]):    
     _internal: dashboard.DashboardDashboardTemplating
 
     def __init__(self):
         self._internal = dashboard.DashboardDashboardTemplating()
 
     def build(self) -> dashboard.DashboardDashboardTemplating:
@@ -1642,39 +1621,14 @@
     
     def properties(self, properties: list[dashboard.DynamicConfigValue]) -> typing.Self:        
         self._internal.properties = properties
     
         return self
     
 
-class DashboardGraphPanelLegend(cogbuilder.Builder[dashboard.DashboardGraphPanelLegend]):    
-    _internal: dashboard.DashboardGraphPanelLegend
-
-    def __init__(self):
-        self._internal = dashboard.DashboardGraphPanelLegend()
-
-    def build(self) -> dashboard.DashboardGraphPanelLegend:
-        return self._internal    
-    
-    def show(self, show: bool) -> typing.Self:        
-        self._internal.show = show
-    
-        return self
-    
-    def sort(self, sort: str) -> typing.Self:        
-        self._internal.sort = sort
-    
-        return self
-    
-    def sort_desc(self, sort_desc: bool) -> typing.Self:        
-        self._internal.sort_desc = sort_desc
-    
-        return self
-    
-
 class QueryVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
 
@@ -1682,23 +1636,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.QUERY
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1745,23 +1690,14 @@
         Data source used to fetch values for a variable. It can be defined but `null`.
         """
             
         self._internal.datasource = datasource
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -1843,23 +1779,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.ADHOC
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1897,23 +1824,14 @@
         Data source used to fetch values for a variable. It can be defined but `null`.
         """
             
         self._internal.datasource = datasource
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
 
 class ConstantVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -1922,23 +1840,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.CONSTANT
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -1967,23 +1876,14 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
 
 class DatasourceVariable(cogbuilder.Builder[dashboard.VariableModel]):    
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
     
     _internal: dashboard.VariableModel
@@ -1992,23 +1892,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.DATASOURCE
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2046,23 +1937,14 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -2117,23 +1999,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.INTERVAL
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2171,23 +2044,14 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -2214,23 +2078,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.TEXTBOX
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2268,23 +2123,14 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
     
@@ -2311,23 +2157,14 @@
         self._internal = dashboard.VariableModel()        
         self._internal.name = name        
         self._internal.type_val = dashboard.VariableType.CUSTOM
 
     def build(self) -> dashboard.VariableModel:
         return self._internal    
     
-    def id_val(self, id_val: str) -> typing.Self:    
-        """
-        Unique numeric identifier for the variable.
-        """
-            
-        self._internal.id_val = id_val
-    
-        return self
-    
     def name(self, name: str) -> typing.Self:    
         """
         Name of variable
         """
             
         self._internal.name = name
     
@@ -2365,23 +2202,14 @@
         Query used to fetch values for a variable
         """
             
         self._internal.query = query
     
         return self
     
-    def all_format(self, all_format: str) -> typing.Self:    
-        """
-        Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-        """
-            
-        self._internal.all_format = all_format
-    
-        return self
-    
     def current(self, current: dashboard.VariableOption) -> typing.Self:    
         """
         Shows current selected variable text/value on the dashboard
         """
             
         self._internal.current = current
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/dashboardlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -480,15 +499,27 @@
         if self._internal.options is None:
             self._internal.options = dashboardlist.Options()
         assert isinstance(self._internal.options, dashboardlist.Options)
         self._internal.options.query = query
     
         return self
     
-    def folder_id(self, folder_id: int) -> typing.Self:        
+    def folder_id(self, folder_id: int) -> typing.Self:    
+        """
+        folderId is deprecated, and migrated to folderUid on panel init
+        """
+            
         if self._internal.options is None:
             self._internal.options = dashboardlist.Options()
         assert isinstance(self._internal.options, dashboardlist.Options)
         self._internal.options.folder_id = folder_id
     
         return self
+    
+    def folder_uid(self, folder_uid: str) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = dashboardlist.Options()
+        assert isinstance(self._internal.options, dashboardlist.Options)
+        self._internal.options.folder_uid = folder_uid
+    
+        return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/expr.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/expr.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/folder.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/folder.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import gauge
+from ..models import geomap
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "gauge"
+        self._internal.type_val = "geomap"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -417,49 +436,49 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def show_threshold_labels(self, show_threshold_labels: bool) -> typing.Self:        
+    def view(self, view: geomap.MapViewConfig) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.show_threshold_labels = show_threshold_labels
+            self._internal.options = geomap.Options()
+        assert isinstance(self._internal.options, geomap.Options)
+        self._internal.options.view = view
     
         return self
     
-    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
+    def controls(self, controls: geomap.ControlsOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        reduce_options_resource = reduce_options.build()
-        self._internal.options.reduce_options = reduce_options_resource
+            self._internal.options = geomap.Options()
+        assert isinstance(self._internal.options, geomap.Options)
+        self._internal.options.controls = controls
     
         return self
     
-    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
+    def basemap(self, basemap: cogbuilder.Builder[common.MapLayerOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        text_resource = text.build()
-        self._internal.options.text = text_resource
+            self._internal.options = geomap.Options()
+        assert isinstance(self._internal.options, geomap.Options)
+        basemap_resource = basemap.build()
+        self._internal.options.basemap = basemap_resource
     
         return self
     
-    def show_threshold_markers(self, show_threshold_markers: bool) -> typing.Self:        
+    def layers(self, layers: list[cogbuilder.Builder[common.MapLayerOptions]]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.show_threshold_markers = show_threshold_markers
+            self._internal.options = geomap.Options()
+        assert isinstance(self._internal.options, geomap.Options)
+        layers_resources = [r1.build() for r1 in layers]
+        self._internal.options.layers = layers_resources
     
         return self
     
-    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
+    def tooltip(self, tooltip: geomap.TooltipOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = gauge.Options()
-        assert isinstance(self._internal.options, gauge.Options)
-        self._internal.options.orientation = orientation
+            self._internal.options = geomap.Options()
+        assert isinstance(self._internal.options, geomap.Options)
+        self._internal.options.tooltip = tooltip
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/stat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import geomap
 from ..models import common
+from ..models import stat
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "geomap"
+        self._internal.type_val = "stat"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -417,49 +436,73 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def view(self, view: geomap.MapViewConfig) -> typing.Self:        
+    def graph_mode(self, graph_mode: common.BigValueGraphMode) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        self._internal.options.graph_mode = graph_mode
+    
+        return self
+    
+    def color_mode(self, color_mode: common.BigValueColorMode) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        self._internal.options.color_mode = color_mode
+    
+        return self
+    
+    def justify_mode(self, justify_mode: common.BigValueJustifyMode) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        self._internal.options.justify_mode = justify_mode
+    
+        return self
+    
+    def text_mode(self, text_mode: common.BigValueTextMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
-        assert isinstance(self._internal.options, geomap.Options)
-        self._internal.options.view = view
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        self._internal.options.text_mode = text_mode
     
         return self
     
-    def controls(self, controls: geomap.ControlsOptions) -> typing.Self:        
+    def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
-        assert isinstance(self._internal.options, geomap.Options)
-        self._internal.options.controls = controls
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        reduce_options_resource = reduce_options.build()
+        self._internal.options.reduce_options = reduce_options_resource
     
         return self
     
-    def basemap(self, basemap: cogbuilder.Builder[common.MapLayerOptions]) -> typing.Self:        
+    def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
-        assert isinstance(self._internal.options, geomap.Options)
-        basemap_resource = basemap.build()
-        self._internal.options.basemap = basemap_resource
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        text_resource = text.build()
+        self._internal.options.text = text_resource
     
         return self
     
-    def layers(self, layers: list[cogbuilder.Builder[common.MapLayerOptions]]) -> typing.Self:        
+    def wide_layout(self, wide_layout: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
-        assert isinstance(self._internal.options, geomap.Options)
-        layers_resources = [r1.build() for r1 in layers]
-        self._internal.options.layers = layers_resources
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        self._internal.options.wide_layout = wide_layout
     
         return self
     
-    def tooltip(self, tooltip: geomap.TooltipOptions) -> typing.Self:        
+    def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = geomap.Options()
-        assert isinstance(self._internal.options, geomap.Options)
-        self._internal.options.tooltip = tooltip
+            self._internal.options = stat.Options()
+        assert isinstance(self._internal.options, stat.Options)
+        self._internal.options.orientation = orientation
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,24 @@
         """
             
         slo_query_resource = slo_query.build()
         self._internal.slo_query = slo_query_resource
     
         return self
     
+    def prom_ql_query(self, prom_ql_query: cogbuilder.Builder[googlecloudmonitoring.PromQLQuery]) -> typing.Self:    
+        """
+        PromQL sub-query properties.
+        """
+            
+        prom_ql_query_resource = prom_ql_query.build()
+        self._internal.prom_ql_query = prom_ql_query_resource
+    
+        return self
+    
     def datasource(self, datasource: object) -> typing.Self:    
         """
         For mixed data sources the selected datasource is on the query level.
         For non mixed scenarios this is undefined.
         TODO find a better way to do this ^ that's friendly to schema
         TODO this shouldn't be unknown but DataSourceRef | null
         """
@@ -181,59 +191,14 @@
         Data view, defaults to FULL.
         """
             
         self._internal.view = view
     
         return self
     
-    def secondary_cross_series_reducer(self, secondary_cross_series_reducer: str) -> typing.Self:    
-        """
-        Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
-        """
-            
-        self._internal.secondary_cross_series_reducer = secondary_cross_series_reducer
-    
-        return self
-    
-    def secondary_alignment_period(self, secondary_alignment_period: str) -> typing.Self:    
-        """
-        Only present if a preprocessor is selected. Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
-        """
-            
-        self._internal.secondary_alignment_period = secondary_alignment_period
-    
-        return self
-    
-    def secondary_per_series_aligner(self, secondary_per_series_aligner: str) -> typing.Self:    
-        """
-        Only present if a preprocessor is selected. Alignment function to be used. Defaults to ALIGN_MEAN.
-        """
-            
-        self._internal.secondary_per_series_aligner = secondary_per_series_aligner
-    
-        return self
-    
-    def secondary_group_bys(self, secondary_group_bys: list[str]) -> typing.Self:    
-        """
-        Only present if a preprocessor is selected. Array of labels to group data by.
-        """
-            
-        self._internal.secondary_group_bys = secondary_group_bys
-    
-        return self
-    
-    def preprocessor(self, preprocessor: googlecloudmonitoring.PreprocessorType) -> typing.Self:    
-        """
-        Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
-        """
-            
-        self._internal.preprocessor = preprocessor
-    
-        return self
-    
     def title(self, title: str) -> typing.Self:    
         """
         Annotation title.
         """
             
         self._internal.title = title
     
@@ -244,91 +209,14 @@
         Annotation text.
         """
             
         self._internal.text = text
     
         return self
     
-
-class AnnotationQuery(cogbuilder.Builder[googlecloudmonitoring.AnnotationQuery]):    
-    """
-    Annotation sub-query properties.
-    """
-    
-    _internal: googlecloudmonitoring.AnnotationQuery
-
-    def __init__(self):
-        self._internal = googlecloudmonitoring.AnnotationQuery()
-
-    def build(self) -> googlecloudmonitoring.AnnotationQuery:
-        return self._internal    
-    
-    def project_name(self, project_name: str) -> typing.Self:    
-        """
-        GCP project to execute the query against.
-        """
-            
-        self._internal.project_name = project_name
-    
-        return self
-    
-    def cross_series_reducer(self, cross_series_reducer: str) -> typing.Self:    
-        """
-        Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
-        """
-            
-        self._internal.cross_series_reducer = cross_series_reducer
-    
-        return self
-    
-    def alignment_period(self, alignment_period: str) -> typing.Self:    
-        """
-        Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
-        """
-            
-        self._internal.alignment_period = alignment_period
-    
-        return self
-    
-    def per_series_aligner(self, per_series_aligner: str) -> typing.Self:    
-        """
-        Alignment function to be used. Defaults to ALIGN_MEAN.
-        """
-            
-        self._internal.per_series_aligner = per_series_aligner
-    
-        return self
-    
-    def group_bys(self, group_bys: list[str]) -> typing.Self:    
-        """
-        Array of labels to group data by.
-        """
-            
-        self._internal.group_bys = group_bys
-    
-        return self
-    
-    def filters(self, filters: list[str]) -> typing.Self:    
-        """
-        Array of filters to query data by. Labels that can be filtered on are defined by the metric.
-        """
-            
-        self._internal.filters = filters
-    
-        return self
-    
-    def view(self, view: str) -> typing.Self:    
-        """
-        Data view, defaults to FULL.
-        """
-            
-        self._internal.view = view
-    
-        return self
-    
     def secondary_cross_series_reducer(self, secondary_cross_series_reducer: str) -> typing.Self:    
         """
         Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
         """
             
         self._internal.secondary_cross_series_reducer = secondary_cross_series_reducer
     
@@ -357,41 +245,23 @@
         Only present if a preprocessor is selected. Array of labels to group data by.
         """
             
         self._internal.secondary_group_bys = secondary_group_bys
     
         return self
     
-    def title(self, title: str) -> typing.Self:    
-        """
-        Annotation title.
-        """
-            
-        self._internal.title = title
-    
-        return self
-    
     def preprocessor(self, preprocessor: googlecloudmonitoring.PreprocessorType) -> typing.Self:    
         """
         Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
         """
             
         self._internal.preprocessor = preprocessor
     
         return self
     
-    def text(self, text: str) -> typing.Self:    
-        """
-        Annotation text.
-        """
-            
-        self._internal.text = text
-    
-        return self
-    
 
 class TimeSeriesQuery(cogbuilder.Builder[googlecloudmonitoring.TimeSeriesQuery]):    
     """
     Time Series sub-query properties.
     """
     
     _internal: googlecloudmonitoring.TimeSeriesQuery
@@ -530,14 +400,55 @@
         """
             
         self._internal.lookback_period = lookback_period
     
         return self
     
 
+class PromQLQuery(cogbuilder.Builder[googlecloudmonitoring.PromQLQuery]):    
+    """
+    PromQL sub-query properties.
+    """
+    
+    _internal: googlecloudmonitoring.PromQLQuery
+
+    def __init__(self):
+        self._internal = googlecloudmonitoring.PromQLQuery()
+
+    def build(self) -> googlecloudmonitoring.PromQLQuery:
+        return self._internal    
+    
+    def project_name(self, project_name: str) -> typing.Self:    
+        """
+        GCP project to execute the query against.
+        """
+            
+        self._internal.project_name = project_name
+    
+        return self
+    
+    def expr(self, expr: str) -> typing.Self:    
+        """
+        PromQL expression/query to be executed.
+        """
+            
+        self._internal.expr = expr
+    
+        return self
+    
+    def step(self, step: str) -> typing.Self:    
+        """
+        PromQL min step
+        """
+            
+        self._internal.step = step
+    
+        return self
+    
+
 class MetricQuery(cogbuilder.Builder[googlecloudmonitoring.MetricQuery]):    
     """
     @deprecated This type is for migration purposes only. Replaced by TimeSeriesList Metric sub-query properties.
     """
     
     _internal: googlecloudmonitoring.MetricQuery
 
@@ -661,15 +572,15 @@
         self._internal.graph_period = graph_period
     
         return self
     
 
 class LegacyCloudMonitoringAnnotationQuery(cogbuilder.Builder[googlecloudmonitoring.LegacyCloudMonitoringAnnotationQuery]):    
     """
-    @deprecated Use AnnotationQuery instead. Legacy annotation query properties for migration purposes.
+    @deprecated Use TimeSeriesList instead. Legacy annotation query properties for migration purposes.
     """
     
     _internal: googlecloudmonitoring.LegacyCloudMonitoringAnnotationQuery
 
     def __init__(self):
         self._internal = googlecloudmonitoring.LegacyCloudMonitoringAnnotationQuery()
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/grafanapyroscope.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/grafanapyroscope.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,23 @@
         Specifies the query label selectors.
         """
             
         self._internal.label_selector = label_selector
     
         return self
     
+    def span_selector(self, span_selector: list[str]) -> typing.Self:    
+        """
+        Specifies the query span selectors.
+        """
+            
+        self._internal.span_selector = span_selector
+    
+        return self
+    
     def profile_type_id(self, profile_type_id: str) -> typing.Self:    
         """
         Specifies the type of profile to query.
         """
             
         self._internal.profile_type_id = profile_type_id
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -639,14 +658,29 @@
         if self._internal.options.tooltip is None:
             self._internal.options.tooltip = heatmap.HeatmapTooltip()
         assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
         self._internal.options.tooltip.y_histogram = False
     
         return self
     
+    def show_color_scale(self, show_color_scale: bool) -> typing.Self:    
+        """
+        Controls if the tooltip shows a color scale in header
+        """
+            
+        if self._internal.options is None:
+            self._internal.options = heatmap.Options()
+        assert isinstance(self._internal.options, heatmap.Options)
+        if self._internal.options.tooltip is None:
+            self._internal.options.tooltip = heatmap.HeatmapTooltip()
+        assert isinstance(self._internal.options.tooltip, heatmap.HeatmapTooltip)
+        self._internal.options.tooltip.show_color_scale = show_color_scale
+    
+        return self
+    
     def exemplars_color(self, color: str) -> typing.Self:    
         """
         Controls exemplar options
         """
             
         if self._internal.options is None:
             self._internal.options = heatmap.Options()
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -624,14 +643,28 @@
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = histogram.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def hide_from(self, hide_from: cogbuilder.Builder[common.HideSeriesConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -658,21 +691,21 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
         self._internal.field_config.defaults.custom.gradient_mode = gradient_mode
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = histogram.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, histogram.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,20 +286,21 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
-    def repeat_panel_id(self, repeat_panel_id: int) -> typing.Self:    
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
         """
-        Id of the repeating panel.
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
         """
             
-        self._internal.repeat_panel_id = repeat_panel_id
+        self._internal.max_per_row = max_per_row
     
         return self
     
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
@@ -355,14 +356,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def options(self, options: object) -> typing.Self:    
         """
         It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
         """
             
         self._internal.options = options
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import logs
-from ..models import common
+from ..models import text
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "logs"
+        self._internal.type_val = "text"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -417,71 +435,31 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def show_labels(self, show_labels: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_labels = show_labels
-    
-        return self
-    
-    def show_common_labels(self, show_common_labels: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_common_labels = show_common_labels
-    
-        return self
-    
-    def show_time(self, show_time: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.show_time = show_time
-    
-        return self
-    
-    def wrap_log_message(self, wrap_log_message: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.wrap_log_message = wrap_log_message
-    
-        return self
-    
-    def prettify_log_message(self, prettify_log_message: bool) -> typing.Self:        
-        if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.prettify_log_message = prettify_log_message
-    
-        return self
-    
-    def enable_log_details(self, enable_log_details: bool) -> typing.Self:        
+    def mode(self, mode: text.TextMode) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.enable_log_details = enable_log_details
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.mode = mode
     
         return self
     
-    def sort_order(self, sort_order: common.LogsSortOrder) -> typing.Self:        
+    def code(self, code: text.CodeOptions) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.sort_order = sort_order
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.code = code
     
         return self
     
-    def dedup_strategy(self, dedup_strategy: common.LogsDedupStrategy) -> typing.Self:        
+    def content(self, content: str) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = logs.Options()
-        assert isinstance(self._internal.options, logs.Options)
-        self._internal.options.dedup_strategy = dedup_strategy
+            self._internal.options = text.Options()
+        assert isinstance(self._internal.options, text.Options)
+        self._internal.options.content = content
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -227,14 +237,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/parca.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import preferences
 
 
 class Preferences(cogbuilder.Builder[preferences.Preferences]):    
+    """
+    Spec defines user, team or org Grafana preferences
+    swagger:model Preferences
+    """
+    
     _internal: preferences.Preferences
 
     def __init__(self):
         self._internal = preferences.Preferences()
 
     def build(self) -> preferences.Preferences:
         return self._internal
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/prometheus.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/prometheus.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
 from ..models import common
-from ..models import stat
+from ..models import bargauge
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "stat"
+        self._internal.type_val = "bargauge"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -417,65 +436,97 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def graph_mode(self, graph_mode: common.BigValueGraphMode) -> typing.Self:        
+    def display_mode(self, display_mode: common.BarGaugeDisplayMode) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.display_mode = display_mode
+    
+        return self
+    
+    def value_mode(self, value_mode: common.BarGaugeValueMode) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.value_mode = value_mode
+    
+        return self
+    
+    def name_placement(self, name_placement: common.BarGaugeNamePlacement) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.name_placement = name_placement
+    
+        return self
+    
+    def show_unfilled(self, show_unfilled: bool) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.show_unfilled = show_unfilled
+    
+        return self
+    
+    def sizing(self, sizing: common.BarGaugeSizing) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.graph_mode = graph_mode
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.sizing = sizing
     
         return self
     
-    def color_mode(self, color_mode: common.BigValueColorMode) -> typing.Self:        
+    def min_viz_width(self, min_viz_width: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.color_mode = color_mode
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.min_viz_width = min_viz_width
     
         return self
     
-    def justify_mode(self, justify_mode: common.BigValueJustifyMode) -> typing.Self:        
+    def min_viz_height(self, min_viz_height: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.justify_mode = justify_mode
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.min_viz_height = min_viz_height
     
         return self
     
     def reduce_options(self, reduce_options: cogbuilder.Builder[common.ReduceDataOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
         reduce_options_resource = reduce_options.build()
         self._internal.options.reduce_options = reduce_options_resource
     
         return self
     
     def text(self, text: cogbuilder.Builder[common.VizTextDisplayOptions]) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
         text_resource = text.build()
         self._internal.options.text = text_resource
     
         return self
     
-    def text_mode(self, text_mode: common.BigValueTextMode) -> typing.Self:        
+    def max_viz_height(self, max_viz_height: int) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
-        self._internal.options.text_mode = text_mode
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
+        self._internal.options.max_viz_height = max_viz_height
     
         return self
     
     def orientation(self, orientation: common.VizOrientation) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = stat.Options()
-        assert isinstance(self._internal.options, stat.Options)
+            self._internal.options = bargauge.Options()
+        assert isinstance(self._internal.options, bargauge.Options)
         self._internal.options.orientation = orientation
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/logs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 from ..cog import builder as cogbuilder
 from ..models import dashboard
 from ..cog import variants as cogvariants
-from ..models import table
+from ..models import logs
 from ..models import common
 
 
 class Panel(cogbuilder.Builder[dashboard.Panel]):    
     """
     Dashboard panels are the basic visualization building blocks.
     """
     
     _internal: dashboard.Panel
 
     def __init__(self):
         self._internal = dashboard.Panel()        
-        self._internal.type_val = "table"
+        self._internal.type_val = "logs"
 
     def build(self) -> dashboard.Panel:
         return self._internal    
     
     def id_val(self, id_val: int) -> typing.Self:    
         """
         Unique identifier of the panel. Generated by Grafana when creating a new panel. It must be unique within a dashboard, but not globally.
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -417,81 +436,71 @@
         self._internal.field_config.overrides.append(dashboard.DashboardFieldConfigSourceOverrides(
             matcher=matcher,
             properties=properties,
         ))
     
         return self
     
-    def frame_index(self, frame_index: float) -> typing.Self:    
-        """
-        Represents the index of the selected frame
-        """
-            
+    def show_labels(self, show_labels: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.frame_index = frame_index
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_labels = show_labels
     
         return self
     
-    def show_header(self, show_header: bool) -> typing.Self:    
-        """
-        Controls whether the panel should show the header
-        """
-            
+    def show_common_labels(self, show_common_labels: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.show_header = show_header
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_common_labels = show_common_labels
     
         return self
     
-    def show_type_icons(self, show_type_icons: bool) -> typing.Self:    
-        """
-        Controls whether the header should show icons for the column types
-        """
-            
+    def show_time(self, show_time: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.show_type_icons = show_type_icons
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.show_time = show_time
     
         return self
     
-    def sort_by(self, sort_by: list[cogbuilder.Builder[common.TableSortByFieldState]]) -> typing.Self:    
-        """
-        Used to control row sorting
-        """
-            
+    def wrap_log_message(self, wrap_log_message: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        sort_by_resources = [r1.build() for r1 in sort_by]
-        self._internal.options.sort_by = sort_by_resources
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.wrap_log_message = wrap_log_message
     
         return self
     
-    def footer(self, footer: cogbuilder.Builder[common.TableFooterOptions]) -> typing.Self:    
-        """
-        Controls footer options
-        """
-            
+    def prettify_log_message(self, prettify_log_message: bool) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        footer_resource = footer.build()
-        self._internal.options.footer = footer_resource
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.prettify_log_message = prettify_log_message
     
         return self
     
-    def cell_height(self, cell_height: common.TableCellHeight) -> typing.Self:    
-        """
-        Controls the height of the rows
-        """
-            
+    def enable_log_details(self, enable_log_details: bool) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.enable_log_details = enable_log_details
+    
+        return self
+    
+    def sort_order(self, sort_order: common.LogsSortOrder) -> typing.Self:        
+        if self._internal.options is None:
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.sort_order = sort_order
+    
+        return self
+    
+    def dedup_strategy(self, dedup_strategy: common.LogsDedupStrategy) -> typing.Self:        
         if self._internal.options is None:
-            self._internal.options = table.Options()
-        assert isinstance(self._internal.options, table.Options)
-        self._internal.options.cell_height = cell_height
+            self._internal.options = logs.Options()
+        assert isinstance(self._internal.options, logs.Options)
+        self._internal.options.dedup_strategy = dedup_strategy
     
         return self
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,29 +123,57 @@
         Defines the maximum number of traces that are returned from Tempo
         """
             
         self._internal.limit = limit
     
         return self
     
+    def spss(self, spss: int) -> typing.Self:    
+        """
+        Defines the maximum number of spans per spanset that are returned from Tempo
+        """
+            
+        self._internal.spss = spss
+    
+        return self
+    
+    def filters(self, filters: list[cogbuilder.Builder[tempo.TraceqlFilter]]) -> typing.Self:        
+        filters_resources = [r1.build() for r1 in filters]
+        self._internal.filters = filters_resources
+    
+        return self
+    
+    def group_by(self, group_by: list[cogbuilder.Builder[tempo.TraceqlFilter]]) -> typing.Self:    
+        """
+        Filters that are used to query the metrics summary
+        """
+            
+        group_by_resources = [r1.build() for r1 in group_by]
+        self._internal.group_by = group_by_resources
+    
+        return self
+    
     def datasource(self, datasource: object) -> typing.Self:    
         """
         For mixed data sources the selected datasource is on the query level.
         For non mixed scenarios this is undefined.
         TODO find a better way to do this ^ that's friendly to schema
         TODO this shouldn't be unknown but DataSourceRef | null
         """
             
         self._internal.datasource = datasource
     
         return self
     
-    def filters(self, filters: list[cogbuilder.Builder[tempo.TraceqlFilter]]) -> typing.Self:        
-        filters_resources = [r1.build() for r1 in filters]
-        self._internal.filters = filters_resources
+    def table_type(self, table_type: tempo.SearchTableType) -> typing.Self:    
+        """
+        The type of the table that is used to display the search results
+        """
+            
+        self._internal.table_type = table_type
     
         return self
     
 
 class TraceqlFilter(cogbuilder.Builder[tempo.TraceqlFilter]):    
     _internal: tempo.TraceqlFilter
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/testdata.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/testdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,19 @@
         Drop percentage (the chance we will lose a point 0-100)
         """
             
         self._internal.drop_percent = drop_percent
     
         return self
     
+    def flamegraph_diff(self, flamegraph_diff: bool) -> typing.Self:        
+        self._internal.flamegraph_diff = flamegraph_diff
+    
+        return self
+    
     def ref_id(self, ref_id: str) -> typing.Self:    
         """
         A unique identifier for the query within the list of targets.
         In server side expressions, the refId is used as a variable name to identify results.
         By default, the UI will assign A->Z; however setting meaningful names may be useful.
         """
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -726,14 +745,28 @@
             self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = timeseries.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -846,25 +879,25 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = timeseries.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, timeseries.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/trend.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -730,14 +749,28 @@
             self._internal.field_config.defaults.custom = trend.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = trend.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def bar_alignment(self, bar_alignment: common.BarAlignment) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -850,25 +883,25 @@
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = trend.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
         self._internal.field_config.defaults.custom.point_symbol = point_symbol
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = trend.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, trend.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
     
         return self
     
     def bar_max_width(self, bar_max_width: float) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/builders/xychart.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,24 @@
         `h` for horizontal, `v` for vertical.
         """
             
         self._internal.repeat_direction = repeat_direction
     
         return self
     
+    def max_per_row(self, max_per_row: float) -> typing.Self:    
+        """
+        Option for repeated panels that controls max items per row
+        Only relevant for horizontally repeated panels
+        """
+            
+        self._internal.max_per_row = max_per_row
+    
+        return self
+    
     def max_data_points(self, max_data_points: float) -> typing.Self:    
         """
         The maximum number of data points that the panel queries are retrieving.
         """
             
         self._internal.max_data_points = max_data_points
     
@@ -228,14 +238,23 @@
         See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
         """
             
         self._internal.time_shift = time_shift
     
         return self
     
+    def hide_time_override(self, hide_time_override: bool) -> typing.Self:    
+        """
+        Controls if the timeFrom or timeShift overrides are shown in the panel header
+        """
+            
+        self._internal.hide_time_override = hide_time_override
+    
+        return self
+    
     def library_panel(self, library_panel: dashboard.LibraryPanelRef) -> typing.Self:    
         """
         Dynamically load the panel
         """
             
         self._internal.library_panel = library_panel
     
@@ -649,14 +668,28 @@
             self._internal.field_config.defaults.custom = xychart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
         scale_distribution_resource = scale_distribution.build()
         self._internal.field_config.defaults.custom.scale_distribution = scale_distribution_resource
     
         return self
     
+    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+        if self._internal.field_config is None:
+            self._internal.field_config = dashboard.FieldConfigSource()
+        assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
+        if self._internal.field_config.defaults is None:
+            self._internal.field_config.defaults = dashboard.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
+        if self._internal.field_config.defaults.custom is None:
+            self._internal.field_config.defaults.custom = xychart.FieldConfig()
+        assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
+        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+    
+        return self
+    
     def label_value(self, label_value: cogbuilder.Builder[common.TextDimensionConfig]) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
@@ -664,25 +697,25 @@
             self._internal.field_config.defaults.custom = xychart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
         label_value_resource = label_value.build()
         self._internal.field_config.defaults.custom.label_value = label_value_resource
     
         return self
     
-    def axis_centered_zero(self, axis_centered_zero: bool) -> typing.Self:        
+    def axis_border_show(self, axis_border_show: bool) -> typing.Self:        
         if self._internal.field_config is None:
             self._internal.field_config = dashboard.FieldConfigSource()
         assert isinstance(self._internal.field_config, dashboard.FieldConfigSource)
         if self._internal.field_config.defaults is None:
             self._internal.field_config.defaults = dashboard.FieldConfig()
         assert isinstance(self._internal.field_config.defaults, dashboard.FieldConfig)
         if self._internal.field_config.defaults.custom is None:
             self._internal.field_config.defaults.custom = xychart.FieldConfig()
         assert isinstance(self._internal.field_config.defaults.custom, xychart.FieldConfig)
-        self._internal.field_config.defaults.custom.axis_centered_zero = axis_centered_zero
+        self._internal.field_config.defaults.custom.axis_border_show = axis_border_show
     
         return self
     
     def series_mapping(self, series_mapping: xychart.SeriesMapping) -> typing.Self:        
         if self._internal.options is None:
             self._internal.options = xychart.Options()
         assert isinstance(self._internal.options, xychart.Options)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/plugins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import elasticsearch
-from ..models import tempo
 from ..models import alertgroups
-from ..models import datagrid
-from ..models import debug
+from ..models import gauge
 from ..models import xychart
-from ..models import loki
-from ..models import news
-from ..models import nodegraph
+from ..models import cloudwatch
+from ..models import parca
+from ..models import statetimeline
 from ..models import table
-from ..models import text
-from ..models import piechart
-from ..models import testdata
-from ..models import trend
 from ..models import azuremonitor
-from ..models import barchart
+from ..models import candlestick
 from ..models import dashboardlist
-from ..models import annotationslist
-from ..models import gauge
+from ..models import grafanapyroscope
+from ..models import heatmap
+from ..models import text
+from ..models import trend
 from ..models import geomap
 from ..models import histogram
 from ..models import prometheus
-from ..models import stat
-from ..models import expr
+from ..models import tempo
+from ..models import timeseries
+from ..models import barchart
+from ..models import debug
+from ..models import testdata
+from ..models import annotationslist
 from ..models import canvas
+from ..models import elasticsearch
+from ..models import logs
+from ..models import stat
+from ..models import datagrid
 from ..models import googlecloudmonitoring
-from ..models import grafanapyroscope
-from ..models import parca
-from ..models import statetimeline
-from ..models import statushistory
-from ..models import timeseries
+from ..models import news
+from ..models import nodegraph
 from ..models import bargauge
-from ..models import candlestick
-from ..models import cloudwatch
-from ..models import heatmap
-from ..models import logs
+from ..models import loki
+from ..models import piechart
+from ..models import statushistory
+from ..models import expr
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
     cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/alertgroups.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/alerting.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/alerting.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Duration in seconds.
 Duration: typing.TypeAlias = int
 
 
 Json: typing.TypeAlias = object
 
 
-MatchRegexps: typing.TypeAlias = dict[str, 'Regexp']
+MatchRegexps: typing.TypeAlias = dict[str, str]
 
 
 MatchType: typing.TypeAlias = int
 
 
 class Matcher:
     name: typing.Optional[str]
@@ -99,19 +99,14 @@
 # slice. Note that some users of Matchers might require it to be sorted.
 ObjectMatchers: typing.TypeAlias = 'Matchers'
 
 
 Provenance: typing.TypeAlias = str
 
 
-# A Regexp is safe for concurrent use by multiple goroutines,
-# except for configuration methods, such as Longest.
-Regexp: typing.TypeAlias = object
-
-
 class RelativeTimeRange:
     """
     RelativeTimeRange is the per query start and end time
     for requests.
     """
 
     # RelativeTimeRange is the per query start and end time
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,62 +312,76 @@
 
     # KQL query to be executed.
     query: typing.Optional[str]
     # Specifies the format results should be returned as.
     result_format: typing.Optional['ResultFormat']
     # Array of resource URIs to be queried.
     resources: typing.Optional[list[str]]
-    # If set to true the intersection of time ranges specified in the query and Grafana will be used. Otherwise the query time ranges will be used. Defaults to false
-    intersect_time: typing.Optional[bool]
-    # Workspace ID. This was removed in Grafana 8, but remains for backwards compat
+    # If set to true the dashboard time range will be used as a filter for the query. Otherwise the query time ranges will be used. Defaults to false.
+    dashboard_time: typing.Optional[bool]
+    # If dashboardTime is set to true this value dictates which column the time filter will be applied to. Defaults to the first tables timeSpan column, the first datetime column found, or TimeGenerated
+    time_column: typing.Optional[str]
+    # Workspace ID. This was removed in Grafana 8, but remains for backwards compat.
     workspace: typing.Optional[str]
     # @deprecated Use resources instead
     resource: typing.Optional[str]
+    # @deprecated Use dashboardTime instead
+    intersect_time: typing.Optional[bool]
 
-    def __init__(self, query: typing.Optional[str] = None, result_format: typing.Optional['ResultFormat'] = None, resources: typing.Optional[list[str]] = None, intersect_time: typing.Optional[bool] = None, workspace: typing.Optional[str] = None, resource: typing.Optional[str] = None):
+    def __init__(self, query: typing.Optional[str] = None, result_format: typing.Optional['ResultFormat'] = None, resources: typing.Optional[list[str]] = None, dashboard_time: typing.Optional[bool] = None, time_column: typing.Optional[str] = None, workspace: typing.Optional[str] = None, resource: typing.Optional[str] = None, intersect_time: typing.Optional[bool] = None):
         self.query = query
         self.result_format = result_format
         self.resources = resources
-        self.intersect_time = intersect_time
+        self.dashboard_time = dashboard_time
+        self.time_column = time_column
         self.workspace = workspace
         self.resource = resource
+        self.intersect_time = intersect_time
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.query is not None:
             payload["query"] = self.query
         if self.result_format is not None:
             payload["resultFormat"] = self.result_format
         if self.resources is not None:
             payload["resources"] = self.resources
-        if self.intersect_time is not None:
-            payload["intersectTime"] = self.intersect_time
+        if self.dashboard_time is not None:
+            payload["dashboardTime"] = self.dashboard_time
+        if self.time_column is not None:
+            payload["timeColumn"] = self.time_column
         if self.workspace is not None:
             payload["workspace"] = self.workspace
         if self.resource is not None:
             payload["resource"] = self.resource
+        if self.intersect_time is not None:
+            payload["intersectTime"] = self.intersect_time
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "query" in data:
             args["query"] = data["query"]
         if "resultFormat" in data:
             args["result_format"] = data["resultFormat"]
         if "resources" in data:
             args["resources"] = data["resources"]
-        if "intersectTime" in data:
-            args["intersect_time"] = data["intersectTime"]
+        if "dashboardTime" in data:
+            args["dashboard_time"] = data["dashboardTime"]
+        if "timeColumn" in data:
+            args["time_column"] = data["timeColumn"]
         if "workspace" in data:
             args["workspace"] = data["workspace"]
         if "resource" in data:
-            args["resource"] = data["resource"]        
+            args["resource"] = data["resource"]
+        if "intersectTime" in data:
+            args["intersect_time"] = data["intersectTime"]        
 
         return cls(**args)
 
 
 class AzureTracesQuery:
     """
     Application Insights Traces sub-query properties
@@ -466,14 +480,15 @@
         return cls(**args)
 
 
 class ResultFormat(enum.StrEnum):
     TABLE = "table"
     TIME_SERIES = "time_series"
     TRACE = "trace"
+    LOGS = "logs"
 
 
 class AzureResourceGraphQuery:
     # Azure Resource Graph KQL query to be executed.
     query: typing.Optional[str]
     # Specifies the format results should be returned as. Defaults to table.
     result_format: typing.Optional[str]
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/barchart.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,34 +128,36 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
+    axis_centered_zero: typing.Optional[bool]
     hide_from: typing.Optional[common.HideSeriesConfig]
     # Threshold rendering
     thresholds_style: typing.Optional[common.GraphThresholdsStyleConfig]
-    axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, thresholds_style: typing.Optional[common.GraphThresholdsStyleConfig] = None, axis_centered_zero: typing.Optional[bool] = None):
+    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, thresholds_style: typing.Optional[common.GraphThresholdsStyleConfig] = None, axis_border_show: typing.Optional[bool] = None):
         self.line_width = line_width
         self.fill_opacity = fill_opacity
         self.gradient_mode = gradient_mode if gradient_mode is not None else common.GraphGradientMode.NONE
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
+        self.axis_centered_zero = axis_centered_zero
         self.hide_from = hide_from
         self.thresholds_style = thresholds_style
-        self.axis_centered_zero = axis_centered_zero
+        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.line_width is not None:
             payload["lineWidth"] = self.line_width
         if self.fill_opacity is not None:
@@ -174,20 +176,22 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
         if self.thresholds_style is not None:
             payload["thresholdsStyle"] = self.thresholds_style
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "lineWidth" in data:
@@ -208,20 +212,22 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "hideFrom" in data:
             args["hide_from"] = common.HideSeriesConfig.from_json(data["hideFrom"])
         if "thresholdsStyle" in data:
             args["thresholds_style"] = common.GraphThresholdsStyleConfig.from_json(data["thresholdsStyle"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]        
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/gauge.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 
 from ..models import common
 import typing
 from ..cog import runtime as cogruntime
 
 
 class Options:
-    display_mode: common.BarGaugeDisplayMode
-    value_mode: common.BarGaugeValueMode
-    show_unfilled: bool
+    show_threshold_labels: bool
+    show_threshold_markers: bool
+    sizing: common.BarGaugeSizing
     min_viz_width: int
     reduce_options: common.ReduceDataOptions
     text: typing.Optional[common.VizTextDisplayOptions]
     min_viz_height: int
     orientation: common.VizOrientation
 
-    def __init__(self, display_mode: typing.Optional[common.BarGaugeDisplayMode] = None, value_mode: typing.Optional[common.BarGaugeValueMode] = None, show_unfilled: bool = True, min_viz_width: int = 0, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, min_viz_height: int = 10, orientation: typing.Optional[common.VizOrientation] = None):
-        self.display_mode = display_mode if display_mode is not None else common.BarGaugeDisplayMode.GRADIENT
-        self.value_mode = value_mode if value_mode is not None else common.BarGaugeValueMode.COLOR
-        self.show_unfilled = show_unfilled
+    def __init__(self, show_threshold_labels: bool = False, show_threshold_markers: bool = True, sizing: typing.Optional[common.BarGaugeSizing] = None, min_viz_width: int = 75, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, min_viz_height: int = 75, orientation: typing.Optional[common.VizOrientation] = None):
+        self.show_threshold_labels = show_threshold_labels
+        self.show_threshold_markers = show_threshold_markers
+        self.sizing = sizing if sizing is not None else common.BarGaugeSizing.AUTO
         self.min_viz_width = min_viz_width
         self.reduce_options = reduce_options if reduce_options is not None else common.ReduceDataOptions()
         self.text = text
         self.min_viz_height = min_viz_height
         self.orientation = orientation if orientation is not None else common.VizOrientation.AUTO
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "displayMode": self.display_mode,
-            "valueMode": self.value_mode,
-            "showUnfilled": self.show_unfilled,
+            "showThresholdLabels": self.show_threshold_labels,
+            "showThresholdMarkers": self.show_threshold_markers,
+            "sizing": self.sizing,
             "minVizWidth": self.min_viz_width,
             "reduceOptions": self.reduce_options,
             "minVizHeight": self.min_viz_height,
             "orientation": self.orientation,
         }
         if self.text is not None:
             payload["text"] = self.text
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "displayMode" in data:
-            args["display_mode"] = data["displayMode"]
-        if "valueMode" in data:
-            args["value_mode"] = data["valueMode"]
-        if "showUnfilled" in data:
-            args["show_unfilled"] = data["showUnfilled"]
+        if "showThresholdLabels" in data:
+            args["show_threshold_labels"] = data["showThresholdLabels"]
+        if "showThresholdMarkers" in data:
+            args["show_threshold_markers"] = data["showThresholdMarkers"]
+        if "sizing" in data:
+            args["sizing"] = data["sizing"]
         if "minVizWidth" in data:
             args["min_viz_width"] = data["minVizWidth"]
         if "reduceOptions" in data:
             args["reduce_options"] = common.ReduceDataOptions.from_json(data["reduceOptions"])
         if "text" in data:
             args["text"] = common.VizTextDisplayOptions.from_json(data["text"])
         if "minVizHeight" in data:
@@ -61,11 +61,11 @@
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
-        identifier="bargauge",
+        identifier="gauge",
         options_from_json_hook=Options.from_json,
         field_config_from_json_hook=None,
     )
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,20 @@
             args["color"] = common.ColorDimensionConfig.from_json(data["color"])
         if "width" in data:
             args["width"] = data["width"]        
 
         return cls(**args)
 
 
+class HttpRequestMethod(enum.StrEnum):
+    GET = "GET"
+    POST = "POST"
+    PUT = "PUT"
+
+
 class ConnectionCoordinates:
     x: float
     y: float
 
     def __init__(self, x: float = 0, y: float = 0):
         self.x = x
         self.y = y
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "select" in data:
             args["select"] = QueryEditorFunctionExpression.from_json(data["select"])
         if "from" in data:
-            decoding_map: dict[str, typing.Union[typing.Type[QueryEditorFunctionExpression], typing.Type[QueryEditorPropertyExpression]]] = {"function": QueryEditorFunctionExpression, "property": QueryEditorPropertyExpression}
+            decoding_map: dict[str, typing.Union[typing.Type[QueryEditorPropertyExpression], typing.Type[QueryEditorFunctionExpression]]] = {"property": QueryEditorPropertyExpression, "function": QueryEditorFunctionExpression}
             args["from_val"] = decoding_map[data["from"]["type"]].from_json(data["from"])
         if "where" in data:
             args["where"] = QueryEditorArrayExpression.from_json(data["where"])
         if "groupBy" in data:
             args["group_by"] = QueryEditorArrayExpression.from_json(data["groupBy"])
         if "orderBy" in data:
             args["order_by"] = QueryEditorFunctionExpression.from_json(data["orderBy"])
@@ -896,15 +896,15 @@
         return cls(**args)
 
 
 CloudWatchQuery: typing.TypeAlias = typing.Union['CloudWatchMetricsQuery', 'CloudWatchLogsQuery', 'CloudWatchAnnotationQuery']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery], typing.Type[CloudWatchAnnotationQuery]]] = {"Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery, "Annotations": CloudWatchAnnotationQuery}
+    decoding_map: dict[str, typing.Union[typing.Type[CloudWatchAnnotationQuery], typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery]]] = {"Annotations": CloudWatchAnnotationQuery, "Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery}
     return cogruntime.DataqueryConfig(
         identifier="cloudwatch",
         from_json_hook=lambda data: decoding_map[data["queryMode"]].from_json(data),
     )
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -827,25 +827,27 @@
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional['ScaleDistributionConfig']
     axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None):
+    def __init__(self, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None, axis_border_show: typing.Optional[bool] = None):
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
         self.axis_centered_zero = axis_centered_zero
+        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.axis_placement is not None:
             payload["axisPlacement"] = self.axis_placement
         if self.axis_color_mode is not None:
@@ -860,14 +862,16 @@
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
         if self.axis_centered_zero is not None:
             payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "axisPlacement" in data:
@@ -883,15 +887,17 @@
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = ScaleDistributionConfig.from_json(data["scaleDistribution"])
         if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]        
+            args["axis_centered_zero"] = data["axisCenteredZero"]
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
 
 
 class HideSeriesConfig:
     """
     TODO docs
@@ -1416,30 +1422,31 @@
     axis_color_mode: typing.Optional['AxisColorMode']
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional['ScaleDistributionConfig']
+    axis_centered_zero: typing.Optional[bool]
     bar_alignment: typing.Optional['BarAlignment']
     bar_width_factor: typing.Optional[float]
     stacking: typing.Optional['StackingConfig']
     hide_from: typing.Optional['HideSeriesConfig']
     transform: typing.Optional['GraphTransform']
     # Indicate if null values should be treated as gaps or connected.
     # When the value is a number, it represents the maximum delta in the
     # X axis that should be considered connected.  For timeseries, this is milliseconds
     span_nulls: typing.Optional[typing.Union[bool, float]]
     fill_below_to: typing.Optional[str]
     point_symbol: typing.Optional[str]
-    axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
     bar_max_width: typing.Optional[float]
     insert_nulls: typing.Optional[typing.Union[bool, int]]
 
-    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_centered_zero: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None, insert_nulls: typing.Optional[typing.Union[bool, int]] = None):
+    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_border_show: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None, insert_nulls: typing.Optional[typing.Union[bool, int]] = None):
         self.draw_style = draw_style
         self.gradient_mode = gradient_mode
         self.thresholds_style = thresholds_style
         self.line_color = line_color
         self.line_width = line_width
         self.line_interpolation = line_interpolation
         self.line_style = line_style
@@ -1452,23 +1459,24 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
+        self.axis_centered_zero = axis_centered_zero
         self.bar_alignment = bar_alignment
         self.bar_width_factor = bar_width_factor
         self.stacking = stacking
         self.hide_from = hide_from
         self.transform = transform
         self.span_nulls = span_nulls
         self.fill_below_to = fill_below_to
         self.point_symbol = point_symbol
-        self.axis_centered_zero = axis_centered_zero
+        self.axis_border_show = axis_border_show
         self.bar_max_width = bar_max_width
         self.insert_nulls = insert_nulls
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.draw_style is not None:
@@ -1507,14 +1515,16 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.bar_alignment is not None:
             payload["barAlignment"] = self.bar_alignment
         if self.bar_width_factor is not None:
             payload["barWidthFactor"] = self.bar_width_factor
         if self.stacking is not None:
             payload["stacking"] = self.stacking
         if self.hide_from is not None:
@@ -1523,16 +1533,16 @@
             payload["transform"] = self.transform
         if self.span_nulls is not None:
             payload["spanNulls"] = self.span_nulls
         if self.fill_below_to is not None:
             payload["fillBelowTo"] = self.fill_below_to
         if self.point_symbol is not None:
             payload["pointSymbol"] = self.point_symbol
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         if self.bar_max_width is not None:
             payload["barMaxWidth"] = self.bar_max_width
         if self.insert_nulls is not None:
             payload["insertNulls"] = self.insert_nulls
         return payload
 
     @classmethod
@@ -1575,14 +1585,16 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "barAlignment" in data:
             args["bar_alignment"] = data["barAlignment"]
         if "barWidthFactor" in data:
             args["bar_width_factor"] = data["barWidthFactor"]
         if "stacking" in data:
             args["stacking"] = StackingConfig.from_json(data["stacking"])
         if "hideFrom" in data:
@@ -1591,16 +1603,16 @@
             args["transform"] = data["transform"]
         if "spanNulls" in data:
             args["span_nulls"] = data["spanNulls"]
         if "fillBelowTo" in data:
             args["fill_below_to"] = data["fillBelowTo"]
         if "pointSymbol" in data:
             args["point_symbol"] = data["pointSymbol"]
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]
         if "barMaxWidth" in data:
             args["bar_max_width"] = data["barMaxWidth"]
         if "insertNulls" in data:
             args["insert_nulls"] = data["insertNulls"]        
 
         return cls(**args)
 
@@ -1693,14 +1705,33 @@
     """
 
     COLOR = "color"
     TEXT = "text"
     HIDDEN = "hidden"
 
 
+class BarGaugeNamePlacement(enum.StrEnum):
+    """
+    Allows for the bar gauge name to be placed explicitly
+    """
+
+    AUTO = "auto"
+    TOP = "top"
+    LEFT = "left"
+
+
+class BarGaugeSizing(enum.StrEnum):
+    """
+    Allows for the bar gauge size to be set explicitly
+    """
+
+    AUTO = "auto"
+    MANUAL = "manual"
+
+
 class VizTooltipOptions:
     """
     TODO docs
     """
 
     mode: 'TooltipDisplayMode'
     sort: 'SortOrder'
@@ -1994,29 +2025,31 @@
     axis_color_mode: typing.Optional['AxisColorMode']
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional['ScaleDistributionConfig']
+    axis_centered_zero: typing.Optional[bool]
     bar_alignment: typing.Optional['BarAlignment']
     bar_width_factor: typing.Optional[float]
     stacking: typing.Optional['StackingConfig']
     hide_from: typing.Optional['HideSeriesConfig']
+    hide_value: typing.Optional[bool]
     transform: typing.Optional['GraphTransform']
     # Indicate if null values should be treated as gaps or connected.
     # When the value is a number, it represents the maximum delta in the
     # X axis that should be considered connected.  For timeseries, this is milliseconds
     span_nulls: typing.Optional[typing.Union[bool, float]]
     fill_below_to: typing.Optional[str]
     point_symbol: typing.Optional[str]
-    axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
     bar_max_width: typing.Optional[float]
 
-    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_centered_zero: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None):
+    def __init__(self, draw_style: typing.Optional['GraphDrawStyle'] = None, gradient_mode: typing.Optional['GraphGradientMode'] = None, thresholds_style: typing.Optional['GraphThresholdsStyleConfig'] = None, line_color: typing.Optional[str] = None, line_width: typing.Optional[float] = None, line_interpolation: typing.Optional['LineInterpolation'] = None, line_style: typing.Optional['LineStyle'] = None, fill_color: typing.Optional[str] = None, fill_opacity: typing.Optional[float] = None, show_points: typing.Optional['VisibilityMode'] = None, point_size: typing.Optional[float] = None, point_color: typing.Optional[str] = None, axis_placement: typing.Optional['AxisPlacement'] = None, axis_color_mode: typing.Optional['AxisColorMode'] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional['ScaleDistributionConfig'] = None, axis_centered_zero: typing.Optional[bool] = None, bar_alignment: typing.Optional['BarAlignment'] = None, bar_width_factor: typing.Optional[float] = None, stacking: typing.Optional['StackingConfig'] = None, hide_from: typing.Optional['HideSeriesConfig'] = None, hide_value: typing.Optional[bool] = None, transform: typing.Optional['GraphTransform'] = None, span_nulls: typing.Optional[typing.Union[bool, float]] = None, fill_below_to: typing.Optional[str] = None, point_symbol: typing.Optional[str] = None, axis_border_show: typing.Optional[bool] = None, bar_max_width: typing.Optional[float] = None):
         self.type_val = "sparkline"
         self.draw_style = draw_style
         self.gradient_mode = gradient_mode
         self.thresholds_style = thresholds_style
         self.line_color = line_color
         self.line_width = line_width
         self.line_interpolation = line_interpolation
@@ -2030,23 +2063,25 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
+        self.axis_centered_zero = axis_centered_zero
         self.bar_alignment = bar_alignment
         self.bar_width_factor = bar_width_factor
         self.stacking = stacking
         self.hide_from = hide_from
+        self.hide_value = hide_value
         self.transform = transform
         self.span_nulls = span_nulls
         self.fill_below_to = fill_below_to
         self.point_symbol = point_symbol
-        self.axis_centered_zero = axis_centered_zero
+        self.axis_border_show = axis_border_show
         self.bar_max_width = bar_max_width
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
         }
         if self.draw_style is not None:
@@ -2085,32 +2120,36 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.bar_alignment is not None:
             payload["barAlignment"] = self.bar_alignment
         if self.bar_width_factor is not None:
             payload["barWidthFactor"] = self.bar_width_factor
         if self.stacking is not None:
             payload["stacking"] = self.stacking
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
+        if self.hide_value is not None:
+            payload["hideValue"] = self.hide_value
         if self.transform is not None:
             payload["transform"] = self.transform
         if self.span_nulls is not None:
             payload["spanNulls"] = self.span_nulls
         if self.fill_below_to is not None:
             payload["fillBelowTo"] = self.fill_below_to
         if self.point_symbol is not None:
             payload["pointSymbol"] = self.point_symbol
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         if self.bar_max_width is not None:
             payload["barMaxWidth"] = self.bar_max_width
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
@@ -2151,32 +2190,36 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "barAlignment" in data:
             args["bar_alignment"] = data["barAlignment"]
         if "barWidthFactor" in data:
             args["bar_width_factor"] = data["barWidthFactor"]
         if "stacking" in data:
             args["stacking"] = StackingConfig.from_json(data["stacking"])
         if "hideFrom" in data:
             args["hide_from"] = HideSeriesConfig.from_json(data["hideFrom"])
+        if "hideValue" in data:
+            args["hide_value"] = data["hideValue"]
         if "transform" in data:
             args["transform"] = data["transform"]
         if "spanNulls" in data:
             args["span_nulls"] = data["spanNulls"]
         if "fillBelowTo" in data:
             args["fill_below_to"] = data["fillBelowTo"]
         if "pointSymbol" in data:
             args["point_symbol"] = data["pointSymbol"]
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]
         if "barMaxWidth" in data:
             args["bar_max_width"] = data["barMaxWidth"]        
 
         return cls(**args)
 
 
 class TableColoredBackgroundCellOptions:
@@ -2450,15 +2493,15 @@
     # This field is deprecated in favor of using cellOptions
     display_mode: typing.Optional['TableCellDisplayMode']
     cell_options: typing.Optional['TableCellOptions']
     # ?? default is missing or false ??
     hidden: typing.Optional[bool]
     inspect: bool
     filterable: typing.Optional[bool]
-    # Hides any header for a column, usefull for columns that show some static content or buttons.
+    # Hides any header for a column, useful for columns that show some static content or buttons.
     hide_header: typing.Optional[bool]
 
     def __init__(self, width: typing.Optional[float] = None, min_width: typing.Optional[float] = None, align: typing.Optional['FieldTextAlignment'] = None, display_mode: typing.Optional['TableCellDisplayMode'] = None, cell_options: typing.Optional['TableCellOptions'] = None, hidden: typing.Optional[bool] = None, inspect: bool = False, filterable: typing.Optional[bool] = None, hide_header: typing.Optional[bool] = None):
         self.width = width
         self.min_width = min_width
         self.align = align if align is not None else FieldTextAlignment.AUTO
         self.display_mode = display_mode
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,29 +19,26 @@
     # This property should only be used in dashboards defined by plugins.  It is a quick check
     # to see if the version has changed since the last time.
     revision: typing.Optional[int]
     # ID of a dashboard imported from the https://grafana.com/grafana/dashboards/ portal
     gnet_id: typing.Optional[str]
     # Tags associated with dashboard.
     tags: typing.Optional[list[str]]
-    # Theme of dashboard.
-    # Default value: dark.
-    style: typing.Literal["light", "dark"]
     # Timezone of dashboard. Accepted values are IANA TZDB zone ID or "browser" or "utc".
     timezone: typing.Optional[str]
     # Whether a dashboard is editable or not.
-    editable: bool
+    editable: typing.Optional[bool]
     # Configuration of dashboard cursor sync behavior.
     # Accepted values are 0 (sync turned off), 1 (shared crosshair), 2 (shared crosshair and tooltip).
-    graph_tooltip: 'DashboardCursorSync'
+    graph_tooltip: typing.Optional['DashboardCursorSync']
     # Time range for dashboard.
     # Accepted values are relative time strings like {from: 'now-6h', to: 'now'} or absolute time strings like {from: '2020-07-10T08:00:00.000Z', to: '2020-07-10T14:00:00.000Z'}.
     time: typing.Optional['DashboardDashboardTime']
     # Configuration of the time picker shown at the top of a dashboard.
-    timepicker: typing.Optional['TimePicker']
+    timepicker: typing.Optional['TimePickerConfig']
     # The month that the fiscal year starts on.  0 = January, 11 = December
     fiscal_year_start_month: typing.Optional[int]
     # When set to true, the dashboard will redraw panels at an interval matching the pixel width.
     # This will keep data "moving left" regardless of the query refresh rate. This setting helps
     # avoid dashboards presenting stale live data
     live_now: typing.Optional[bool]
     # Day when the week starts. Expressed by the name of the day in lowercase, e.g. "monday".
@@ -63,23 +60,22 @@
     # See https://grafana.com/docs/grafana/latest/dashboards/build-dashboards/annotate-visualizations/
     annotations: 'AnnotationContainer'
     # Links with references to other dashboards or external websites.
     links: typing.Optional[list['DashboardLink']]
     # Snapshot options. They are present only if the dashboard is a snapshot.
     snapshot: typing.Optional['Snapshot']
 
-    def __init__(self, id_val: typing.Optional[int] = None, uid: typing.Optional[str] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, revision: typing.Optional[int] = None, gnet_id: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, style: typing.Optional[typing.Literal["light", "dark"]] = None, timezone: typing.Optional[str] = "browser", editable: bool = True, graph_tooltip: typing.Optional['DashboardCursorSync'] = None, time: typing.Optional['DashboardDashboardTime'] = None, timepicker: typing.Optional['TimePicker'] = None, fiscal_year_start_month: typing.Optional[int] = 0, live_now: typing.Optional[bool] = None, week_start: typing.Optional[str] = None, refresh: typing.Optional[typing.Union[str, typing.Literal[False]]] = None, schema_version: int = 36, version: typing.Optional[int] = None, panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]] = None, templating: typing.Optional['DashboardDashboardTemplating'] = None, annotations: typing.Optional['AnnotationContainer'] = None, links: typing.Optional[list['DashboardLink']] = None, snapshot: typing.Optional['Snapshot'] = None):
+    def __init__(self, id_val: typing.Optional[int] = None, uid: typing.Optional[str] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, revision: typing.Optional[int] = None, gnet_id: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, timezone: typing.Optional[str] = "browser", editable: typing.Optional[bool] = True, graph_tooltip: typing.Optional['DashboardCursorSync'] = None, time: typing.Optional['DashboardDashboardTime'] = None, timepicker: typing.Optional['TimePickerConfig'] = None, fiscal_year_start_month: typing.Optional[int] = 0, live_now: typing.Optional[bool] = None, week_start: typing.Optional[str] = None, refresh: typing.Optional[typing.Union[str, typing.Literal[False]]] = None, schema_version: int = 36, version: typing.Optional[int] = None, panels: typing.Optional[list[typing.Union['Panel', 'RowPanel']]] = None, templating: typing.Optional['DashboardDashboardTemplating'] = None, annotations: typing.Optional['AnnotationContainer'] = None, links: typing.Optional[list['DashboardLink']] = None, snapshot: typing.Optional['Snapshot'] = None):
         self.id_val = id_val
         self.uid = uid
         self.title = title
         self.description = description
         self.revision = revision
         self.gnet_id = gnet_id
         self.tags = tags
-        self.style = style if style is not None else "dark"
         self.timezone = timezone
         self.editable = editable
         self.graph_tooltip = graph_tooltip if graph_tooltip is not None else DashboardCursorSync.OFF
         self.time = time
         self.timepicker = timepicker
         self.fiscal_year_start_month = fiscal_year_start_month
         self.live_now = live_now
@@ -91,17 +87,14 @@
         self.templating = templating if templating is not None else DashboardDashboardTemplating()
         self.annotations = annotations if annotations is not None else AnnotationContainer()
         self.links = links
         self.snapshot = snapshot
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "style": self.style,
-            "editable": self.editable,
-            "graphTooltip": self.graph_tooltip,
             "schemaVersion": self.schema_version,
             "templating": self.templating,
             "annotations": self.annotations,
         }
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.uid is not None:
@@ -114,14 +107,18 @@
             payload["revision"] = self.revision
         if self.gnet_id is not None:
             payload["gnetId"] = self.gnet_id
         if self.tags is not None:
             payload["tags"] = self.tags
         if self.timezone is not None:
             payload["timezone"] = self.timezone
+        if self.editable is not None:
+            payload["editable"] = self.editable
+        if self.graph_tooltip is not None:
+            payload["graphTooltip"] = self.graph_tooltip
         if self.time is not None:
             payload["time"] = self.time
         if self.timepicker is not None:
             payload["timepicker"] = self.timepicker
         if self.fiscal_year_start_month is not None:
             payload["fiscalYearStartMonth"] = self.fiscal_year_start_month
         if self.live_now is not None:
@@ -154,26 +151,24 @@
             args["description"] = data["description"]
         if "revision" in data:
             args["revision"] = data["revision"]
         if "gnetId" in data:
             args["gnet_id"] = data["gnetId"]
         if "tags" in data:
             args["tags"] = data["tags"]
-        if "style" in data:
-            args["style"] = data["style"]
         if "timezone" in data:
             args["timezone"] = data["timezone"]
         if "editable" in data:
             args["editable"] = data["editable"]
         if "graphTooltip" in data:
             args["graph_tooltip"] = data["graphTooltip"]
         if "time" in data:
             args["time"] = DashboardDashboardTime.from_json(data["time"])
         if "timepicker" in data:
-            args["timepicker"] = TimePicker.from_json(data["timepicker"])
+            args["timepicker"] = TimePickerConfig.from_json(data["timepicker"])
         if "fiscalYearStartMonth" in data:
             args["fiscal_year_start_month"] = data["fiscalYearStartMonth"]
         if "liveNow" in data:
             args["live_now"] = data["liveNow"]
         if "weekStart" in data:
             args["week_start"] = data["weekStart"]
         if "refresh" in data:
@@ -327,24 +322,27 @@
     icon_color: str
     # Filters to apply when fetching annotations
     filter_val: typing.Optional['AnnotationPanelFilter']
     # TODO.. this should just be a normal query target
     target: typing.Optional['AnnotationTarget']
     # TODO -- this should not exist here, it is based on the --grafana-- datasource
     type_val: typing.Optional[str]
+    # Set to 1 for the standard annotation query all dashboards have by default.
+    built_in: typing.Optional[float]
 
-    def __init__(self, name: str = "", datasource: typing.Optional['DataSourceRef'] = None, enable: bool = True, hide: typing.Optional[bool] = False, icon_color: str = "", filter_val: typing.Optional['AnnotationPanelFilter'] = None, target: typing.Optional['AnnotationTarget'] = None, type_val: typing.Optional[str] = None):
+    def __init__(self, name: str = "", datasource: typing.Optional['DataSourceRef'] = None, enable: bool = True, hide: typing.Optional[bool] = False, icon_color: str = "", filter_val: typing.Optional['AnnotationPanelFilter'] = None, target: typing.Optional['AnnotationTarget'] = None, type_val: typing.Optional[str] = None, built_in: typing.Optional[float] = 0):
         self.name = name
         self.datasource = datasource if datasource is not None else DataSourceRef()
         self.enable = enable
         self.hide = hide
         self.icon_color = icon_color
         self.filter_val = filter_val
         self.target = target
         self.type_val = type_val
+        self.built_in = built_in
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "name": self.name,
             "datasource": self.datasource,
             "enable": self.enable,
             "iconColor": self.icon_color,
@@ -353,14 +351,16 @@
             payload["hide"] = self.hide
         if self.filter_val is not None:
             payload["filter"] = self.filter_val
         if self.target is not None:
             payload["target"] = self.target
         if self.type_val is not None:
             payload["type"] = self.type_val
+        if self.built_in is not None:
+            payload["builtIn"] = self.built_in
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "name" in data:
@@ -374,44 +374,42 @@
         if "iconColor" in data:
             args["icon_color"] = data["iconColor"]
         if "filter" in data:
             args["filter_val"] = AnnotationPanelFilter.from_json(data["filter"])
         if "target" in data:
             args["target"] = AnnotationTarget.from_json(data["target"])
         if "type" in data:
-            args["type_val"] = data["type"]        
+            args["type_val"] = data["type"]
+        if "builtIn" in data:
+            args["built_in"] = data["builtIn"]        
 
         return cls(**args)
 
 
 class VariableModel:
     """
     A variable is a placeholder for a value. You can use variables in metric queries and in panel titles.
     """
 
-    # Unique numeric identifier for the variable.
-    id_val: str
     # Type of variable
     type_val: 'VariableType'
     # Name of variable
     name: str
     # Optional display name
     label: typing.Optional[str]
     # Visibility configuration for the variable
-    hide: 'VariableHide'
+    hide: typing.Optional['VariableHide']
     # Whether the variable value should be managed by URL query params or not
-    skip_url_sync: bool
+    skip_url_sync: typing.Optional[bool]
     # Description of variable. It can be defined but `null`.
     description: typing.Optional[str]
     # Query used to fetch values for a variable
     query: typing.Optional[typing.Union[str, dict[str, object]]]
     # Data source used to fetch values for a variable. It can be defined but `null`.
     datasource: typing.Optional['DataSourceRef']
-    # Format to use while fetching all values from data source, eg: wildcard, glob, regex, pipe, etc.
-    all_format: typing.Optional[str]
     # Shows current selected variable text/value on the dashboard
     current: typing.Optional['VariableOption']
     # Whether multiple values can be selected or not from variable value list
     multi: typing.Optional[bool]
     # Options that can be selected for a variable.
     options: typing.Optional[list['VariableOption']]
     # Options to config when to refresh a variable
@@ -422,52 +420,49 @@
     include_all: typing.Optional[bool]
     # Custom all value
     all_value: typing.Optional[str]
     # Optional field, if you want to extract part of a series name or metric node segment.
     # Named capture groups can be used to separate the display text and value.
     regex: typing.Optional[str]
 
-    def __init__(self, id_val: str = "00000000-0000-0000-0000-000000000000", type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: bool = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, dict[str, object]]] = None, datasource: typing.Optional['DataSourceRef'] = None, all_format: typing.Optional[str] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None, include_all: typing.Optional[bool] = False, all_value: typing.Optional[str] = None, regex: typing.Optional[str] = None):
-        self.id_val = id_val
+    def __init__(self, type_val: typing.Optional['VariableType'] = None, name: str = "", label: typing.Optional[str] = None, hide: typing.Optional['VariableHide'] = None, skip_url_sync: typing.Optional[bool] = False, description: typing.Optional[str] = None, query: typing.Optional[typing.Union[str, dict[str, object]]] = None, datasource: typing.Optional['DataSourceRef'] = None, current: typing.Optional['VariableOption'] = None, multi: typing.Optional[bool] = False, options: typing.Optional[list['VariableOption']] = None, refresh: typing.Optional['VariableRefresh'] = None, sort: typing.Optional['VariableSort'] = None, include_all: typing.Optional[bool] = False, all_value: typing.Optional[str] = None, regex: typing.Optional[str] = None):
         self.type_val = type_val if type_val is not None else VariableType.QUERY
         self.name = name
         self.label = label
-        self.hide = hide if hide is not None else VariableHide.DONT_HIDE
+        self.hide = hide
         self.skip_url_sync = skip_url_sync
         self.description = description
         self.query = query
         self.datasource = datasource
-        self.all_format = all_format
         self.current = current
         self.multi = multi
         self.options = options
         self.refresh = refresh
         self.sort = sort
         self.include_all = include_all
         self.all_value = all_value
         self.regex = regex
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "id": self.id_val,
             "type": self.type_val,
             "name": self.name,
-            "hide": self.hide,
-            "skipUrlSync": self.skip_url_sync,
         }
         if self.label is not None:
             payload["label"] = self.label
+        if self.hide is not None:
+            payload["hide"] = self.hide
+        if self.skip_url_sync is not None:
+            payload["skipUrlSync"] = self.skip_url_sync
         if self.description is not None:
             payload["description"] = self.description
         if self.query is not None:
             payload["query"] = self.query
         if self.datasource is not None:
             payload["datasource"] = self.datasource
-        if self.all_format is not None:
-            payload["allFormat"] = self.all_format
         if self.current is not None:
             payload["current"] = self.current
         if self.multi is not None:
             payload["multi"] = self.multi
         if self.options is not None:
             payload["options"] = self.options
         if self.refresh is not None:
@@ -482,16 +477,14 @@
             payload["regex"] = self.regex
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "id" in data:
-            args["id_val"] = data["id"]
         if "type" in data:
             args["type_val"] = data["type"]
         if "name" in data:
             args["name"] = data["name"]
         if "label" in data:
             args["label"] = data["label"]
         if "hide" in data:
@@ -500,16 +493,14 @@
             args["skip_url_sync"] = data["skipUrlSync"]
         if "description" in data:
             args["description"] = data["description"]
         if "query" in data:
             args["query"] = data["query"]
         if "datasource" in data:
             args["datasource"] = DataSourceRef.from_json(data["datasource"])
-        if "allFormat" in data:
-            args["all_format"] = data["allFormat"]
         if "current" in data:
             args["current"] = VariableOption.from_json(data["current"])
         if "multi" in data:
             args["multi"] = data["multi"]
         if "options" in data:
             args["options"] = data["options"]
         if "refresh" in data:
@@ -597,36 +588,27 @@
     `0`: No sorting
     `1`: Alphabetical ASC
     `2`: Alphabetical DESC
     `3`: Numerical ASC
     `4`: Numerical DESC
     `5`: Alphabetical Case Insensitive ASC
     `6`: Alphabetical Case Insensitive DESC
+    `7`: Natural ASC
+    `8`: Natural DESC
     """
 
     DISABLED = 0
     ALPHABETICAL_ASC = 1
     ALPHABETICAL_DESC = 2
     NUMERICAL_ASC = 3
     NUMERICAL_DESC = 4
     ALPHABETICAL_CASE_INSENSITIVE_ASC = 5
     ALPHABETICAL_CASE_INSENSITIVE_DESC = 6
-
-
-class LoadingState(enum.StrEnum):
-    """
-    Loading status
-    Accepted values are `NotStarted` (the request is not started), `Loading` (waiting for response), `Streaming` (pulling continuous data), `Done` (response received successfully) or `Error` (failed request).
-    """
-
-    NOT_STARTED = "NotStarted"
-    LOADING = "Loading"
-    STREAMING = "Streaming"
-    DONE = "Done"
-    ERROR = "Error"
+    NATURAL_ASC = 7
+    NATURAL_DESC = 8
 
 
 class DataSourceRef:
     """
     Ref to a DataSource instance
     """
 
@@ -670,27 +652,27 @@
     # Link type. Accepted values are dashboards (to refer to another dashboard) and link (to refer to an external resource)
     type_val: 'DashboardLinkType'
     # Icon name to be displayed with the link
     icon: str
     # Tooltip to display when the user hovers their mouse over it
     tooltip: str
     # Link URL. Only required/valid if the type is link
-    url: str
+    url: typing.Optional[str]
     # List of tags to limit the linked dashboards. If empty, all dashboards will be displayed. Only valid if the type is dashboards
     tags: list[str]
     # If true, all dashboards links will be displayed in a dropdown. If false, all dashboards links will be displayed side by side. Only valid if the type is dashboards
     as_dropdown: bool
     # If true, the link will be opened in a new tab
     target_blank: bool
     # If true, includes current template variables values in the link as query params
     include_vars: bool
     # If true, includes current time range in the link as query params
     keep_time: bool
 
-    def __init__(self, title: str = "", type_val: typing.Optional['DashboardLinkType'] = None, icon: str = "", tooltip: str = "", url: str = "", tags: typing.Optional[list[str]] = None, as_dropdown: bool = False, target_blank: bool = False, include_vars: bool = False, keep_time: bool = False):
+    def __init__(self, title: str = "", type_val: typing.Optional['DashboardLinkType'] = None, icon: str = "", tooltip: str = "", url: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, as_dropdown: bool = False, target_blank: bool = False, include_vars: bool = False, keep_time: bool = False):
         self.title = title
         self.type_val = type_val if type_val is not None else DashboardLinkType.LINK
         self.icon = icon
         self.tooltip = tooltip
         self.url = url
         self.tags = tags if tags is not None else []
         self.as_dropdown = as_dropdown
@@ -700,21 +682,22 @@
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "title": self.title,
             "type": self.type_val,
             "icon": self.icon,
             "tooltip": self.tooltip,
-            "url": self.url,
             "tags": self.tags,
             "asDropdown": self.as_dropdown,
             "targetBlank": self.target_blank,
             "includeVars": self.include_vars,
             "keepTime": self.keep_time,
         }
+        if self.url is not None:
+            payload["url"] = self.url
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "title" in data:
@@ -1243,14 +1226,54 @@
             args["filter_val"] = MatcherConfig.from_json(data["filter"])
         if "options" in data:
             args["options"] = data["options"]        
 
         return cls(**args)
 
 
+class TimePickerConfig:
+    """
+    Time picker configuration
+    It defines the default config for the time picker and the refresh picker for the specific dashboard.
+    """
+
+    # Whether timepicker is visible or not.
+    hidden: bool
+    # Interval options available in the refresh picker dropdown.
+    refresh_intervals: list[str]
+    # Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
+    time_options: list[str]
+
+    def __init__(self, hidden: bool = False, refresh_intervals: typing.Optional[list[str]] = None, time_options: typing.Optional[list[str]] = None):
+        self.hidden = hidden
+        self.refresh_intervals = refresh_intervals if refresh_intervals is not None else ["5s", "10s", "30s", "1m", "5m", "15m", "30m", "1h", "2h", "1d"]
+        self.time_options = time_options if time_options is not None else ["5m", "15m", "1h", "6h", "12h", "24h", "2d", "7d", "30d"]
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "hidden": self.hidden,
+            "refresh_intervals": self.refresh_intervals,
+            "time_options": self.time_options,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "hidden" in data:
+            args["hidden"] = data["hidden"]
+        if "refresh_intervals" in data:
+            args["refresh_intervals"] = data["refresh_intervals"]
+        if "time_options" in data:
+            args["time_options"] = data["time_options"]        
+
+        return cls(**args)
+
+
 class DashboardCursorSync(enum.IntEnum):
     """
     0 for no shared crosshair or tooltip (default).
     1 for shared crosshair.
     2 for shared crosshair AND shared tooltip.
     """
 
@@ -1373,34 +1396,35 @@
     # Depends on the panel plugin. See the plugin documentation for details.
     targets: typing.Optional[list[cogvariants.Dataquery]]
     # Panel title.
     title: typing.Optional[str]
     # Panel description.
     description: typing.Optional[str]
     # Whether to display the panel without a background.
-    transparent: bool
+    transparent: typing.Optional[bool]
     # The datasource used in all targets.
     datasource: typing.Optional['DataSourceRef']
     # Grid position.
     grid_pos: typing.Optional['GridPos']
     # Panel links.
     links: typing.Optional[list['DashboardLink']]
     # Name of template variable to repeat for.
     repeat: typing.Optional[str]
     # Direction to repeat in if 'repeat' is set.
     # `h` for horizontal, `v` for vertical.
     repeat_direction: typing.Optional[typing.Literal["h", "v"]]
-    # Id of the repeating panel.
-    repeat_panel_id: typing.Optional[int]
+    # Option for repeated panels that controls max items per row
+    # Only relevant for horizontally repeated panels
+    max_per_row: typing.Optional[float]
     # The maximum number of data points that the panel queries are retrieving.
     max_data_points: typing.Optional[float]
     # List of transformations that are applied to the panel data before rendering.
     # When there are multiple transformations, Grafana applies them in the order they are listed.
     # Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
-    transformations: list['DataTransformerConfig']
+    transformations: typing.Optional[list['DataTransformerConfig']]
     # The min time interval setting defines a lower limit for the $__interval and $__interval_ms variables.
     # This value must be formatted as a number followed by a valid time
     # identifier like: "40s", "3d", etc.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     interval: typing.Optional[str]
     # Overrides the relative time range for individual panels,
     # which causes them to be different than what is selected in
@@ -1412,87 +1436,96 @@
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_from: typing.Optional[str]
     # Overrides the time range for individual panels by shifting its start and end relative to the time picker.
     # For example, you can shift the time range for the panel to be two hours earlier than the dashboard time picker setting `2h`.
     # Note: Panel time overrides have no effect when the dashboard’s time range is absolute.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_shift: typing.Optional[str]
+    # Controls if the timeFrom or timeShift overrides are shown in the panel header
+    hide_time_override: typing.Optional[bool]
     # Dynamically load the panel
     library_panel: typing.Optional['LibraryPanelRef']
     # It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
-    options: object
+    options: typing.Optional[object]
     # Field options allow you to change how the data is displayed in your visualizations.
-    field_config: 'FieldConfigSource'
+    field_config: typing.Optional['FieldConfigSource']
 
-    def __init__(self, type_val: str = "", id_val: typing.Optional[int] = None, plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: bool = False, datasource: typing.Optional['DataSourceRef'] = None, grid_pos: typing.Optional['GridPos'] = None, links: typing.Optional[list['DashboardLink']] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, repeat_panel_id: typing.Optional[int] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list['DataTransformerConfig']] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, library_panel: typing.Optional['LibraryPanelRef'] = None, options: object = None, field_config: typing.Optional['FieldConfigSource'] = None):
+    def __init__(self, type_val: str = "", id_val: typing.Optional[int] = None, plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional['DataSourceRef'] = None, grid_pos: typing.Optional['GridPos'] = None, links: typing.Optional[list['DashboardLink']] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list['DataTransformerConfig']] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, library_panel: typing.Optional['LibraryPanelRef'] = None, options: typing.Optional[object] = None, field_config: typing.Optional['FieldConfigSource'] = None):
         self.type_val = type_val
         self.id_val = id_val
         self.plugin_version = plugin_version
         self.tags = tags
         self.targets = targets
         self.title = title
         self.description = description
         self.transparent = transparent
         self.datasource = datasource
         self.grid_pos = grid_pos
         self.links = links
         self.repeat = repeat
         self.repeat_direction = repeat_direction if repeat_direction is not None else "h"
-        self.repeat_panel_id = repeat_panel_id
+        self.max_per_row = max_per_row
         self.max_data_points = max_data_points
-        self.transformations = transformations if transformations is not None else []
+        self.transformations = transformations
         self.interval = interval
         self.time_from = time_from
         self.time_shift = time_shift
+        self.hide_time_override = hide_time_override
         self.library_panel = library_panel
         self.options = options
-        self.field_config = field_config if field_config is not None else FieldConfigSource()
+        self.field_config = field_config
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
-            "transparent": self.transparent,
-            "transformations": self.transformations,
-            "options": self.options,
-            "fieldConfig": self.field_config,
         }
         if self.id_val is not None:
             payload["id"] = self.id_val
         if self.plugin_version is not None:
             payload["pluginVersion"] = self.plugin_version
         if self.tags is not None:
             payload["tags"] = self.tags
         if self.targets is not None:
             payload["targets"] = self.targets
         if self.title is not None:
             payload["title"] = self.title
         if self.description is not None:
             payload["description"] = self.description
+        if self.transparent is not None:
+            payload["transparent"] = self.transparent
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         if self.grid_pos is not None:
             payload["gridPos"] = self.grid_pos
         if self.links is not None:
             payload["links"] = self.links
         if self.repeat is not None:
             payload["repeat"] = self.repeat
         if self.repeat_direction is not None:
             payload["repeatDirection"] = self.repeat_direction
-        if self.repeat_panel_id is not None:
-            payload["repeatPanelId"] = self.repeat_panel_id
+        if self.max_per_row is not None:
+            payload["maxPerRow"] = self.max_per_row
         if self.max_data_points is not None:
             payload["maxDataPoints"] = self.max_data_points
+        if self.transformations is not None:
+            payload["transformations"] = self.transformations
         if self.interval is not None:
             payload["interval"] = self.interval
         if self.time_from is not None:
             payload["timeFrom"] = self.time_from
         if self.time_shift is not None:
             payload["timeShift"] = self.time_shift
+        if self.hide_time_override is not None:
+            payload["hideTimeOverride"] = self.hide_time_override
         if self.library_panel is not None:
             payload["libraryPanel"] = self.library_panel
+        if self.options is not None:
+            payload["options"] = self.options
+        if self.field_config is not None:
+            payload["fieldConfig"] = self.field_config
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
@@ -1517,26 +1550,28 @@
             args["grid_pos"] = GridPos.from_json(data["gridPos"])
         if "links" in data:
             args["links"] = data["links"]
         if "repeat" in data:
             args["repeat"] = data["repeat"]
         if "repeatDirection" in data:
             args["repeat_direction"] = data["repeatDirection"]
-        if "repeatPanelId" in data:
-            args["repeat_panel_id"] = data["repeatPanelId"]
+        if "maxPerRow" in data:
+            args["max_per_row"] = data["maxPerRow"]
         if "maxDataPoints" in data:
             args["max_data_points"] = data["maxDataPoints"]
         if "transformations" in data:
             args["transformations"] = data["transformations"]
         if "interval" in data:
             args["interval"] = data["interval"]
         if "timeFrom" in data:
             args["time_from"] = data["timeFrom"]
         if "timeShift" in data:
             args["time_shift"] = data["timeShift"]
+        if "hideTimeOverride" in data:
+            args["hide_time_override"] = data["hideTimeOverride"]
         if "libraryPanel" in data:
             args["library_panel"] = LibraryPanelRef.from_json(data["libraryPanel"])
         if "options" in data:
             config = cogruntime.panelcfg_config(data.get("type", ""))
             if config is not None and config.options_from_json_hook is not None:
                 args["options"] = config.options_from_json_hook(data["options"])
             else:
@@ -1907,116 +1942,14 @@
             args["panels"] = data["panels"]
         if "repeat" in data:
             args["repeat"] = data["repeat"]        
 
         return cls(**args)
 
 
-class GraphPanel:
-    """
-    Support for legacy graph panel.
-    @deprecated this a deprecated panel type
-    """
-
-    type_val: typing.Literal["graph"]
-    # @deprecated this is part of deprecated graph panel
-    legend: typing.Optional['DashboardGraphPanelLegend']
-
-    def __init__(self, legend: typing.Optional['DashboardGraphPanelLegend'] = None):
-        self.type_val = "graph"
-        self.legend = legend
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "type": self.type_val,
-        }
-        if self.legend is not None:
-            payload["legend"] = self.legend
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "legend" in data:
-            args["legend"] = DashboardGraphPanelLegend.from_json(data["legend"])        
-
-        return cls(**args)
-
-
-class HeatmapPanel:
-    """
-    Support for legacy heatmap panel.
-    @deprecated this a deprecated panel type
-    """
-
-    type_val: typing.Literal["heatmap"]
-
-    def __init__(self, ):
-        self.type_val = "heatmap"
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "type": self.type_val,
-        }
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        return cls(**args)
-
-
-class TimePicker:
-    # Whether timepicker is visible or not.
-    hidden: bool
-    # Interval options available in the refresh picker dropdown.
-    refresh_intervals: list[str]
-    # Whether timepicker is collapsed or not. Has no effect on provisioned dashboard.
-    collapse: bool
-    # Whether timepicker is enabled or not. Has no effect on provisioned dashboard.
-    enable: bool
-    # Selectable options available in the time picker dropdown. Has no effect on provisioned dashboard.
-    time_options: list[str]
-
-    def __init__(self, hidden: bool = False, refresh_intervals: typing.Optional[list[str]] = None, collapse: bool = False, enable: bool = True, time_options: typing.Optional[list[str]] = None):
-        self.hidden = hidden
-        self.refresh_intervals = refresh_intervals if refresh_intervals is not None else ["5s", "10s", "30s", "1m", "5m", "15m", "30m", "1h", "2h", "1d"]
-        self.collapse = collapse
-        self.enable = enable
-        self.time_options = time_options if time_options is not None else ["5m", "15m", "1h", "6h", "12h", "24h", "2d", "7d", "30d"]
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "hidden": self.hidden,
-            "refresh_intervals": self.refresh_intervals,
-            "collapse": self.collapse,
-            "enable": self.enable,
-            "time_options": self.time_options,
-        }
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "hidden" in data:
-            args["hidden"] = data["hidden"]
-        if "refresh_intervals" in data:
-            args["refresh_intervals"] = data["refresh_intervals"]
-        if "collapse" in data:
-            args["collapse"] = data["collapse"]
-        if "enable" in data:
-            args["enable"] = data["enable"]
-        if "time_options" in data:
-            args["time_options"] = data["time_options"]        
-
-        return cls(**args)
-
-
 class DashboardDashboardTime:
     from_val: str
     to: str
 
     def __init__(self, from_val: str = "now-6h", to: str = "now"):
         self.from_val = from_val
         self.to = to
@@ -2180,42 +2113,8 @@
             args["matcher"] = MatcherConfig.from_json(data["matcher"])
         if "properties" in data:
             args["properties"] = data["properties"]        
 
         return cls(**args)
 
 
-class DashboardGraphPanelLegend:
-    show: bool
-    sort: typing.Optional[str]
-    sort_desc: typing.Optional[bool]
-
-    def __init__(self, show: bool = True, sort: typing.Optional[str] = None, sort_desc: typing.Optional[bool] = None):
-        self.show = show
-        self.sort = sort
-        self.sort_desc = sort_desc
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "show": self.show,
-        }
-        if self.sort is not None:
-            payload["sort"] = self.sort
-        if self.sort_desc is not None:
-            payload["sortDesc"] = self.sort_desc
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "show" in data:
-            args["show"] = data["show"]
-        if "sort" in data:
-            args["sort"] = data["sort"]
-        if "sortDesc" in data:
-            args["sort_desc"] = data["sortDesc"]        
-
-        return cls(**args)
-
-
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,31 @@
     include_vars: bool
     show_starred: bool
     show_recently_viewed: bool
     show_search: bool
     show_headings: bool
     max_items: int
     query: str
-    folder_id: typing.Optional[int]
     tags: list[str]
+    # folderId is deprecated, and migrated to folderUid on panel init
+    folder_id: typing.Optional[int]
+    folder_uid: typing.Optional[str]
 
-    def __init__(self, keep_time: bool = False, include_vars: bool = False, show_starred: bool = True, show_recently_viewed: bool = False, show_search: bool = False, show_headings: bool = True, max_items: int = 10, query: str = "", folder_id: typing.Optional[int] = None, tags: typing.Optional[list[str]] = None):
+    def __init__(self, keep_time: bool = False, include_vars: bool = False, show_starred: bool = True, show_recently_viewed: bool = False, show_search: bool = False, show_headings: bool = True, max_items: int = 10, query: str = "", tags: typing.Optional[list[str]] = None, folder_id: typing.Optional[int] = None, folder_uid: typing.Optional[str] = None):
         self.keep_time = keep_time
         self.include_vars = include_vars
         self.show_starred = show_starred
         self.show_recently_viewed = show_recently_viewed
         self.show_search = show_search
         self.show_headings = show_headings
         self.max_items = max_items
         self.query = query
-        self.folder_id = folder_id
         self.tags = tags if tags is not None else []
+        self.folder_id = folder_id
+        self.folder_uid = folder_uid
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "keepTime": self.keep_time,
             "includeVars": self.include_vars,
             "showStarred": self.show_starred,
             "showRecentlyViewed": self.show_recently_viewed,
@@ -38,14 +41,16 @@
             "showHeadings": self.show_headings,
             "maxItems": self.max_items,
             "query": self.query,
             "tags": self.tags,
         }
         if self.folder_id is not None:
             payload["folderId"] = self.folder_id
+        if self.folder_uid is not None:
+            payload["folderUID"] = self.folder_uid
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "keepTime" in data:
@@ -60,18 +65,20 @@
             args["show_search"] = data["showSearch"]
         if "showHeadings" in data:
             args["show_headings"] = data["showHeadings"]
         if "maxItems" in data:
             args["max_items"] = data["maxItems"]
         if "query" in data:
             args["query"] = data["query"]
+        if "tags" in data:
+            args["tags"] = data["tags"]
         if "folderId" in data:
             args["folder_id"] = data["folderId"]
-        if "tags" in data:
-            args["tags"] = data["tags"]        
+        if "folderUID" in data:
+            args["folder_uid"] = data["folderUID"]        
 
         return cls(**args)
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
         identifier="dashlist",
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/expr.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..cog import variants as cogvariants
 
 
 Expr: typing.TypeAlias = typing.Union['TypeMath', 'TypeReduce', 'TypeResample', 'TypeClassicConditions', 'TypeThreshold', 'TypeSql']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
-    decoding_map: dict[str, typing.Union[typing.Type[TypeResample], typing.Type[TypeClassicConditions], typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath], typing.Type[TypeReduce]]] = {"resample": TypeResample, "classic_conditions": TypeClassicConditions, "threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath, "reduce": TypeReduce}
+    decoding_map: dict[str, typing.Union[typing.Type[TypeThreshold], typing.Type[TypeSql], typing.Type[TypeMath], typing.Type[TypeReduce], typing.Type[TypeResample], typing.Type[TypeClassicConditions]]] = {"threshold": TypeThreshold, "sql": TypeSql, "math": TypeMath, "reduce": TypeReduce, "resample": TypeResample, "classic_conditions": TypeClassicConditions}
     return cogruntime.DataqueryConfig(
         identifier="__expr__",
         from_json_hook=lambda data: decoding_map[data["type"]].from_json(data),
     )
 
 
 class TypeMath(cogvariants.Dataquery):
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/folder.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/folder.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,30 +24,33 @@
     # queryType: #QueryType
     # Time Series List sub-query properties.
     time_series_list: typing.Optional['TimeSeriesList']
     # Time Series sub-query properties.
     time_series_query: typing.Optional['TimeSeriesQuery']
     # SLO sub-query properties.
     slo_query: typing.Optional['SLOQuery']
+    # PromQL sub-query properties.
+    prom_ql_query: typing.Optional['PromQLQuery']
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
     # Time interval in milliseconds.
     interval_ms: typing.Optional[float]
 
-    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, alias_by: typing.Optional[str] = None, time_series_list: typing.Optional['TimeSeriesList'] = None, time_series_query: typing.Optional['TimeSeriesQuery'] = None, slo_query: typing.Optional['SLOQuery'] = None, datasource: typing.Optional[object] = None, interval_ms: typing.Optional[float] = None):
+    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, alias_by: typing.Optional[str] = None, time_series_list: typing.Optional['TimeSeriesList'] = None, time_series_query: typing.Optional['TimeSeriesQuery'] = None, slo_query: typing.Optional['SLOQuery'] = None, prom_ql_query: typing.Optional['PromQLQuery'] = None, datasource: typing.Optional[object] = None, interval_ms: typing.Optional[float] = None):
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.alias_by = alias_by
         self.time_series_list = time_series_list
         self.time_series_query = time_series_query
         self.slo_query = slo_query
+        self.prom_ql_query = prom_ql_query
         self.datasource = datasource
         self.interval_ms = interval_ms
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "refId": self.ref_id,
         }
@@ -59,14 +62,16 @@
             payload["aliasBy"] = self.alias_by
         if self.time_series_list is not None:
             payload["timeSeriesList"] = self.time_series_list
         if self.time_series_query is not None:
             payload["timeSeriesQuery"] = self.time_series_query
         if self.slo_query is not None:
             payload["sloQuery"] = self.slo_query
+        if self.prom_ql_query is not None:
+            payload["promQLQuery"] = self.prom_ql_query
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         if self.interval_ms is not None:
             payload["intervalMs"] = self.interval_ms
         return payload
 
     @classmethod
@@ -83,14 +88,16 @@
             args["alias_by"] = data["aliasBy"]
         if "timeSeriesList" in data:
             args["time_series_list"] = TimeSeriesList.from_json(data["timeSeriesList"])
         if "timeSeriesQuery" in data:
             args["time_series_query"] = TimeSeriesQuery.from_json(data["timeSeriesQuery"])
         if "sloQuery" in data:
             args["slo_query"] = SLOQuery.from_json(data["sloQuery"])
+        if "promQLQuery" in data:
+            args["prom_ql_query"] = PromQLQuery.from_json(data["promQLQuery"])
         if "datasource" in data:
             args["datasource"] = data["datasource"]
         if "intervalMs" in data:
             args["interval_ms"] = data["intervalMs"]        
 
         return cls(**args)
 
@@ -107,14 +114,15 @@
     Defines the supported queryTypes.
     """
 
     TIME_SERIES_LIST = "timeSeriesList"
     TIME_SERIES_QUERY = "timeSeriesQuery"
     SLO = "slo"
     ANNOTATION = "annotation"
+    PROMQL = "promQL"
 
 
 class TimeSeriesList:
     """
     Time Series List sub-query properties.
     """
 
@@ -128,44 +136,44 @@
     per_series_aligner: typing.Optional[str]
     # Array of labels to group data by.
     group_bys: typing.Optional[list[str]]
     # Array of filters to query data by. Labels that can be filtered on are defined by the metric.
     filters: typing.Optional[list[str]]
     # Data view, defaults to FULL.
     view: typing.Optional[str]
+    # Annotation title.
+    title: typing.Optional[str]
+    # Annotation text.
+    text: typing.Optional[str]
     # Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
     secondary_cross_series_reducer: typing.Optional[str]
     # Only present if a preprocessor is selected. Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
     secondary_alignment_period: typing.Optional[str]
     # Only present if a preprocessor is selected. Alignment function to be used. Defaults to ALIGN_MEAN.
     secondary_per_series_aligner: typing.Optional[str]
     # Only present if a preprocessor is selected. Array of labels to group data by.
     secondary_group_bys: typing.Optional[list[str]]
     # Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
     preprocessor: typing.Optional['PreprocessorType']
-    # Annotation title.
-    title: typing.Optional[str]
-    # Annotation text.
-    text: typing.Optional[str]
 
-    def __init__(self, project_name: str = "", cross_series_reducer: str = "", alignment_period: typing.Optional[str] = None, per_series_aligner: typing.Optional[str] = None, group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, view: typing.Optional[str] = None, secondary_cross_series_reducer: typing.Optional[str] = None, secondary_alignment_period: typing.Optional[str] = None, secondary_per_series_aligner: typing.Optional[str] = None, secondary_group_bys: typing.Optional[list[str]] = None, preprocessor: typing.Optional['PreprocessorType'] = None, title: typing.Optional[str] = None, text: typing.Optional[str] = None):
+    def __init__(self, project_name: str = "", cross_series_reducer: str = "", alignment_period: typing.Optional[str] = None, per_series_aligner: typing.Optional[str] = None, group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, view: typing.Optional[str] = None, title: typing.Optional[str] = None, text: typing.Optional[str] = None, secondary_cross_series_reducer: typing.Optional[str] = None, secondary_alignment_period: typing.Optional[str] = None, secondary_per_series_aligner: typing.Optional[str] = None, secondary_group_bys: typing.Optional[list[str]] = None, preprocessor: typing.Optional['PreprocessorType'] = None):
         self.project_name = project_name
         self.cross_series_reducer = cross_series_reducer
         self.alignment_period = alignment_period
         self.per_series_aligner = per_series_aligner
         self.group_bys = group_bys
         self.filters = filters
         self.view = view
+        self.title = title
+        self.text = text
         self.secondary_cross_series_reducer = secondary_cross_series_reducer
         self.secondary_alignment_period = secondary_alignment_period
         self.secondary_per_series_aligner = secondary_per_series_aligner
         self.secondary_group_bys = secondary_group_bys
         self.preprocessor = preprocessor
-        self.title = title
-        self.text = text
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "projectName": self.project_name,
             "crossSeriesReducer": self.cross_series_reducer,
         }
         if self.alignment_period is not None:
@@ -174,28 +182,28 @@
             payload["perSeriesAligner"] = self.per_series_aligner
         if self.group_bys is not None:
             payload["groupBys"] = self.group_bys
         if self.filters is not None:
             payload["filters"] = self.filters
         if self.view is not None:
             payload["view"] = self.view
+        if self.title is not None:
+            payload["title"] = self.title
+        if self.text is not None:
+            payload["text"] = self.text
         if self.secondary_cross_series_reducer is not None:
             payload["secondaryCrossSeriesReducer"] = self.secondary_cross_series_reducer
         if self.secondary_alignment_period is not None:
             payload["secondaryAlignmentPeriod"] = self.secondary_alignment_period
         if self.secondary_per_series_aligner is not None:
             payload["secondaryPerSeriesAligner"] = self.secondary_per_series_aligner
         if self.secondary_group_bys is not None:
             payload["secondaryGroupBys"] = self.secondary_group_bys
         if self.preprocessor is not None:
             payload["preprocessor"] = self.preprocessor
-        if self.title is not None:
-            payload["title"] = self.title
-        if self.text is not None:
-            payload["text"] = self.text
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "projectName" in data:
@@ -208,159 +216,42 @@
             args["per_series_aligner"] = data["perSeriesAligner"]
         if "groupBys" in data:
             args["group_bys"] = data["groupBys"]
         if "filters" in data:
             args["filters"] = data["filters"]
         if "view" in data:
             args["view"] = data["view"]
+        if "title" in data:
+            args["title"] = data["title"]
+        if "text" in data:
+            args["text"] = data["text"]
         if "secondaryCrossSeriesReducer" in data:
             args["secondary_cross_series_reducer"] = data["secondaryCrossSeriesReducer"]
         if "secondaryAlignmentPeriod" in data:
             args["secondary_alignment_period"] = data["secondaryAlignmentPeriod"]
         if "secondaryPerSeriesAligner" in data:
             args["secondary_per_series_aligner"] = data["secondaryPerSeriesAligner"]
         if "secondaryGroupBys" in data:
             args["secondary_group_bys"] = data["secondaryGroupBys"]
         if "preprocessor" in data:
-            args["preprocessor"] = data["preprocessor"]
-        if "title" in data:
-            args["title"] = data["title"]
-        if "text" in data:
-            args["text"] = data["text"]        
+            args["preprocessor"] = data["preprocessor"]        
 
         return cls(**args)
 
 
 class PreprocessorType(enum.StrEnum):
     """
     Types of pre-processor available. Defined by the metric.
     """
 
     NONE = "none"
     RATE = "rate"
     DELTA = "delta"
 
 
-class AnnotationQuery:
-    """
-    Annotation sub-query properties.
-    """
-
-    # GCP project to execute the query against.
-    project_name: str
-    # Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
-    cross_series_reducer: str
-    # Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
-    alignment_period: typing.Optional[str]
-    # Alignment function to be used. Defaults to ALIGN_MEAN.
-    per_series_aligner: typing.Optional[str]
-    # Array of labels to group data by.
-    group_bys: typing.Optional[list[str]]
-    # Array of filters to query data by. Labels that can be filtered on are defined by the metric.
-    filters: typing.Optional[list[str]]
-    # Data view, defaults to FULL.
-    view: typing.Optional[str]
-    # Only present if a preprocessor is selected. Reducer applied across a set of time-series values. Defaults to REDUCE_NONE.
-    secondary_cross_series_reducer: typing.Optional[str]
-    # Only present if a preprocessor is selected. Alignment period to use when regularizing data. Defaults to cloud-monitoring-auto.
-    secondary_alignment_period: typing.Optional[str]
-    # Only present if a preprocessor is selected. Alignment function to be used. Defaults to ALIGN_MEAN.
-    secondary_per_series_aligner: typing.Optional[str]
-    # Only present if a preprocessor is selected. Array of labels to group data by.
-    secondary_group_bys: typing.Optional[list[str]]
-    # Annotation title.
-    title: typing.Optional[str]
-    # Preprocessor is not part of the API, but is used to store the preprocessor and not affect the UI for the rest of parameters
-    preprocessor: typing.Optional['PreprocessorType']
-    # Annotation text.
-    text: typing.Optional[str]
-
-    def __init__(self, project_name: str = "", cross_series_reducer: str = "", alignment_period: typing.Optional[str] = None, per_series_aligner: typing.Optional[str] = None, group_bys: typing.Optional[list[str]] = None, filters: typing.Optional[list[str]] = None, view: typing.Optional[str] = None, secondary_cross_series_reducer: typing.Optional[str] = None, secondary_alignment_period: typing.Optional[str] = None, secondary_per_series_aligner: typing.Optional[str] = None, secondary_group_bys: typing.Optional[list[str]] = None, title: typing.Optional[str] = None, preprocessor: typing.Optional['PreprocessorType'] = None, text: typing.Optional[str] = None):
-        self.project_name = project_name
-        self.cross_series_reducer = cross_series_reducer
-        self.alignment_period = alignment_period
-        self.per_series_aligner = per_series_aligner
-        self.group_bys = group_bys
-        self.filters = filters
-        self.view = view
-        self.secondary_cross_series_reducer = secondary_cross_series_reducer
-        self.secondary_alignment_period = secondary_alignment_period
-        self.secondary_per_series_aligner = secondary_per_series_aligner
-        self.secondary_group_bys = secondary_group_bys
-        self.title = title
-        self.preprocessor = preprocessor
-        self.text = text
-
-    def to_json(self) -> dict[str, object]:
-        payload: dict[str, object] = {
-            "projectName": self.project_name,
-            "crossSeriesReducer": self.cross_series_reducer,
-        }
-        if self.alignment_period is not None:
-            payload["alignmentPeriod"] = self.alignment_period
-        if self.per_series_aligner is not None:
-            payload["perSeriesAligner"] = self.per_series_aligner
-        if self.group_bys is not None:
-            payload["groupBys"] = self.group_bys
-        if self.filters is not None:
-            payload["filters"] = self.filters
-        if self.view is not None:
-            payload["view"] = self.view
-        if self.secondary_cross_series_reducer is not None:
-            payload["secondaryCrossSeriesReducer"] = self.secondary_cross_series_reducer
-        if self.secondary_alignment_period is not None:
-            payload["secondaryAlignmentPeriod"] = self.secondary_alignment_period
-        if self.secondary_per_series_aligner is not None:
-            payload["secondaryPerSeriesAligner"] = self.secondary_per_series_aligner
-        if self.secondary_group_bys is not None:
-            payload["secondaryGroupBys"] = self.secondary_group_bys
-        if self.title is not None:
-            payload["title"] = self.title
-        if self.preprocessor is not None:
-            payload["preprocessor"] = self.preprocessor
-        if self.text is not None:
-            payload["text"] = self.text
-        return payload
-
-    @classmethod
-    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
-        args: dict[str, typing.Any] = {}
-        
-        if "projectName" in data:
-            args["project_name"] = data["projectName"]
-        if "crossSeriesReducer" in data:
-            args["cross_series_reducer"] = data["crossSeriesReducer"]
-        if "alignmentPeriod" in data:
-            args["alignment_period"] = data["alignmentPeriod"]
-        if "perSeriesAligner" in data:
-            args["per_series_aligner"] = data["perSeriesAligner"]
-        if "groupBys" in data:
-            args["group_bys"] = data["groupBys"]
-        if "filters" in data:
-            args["filters"] = data["filters"]
-        if "view" in data:
-            args["view"] = data["view"]
-        if "secondaryCrossSeriesReducer" in data:
-            args["secondary_cross_series_reducer"] = data["secondaryCrossSeriesReducer"]
-        if "secondaryAlignmentPeriod" in data:
-            args["secondary_alignment_period"] = data["secondaryAlignmentPeriod"]
-        if "secondaryPerSeriesAligner" in data:
-            args["secondary_per_series_aligner"] = data["secondaryPerSeriesAligner"]
-        if "secondaryGroupBys" in data:
-            args["secondary_group_bys"] = data["secondaryGroupBys"]
-        if "title" in data:
-            args["title"] = data["title"]
-        if "preprocessor" in data:
-            args["preprocessor"] = data["preprocessor"]
-        if "text" in data:
-            args["text"] = data["text"]        
-
-        return cls(**args)
-
-
 class TimeSeriesQuery:
     """
     Time Series sub-query properties.
     """
 
     # GCP project to execute the query against.
     project_name: str
@@ -478,14 +369,53 @@
             args["goal"] = data["goal"]
         if "lookbackPeriod" in data:
             args["lookback_period"] = data["lookbackPeriod"]        
 
         return cls(**args)
 
 
+class PromQLQuery:
+    """
+    PromQL sub-query properties.
+    """
+
+    # GCP project to execute the query against.
+    project_name: str
+    # PromQL expression/query to be executed.
+    expr: str
+    # PromQL min step
+    step: str
+
+    def __init__(self, project_name: str = "", expr: str = "", step: str = ""):
+        self.project_name = project_name
+        self.expr = expr
+        self.step = step
+
+    def to_json(self) -> dict[str, object]:
+        payload: dict[str, object] = {
+            "projectName": self.project_name,
+            "expr": self.expr,
+            "step": self.step,
+        }
+        return payload
+
+    @classmethod
+    def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
+        args: dict[str, typing.Any] = {}
+        
+        if "projectName" in data:
+            args["project_name"] = data["projectName"]
+        if "expr" in data:
+            args["expr"] = data["expr"]
+        if "step" in data:
+            args["step"] = data["step"]        
+
+        return cls(**args)
+
+
 class MetricQuery:
     """
     @deprecated This type is for migration purposes only. Replaced by TimeSeriesList Metric sub-query properties.
     """
 
     # GCP project to execute the query against.
     project_name: str
@@ -635,15 +565,15 @@
     ALIGN_PERCENTILE_05 = "ALIGN_PERCENTILE_05"
     ALIGN_PERCENT_CHANGE = "ALIGN_PERCENT_CHANGE"
     ALIGN_NONE = "ALIGN_NONE"
 
 
 class LegacyCloudMonitoringAnnotationQuery:
     """
-    @deprecated Use AnnotationQuery instead. Legacy annotation query properties for migration purposes.
+    @deprecated Use TimeSeriesList instead. Legacy annotation query properties for migration purposes.
     """
 
     # GCP project to execute the query against.
     project_name: str
     metric_type: str
     # Query refId.
     ref_id: str
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/grafanapyroscope.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/parca.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,25 @@
 
 import enum
 from ..cog import variants as cogvariants
 import typing
 from ..cog import runtime as cogruntime
 
 
-class PhlareQueryType(enum.StrEnum):
+class ParcaQueryType(enum.StrEnum):
     METRICS = "metrics"
     PROFILE = "profile"
     BOTH = "both"
 
 
 class Dataquery(cogvariants.Dataquery):
     # Specifies the query label selectors.
     label_selector: str
     # Specifies the type of profile to query.
     profile_type_id: str
-    # Allows to group the results.
-    group_by: list[str]
-    # Sets the maximum number of nodes in the flamegraph.
-    max_nodes: typing.Optional[int]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
     # true if query is disabled (ie should not be returned to the dashboard)
     # Note this does not always imply that the query should not be executed since
     # the results from a hidden query may be used as the input to other queries (SSE etc)
@@ -34,33 +30,28 @@
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
 
-    def __init__(self, label_selector: str = "{}", profile_type_id: str = "", group_by: typing.Optional[list[str]] = None, max_nodes: typing.Optional[int] = None, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
+    def __init__(self, label_selector: str = "{}", profile_type_id: str = "", ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
         self.label_selector = label_selector
         self.profile_type_id = profile_type_id
-        self.group_by = group_by if group_by is not None else []
-        self.max_nodes = max_nodes
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.datasource = datasource
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "labelSelector": self.label_selector,
             "profileTypeId": self.profile_type_id,
-            "groupBy": self.group_by,
             "refId": self.ref_id,
         }
-        if self.max_nodes is not None:
-            payload["maxNodes"] = self.max_nodes
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         return payload
@@ -69,31 +60,27 @@
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "labelSelector" in data:
             args["label_selector"] = data["labelSelector"]
         if "profileTypeId" in data:
             args["profile_type_id"] = data["profileTypeId"]
-        if "groupBy" in data:
-            args["group_by"] = data["groupBy"]
-        if "maxNodes" in data:
-            args["max_nodes"] = data["maxNodes"]
         if "refId" in data:
             args["ref_id"] = data["refId"]
         if "hide" in data:
             args["hide"] = data["hide"]
         if "queryType" in data:
             args["query_type"] = data["queryType"]
         if "datasource" in data:
             args["datasource"] = data["datasource"]        
 
         return cls(**args)
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
     return cogruntime.DataqueryConfig(
-        identifier="grafanapyroscope",
+        identifier="parca",
         from_json_hook=Dataquery.from_json,
     )
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,33 +120,35 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
+    axis_centered_zero: typing.Optional[bool]
     # Sets the maximum value for the yAxis
     max_val: typing.Optional[float]
-    axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, unit: typing.Optional[str] = None, reverse: typing.Optional[bool] = None, decimals: typing.Optional[float] = None, min_val: typing.Optional[float] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, max_val: typing.Optional[float] = None, axis_centered_zero: typing.Optional[bool] = None):
+    def __init__(self, unit: typing.Optional[str] = None, reverse: typing.Optional[bool] = None, decimals: typing.Optional[float] = None, min_val: typing.Optional[float] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, max_val: typing.Optional[float] = None, axis_border_show: typing.Optional[bool] = None):
         self.unit = unit
         self.reverse = reverse
         self.decimals = decimals
         self.min_val = min_val
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.max_val = max_val
         self.axis_centered_zero = axis_centered_zero
+        self.max_val = max_val
+        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.unit is not None:
             payload["unit"] = self.unit
         if self.reverse is not None:
@@ -167,18 +169,20 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.max_val is not None:
-            payload["max"] = self.max_val
         if self.axis_centered_zero is not None:
             payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.max_val is not None:
+            payload["max"] = self.max_val
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "unit" in data:
@@ -201,18 +205,20 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "max" in data:
             args["max_val"] = data["max"]
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]        
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
 
 
 class CellValues:
     """
     Controls cell value options
@@ -288,35 +294,42 @@
     Controls tooltip options
     """
 
     # Controls if the tooltip is shown
     show: bool
     # Controls if the tooltip shows a histogram of the y-axis values
     y_histogram: typing.Optional[bool]
+    # Controls if the tooltip shows a color scale in header
+    show_color_scale: typing.Optional[bool]
 
-    def __init__(self, show: bool = False, y_histogram: typing.Optional[bool] = None):
+    def __init__(self, show: bool = False, y_histogram: typing.Optional[bool] = None, show_color_scale: typing.Optional[bool] = None):
         self.show = show
         self.y_histogram = y_histogram
+        self.show_color_scale = show_color_scale
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "show": self.show,
         }
         if self.y_histogram is not None:
             payload["yHistogram"] = self.y_histogram
+        if self.show_color_scale is not None:
+            payload["showColorScale"] = self.show_color_scale
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "show" in data:
             args["show"] = data["show"]
         if "yHistogram" in data:
-            args["y_histogram"] = data["yHistogram"]        
+            args["y_histogram"] = data["yHistogram"]
+        if "showColorScale" in data:
+            args["show_color_scale"] = data["showColorScale"]        
 
         return cls(**args)
 
 
 class HeatmapLegend:
     """
     Controls legend options
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/histogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,34 +62,36 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
+    axis_centered_zero: typing.Optional[bool]
     hide_from: typing.Optional[common.HideSeriesConfig]
     # Set the mode of the gradient fill. Fill gradient is based on the line color. To change the color, use the standard color scheme field option.
     # Gradient appearance is influenced by the Fill opacity setting.
     gradient_mode: typing.Optional[common.GraphGradientMode]
-    axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_centered_zero: typing.Optional[bool] = None):
+    def __init__(self, line_width: typing.Optional[int] = 1, fill_opacity: typing.Optional[int] = 80, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, gradient_mode: typing.Optional[common.GraphGradientMode] = None, axis_border_show: typing.Optional[bool] = None):
         self.line_width = line_width
         self.fill_opacity = fill_opacity
         self.axis_placement = axis_placement
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
+        self.axis_centered_zero = axis_centered_zero
         self.hide_from = hide_from
         self.gradient_mode = gradient_mode if gradient_mode is not None else common.GraphGradientMode.NONE
-        self.axis_centered_zero = axis_centered_zero
+        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.line_width is not None:
             payload["lineWidth"] = self.line_width
         if self.fill_opacity is not None:
@@ -106,20 +108,22 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.hide_from is not None:
             payload["hideFrom"] = self.hide_from
         if self.gradient_mode is not None:
             payload["gradientMode"] = self.gradient_mode
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "lineWidth" in data:
@@ -138,20 +142,22 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "hideFrom" in data:
             args["hide_from"] = common.HideSeriesConfig.from_json(data["hideFrom"])
         if "gradientMode" in data:
             args["gradient_mode"] = data["gradientMode"]
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]        
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,32 +176,33 @@
     # Depends on the panel plugin. See the plugin documentation for details.
     targets: typing.Optional[list[cogvariants.Dataquery]]
     # Panel title.
     title: typing.Optional[str]
     # Panel description.
     description: typing.Optional[str]
     # Whether to display the panel without a background.
-    transparent: bool
+    transparent: typing.Optional[bool]
     # The datasource used in all targets.
     datasource: typing.Optional[dashboard.DataSourceRef]
     # Panel links.
     links: typing.Optional[list[dashboard.DashboardLink]]
     # Name of template variable to repeat for.
     repeat: typing.Optional[str]
     # Direction to repeat in if 'repeat' is set.
     # `h` for horizontal, `v` for vertical.
     repeat_direction: typing.Optional[typing.Literal["h", "v"]]
-    # Id of the repeating panel.
-    repeat_panel_id: typing.Optional[int]
+    # Option for repeated panels that controls max items per row
+    # Only relevant for horizontally repeated panels
+    max_per_row: typing.Optional[float]
     # The maximum number of data points that the panel queries are retrieving.
     max_data_points: typing.Optional[float]
     # List of transformations that are applied to the panel data before rendering.
     # When there are multiple transformations, Grafana applies them in the order they are listed.
     # Each transformation creates a result set that then passes on to the next transformation in the processing pipeline.
-    transformations: list[dashboard.DataTransformerConfig]
+    transformations: typing.Optional[list[dashboard.DataTransformerConfig]]
     # The min time interval setting defines a lower limit for the $__interval and $__interval_ms variables.
     # This value must be formatted as a number followed by a valid time
     # identifier like: "40s", "3d", etc.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     interval: typing.Optional[str]
     # Overrides the relative time range for individual panels,
     # which causes them to be different than what is selected in
@@ -213,76 +214,85 @@
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_from: typing.Optional[str]
     # Overrides the time range for individual panels by shifting its start and end relative to the time picker.
     # For example, you can shift the time range for the panel to be two hours earlier than the dashboard time picker setting `2h`.
     # Note: Panel time overrides have no effect when the dashboard’s time range is absolute.
     # See: https://grafana.com/docs/grafana/latest/panels-visualizations/query-transform-data/#query-options
     time_shift: typing.Optional[str]
+    # Controls if the timeFrom or timeShift overrides are shown in the panel header
+    hide_time_override: typing.Optional[bool]
     # It depends on the panel plugin. They are specified by the Options field in panel plugin schemas.
-    options: object
+    options: typing.Optional[object]
     # Field options allow you to change how the data is displayed in your visualizations.
-    field_config: dashboard.FieldConfigSource
+    field_config: typing.Optional[dashboard.FieldConfigSource]
 
-    def __init__(self, type_val: str = "", plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: bool = False, datasource: typing.Optional[dashboard.DataSourceRef] = None, links: typing.Optional[list[dashboard.DashboardLink]] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, repeat_panel_id: typing.Optional[int] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list[dashboard.DataTransformerConfig]] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, options: object = None, field_config: typing.Optional[dashboard.FieldConfigSource] = None):
+    def __init__(self, type_val: str = "", plugin_version: typing.Optional[str] = None, tags: typing.Optional[list[str]] = None, targets: typing.Optional[list[cogvariants.Dataquery]] = None, title: typing.Optional[str] = None, description: typing.Optional[str] = None, transparent: typing.Optional[bool] = False, datasource: typing.Optional[dashboard.DataSourceRef] = None, links: typing.Optional[list[dashboard.DashboardLink]] = None, repeat: typing.Optional[str] = None, repeat_direction: typing.Optional[typing.Literal["h", "v"]] = None, max_per_row: typing.Optional[float] = None, max_data_points: typing.Optional[float] = None, transformations: typing.Optional[list[dashboard.DataTransformerConfig]] = None, interval: typing.Optional[str] = None, time_from: typing.Optional[str] = None, time_shift: typing.Optional[str] = None, hide_time_override: typing.Optional[bool] = None, options: typing.Optional[object] = None, field_config: typing.Optional[dashboard.FieldConfigSource] = None):
         self.type_val = type_val
         self.plugin_version = plugin_version
         self.tags = tags
         self.targets = targets
         self.title = title
         self.description = description
         self.transparent = transparent
         self.datasource = datasource
         self.links = links
         self.repeat = repeat
         self.repeat_direction = repeat_direction if repeat_direction is not None else "h"
-        self.repeat_panel_id = repeat_panel_id
+        self.max_per_row = max_per_row
         self.max_data_points = max_data_points
-        self.transformations = transformations if transformations is not None else []
+        self.transformations = transformations
         self.interval = interval
         self.time_from = time_from
         self.time_shift = time_shift
+        self.hide_time_override = hide_time_override
         self.options = options
-        self.field_config = field_config if field_config is not None else dashboard.FieldConfigSource()
+        self.field_config = field_config
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "type": self.type_val,
-            "transparent": self.transparent,
-            "transformations": self.transformations,
-            "options": self.options,
-            "fieldConfig": self.field_config,
         }
         if self.plugin_version is not None:
             payload["pluginVersion"] = self.plugin_version
         if self.tags is not None:
             payload["tags"] = self.tags
         if self.targets is not None:
             payload["targets"] = self.targets
         if self.title is not None:
             payload["title"] = self.title
         if self.description is not None:
             payload["description"] = self.description
+        if self.transparent is not None:
+            payload["transparent"] = self.transparent
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         if self.links is not None:
             payload["links"] = self.links
         if self.repeat is not None:
             payload["repeat"] = self.repeat
         if self.repeat_direction is not None:
             payload["repeatDirection"] = self.repeat_direction
-        if self.repeat_panel_id is not None:
-            payload["repeatPanelId"] = self.repeat_panel_id
+        if self.max_per_row is not None:
+            payload["maxPerRow"] = self.max_per_row
         if self.max_data_points is not None:
             payload["maxDataPoints"] = self.max_data_points
+        if self.transformations is not None:
+            payload["transformations"] = self.transformations
         if self.interval is not None:
             payload["interval"] = self.interval
         if self.time_from is not None:
             payload["timeFrom"] = self.time_from
         if self.time_shift is not None:
             payload["timeShift"] = self.time_shift
+        if self.hide_time_override is not None:
+            payload["hideTimeOverride"] = self.hide_time_override
+        if self.options is not None:
+            payload["options"] = self.options
+        if self.field_config is not None:
+            payload["fieldConfig"] = self.field_config
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "type" in data:
@@ -303,26 +313,28 @@
             args["datasource"] = dashboard.DataSourceRef.from_json(data["datasource"])
         if "links" in data:
             args["links"] = data["links"]
         if "repeat" in data:
             args["repeat"] = data["repeat"]
         if "repeatDirection" in data:
             args["repeat_direction"] = data["repeatDirection"]
-        if "repeatPanelId" in data:
-            args["repeat_panel_id"] = data["repeatPanelId"]
+        if "maxPerRow" in data:
+            args["max_per_row"] = data["maxPerRow"]
         if "maxDataPoints" in data:
             args["max_data_points"] = data["maxDataPoints"]
         if "transformations" in data:
             args["transformations"] = data["transformations"]
         if "interval" in data:
             args["interval"] = data["interval"]
         if "timeFrom" in data:
             args["time_from"] = data["timeFrom"]
         if "timeShift" in data:
             args["time_shift"] = data["timeShift"]
+        if "hideTimeOverride" in data:
+            args["hide_time_override"] = data["hideTimeOverride"]
         if "options" in data:
             args["options"] = data["options"]
         if "fieldConfig" in data:
             args["field_config"] = dashboard.FieldConfigSource.from_json(data["fieldConfig"])        
 
         return cls(**args)
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/grafanapyroscope.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 
 import enum
 from ..cog import variants as cogvariants
 import typing
 from ..cog import runtime as cogruntime
 
 
-class ParcaQueryType(enum.StrEnum):
+class PyroscopeQueryType(enum.StrEnum):
     METRICS = "metrics"
     PROFILE = "profile"
     BOTH = "both"
 
 
 class Dataquery(cogvariants.Dataquery):
     # Specifies the query label selectors.
     label_selector: str
+    # Specifies the query span selectors.
+    span_selector: typing.Optional[list[str]]
     # Specifies the type of profile to query.
     profile_type_id: str
+    # Allows to group the results.
+    group_by: list[str]
+    # Sets the maximum number of nodes in the flamegraph.
+    max_nodes: typing.Optional[int]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
     # true if query is disabled (ie should not be returned to the dashboard)
     # Note this does not always imply that the query should not be executed since
     # the results from a hidden query may be used as the input to other queries (SSE etc)
@@ -30,57 +36,71 @@
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
 
-    def __init__(self, label_selector: str = "{}", profile_type_id: str = "", ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
+    def __init__(self, label_selector: str = "{}", span_selector: typing.Optional[list[str]] = None, profile_type_id: str = "", group_by: typing.Optional[list[str]] = None, max_nodes: typing.Optional[int] = None, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
         self.label_selector = label_selector
+        self.span_selector = span_selector
         self.profile_type_id = profile_type_id
+        self.group_by = group_by if group_by is not None else []
+        self.max_nodes = max_nodes
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.datasource = datasource
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "labelSelector": self.label_selector,
             "profileTypeId": self.profile_type_id,
+            "groupBy": self.group_by,
             "refId": self.ref_id,
         }
+        if self.span_selector is not None:
+            payload["spanSelector"] = self.span_selector
+        if self.max_nodes is not None:
+            payload["maxNodes"] = self.max_nodes
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "labelSelector" in data:
             args["label_selector"] = data["labelSelector"]
+        if "spanSelector" in data:
+            args["span_selector"] = data["spanSelector"]
         if "profileTypeId" in data:
             args["profile_type_id"] = data["profileTypeId"]
+        if "groupBy" in data:
+            args["group_by"] = data["groupBy"]
+        if "maxNodes" in data:
+            args["max_nodes"] = data["maxNodes"]
         if "refId" in data:
             args["ref_id"] = data["refId"]
         if "hide" in data:
             args["hide"] = data["hide"]
         if "queryType" in data:
             args["query_type"] = data["queryType"]
         if "datasource" in data:
             args["datasource"] = data["datasource"]        
 
         return cls(**args)
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
     return cogruntime.DataqueryConfig(
-        identifier="parca",
+        identifier="grafanapyroscope",
         from_json_hook=Dataquery.from_json,
     )
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/playlist.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,100 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
+import enum
 import typing
+from ..cog import runtime as cogruntime
 
 
-class Playlist:
-    # Unique playlist identifier. Generated on creation, either by the
-    # creator of the playlist of by the application.
-    uid: str
-    # Name of the playlist.
-    name: str
-    # Interval sets the time between switching views in a playlist.
-    # FIXME: Is this based on a standardized format or what options are available? Can datemath be used?
-    interval: str
-    # The ordered list of items that the playlist will iterate over.
-    # FIXME! This should not be optional, but changing it makes the godegen awkward
-    items: typing.Optional[list['PlaylistItem']]
-
-    def __init__(self, uid: str = "", name: str = "", interval: str = "5m", items: typing.Optional[list['PlaylistItem']] = None):
-        self.uid = uid
-        self.name = name
-        self.interval = interval
-        self.items = items
+class TextMode(enum.StrEnum):
+    HTML = "html"
+    MARKDOWN = "markdown"
+    CODE = "code"
+
+
+class CodeLanguage(enum.StrEnum):
+    JSON = "json"
+    YAML = "yaml"
+    XML = "xml"
+    TYPESCRIPT = "typescript"
+    SQL = "sql"
+    GO = "go"
+    MARKDOWN = "markdown"
+    HTML = "html"
+    PLAINTEXT = "plaintext"
+
+
+class CodeOptions:
+    # The language passed to monaco code editor
+    language: 'CodeLanguage'
+    show_line_numbers: bool
+    show_mini_map: bool
+
+    def __init__(self, language: typing.Optional['CodeLanguage'] = None, show_line_numbers: bool = False, show_mini_map: bool = False):
+        self.language = language if language is not None else CodeLanguage.PLAINTEXT
+        self.show_line_numbers = show_line_numbers
+        self.show_mini_map = show_mini_map
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "uid": self.uid,
-            "name": self.name,
-            "interval": self.interval,
+            "language": self.language,
+            "showLineNumbers": self.show_line_numbers,
+            "showMiniMap": self.show_mini_map,
         }
-        if self.items is not None:
-            payload["items"] = self.items
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "uid" in data:
-            args["uid"] = data["uid"]
-        if "name" in data:
-            args["name"] = data["name"]
-        if "interval" in data:
-            args["interval"] = data["interval"]
-        if "items" in data:
-            args["items"] = data["items"]        
+        if "language" in data:
+            args["language"] = data["language"]
+        if "showLineNumbers" in data:
+            args["show_line_numbers"] = data["showLineNumbers"]
+        if "showMiniMap" in data:
+            args["show_mini_map"] = data["showMiniMap"]        
 
         return cls(**args)
 
 
-class PlaylistItem:
-    # Type of the item.
-    type_val: typing.Literal["dashboard_by_uid", "dashboard_by_id", "dashboard_by_tag"]
-    # Value depends on type and describes the playlist item.
-    # 
-    #  - dashboard_by_id: The value is an internal numerical identifier set by Grafana. This
-    #  is not portable as the numerical identifier is non-deterministic between different instances.
-    #  Will be replaced by dashboard_by_uid in the future. (deprecated)
-    #  - dashboard_by_tag: The value is a tag which is set on any number of dashboards. All
-    #  dashboards behind the tag will be added to the playlist.
-    #  - dashboard_by_uid: The value is the dashboard UID
-    value: str
-    # Title is an unused property -- it will be removed in the future
-    title: typing.Optional[str]
-
-    def __init__(self, type_val: typing.Optional[typing.Literal["dashboard_by_uid", "dashboard_by_id", "dashboard_by_tag"]] = None, value: str = "", title: typing.Optional[str] = None):
-        self.type_val = type_val if type_val is not None else "dashboard_by_uid"
-        self.value = value
-        self.title = title
+class Options:
+    mode: 'TextMode'
+    code: typing.Optional['CodeOptions']
+    content: str
+
+    def __init__(self, mode: typing.Optional['TextMode'] = None, code: typing.Optional['CodeOptions'] = None, content: str = "# Title\n\nFor markdown syntax help: [commonmark.org/help](https://commonmark.org/help/)"):
+        self.mode = mode if mode is not None else TextMode.MARKDOWN
+        self.code = code
+        self.content = content
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
-            "type": self.type_val,
-            "value": self.value,
+            "mode": self.mode,
+            "content": self.content,
         }
-        if self.title is not None:
-            payload["title"] = self.title
+        if self.code is not None:
+            payload["code"] = self.code
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
-        if "type" in data:
-            args["type_val"] = data["type"]
-        if "value" in data:
-            args["value"] = data["value"]
-        if "title" in data:
-            args["title"] = data["title"]        
+        if "mode" in data:
+            args["mode"] = data["mode"]
+        if "code" in data:
+            args["code"] = CodeOptions.from_json(data["code"])
+        if "content" in data:
+            args["content"] = data["content"]        
 
         return cls(**args)
 
 
 
+
+
+def variant_config():
+    return cogruntime.PanelCfgConfig(
+        identifier="text",
+        options_from_json_hook=Options.from_json,
+        field_config_from_json_hook=None,
+    )
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/preferences.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
 import typing
 
 
 class Preferences:
+    """
+    Spec defines user, team or org Grafana preferences
+    swagger:model Preferences
+    """
+
     # UID for the home dashboard
     home_dashboard_uid: typing.Optional[str]
     # The timezone selection
     # TODO: this should use the timezone defined in common
     timezone: typing.Optional[str]
     # day of the week (sunday, monday, etc)
     week_start: typing.Optional[str]
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/prometheus.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/prometheus.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/stat.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 from ..cog import runtime as cogruntime
 
 
 class Options:
     graph_mode: common.BigValueGraphMode
     color_mode: common.BigValueColorMode
     justify_mode: common.BigValueJustifyMode
+    text_mode: common.BigValueTextMode
     reduce_options: common.ReduceDataOptions
     text: typing.Optional[common.VizTextDisplayOptions]
-    text_mode: common.BigValueTextMode
+    wide_layout: bool
     orientation: common.VizOrientation
 
-    def __init__(self, graph_mode: typing.Optional[common.BigValueGraphMode] = None, color_mode: typing.Optional[common.BigValueColorMode] = None, justify_mode: typing.Optional[common.BigValueJustifyMode] = None, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, text_mode: typing.Optional[common.BigValueTextMode] = None, orientation: typing.Optional[common.VizOrientation] = None):
+    def __init__(self, graph_mode: typing.Optional[common.BigValueGraphMode] = None, color_mode: typing.Optional[common.BigValueColorMode] = None, justify_mode: typing.Optional[common.BigValueJustifyMode] = None, text_mode: typing.Optional[common.BigValueTextMode] = None, reduce_options: typing.Optional[common.ReduceDataOptions] = None, text: typing.Optional[common.VizTextDisplayOptions] = None, wide_layout: bool = True, orientation: typing.Optional[common.VizOrientation] = None):
         self.graph_mode = graph_mode if graph_mode is not None else common.BigValueGraphMode.AREA
         self.color_mode = color_mode if color_mode is not None else common.BigValueColorMode.VALUE
         self.justify_mode = justify_mode if justify_mode is not None else common.BigValueJustifyMode.AUTO
+        self.text_mode = text_mode if text_mode is not None else common.BigValueTextMode.AUTO
         self.reduce_options = reduce_options if reduce_options is not None else common.ReduceDataOptions()
         self.text = text
-        self.text_mode = text_mode if text_mode is not None else common.BigValueTextMode.AUTO
+        self.wide_layout = wide_layout
         self.orientation = orientation if orientation is not None else common.VizOrientation.AUTO
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "graphMode": self.graph_mode,
             "colorMode": self.color_mode,
             "justifyMode": self.justify_mode,
-            "reduceOptions": self.reduce_options,
             "textMode": self.text_mode,
+            "reduceOptions": self.reduce_options,
+            "wideLayout": self.wide_layout,
             "orientation": self.orientation,
         }
         if self.text is not None:
             payload["text"] = self.text
         return payload
 
     @classmethod
@@ -42,20 +45,22 @@
         
         if "graphMode" in data:
             args["graph_mode"] = data["graphMode"]
         if "colorMode" in data:
             args["color_mode"] = data["colorMode"]
         if "justifyMode" in data:
             args["justify_mode"] = data["justifyMode"]
+        if "textMode" in data:
+            args["text_mode"] = data["textMode"]
         if "reduceOptions" in data:
             args["reduce_options"] = common.ReduceDataOptions.from_json(data["reduceOptions"])
         if "text" in data:
             args["text"] = common.VizTextDisplayOptions.from_json(data["text"])
-        if "textMode" in data:
-            args["text_mode"] = data["textMode"]
+        if "wideLayout" in data:
+            args["wide_layout"] = data["wideLayout"]
         if "orientation" in data:
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
 def variant_config():
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/table.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,13 +58,19 @@
             args["footer"] = common.TableFooterOptions.from_json(data["footer"])
         if "cellHeight" in data:
             args["cell_height"] = data["cellHeight"]        
 
         return cls(**args)
 
 
+FieldConfig: typing.TypeAlias = common.TableFieldOptions
+
+
+
+
+
 def variant_config():
     return cogruntime.PanelCfgConfig(
         identifier="table",
         options_from_json_hook=Options.from_json,
-        field_config_from_json_hook=None,
+        field_config_from_json_hook=FieldConfig.from_json,
     )
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/tempo.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # Note this does not always imply that the query should not be executed since
     # the results from a hidden query may be used as the input to other queries (SSE etc)
     hide: typing.Optional[bool]
     # Specify the query flavor
     # TODO make this required and give it a default
     query_type: typing.Optional[str]
     # TraceQL query or trace ID
-    query: str
+    query: typing.Optional[str]
     # @deprecated Logfmt query to filter traces by their tags. Example: http.status_code=200 error=true
     search: typing.Optional[str]
     # @deprecated Query traces by service name
     service_name: typing.Optional[str]
     # @deprecated Query traces by span name
     span_name: typing.Optional[str]
     # @deprecated Define the minimum duration to select traces. Use duration format, for example: 1.2s, 100ms
@@ -32,47 +32,57 @@
     max_duration: typing.Optional[str]
     # Filters to be included in a PromQL query to select data for the service graph. Example: {client="app",service="app"}
     service_map_query: typing.Optional[str]
     # Use service.namespace in addition to service.name to uniquely identify a service.
     service_map_include_namespace: typing.Optional[bool]
     # Defines the maximum number of traces that are returned from Tempo
     limit: typing.Optional[int]
+    # Defines the maximum number of spans per spanset that are returned from Tempo
+    spss: typing.Optional[int]
+    filters: list['TraceqlFilter']
+    # Filters that are used to query the metrics summary
+    group_by: typing.Optional[list['TraceqlFilter']]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
-    filters: list['TraceqlFilter']
+    # The type of the table that is used to display the search results
+    table_type: typing.Optional['SearchTableType']
 
-    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, query: str = "", search: typing.Optional[str] = None, service_name: typing.Optional[str] = None, span_name: typing.Optional[str] = None, min_duration: typing.Optional[str] = None, max_duration: typing.Optional[str] = None, service_map_query: typing.Optional[str] = None, service_map_include_namespace: typing.Optional[bool] = None, limit: typing.Optional[int] = None, datasource: typing.Optional[object] = None, filters: typing.Optional[list['TraceqlFilter']] = None):
+    def __init__(self, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, query: typing.Optional[str] = None, search: typing.Optional[str] = None, service_name: typing.Optional[str] = None, span_name: typing.Optional[str] = None, min_duration: typing.Optional[str] = None, max_duration: typing.Optional[str] = None, service_map_query: typing.Optional[str] = None, service_map_include_namespace: typing.Optional[bool] = None, limit: typing.Optional[int] = None, spss: typing.Optional[int] = None, filters: typing.Optional[list['TraceqlFilter']] = None, group_by: typing.Optional[list['TraceqlFilter']] = None, datasource: typing.Optional[object] = None, table_type: typing.Optional['SearchTableType'] = None):
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.query = query
         self.search = search
         self.service_name = service_name
         self.span_name = span_name
         self.min_duration = min_duration
         self.max_duration = max_duration
         self.service_map_query = service_map_query
         self.service_map_include_namespace = service_map_include_namespace
         self.limit = limit
-        self.datasource = datasource
+        self.spss = spss
         self.filters = filters if filters is not None else []
+        self.group_by = group_by
+        self.datasource = datasource
+        self.table_type = table_type
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
             "refId": self.ref_id,
-            "query": self.query,
             "filters": self.filters,
         }
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
+        if self.query is not None:
+            payload["query"] = self.query
         if self.search is not None:
             payload["search"] = self.search
         if self.service_name is not None:
             payload["serviceName"] = self.service_name
         if self.span_name is not None:
             payload["spanName"] = self.span_name
         if self.min_duration is not None:
@@ -81,16 +91,22 @@
             payload["maxDuration"] = self.max_duration
         if self.service_map_query is not None:
             payload["serviceMapQuery"] = self.service_map_query
         if self.service_map_include_namespace is not None:
             payload["serviceMapIncludeNamespace"] = self.service_map_include_namespace
         if self.limit is not None:
             payload["limit"] = self.limit
+        if self.spss is not None:
+            payload["spss"] = self.spss
+        if self.group_by is not None:
+            payload["groupBy"] = self.group_by
         if self.datasource is not None:
             payload["datasource"] = self.datasource
+        if self.table_type is not None:
+            payload["tableType"] = self.table_type
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "refId" in data:
@@ -113,18 +129,24 @@
             args["max_duration"] = data["maxDuration"]
         if "serviceMapQuery" in data:
             args["service_map_query"] = data["serviceMapQuery"]
         if "serviceMapIncludeNamespace" in data:
             args["service_map_include_namespace"] = data["serviceMapIncludeNamespace"]
         if "limit" in data:
             args["limit"] = data["limit"]
+        if "spss" in data:
+            args["spss"] = data["spss"]
+        if "filters" in data:
+            args["filters"] = data["filters"]
+        if "groupBy" in data:
+            args["group_by"] = data["groupBy"]
         if "datasource" in data:
             args["datasource"] = data["datasource"]
-        if "filters" in data:
-            args["filters"] = data["filters"]        
+        if "tableType" in data:
+            args["table_type"] = data["tableType"]        
 
         return cls(**args)
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
     return cogruntime.DataqueryConfig(
         identifier="tempo",
@@ -154,19 +176,29 @@
 
     PENDING = "pending"
     STREAMING = "streaming"
     DONE = "done"
     ERROR = "error"
 
 
+class SearchTableType(enum.StrEnum):
+    """
+    The type of the table that is used to display the search results
+    """
+
+    TRACES = "traces"
+    SPANS = "spans"
+
+
 class TraceqlSearchScope(enum.StrEnum):
     """
     static fields are pre-set in the UI, dynamic fields are added by the user
     """
 
+    INTRINSIC = "intrinsic"
     UNSCOPED = "unscoped"
     RESOURCE = "resource"
     SPAN = "span"
 
 
 class TraceqlFilter:
     # Uniquely identify the filter, will not be used in the query generation
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/testdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,14 +352,15 @@
     series_count: typing.Optional[int]
     usa: typing.Optional['USAQuery']
     error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]]
     span_count: typing.Optional[int]
     points: typing.Optional[list[list[typing.Union[str, int]]]]
     # Drop percentage (the chance we will lose a point 0-100)
     drop_percent: typing.Optional[float]
+    flamegraph_diff: typing.Optional[bool]
     # A unique identifier for the query within the list of targets.
     # In server side expressions, the refId is used as a variable name to identify results.
     # By default, the UI will assign A->Z; however setting meaningful names may be useful.
     ref_id: str
     # true if query is disabled (ie should not be returned to the dashboard)
     # Note this does not always imply that the query should not be executed since
     # the results from a hidden query may be used as the input to other queries (SSE etc)
@@ -369,15 +370,15 @@
     query_type: typing.Optional[str]
     # For mixed data sources the selected datasource is on the query level.
     # For non mixed scenarios this is undefined.
     # TODO find a better way to do this ^ that's friendly to schema
     # TODO this shouldn't be unknown but DataSourceRef | null
     datasource: typing.Optional[object]
 
-    def __init__(self, alias: typing.Optional[str] = None, scenario_id: typing.Optional['TestDataQueryType'] = None, string_input: typing.Optional[str] = None, stream: typing.Optional['StreamingQuery'] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, sim: typing.Optional['SimulationQuery'] = None, csv_wave: typing.Optional[list['CSVWave']] = None, labels: typing.Optional[str] = None, lines: typing.Optional[int] = None, level_column: typing.Optional[bool] = None, channel: typing.Optional[str] = None, nodes: typing.Optional['NodesQuery'] = None, csv_file_name: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, series_count: typing.Optional[int] = None, usa: typing.Optional['USAQuery'] = None, error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]] = None, span_count: typing.Optional[int] = None, points: typing.Optional[list[list[typing.Union[str, int]]]] = None, drop_percent: typing.Optional[float] = None, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
+    def __init__(self, alias: typing.Optional[str] = None, scenario_id: typing.Optional['TestDataQueryType'] = None, string_input: typing.Optional[str] = None, stream: typing.Optional['StreamingQuery'] = None, pulse_wave: typing.Optional['PulseWaveQuery'] = None, sim: typing.Optional['SimulationQuery'] = None, csv_wave: typing.Optional[list['CSVWave']] = None, labels: typing.Optional[str] = None, lines: typing.Optional[int] = None, level_column: typing.Optional[bool] = None, channel: typing.Optional[str] = None, nodes: typing.Optional['NodesQuery'] = None, csv_file_name: typing.Optional[str] = None, csv_content: typing.Optional[str] = None, raw_frame_content: typing.Optional[str] = None, series_count: typing.Optional[int] = None, usa: typing.Optional['USAQuery'] = None, error_type: typing.Optional[typing.Literal["server_panic", "frontend_exception", "frontend_observable"]] = None, span_count: typing.Optional[int] = None, points: typing.Optional[list[list[typing.Union[str, int]]]] = None, drop_percent: typing.Optional[float] = None, flamegraph_diff: typing.Optional[bool] = None, ref_id: str = "", hide: typing.Optional[bool] = None, query_type: typing.Optional[str] = None, datasource: typing.Optional[object] = None):
         self.alias = alias
         self.scenario_id = scenario_id if scenario_id is not None else TestDataQueryType.RANDOM_WALK
         self.string_input = string_input
         self.stream = stream
         self.pulse_wave = pulse_wave
         self.sim = sim
         self.csv_wave = csv_wave
@@ -391,14 +392,15 @@
         self.raw_frame_content = raw_frame_content
         self.series_count = series_count
         self.usa = usa
         self.error_type = error_type
         self.span_count = span_count
         self.points = points
         self.drop_percent = drop_percent
+        self.flamegraph_diff = flamegraph_diff
         self.ref_id = ref_id
         self.hide = hide
         self.query_type = query_type
         self.datasource = datasource
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
@@ -442,14 +444,16 @@
             payload["errorType"] = self.error_type
         if self.span_count is not None:
             payload["spanCount"] = self.span_count
         if self.points is not None:
             payload["points"] = self.points
         if self.drop_percent is not None:
             payload["dropPercent"] = self.drop_percent
+        if self.flamegraph_diff is not None:
+            payload["flamegraphDiff"] = self.flamegraph_diff
         if self.hide is not None:
             payload["hide"] = self.hide
         if self.query_type is not None:
             payload["queryType"] = self.query_type
         if self.datasource is not None:
             payload["datasource"] = self.datasource
         return payload
@@ -496,14 +500,16 @@
             args["error_type"] = data["errorType"]
         if "spanCount" in data:
             args["span_count"] = data["spanCount"]
         if "points" in data:
             args["points"] = data["points"]
         if "dropPercent" in data:
             args["drop_percent"] = data["dropPercent"]
+        if "flamegraphDiff" in data:
+            args["flamegraph_diff"] = data["flamegraphDiff"]
         if "refId" in data:
             args["ref_id"] = data["refId"]
         if "hide" in data:
             args["hide"] = data["hide"]
         if "queryType" in data:
             args["query_type"] = data["queryType"]
         if "datasource" in data:
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/trend.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1717160602!10.2.0/grafana_foundation_sdk/models/xychart.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,18 +64,19 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
-    label_value: typing.Optional[common.TextDimensionConfig]
     axis_centered_zero: typing.Optional[bool]
+    label_value: typing.Optional[common.TextDimensionConfig]
+    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_centered_zero: typing.Optional[bool] = None):
+    def __init__(self, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_border_show: typing.Optional[bool] = None):
         self.show = show if show is not None else ScatterShow.POINTS
         self.point_size = point_size
         self.point_color = point_color
         self.line_color = line_color
         self.line_width = line_width
         self.line_style = line_style
         self.label = label if label is not None else common.VisibilityMode.AUTO
@@ -84,16 +85,17 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
-        self.label_value = label_value
         self.axis_centered_zero = axis_centered_zero
+        self.label_value = label_value
+        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.show is not None:
             payload["show"] = self.show
         if self.point_size is not None:
@@ -122,18 +124,20 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
-        if self.label_value is not None:
-            payload["labelValue"] = self.label_value
         if self.axis_centered_zero is not None:
             payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.label_value is not None:
+            payload["labelValue"] = self.label_value
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "show" in data:
@@ -164,18 +168,20 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "labelValue" in data:
             args["label_value"] = common.TextDimensionConfig.from_json(data["labelValue"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]        
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
 
 
 class ScatterSeriesConfig:
     x: typing.Optional[str]
     y: typing.Optional[str]
@@ -191,19 +197,20 @@
     axis_color_mode: typing.Optional[common.AxisColorMode]
     axis_label: typing.Optional[str]
     axis_width: typing.Optional[float]
     axis_soft_min: typing.Optional[float]
     axis_soft_max: typing.Optional[float]
     axis_grid_show: typing.Optional[bool]
     scale_distribution: typing.Optional[common.ScaleDistributionConfig]
+    axis_centered_zero: typing.Optional[bool]
     name: typing.Optional[str]
     label_value: typing.Optional[common.TextDimensionConfig]
-    axis_centered_zero: typing.Optional[bool]
+    axis_border_show: typing.Optional[bool]
 
-    def __init__(self, x: typing.Optional[str] = None, y: typing.Optional[str] = None, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, name: typing.Optional[str] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_centered_zero: typing.Optional[bool] = None):
+    def __init__(self, x: typing.Optional[str] = None, y: typing.Optional[str] = None, show: typing.Optional['ScatterShow'] = None, point_size: typing.Optional[common.ScaleDimensionConfig] = None, point_color: typing.Optional[common.ColorDimensionConfig] = None, line_color: typing.Optional[common.ColorDimensionConfig] = None, line_width: typing.Optional[int] = None, line_style: typing.Optional[common.LineStyle] = None, label: typing.Optional[common.VisibilityMode] = None, hide_from: typing.Optional[common.HideSeriesConfig] = None, axis_placement: typing.Optional[common.AxisPlacement] = None, axis_color_mode: typing.Optional[common.AxisColorMode] = None, axis_label: typing.Optional[str] = None, axis_width: typing.Optional[float] = None, axis_soft_min: typing.Optional[float] = None, axis_soft_max: typing.Optional[float] = None, axis_grid_show: typing.Optional[bool] = None, scale_distribution: typing.Optional[common.ScaleDistributionConfig] = None, axis_centered_zero: typing.Optional[bool] = None, name: typing.Optional[str] = None, label_value: typing.Optional[common.TextDimensionConfig] = None, axis_border_show: typing.Optional[bool] = None):
         self.x = x
         self.y = y
         self.show = show if show is not None else ScatterShow.POINTS
         self.point_size = point_size
         self.point_color = point_color
         self.line_color = line_color
         self.line_width = line_width
@@ -214,17 +221,18 @@
         self.axis_color_mode = axis_color_mode
         self.axis_label = axis_label
         self.axis_width = axis_width
         self.axis_soft_min = axis_soft_min
         self.axis_soft_max = axis_soft_max
         self.axis_grid_show = axis_grid_show
         self.scale_distribution = scale_distribution
+        self.axis_centered_zero = axis_centered_zero
         self.name = name
         self.label_value = label_value
-        self.axis_centered_zero = axis_centered_zero
+        self.axis_border_show = axis_border_show
 
     def to_json(self) -> dict[str, object]:
         payload: dict[str, object] = {
         }
         if self.x is not None:
             payload["x"] = self.x
         if self.y is not None:
@@ -257,20 +265,22 @@
             payload["axisSoftMin"] = self.axis_soft_min
         if self.axis_soft_max is not None:
             payload["axisSoftMax"] = self.axis_soft_max
         if self.axis_grid_show is not None:
             payload["axisGridShow"] = self.axis_grid_show
         if self.scale_distribution is not None:
             payload["scaleDistribution"] = self.scale_distribution
+        if self.axis_centered_zero is not None:
+            payload["axisCenteredZero"] = self.axis_centered_zero
         if self.name is not None:
             payload["name"] = self.name
         if self.label_value is not None:
             payload["labelValue"] = self.label_value
-        if self.axis_centered_zero is not None:
-            payload["axisCenteredZero"] = self.axis_centered_zero
+        if self.axis_border_show is not None:
+            payload["axisBorderShow"] = self.axis_border_show
         return payload
 
     @classmethod
     def from_json(cls, data: dict[str, typing.Any]) -> typing.Self:
         args: dict[str, typing.Any] = {}
         
         if "x" in data:
@@ -305,20 +315,22 @@
             args["axis_soft_min"] = data["axisSoftMin"]
         if "axisSoftMax" in data:
             args["axis_soft_max"] = data["axisSoftMax"]
         if "axisGridShow" in data:
             args["axis_grid_show"] = data["axisGridShow"]
         if "scaleDistribution" in data:
             args["scale_distribution"] = common.ScaleDistributionConfig.from_json(data["scaleDistribution"])
+        if "axisCenteredZero" in data:
+            args["axis_centered_zero"] = data["axisCenteredZero"]
         if "name" in data:
             args["name"] = data["name"]
         if "labelValue" in data:
             args["label_value"] = common.TextDimensionConfig.from_json(data["labelValue"])
-        if "axisCenteredZero" in data:
-            args["axis_centered_zero"] = data["axisCenteredZero"]        
+        if "axisBorderShow" in data:
+            args["axis_border_show"] = data["axisBorderShow"]        
 
         return cls(**args)
 
 
 class Options:
     series_mapping: typing.Optional['SeriesMapping']
     dims: 'XYDimensionConfig'
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/LICENSE.md` & `grafana_foundation_sdk-1717160602!10.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/README.md` & `grafana_foundation_sdk-1717160602!10.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v10.1.x.**
+> This branch contains **types and builders generated for Grafana v10.2.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1717160592!10.1.0'
+python3 -m pip install 'grafana_foundation_sdk==1717160602!10.2.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/pyproject.toml` & `grafana_foundation_sdk-1717160602!10.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1717160592!10.1.0"
+version = "1717160602!10.2.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1717160592!10.1.0/PKG-INFO` & `grafana_foundation_sdk-1717160602!10.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1717160592!10.1.0
+Version: 1717160602!10.2.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -21,21 +21,21 @@
 Description-Content-Type: text/markdown
 
 # Grafana Foundation SDK – Python
 
 A set of tools, types and *builder libraries* for building and manipulating Grafana objects in Python.
 
 > [!NOTE]
-> This branch contains **types and builders generated for Grafana v10.1.x.**
+> This branch contains **types and builders generated for Grafana v10.2.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1717160592!10.1.0'
+python3 -m pip install 'grafana_foundation_sdk==1717160602!10.2.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

