# Comparing `tmp/kthcloud-0.1.0a0.tar.gz` & `tmp/kthcloud-0.2.0a0.tar.gz`

## Comparing `kthcloud-0.1.0a0.tar` & `kthcloud-0.2.0a0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_base_client.py
--rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_constants.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_qs.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_resource.py
--rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_response.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_streaming.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_types.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/lib/.keep
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py
--rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_params.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_response.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_created.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_deleted.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_response.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_updated.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_params.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_response.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_action_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_action_created.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_created.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_deleted.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_list_response.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_snapshot_created.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_updated.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/shared/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/shared/vm_snapshot_read.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vms/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vms/vm_snapshot_deleted.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/.gitignore
--rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_base_client.py
+-rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_constants.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_qs.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_resource.py
+-rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_response.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_streaming.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_types.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/lib/.keep
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_params.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_response.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_created.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_deleted.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_response.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_updated.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_params.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_response.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_action_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_action_created.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_created.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_deleted.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_list_response.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_snapshot_created.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_updated.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/shared/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/shared/vm_snapshot_read.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vms/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vms/vm_snapshot_deleted.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/.gitignore
+-rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 kthcloud-0.2.0a0/PKG-INFO
```

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/__init__.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_base_client.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_base_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_client.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_compat.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_compat.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_exceptions.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_exceptions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_files.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_files.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_models.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_models.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_qs.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_qs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_resource.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_resource.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_response.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_response.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_streaming.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_streaming.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_types.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_types.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/__init__.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py` & `kthcloud-0.2.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/LICENSE` & `kthcloud-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthcloud-0.1.0a0/pyproject.toml` & `kthcloud-0.2.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kthcloud"
-version = "0.1.0-alpha"
+version = "0.2.0-alpha"
 description = "The official Python library for the kthcloud-go-deploy-v2 API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Kthcloud Go Deploy V2", email = "dev@cloud.cbh.kth.se" },
 ]
 dependencies = [
```

### Comparing `kthcloud-0.1.0a0/PKG-INFO` & `kthcloud-0.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kthcloud
-Version: 0.1.0a0
+Version: 0.2.0a0
 Summary: The official Python library for the kthcloud-go-deploy-v2 API
 Project-URL: Homepage, https://github.com/kthcloud/python-sdk
 Project-URL: Repository, https://github.com/kthcloud/python-sdk
 Author-email: Kthcloud Go Deploy V2 <dev@cloud.cbh.kth.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 Requires-Dist: distro<2,>=1.7.0
 Requires-Dist: httpx<1,>=0.23.0
 Requires-Dist: pydantic<3,>=1.9.0
 Requires-Dist: sniffio
 Requires-Dist: typing-extensions<5,>=4.7
 Description-Content-Type: text/markdown
 
-# Kthcloud Go Deploy V2 Python API library
+# kthcloud Python SDK
 
 [![PyPI version](https://img.shields.io/pypi/v/kthcloud.svg)](https://pypi.org/project/kthcloud/)
 
 The Kthcloud Go Deploy V2 Python library provides convenient access to the Kthcloud Go Deploy V2 REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
```

