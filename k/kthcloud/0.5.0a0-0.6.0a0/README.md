# Comparing `tmp/kthcloud-0.5.0a0.tar.gz` & `tmp/kthcloud-0.6.0a0.tar.gz`

## Comparing `kthcloud-0.5.0a0.tar` & `kthcloud-0.6.0a0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_base_client.py
--rw-r--r--   0        0        0    17326 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_constants.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_qs.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_resource.py
--rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_response.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_streaming.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/__init__.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/lib/.keep
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/__init__.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/gpu_groups.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/gpu_leases.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/snapshots.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vm_actions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vms/__init__.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vms/snapshot.py
--rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vms/vms.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_group.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_group_list_params.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_group_list_response.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_created.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_deleted.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_list_params.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_list_response.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_read.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_update_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_updated.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/snapshot_list_params.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/snapshot_list_response.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_action_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_action_created.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_create_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_created.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_deleted.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_list_params.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_list_response.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_read.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_snapshot_created.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_update_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_updated.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/shared/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/shared/vm_snapshot_read.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vms/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vms/vm_snapshot_deleted.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud_go_deploy_v2/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud_go_deploy_v_/lib/.keep
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/LICENSE
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/pyproject.toml
--rw-r--r--   0        0        0    12219 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/PKG-INFO
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_base_client.py
+-rw-r--r--   0        0        0    17326 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_constants.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_qs.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_resource.py
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_response.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/lib/.keep
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/__init__.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/gpu_groups.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/gpu_leases.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/snapshots.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/vm_actions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/vms/__init__.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/vms/snapshot.py
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/resources/vms/vms.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_group.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_group_list_params.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_group_list_response.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_created.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_deleted.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_list_params.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_list_response.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_read.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_update_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_updated.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/snapshot_list_params.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/snapshot_list_response.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_action_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_action_created.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_create_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_created.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_deleted.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_list_params.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_list_response.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_read.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_snapshot_created.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_update_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vm_updated.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/shared/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/shared/vm_snapshot_read.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vms/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud/types/vms/vm_snapshot_deleted.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud_go_deploy_v2/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/src/kthcloud_go_deploy_v_/lib/.keep
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/LICENSE
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12219 2020-02-02 00:00:00.000000 kthcloud-0.6.0a0/PKG-INFO
```

### Comparing `kthcloud-0.5.0a0/src/kthcloud/__init__.py` & `kthcloud-0.6.0a0/src/kthcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_base_client.py` & `kthcloud-0.6.0a0/src/kthcloud/_base_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_client.py` & `kthcloud-0.6.0a0/src/kthcloud/_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_compat.py` & `kthcloud-0.6.0a0/src/kthcloud/_compat.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_exceptions.py` & `kthcloud-0.6.0a0/src/kthcloud/_exceptions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_files.py` & `kthcloud-0.6.0a0/src/kthcloud/_files.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_models.py` & `kthcloud-0.6.0a0/src/kthcloud/_models.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_qs.py` & `kthcloud-0.6.0a0/src/kthcloud/_qs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_resource.py` & `kthcloud-0.6.0a0/src/kthcloud/_resource.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_response.py` & `kthcloud-0.6.0a0/src/kthcloud/_response.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_streaming.py` & `kthcloud-0.6.0a0/src/kthcloud/_streaming.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_types.py` & `kthcloud-0.6.0a0/src/kthcloud/_types.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/__init__.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/_logs.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/_proxy.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/_sync.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/_transform.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/_typing.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/_utils/_utils.py` & `kthcloud-0.6.0a0/src/kthcloud/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     overload,
 )
 from pathlib import Path
 from typing_extensions import TypeGuard
 
 import sniffio
 
-from .._types import Headers, NotGiven, FileTypes, NotGivenOr, HeadersLike
+from .._types import NotGiven, FileTypes, NotGivenOr, HeadersLike
 from .._compat import parse_date as parse_date, parse_datetime as parse_datetime
 
 _T = TypeVar("_T")
 _TupleT = TypeVar("_TupleT", bound=Tuple[object, ...])
 _MappingT = TypeVar("_MappingT", bound=Mapping[str, object])
 _SequenceT = TypeVar("_SequenceT", bound=Sequence[object])
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
@@ -366,15 +366,14 @@
     file_name = os.path.basename(path)
     return (file_name, contents)
 
 
 def get_required_header(headers: HeadersLike, header: str) -> str:
     lower_header = header.lower()
     if isinstance(headers, Mapping):
-        headers = cast(Headers, headers)
         for k, v in headers.items():
             if k.lower() == lower_header and isinstance(v, str):
                 return v
 
     """ to deal with the case where the header looks like Stainless-Event-Id """
     intercaps_header = re.sub(r"([^\w])(\w)", lambda pat: pat.group(1) + pat.group(2).upper(), header.capitalize())
```

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/__init__.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/gpu_groups.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/gpu_groups.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/gpu_leases.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/gpu_leases.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/snapshots.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/snapshots.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/vm_actions.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/vm_actions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/vms/__init__.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/vms/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/vms/snapshot.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/vms/snapshot.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/resources/vms/vms.py` & `kthcloud-0.6.0a0/src/kthcloud/resources/vms/vms.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/__init__.py` & `kthcloud-0.6.0a0/src/kthcloud/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/gpu_group.py` & `kthcloud-0.6.0a0/src/kthcloud/types/gpu_group.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_create_params.py` & `kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_list_params.py` & `kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_read.py` & `kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_update_params.py` & `kthcloud-0.6.0a0/src/kthcloud/types/gpu_lease_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/vm_create_params.py` & `kthcloud-0.6.0a0/src/kthcloud/types/vm_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/vm_list_params.py` & `kthcloud-0.6.0a0/src/kthcloud/types/vm_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/vm_read.py` & `kthcloud-0.6.0a0/src/kthcloud/types/vm_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/src/kthcloud/types/vm_update_params.py` & `kthcloud-0.6.0a0/src/kthcloud/types/vm_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/LICENSE` & `kthcloud-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthcloud-0.5.0a0/pyproject.toml` & `kthcloud-0.6.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kthcloud"
-version = "0.5.0-alpha"
+version = "0.6.0-alpha"
 description = "The official Python library for the kthcloud API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Kthcloud", email = "dev@cloud.cbh.kth.se" },
 ]
 dependencies = [
```

### Comparing `kthcloud-0.5.0a0/PKG-INFO` & `kthcloud-0.6.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kthcloud
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: The official Python library for the kthcloud API
 Project-URL: Homepage, https://github.com/kthcloud/python-sdk
 Project-URL: Repository, https://github.com/kthcloud/python-sdk
 Author-email: Kthcloud <dev@cloud.cbh.kth.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

