# Comparing `tmp/kthcloud-0.0.1a0.tar.gz` & `tmp/kthcloud-0.1.0a0.tar.gz`

## Comparing `kthcloud-0.0.1a0.tar` & `kthcloud-0.1.0a0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_base_client.py
--rw-r--r--   0        0        0    17636 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_constants.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_qs.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_resource.py
--rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_response.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_streaming.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_types.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/lib/.keep
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/__init__.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/snapshots.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py
--rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_group.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_params.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_response.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_created.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_deleted.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_response.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_updated.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/snapshot_list_params.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/snapshot_list_response.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_action_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_action_created.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_created.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_deleted.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_list_response.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_read.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_snapshot_created.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_updated.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/shared/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/shared/vm_snapshot_read.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vms/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vms/vm_snapshot_deleted.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/.gitignore
--rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 kthcloud-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_base_client.py
+-rw-r--r--   0        0        0    17634 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_constants.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_qs.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_resource.py
+-rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_response.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_streaming.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_types.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/lib/.keep
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_params.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_response.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_created.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_deleted.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_response.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_updated.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_params.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_response.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_action_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_action_created.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_created.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_deleted.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_list_response.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_snapshot_created.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_updated.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/shared/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/shared/vm_snapshot_read.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vms/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vms/vm_snapshot_deleted.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/.gitignore
+-rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 kthcloud-0.1.0a0/PKG-INFO
```

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/__init__.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_base_client.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_base_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_client.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,28 +78,28 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous kthcloud-go-deploy-v2 client instance.
 
-        This automatically infers the `api_key` argument from the `KTHCLOUD_GO_DEPLOY_V2_API_KEY` environment variable if it is not provided.
+        This automatically infers the `api_key` argument from the `KTHCLOUD_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
-            api_key = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_API_KEY")
+            api_key = os.environ.get("KTHCLOUD_API_KEY")
         if api_key is None:
             raise KthcloudGoDeployV2Error(
-                "The api_key client option must be set either by passing api_key to the client or by setting the KTHCLOUD_GO_DEPLOY_V2_API_KEY environment variable"
+                "The api_key client option must be set either by passing api_key to the client or by setting the KTHCLOUD_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_BASE_URL")
         if base_url is None:
-            base_url = f"/"
+            base_url = f"https://api.cloud.cbh.kth.se/deploy/v2/"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -254,28 +254,28 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async kthcloud-go-deploy-v2 client instance.
 
-        This automatically infers the `api_key` argument from the `KTHCLOUD_GO_DEPLOY_V2_API_KEY` environment variable if it is not provided.
+        This automatically infers the `api_key` argument from the `KTHCLOUD_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
-            api_key = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_API_KEY")
+            api_key = os.environ.get("KTHCLOUD_API_KEY")
         if api_key is None:
             raise KthcloudGoDeployV2Error(
-                "The api_key client option must be set either by passing api_key to the client or by setting the KTHCLOUD_GO_DEPLOY_V2_API_KEY environment variable"
+                "The api_key client option must be set either by passing api_key to the client or by setting the KTHCLOUD_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_BASE_URL")
         if base_url is None:
-            base_url = f"/"
+            base_url = f"https://api.cloud.cbh.kth.se/deploy/v2/"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
```

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_compat.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_compat.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_exceptions.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_exceptions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_files.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_files.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_models.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_models.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_qs.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_qs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_resource.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_resource.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_response.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_response.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_streaming.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_streaming.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_types.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_types.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/__init__.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_logs.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_sync.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_transform.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_typing.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/_utils/_utils.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/__init__.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/snapshots.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/__init__.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_group.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_read.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py` & `kthcloud-0.1.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/LICENSE` & `kthcloud-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthcloud-0.0.1a0/pyproject.toml` & `kthcloud-0.1.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "kthcloud"
-version = "0.0.1-alpha"
+version = "0.1.0-alpha"
 description = "The official Python library for the kthcloud-go-deploy-v2 API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
-{ name = "Kthcloud Go Deploy V2", email = "dev-feedback@kthcloud-go-deploy-v2.com" },
+{ name = "Kthcloud Go Deploy V2", email = "dev@cloud.cbh.kth.se" },
 ]
 dependencies = [
     "httpx>=0.23.0, <1",
     "pydantic>=1.9.0, <3",
     "typing-extensions>=4.7, <5",
     "anyio>=3.5.0, <5",
     "distro>=1.7.0, <2",
```

### Comparing `kthcloud-0.0.1a0/PKG-INFO` & `kthcloud-0.1.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: kthcloud
-Version: 0.0.1a0
+Version: 0.1.0a0
 Summary: The official Python library for the kthcloud-go-deploy-v2 API
 Project-URL: Homepage, https://github.com/kthcloud/python-sdk
 Project-URL: Repository, https://github.com/kthcloud/python-sdk
-Author-email: Kthcloud Go Deploy V2 <dev-feedback@kthcloud-go-deploy-v2.com>
+Author-email: Kthcloud Go Deploy V2 <dev@cloud.cbh.kth.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
@@ -70,15 +70,15 @@
     ssh_public_key="string",
 )
 print(vm_created.id)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
-to add `KTHCLOUD_GO_DEPLOY_V2_API_KEY="My API Key"` to your `.env` file
+to add `KTHCLOUD_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
 ## Async usage
 
 Simply import `AsyncKthcloudGoDeployV2` instead of `KthcloudGoDeployV2` and use `await` with each API call:
 
 ```python
```

