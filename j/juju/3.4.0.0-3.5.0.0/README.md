# Comparing `tmp/juju-3.4.0.0.tar.gz` & `tmp/juju-3.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juju-3.4.0.0.tar", last modified: Thu Mar 28 18:08:28 2024, max compression
+gzip compressed data, was "juju-3.5.0.0.tar", last modified: Fri May 31 13:56:59 2024, max compression
```

## Comparing `juju-3.4.0.0.tar` & `juju-3.5.0.0.tar`

### file list

```diff
@@ -1,171 +1,172 @@
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      155 2024-03-28 18:05:09.000000 juju-3.4.0.0/CONTRIBUTORS
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11344 2024-03-28 18:05:09.000000 juju-3.4.0.0/LICENSE
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      151 2024-03-28 18:05:09.000000 juju-3.4.0.0/MANIFEST.in
--rw-r--r--   0 aflynn    (1000) aflynn    (1000)    42136 2024-03-28 18:08:28.989335 juju-3.4.0.0/PKG-INFO
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3238 2024-03-28 18:05:09.000000 juju-3.4.0.0/README.rst
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.885335 juju-3.4.0.0/docs/
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.893335 juju-3.4.0.0/docs/api/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      190 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.action.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.annotation.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      210 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.application.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2352 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.client.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      210 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.constraints.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.controller.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.delta.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      190 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.errors.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.exceptions.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.juju.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.loop.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      194 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.machine.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.model.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      202 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.placement.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      198 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.relation.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      178 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.tag.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.unit.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.utils.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      575 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/modules.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    37933 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/changelog.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      666 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/index.rst
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.893335 juju-3.4.0.0/docs/narrative/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3034 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/application.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2747 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/controller.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      100 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/index.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     8713 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/model.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1469 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/unit.rst
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3238 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/readme.rst
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.893335 juju-3.4.0.0/docs/upstream-updates/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6676 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/upstream-updates/index.rst
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.909335 juju-3.4.0.0/examples/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1254 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/action.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1757 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_k8s.py
--rwxrwxr-x   0 aflynn    (1000) aflynn    (1000)     1688 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_machine.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1784 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_model.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2073 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_secrets_backend.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      914 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/allwatcher.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1033 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_deploy_k8s.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      925 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_deploy_machine.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      956 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_find.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      796 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_info.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      627 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/cloud.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      651 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/clouds.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1484 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/config.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      798 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/connect_current_model.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1050 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/controller.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1541 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/credential.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2243 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2356 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel_bundle.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2561 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel_controller.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2974 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel_relation.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      936 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/debug-log.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      983 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1557 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_bundle.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      958 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_bundle_charmhub.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1170 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_bundle_with_trust.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1045 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_constraints.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      832 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_big_k8s_bundle.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1155 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_bundle_with_resources.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1315 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_file_resource.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1298 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_resource.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      898 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_with_revision.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2552 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/expose-application.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1331 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/formatted_status.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      517 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/fullstatus.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1165 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/future.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      737 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/get_cloud.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      678 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/leadership.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      345 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/list_secrets.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      764 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/livemodel.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      776 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/local_refresh.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      824 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/localcharm.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1169 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/machine_hostname.py
--rwxrwxr-x   0 aflynn    (1000) aflynn    (1000)      827 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/model.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1141 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/modelsummaries.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3334 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/relate.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      947 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/run_action.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1209 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/scp.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1290 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/status.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1714 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/unitrun.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1289 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/upgrade_local_charm_k8s.py
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.917335 juju-3.4.0.0/juju/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/__init__.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1341 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/access.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      737 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/action.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      214 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/annotation.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1167 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/annotationhelper.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38148 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/application.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    45606 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/bundle.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      208 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/charm.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     7284 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/charmhub.py
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.985335 juju-3.4.0.0/juju/client/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/__init__.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     8864 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   730276 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client1.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    41464 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client10.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   196254 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client11.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   245218 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client12.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   244188 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client13.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   115453 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client14.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   108914 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client15.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   103511 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client16.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   103511 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client17.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   369413 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client18.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   364812 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client19.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   406826 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client2.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   192763 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client3.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   201775 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client4.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    41639 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client5.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   162501 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client6.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   247072 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client7.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    45251 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client8.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    56944 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client9.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)  1236275 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_definitions.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1319 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/client.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1442 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/codegen.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    40536 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/connection.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     9267 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/connector.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    32274 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/facade.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      416 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/flags.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3755 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/gocookies.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     7148 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/jujudata.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    12560 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/overrides.py
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/juju/client/proxy/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      774 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/proxy/factory.py
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/juju/client/proxy/kubernetes/
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2210 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/proxy/kubernetes/proxy.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      563 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/proxy/proxy.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      894 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/runner.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     4573 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/constraints.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38332 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/controller.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2732 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/delta.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3726 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/errors.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      142 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/exceptions.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3763 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/jasyncio.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1257 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/juju.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      231 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/loop.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11122 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/machine.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   125230 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/model.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2229 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/names.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6545 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/offerendpoints.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     5893 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/origin.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1924 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/placement.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11518 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/provisioner.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/py.typed
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     5049 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/relation.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      951 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/remoteapplication.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3877 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/secrets.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6616 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/status.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1408 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/tag.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    15858 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/unit.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     4863 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/url.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6486 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/user.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    18997 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/utils.py
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      230 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/version.py
-drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/juju.egg-info/
--rw-r--r--   0 aflynn    (1000) aflynn    (1000)    42136 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/PKG-INFO
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3668 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/SOURCES.txt
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        1 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/dependency_links.txt
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      178 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/requires.txt
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        5 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/top_level.txt
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)       38 2024-03-28 18:08:28.989335 juju-3.4.0.0/setup.cfg
--rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1747 2024-03-28 18:05:09.000000 juju-3.4.0.0/setup.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.341721 juju-3.5.0.0/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      155 2024-05-31 13:45:45.000000 juju-3.5.0.0/CONTRIBUTORS
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11344 2024-05-31 13:45:45.000000 juju-3.5.0.0/LICENSE
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      151 2024-05-31 13:45:45.000000 juju-3.5.0.0/MANIFEST.in
+-rw-r--r--   0 aflynn    (1000) aflynn    (1000)    42774 2024-05-31 13:56:59.341721 juju-3.5.0.0/PKG-INFO
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3238 2024-05-31 13:45:45.000000 juju-3.5.0.0/README.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.317721 juju-3.5.0.0/docs/
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.319721 juju-3.5.0.0/docs/api/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      190 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.action.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.annotation.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      210 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.application.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2352 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.client.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      210 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.constraints.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.controller.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.delta.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      190 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.errors.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.exceptions.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.juju.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.loop.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      194 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.machine.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.model.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      202 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.placement.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      198 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.relation.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      178 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.tag.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.unit.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      183 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.user.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/juju.utils.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      589 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/api/modules.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38571 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/changelog.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      666 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/index.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.319721 juju-3.5.0.0/docs/narrative/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3034 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/narrative/application.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2747 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/narrative/controller.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      100 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/narrative/index.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     8713 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/narrative/model.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1469 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/narrative/unit.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3238 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/readme.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.319721 juju-3.5.0.0/docs/upstream-updates/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6676 2024-05-31 13:45:45.000000 juju-3.5.0.0/docs/upstream-updates/index.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.325721 juju-3.5.0.0/examples/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1254 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/action.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1757 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/add_k8s.py
+-rwxrwxr-x   0 aflynn    (1000) aflynn    (1000)     1688 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/add_machine.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1784 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/add_model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2073 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/add_secrets_backend.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      914 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/allwatcher.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1033 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/charmhub_deploy_k8s.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      925 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/charmhub_deploy_machine.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      956 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/charmhub_find.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      796 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/charmhub_info.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      627 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/cloud.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      651 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/clouds.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1484 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/config.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      798 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/connect_current_model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1050 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/controller.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1541 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/credential.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2243 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/crossmodel.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2356 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/crossmodel_bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2561 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/crossmodel_controller.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2974 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/crossmodel_relation.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      936 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/debug-log.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      983 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1557 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      958 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_bundle_charmhub.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1170 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_bundle_with_trust.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1045 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_constraints.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      832 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_local_big_k8s_bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1155 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_local_bundle_with_resources.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1315 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_local_file_resource.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1298 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_local_resource.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      898 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/deploy_with_revision.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2552 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/expose-application.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1331 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/formatted_status.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      517 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/fullstatus.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1165 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/future.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      737 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/get_cloud.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      678 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/leadership.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      345 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/list_secrets.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      764 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/livemodel.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      776 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/local_refresh.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      824 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/localcharm.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1169 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/machine_hostname.py
+-rwxrwxr-x   0 aflynn    (1000) aflynn    (1000)      827 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1141 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/modelsummaries.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3334 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/relate.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      947 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/run_action.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1209 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/scp.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1290 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/status.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1714 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/unitrun.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1289 2024-05-31 13:45:45.000000 juju-3.5.0.0/examples/upgrade_local_charm_k8s.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.329721 juju-3.5.0.0/juju/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/__init__.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1341 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/access.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      737 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/action.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      214 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/annotation.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1167 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/annotationhelper.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38148 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/application.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    45784 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      208 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/charm.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     7284 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/charmhub.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.340721 juju-3.5.0.0/juju/client/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/__init__.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     8864 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   730276 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client1.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    41464 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client10.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   196254 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client11.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   245218 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client12.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   244188 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client13.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   115453 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client14.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   108914 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client15.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   103511 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client16.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   103511 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client17.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   369413 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client18.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   364812 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client19.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   406826 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client2.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   192763 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client3.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   201775 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client4.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    41639 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client5.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   162501 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client6.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   247072 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client7.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    45251 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client8.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    56944 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_client9.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)  1236275 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/_definitions.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1319 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/client.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1442 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/codegen.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    40536 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/connection.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     9267 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/connector.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    32274 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/facade.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      416 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/flags.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3755 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/gocookies.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     7148 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/jujudata.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    12560 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/overrides.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.340721 juju-3.5.0.0/juju/client/proxy/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      774 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/proxy/factory.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.340721 juju-3.5.0.0/juju/client/proxy/kubernetes/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2456 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/proxy/kubernetes/proxy.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      563 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/proxy/proxy.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      894 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/client/runner.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     4573 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/constraints.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38332 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/controller.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2732 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/delta.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3726 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/errors.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      142 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/exceptions.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3763 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/jasyncio.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1257 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/juju.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      231 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/loop.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11122 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/machine.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   125597 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2229 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/names.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6545 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/offerendpoints.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     5893 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/origin.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1924 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/placement.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11518 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/provisioner.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/py.typed
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     5049 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/relation.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      951 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/remoteapplication.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3877 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/secrets.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6616 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/status.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1408 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/tag.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    15858 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/unit.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     4863 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/url.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6486 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/user.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    18997 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/utils.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      230 2024-05-31 13:45:45.000000 juju-3.5.0.0/juju/version.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-05-31 13:56:59.340721 juju-3.5.0.0/juju.egg-info/
+-rw-r--r--   0 aflynn    (1000) aflynn    (1000)    42774 2024-05-31 13:56:59.000000 juju-3.5.0.0/juju.egg-info/PKG-INFO
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3691 2024-05-31 13:56:59.000000 juju-3.5.0.0/juju.egg-info/SOURCES.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        1 2024-05-31 13:56:59.000000 juju-3.5.0.0/juju.egg-info/dependency_links.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      178 2024-05-31 13:56:59.000000 juju-3.5.0.0/juju.egg-info/requires.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        5 2024-05-31 13:56:59.000000 juju-3.5.0.0/juju.egg-info/top_level.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)       38 2024-05-31 13:56:59.341721 juju-3.5.0.0/setup.cfg
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1747 2024-05-31 13:45:45.000000 juju-3.5.0.0/setup.py
```

### Comparing `juju-3.4.0.0/LICENSE` & `juju-3.5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/PKG-INFO` & `juju-3.5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.4.0.0
+Version: 3.5.0.0
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -159,14 +159,27 @@
 a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.5.0.0
+^^^^^^^
+
+Thursday 30th May 2024
+
+## What's Changed
+
+* Make consume respect the controller name in the url by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1038
+* Fix multiline description in textarea in bug template GH workflow by @cderici in https://github.com/juju/python-libjuju/pull/1041
+* Fix issue with microk8s proxy by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1044
+* add missing "revision" parameter to addModel step. by @Thanhphan1147 in https://github.com/juju/python-libjuju/pull/1043
+* Add user api to pylibjuju documentation by @cderici in https://github.com/juju/python-libjuju/pull/1049
+
 3.4.0.0
 ^^^^^^^
 
 Monday 25th Mar 2024
 
 ## What's Changed
```

### Comparing `juju-3.4.0.0/README.rst` & `juju-3.5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/api/juju.client.rst` & `juju-3.5.0.0/docs/api/juju.client.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/api/modules.rst` & `juju-3.5.0.0/docs/api/modules.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,14 @@
     juju.loop
     juju.machine
     juju.model
     juju.placement
     juju.relation
     juju.tag
     juju.unit
+    juju.user
     juju.utils
 
 .. automodule:: juju
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `juju-3.4.0.0/docs/changelog.rst` & `juju-3.5.0.0/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 ---------
 
+3.5.0.0
+^^^^^^^
+
+Thursday 30th May 2024
+
+## What's Changed
+
+* Make consume respect the controller name in the url by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1038
+* Fix multiline description in textarea in bug template GH workflow by @cderici in https://github.com/juju/python-libjuju/pull/1041
+* Fix issue with microk8s proxy by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1044
+* add missing "revision" parameter to addModel step. by @Thanhphan1147 in https://github.com/juju/python-libjuju/pull/1043
+* Add user api to pylibjuju documentation by @cderici in https://github.com/juju/python-libjuju/pull/1049
+
 3.4.0.0
 ^^^^^^^
 
 Monday 25th Mar 2024
 
 ## What's Changed
```

### Comparing `juju-3.4.0.0/docs/index.rst` & `juju-3.5.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/narrative/application.rst` & `juju-3.5.0.0/docs/narrative/application.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/narrative/controller.rst` & `juju-3.5.0.0/docs/narrative/controller.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/narrative/model.rst` & `juju-3.5.0.0/docs/narrative/model.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/narrative/unit.rst` & `juju-3.5.0.0/docs/narrative/unit.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/readme.rst` & `juju-3.5.0.0/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/docs/upstream-updates/index.rst` & `juju-3.5.0.0/docs/upstream-updates/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/action.py` & `juju-3.5.0.0/examples/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/add_k8s.py` & `juju-3.5.0.0/examples/add_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/add_machine.py` & `juju-3.5.0.0/examples/add_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/add_model.py` & `juju-3.5.0.0/examples/add_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/add_secrets_backend.py` & `juju-3.5.0.0/examples/add_secrets_backend.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/allwatcher.py` & `juju-3.5.0.0/examples/allwatcher.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/charmhub_deploy_k8s.py` & `juju-3.5.0.0/examples/charmhub_deploy_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/charmhub_deploy_machine.py` & `juju-3.5.0.0/examples/charmhub_deploy_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/charmhub_find.py` & `juju-3.5.0.0/examples/charmhub_find.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/charmhub_info.py` & `juju-3.5.0.0/examples/charmhub_info.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/cloud.py` & `juju-3.5.0.0/examples/cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/clouds.py` & `juju-3.5.0.0/examples/clouds.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/config.py` & `juju-3.5.0.0/examples/config.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/connect_current_model.py` & `juju-3.5.0.0/examples/connect_current_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/controller.py` & `juju-3.5.0.0/examples/controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/credential.py` & `juju-3.5.0.0/examples/credential.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/crossmodel.py` & `juju-3.5.0.0/examples/crossmodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/crossmodel_bundle.py` & `juju-3.5.0.0/examples/crossmodel_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/crossmodel_controller.py` & `juju-3.5.0.0/examples/crossmodel_controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/crossmodel_relation.py` & `juju-3.5.0.0/examples/crossmodel_relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/debug-log.py` & `juju-3.5.0.0/examples/debug-log.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy.py` & `juju-3.5.0.0/examples/deploy.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_bundle.py` & `juju-3.5.0.0/examples/deploy_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_bundle_charmhub.py` & `juju-3.5.0.0/examples/deploy_bundle_charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_bundle_with_trust.py` & `juju-3.5.0.0/examples/deploy_bundle_with_trust.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_constraints.py` & `juju-3.5.0.0/examples/deploy_constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_local_big_k8s_bundle.py` & `juju-3.5.0.0/examples/deploy_local_big_k8s_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_local_bundle_with_resources.py` & `juju-3.5.0.0/examples/deploy_local_bundle_with_resources.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_local_file_resource.py` & `juju-3.5.0.0/examples/deploy_local_file_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_local_resource.py` & `juju-3.5.0.0/examples/deploy_local_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/deploy_with_revision.py` & `juju-3.5.0.0/examples/deploy_with_revision.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/expose-application.py` & `juju-3.5.0.0/examples/expose-application.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/formatted_status.py` & `juju-3.5.0.0/examples/formatted_status.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/fullstatus.py` & `juju-3.5.0.0/examples/fullstatus.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/future.py` & `juju-3.5.0.0/examples/future.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/get_cloud.py` & `juju-3.5.0.0/examples/get_cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/leadership.py` & `juju-3.5.0.0/examples/leadership.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/livemodel.py` & `juju-3.5.0.0/examples/livemodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/local_refresh.py` & `juju-3.5.0.0/examples/local_refresh.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/localcharm.py` & `juju-3.5.0.0/examples/localcharm.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/machine_hostname.py` & `juju-3.5.0.0/examples/machine_hostname.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/model.py` & `juju-3.5.0.0/examples/model.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/modelsummaries.py` & `juju-3.5.0.0/examples/modelsummaries.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/relate.py` & `juju-3.5.0.0/examples/relate.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/run_action.py` & `juju-3.5.0.0/examples/run_action.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/scp.py` & `juju-3.5.0.0/examples/scp.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/status.py` & `juju-3.5.0.0/examples/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/unitrun.py` & `juju-3.5.0.0/examples/unitrun.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/examples/upgrade_local_charm_k8s.py` & `juju-3.5.0.0/examples/upgrade_local_charm_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/access.py` & `juju-3.5.0.0/juju/access.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/action.py` & `juju-3.5.0.0/juju/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/annotationhelper.py` & `juju-3.5.0.0/juju/annotationhelper.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/application.py` & `juju-3.5.0.0/juju/application.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/bundle.py` & `juju-3.5.0.0/juju/bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,14 +655,15 @@
                                                                                            charm=self.charm)
 
 
 class AddCharmChange(ChangeInfo):
     _toPy = {'charm': 'charm',
              'series': 'series',
              'channel': 'channel',
+             'revision': 'revision',
              'architecture': 'architecture'}
 
     """AddCharmChange holds a change for adding a charm to the environment.
 
     :change_id: id of the change that will be used to identify the current
         change
     :requires: is a slice of dependencies that are required to happen.
@@ -671,14 +672,15 @@
         return results.
 
     Params holds the following values:
         :charm: URL of the charm to be added.
         :series: series of the charm to be added if the charm default is
            not sufficient.
         :channel: preferred channel for obtaining the charm.
+        :revision: specified revision of the charm to be added if specified.
     """
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "addCharm"
 
@@ -706,14 +708,15 @@
             if not arch:
                 arch = await context.model._resolve_architecture(url)
             base = get_base_from_origin_or_channel(ch, self.series)
             origin = client.CharmOrigin(source=Source.CHARM_HUB.value,
                                         architecture=arch,
                                         risk=ch.risk,
                                         track=ch.track,
+                                        revision=self.revision,
                                         base=base)
             identifier, origin = await context.model._resolve_charm(url, origin)
 
         if identifier is None:
             raise JujuError('unknown charm {}'.format(self.charm))
 
         await context.model._add_charm(str(identifier), origin)
```

### Comparing `juju-3.4.0.0/juju/charmhub.py` & `juju-3.5.0.0/juju/charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client.py` & `juju-3.5.0.0/juju/client/_client.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client1.py` & `juju-3.5.0.0/juju/client/_client1.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client10.py` & `juju-3.5.0.0/juju/client/_client10.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client11.py` & `juju-3.5.0.0/juju/client/_client11.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client12.py` & `juju-3.5.0.0/juju/client/_client12.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client13.py` & `juju-3.5.0.0/juju/client/_client13.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client14.py` & `juju-3.5.0.0/juju/client/_client14.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client15.py` & `juju-3.5.0.0/juju/client/_client15.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client16.py` & `juju-3.5.0.0/juju/client/_client16.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client17.py` & `juju-3.5.0.0/juju/client/_client17.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client18.py` & `juju-3.5.0.0/juju/client/_client18.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client19.py` & `juju-3.5.0.0/juju/client/_client19.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client2.py` & `juju-3.5.0.0/juju/client/_client2.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client3.py` & `juju-3.5.0.0/juju/client/_client3.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client4.py` & `juju-3.5.0.0/juju/client/_client4.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client5.py` & `juju-3.5.0.0/juju/client/_client5.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client6.py` & `juju-3.5.0.0/juju/client/_client6.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client7.py` & `juju-3.5.0.0/juju/client/_client7.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client8.py` & `juju-3.5.0.0/juju/client/_client8.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_client9.py` & `juju-3.5.0.0/juju/client/_client9.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/_definitions.py` & `juju-3.5.0.0/juju/client/_definitions.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/client.py` & `juju-3.5.0.0/juju/client/client.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/codegen.py` & `juju-3.5.0.0/juju/client/codegen.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/connection.py` & `juju-3.5.0.0/juju/client/connection.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/connector.py` & `juju-3.5.0.0/juju/client/connector.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/facade.py` & `juju-3.5.0.0/juju/client/facade.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/gocookies.py` & `juju-3.5.0.0/juju/client/gocookies.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/jujudata.py` & `juju-3.5.0.0/juju/client/jujudata.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/overrides.py` & `juju-3.5.0.0/juju/client/overrides.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/proxy/factory.py` & `juju-3.5.0.0/juju/client/proxy/factory.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/proxy/kubernetes/proxy.py` & `juju-3.5.0.0/juju/client/proxy/kubernetes/proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright 2023 Canonical Ltd.
 # Licensed under the Apache V2, see LICENCE file for details.
-
+import os
 import tempfile
+import logging
 
 from juju.client.proxy.proxy import Proxy, ProxyNotConnectedError
 from kubernetes import client
 from kubernetes.stream import portforward
 
+log = logging.getLogger('juju.client.connection')
+
 
 class KubernetesProxy(Proxy):
     def __init__(
             self,
             api_host,
             namespace,
             remote_port,
@@ -29,15 +32,15 @@
 
         try:
             self.remote_port = int(remote_port)
         except ValueError:
             raise ValueError("Invalid port number: {}".format(remote_port))
 
         if ca_cert:
-            self.temp_ca_file = tempfile.NamedTemporaryFile()
+            self.temp_ca_file = tempfile.NamedTemporaryFile(delete=False)
             self.temp_ca_file.write(bytes(ca_cert, 'utf-8'))
             self.temp_ca_file.flush()
             config.ssl_ca_cert = self.temp_ca_file.name
 
         self.api_client = client.ApiClient(config)
 
     def connect(self):
@@ -56,14 +59,18 @@
             pods.items[0].metadata.name,
             self.namespace,
             ports=str(self.remote_port),
         )
 
     def __del__(self):
         self.close()
+        try:
+            os.unlink(self.temp_ca_file.name)
+        except FileNotFoundError:
+            log.debug(f"file {self.temp_ca_file.name} not found")
 
     def close(self):
         try:
             self.port_forwarder.close()
             self.temp_ca_file.close()
         except AttributeError:
             pass
```

### Comparing `juju-3.4.0.0/juju/client/proxy/proxy.py` & `juju-3.5.0.0/juju/client/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/client/runner.py` & `juju-3.5.0.0/juju/client/runner.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/constraints.py` & `juju-3.5.0.0/juju/constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/controller.py` & `juju-3.5.0.0/juju/controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/delta.py` & `juju-3.5.0.0/juju/delta.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/errors.py` & `juju-3.5.0.0/juju/errors.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/jasyncio.py` & `juju-3.5.0.0/juju/jasyncio.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/juju.py` & `juju-3.5.0.0/juju/juju.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/machine.py` & `juju-3.5.0.0/juju/machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/model.py` & `juju-3.5.0.0/juju/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1522,16 +1522,15 @@
                 raise JujuError("cannot add relation to {}: remote endpoints not supported".format(remote_endpoint.string()))
 
             if remote_endpoint.has_empty_source():
                 async with ConnectedController(self.connection()) as current:
                     remote_endpoint.source = current.controller_name
             # consume the remote endpoint
             await self.consume(remote_endpoint.string(),
-                               application_alias=remote_endpoint.application,
-                               controller_name=remote_endpoint.source)
+                               application_alias=remote_endpoint.application)
 
         log.debug(
             'Adding relation %s <-> %s', endpoints[0], endpoints[1])
 
         def _find_relation(*specs):
             for rel in self.relations:
                 if rel.matches(*specs):
@@ -2531,31 +2530,42 @@
         async with ConnectedController(self.connection()) as controller:
             return await controller.remove_offer(self.info.uuid, endpoint, force)
 
     async def consume(self, endpoint, application_alias="", controller_name=None, controller=None):
         """
         Adds a remote offer to the model. Relations can be created later using
         "juju relate".
+
+        If consuming a relation from a model on different controller the
+        controller name must be included in the endpoint. The controller_name
+        argument is being deprecated.
         """
+
         if controller and controller_name:
             raise JujuError("cannot set both controller_name and controller")
         try:
             offer = parse_offer_url(endpoint)
         except OfferParseError as e:
             log.error(e.message)
             raise
         if offer.has_endpoint():
             raise JujuError("remote offer {} should not include an endpoint".format(endpoint))
         if offer.user == "":
             offer.user = self.info.username
             endpoint = offer.string()
 
-        source = None
         if controller_name:
-            source = await self._get_source_api(offer, controller_name=controller_name)
+            log.warning(
+                'controller_name argument will soon be deprecated, controller '
+                'should be specified in endpoint url')
+            if offer.source == "":
+                offer.source = controller_name
+
+        if offer.source:
+            source = await self._get_source_api(offer)
         else:
             if controller:
                 source = controller
             else:
                 source = Controller()
                 kwargs = self.connection().connect_params()
                 kwargs["uuid"] = None
@@ -2762,20 +2772,23 @@
             label=secret_name)
         if len(results.results) != 1:
             raise JujuAPIError(f"expected 1 result, got {len(results.results)}")
         result_error = results.results[0]
         if result_error.error is not None:
             raise JujuAPIError(result_error.error)
 
-    async def _get_source_api(self, url, controller_name=None):
+    async def _get_source_api(self, url):
         controller = Controller()
         if url.has_empty_source():
             async with ConnectedController(self.connection()) as current:
                 if current.controller_name is not None:
                     controller_name = current.controller_name
+        else:
+            controller_name = url.source
+
         await controller.connect(controller_name=controller_name)
         return controller
 
     async def wait_for_idle(self, apps=None, raise_on_error=True, raise_on_blocked=False,
                             wait_for_active=False, timeout=10 * 60, idle_period=15, check_freq=0.5,
                             status=None, wait_for_at_least_units=None, wait_for_exact_units=None):
         """Wait for applications in the model to settle into an idle state.
```

### Comparing `juju-3.4.0.0/juju/names.py` & `juju-3.5.0.0/juju/names.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/offerendpoints.py` & `juju-3.5.0.0/juju/offerendpoints.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/origin.py` & `juju-3.5.0.0/juju/origin.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/placement.py` & `juju-3.5.0.0/juju/placement.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/provisioner.py` & `juju-3.5.0.0/juju/provisioner.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/relation.py` & `juju-3.5.0.0/juju/relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/remoteapplication.py` & `juju-3.5.0.0/juju/remoteapplication.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/secrets.py` & `juju-3.5.0.0/juju/secrets.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/status.py` & `juju-3.5.0.0/juju/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/tag.py` & `juju-3.5.0.0/juju/tag.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/unit.py` & `juju-3.5.0.0/juju/unit.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/url.py` & `juju-3.5.0.0/juju/url.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/user.py` & `juju-3.5.0.0/juju/user.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju/utils.py` & `juju-3.5.0.0/juju/utils.py`

 * *Files identical despite different names*

### Comparing `juju-3.4.0.0/juju.egg-info/PKG-INFO` & `juju-3.5.0.0/juju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.4.0.0
+Version: 3.5.0.0
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -159,14 +159,27 @@
 a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.5.0.0
+^^^^^^^
+
+Thursday 30th May 2024
+
+## What's Changed
+
+* Make consume respect the controller name in the url by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1038
+* Fix multiline description in textarea in bug template GH workflow by @cderici in https://github.com/juju/python-libjuju/pull/1041
+* Fix issue with microk8s proxy by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1044
+* add missing "revision" parameter to addModel step. by @Thanhphan1147 in https://github.com/juju/python-libjuju/pull/1043
+* Add user api to pylibjuju documentation by @cderici in https://github.com/juju/python-libjuju/pull/1049
+
 3.4.0.0
 ^^^^^^^
 
 Monday 25th Mar 2024
 
 ## What's Changed
```

### Comparing `juju-3.4.0.0/juju.egg-info/SOURCES.txt` & `juju-3.5.0.0/juju.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/api/juju.loop.rst
 docs/api/juju.machine.rst
 docs/api/juju.model.rst
 docs/api/juju.placement.rst
 docs/api/juju.relation.rst
 docs/api/juju.tag.rst
 docs/api/juju.unit.rst
+docs/api/juju.user.rst
 docs/api/juju.utils.rst
 docs/api/modules.rst
 docs/narrative/application.rst
 docs/narrative/controller.rst
 docs/narrative/index.rst
 docs/narrative/model.rst
 docs/narrative/unit.rst
```

### Comparing `juju-3.4.0.0/setup.py` & `juju-3.5.0.0/setup.py`

 * *Files identical despite different names*

