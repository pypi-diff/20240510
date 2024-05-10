# Comparing `tmp/pulumi_vsphere-4.9.1.tar.gz` & `tmp/pulumi_vsphere-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vsphere-4.9.1.tar", last modified: Wed Dec 13 02:47:41 2023, max compression
+gzip compressed data, was "pulumi_vsphere-4.9.2.tar", last modified: Fri Feb  9 17:47:54 2024, max compression
```

## Comparing `pulumi_vsphere-4.9.1.tar` & `pulumi_vsphere-4.9.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 02:47:41.333972 pulumi_vsphere-4.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2023-12-13 02:47:41.333972 pulumi_vsphere-4.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 02:47:41.333972 pulumi_vsphere-4.9.1/pulumi_vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   113081 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   245818 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13437 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_host_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24459 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    17554 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_dependency_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24422 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_host_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 02:47:41.333972 pulumi_vsphere-4.9.1/pulumi_vsphere/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15087 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/content_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    15640 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/content_library_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    90156 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/datastore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    16842 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)   134499 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/distributed_port_group.py
--rw-r--r--   0 runner    (1001) docker     (127)   263381 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/distributed_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15371 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/dpm_host_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    16657 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/drs_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/entity_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23387 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    25630 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_compute_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_compute_cluster_host_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_content_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_content_library_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_datastore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_distributed_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_guest_os_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_host_pci_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_host_thumbprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    32673 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_ovf_vm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_tag_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_vapp_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    56393 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/get_vmfs_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/guest_os_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    58963 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/ha_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    45915 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/host.py
--rw-r--r--   0 runner    (1001) docker     (127)    56784 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/host_port_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    61643 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/host_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/license.py
--rw-r--r--   0 runner    (1001) docker     (127)    48202 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/nas_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)   119399 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20511 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54091 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    20828 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/storage_drs_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    15120 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/tag_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    48255 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/vapp_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    29555 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/vapp_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    28723 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/virtual_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)   268912 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    23926 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/virtual_machine_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    20958 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/vm_storage_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    34596 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/vmfs_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    30381 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pulumi_vsphere/vnic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 02:47:41.333972 pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2023-12-13 02:47:41.000000 pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-12-13 02:47:41.000000 pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 02:47:41.000000 pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-13 02:47:41.000000 pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 02:47:41.000000 pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-13 02:47:30.000000 pulumi_vsphere-4.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 02:47:41.333972 pulumi_vsphere-4.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:47:54.444101 pulumi_vsphere-4.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-09 17:47:54.444101 pulumi_vsphere-4.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:47:54.440101 pulumi_vsphere-4.9.2/pulumi_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136728 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   245818 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24459 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_dependency_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24422 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_host_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:47:54.444101 pulumi_vsphere-4.9.2/pulumi_vsphere/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/content_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/content_library_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90156 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/datastore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)   134499 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/distributed_port_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)   263381 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/distributed_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15371 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/dpm_host_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/drs_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/entity_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23387 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25630 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_compute_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_compute_cluster_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_content_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_content_library_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_datastore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_distributed_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_guest_os_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_host_pci_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_host_thumbprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32673 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_ovf_vm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_tag_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_vapp_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/get_vmfs_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/guest_os_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58963 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/ha_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45915 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56784 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/host_port_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61643 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/host_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48202 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/nas_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148166 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20511 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54091 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20828 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/storage_drs_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/tag_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48255 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/vapp_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29555 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/vapp_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28723 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/virtual_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)   268912 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23926 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/virtual_machine_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20958 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/vm_storage_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34596 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/vmfs_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30381 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pulumi_vsphere/vnic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:47:54.444101 pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-09 17:47:54.000000 pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-02-09 17:47:54.000000 pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 17:47:54.000000 pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-09 17:47:54.000000 pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-09 17:47:54.000000 pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-09 17:47:42.000000 pulumi_vsphere-4.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 17:47:54.444101 pulumi_vsphere-4.9.2/setup.cfg
```

### Comparing `pulumi_vsphere-4.9.1/PKG-INFO` & `pulumi_vsphere-4.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi_vsphere
-Version: 4.9.1
+Version: 4.9.2
 Summary: A Pulumi package for creating vsphere resources
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vsphere
 Keywords: pulumi,vsphere
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0
 Requires-Dist: semver>=2.8.1
 
 [![Actions Status](https://github.com/pulumi/pulumi-vsphere/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-vsphere/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_vsphere-4.9.1/README.md` & `pulumi_vsphere-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/__init__.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/_inputs.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/_inputs.py`

 * *Files 26% similar despite different names*

```diff
@@ -509,29 +509,39 @@
 
 
 @pulumi.input_type
 class DistributedPortGroupVlanRangeArgs:
     def __init__(__self__, *,
                  max_vlan: pulumi.Input[int],
                  min_vlan: pulumi.Input[int]):
+        """
+        :param pulumi.Input[int] max_vlan: The minimum VLAN to use in the range.
+        :param pulumi.Input[int] min_vlan: The minimum VLAN to use in the range.
+        """
         pulumi.set(__self__, "max_vlan", max_vlan)
         pulumi.set(__self__, "min_vlan", min_vlan)
 
     @property
     @pulumi.getter(name="maxVlan")
     def max_vlan(self) -> pulumi.Input[int]:
+        """
+        The minimum VLAN to use in the range.
+        """
         return pulumi.get(self, "max_vlan")
 
     @max_vlan.setter
     def max_vlan(self, value: pulumi.Input[int]):
         pulumi.set(self, "max_vlan", value)
 
     @property
     @pulumi.getter(name="minVlan")
     def min_vlan(self) -> pulumi.Input[int]:
+        """
+        The minimum VLAN to use in the range.
+        """
         return pulumi.get(self, "min_vlan")
 
     @min_vlan.setter
     def min_vlan(self, value: pulumi.Input[int]):
         pulumi.set(self, "min_vlan", value)
 
 
@@ -636,29 +646,39 @@
 
 
 @pulumi.input_type
 class DistributedVirtualSwitchVlanRangeArgs:
     def __init__(__self__, *,
                  max_vlan: pulumi.Input[int],
                  min_vlan: pulumi.Input[int]):
+        """
+        :param pulumi.Input[int] max_vlan: The minimum VLAN to use in the range.
+        :param pulumi.Input[int] min_vlan: The minimum VLAN to use in the range.
+        """
         pulumi.set(__self__, "max_vlan", max_vlan)
         pulumi.set(__self__, "min_vlan", min_vlan)
 
     @property
     @pulumi.getter(name="maxVlan")
     def max_vlan(self) -> pulumi.Input[int]:
+        """
+        The minimum VLAN to use in the range.
+        """
         return pulumi.get(self, "max_vlan")
 
     @max_vlan.setter
     def max_vlan(self, value: pulumi.Input[int]):
         pulumi.set(self, "max_vlan", value)
 
     @property
     @pulumi.getter(name="minVlan")
     def min_vlan(self) -> pulumi.Input[int]:
+        """
+        The minimum VLAN to use in the range.
+        """
         return pulumi.get(self, "min_vlan")
 
     @min_vlan.setter
     def min_vlan(self, value: pulumi.Input[int]):
         pulumi.set(self, "min_vlan", value)
 
 
@@ -736,14 +756,24 @@
                  dns_suffix_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv4_gateway: Optional[pulumi.Input[str]] = None,
                  ipv6_gateway: Optional[pulumi.Input[str]] = None,
                  linux_options: Optional[pulumi.Input['GuestOsCustomizationSpecLinuxOptionsArgs']] = None,
                  network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input['GuestOsCustomizationSpecNetworkInterfaceArgs']]]] = None,
                  windows_options: Optional[pulumi.Input['GuestOsCustomizationSpecWindowsOptionsArgs']] = None,
                  windows_sysprep_text: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_server_lists: The list of DNS servers for a virtual network adapter with a static IP address.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_suffix_lists: A list of DNS search domains to add to the DNS configuration on the virtual machine.
+        :param pulumi.Input[str] ipv4_gateway: The IPv4 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        :param pulumi.Input[str] ipv6_gateway: The IPv6 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        :param pulumi.Input['GuestOsCustomizationSpecLinuxOptionsArgs'] linux_options: A list of configuration options specific to Linux virtual machines.
+        :param pulumi.Input[Sequence[pulumi.Input['GuestOsCustomizationSpecNetworkInterfaceArgs']]] network_interfaces: A specification of network interface configuration options.
+        :param pulumi.Input['GuestOsCustomizationSpecWindowsOptionsArgs'] windows_options: A list of configuration options specific to Windows virtual machines.
+        :param pulumi.Input[str] windows_sysprep_text: Use this option to specify a windows sysprep file directly.
+        """
         if dns_server_lists is not None:
             pulumi.set(__self__, "dns_server_lists", dns_server_lists)
         if dns_suffix_lists is not None:
             pulumi.set(__self__, "dns_suffix_lists", dns_suffix_lists)
         if ipv4_gateway is not None:
             pulumi.set(__self__, "ipv4_gateway", ipv4_gateway)
         if ipv6_gateway is not None:
@@ -756,77 +786,101 @@
             pulumi.set(__self__, "windows_options", windows_options)
         if windows_sysprep_text is not None:
             pulumi.set(__self__, "windows_sysprep_text", windows_sysprep_text)
 
     @property
     @pulumi.getter(name="dnsServerLists")
     def dns_server_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The list of DNS servers for a virtual network adapter with a static IP address.
+        """
         return pulumi.get(self, "dns_server_lists")
 
     @dns_server_lists.setter
     def dns_server_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_server_lists", value)
 
     @property
     @pulumi.getter(name="dnsSuffixLists")
     def dns_suffix_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of DNS search domains to add to the DNS configuration on the virtual machine.
+        """
         return pulumi.get(self, "dns_suffix_lists")
 
     @dns_suffix_lists.setter
     def dns_suffix_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_suffix_lists", value)
 
     @property
     @pulumi.getter(name="ipv4Gateway")
     def ipv4_gateway(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv4 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        """
         return pulumi.get(self, "ipv4_gateway")
 
     @ipv4_gateway.setter
     def ipv4_gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv4_gateway", value)
 
     @property
     @pulumi.getter(name="ipv6Gateway")
     def ipv6_gateway(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv6 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        """
         return pulumi.get(self, "ipv6_gateway")
 
     @ipv6_gateway.setter
     def ipv6_gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv6_gateway", value)
 
     @property
     @pulumi.getter(name="linuxOptions")
     def linux_options(self) -> Optional[pulumi.Input['GuestOsCustomizationSpecLinuxOptionsArgs']]:
+        """
+        A list of configuration options specific to Linux virtual machines.
+        """
         return pulumi.get(self, "linux_options")
 
     @linux_options.setter
     def linux_options(self, value: Optional[pulumi.Input['GuestOsCustomizationSpecLinuxOptionsArgs']]):
         pulumi.set(self, "linux_options", value)
 
     @property
     @pulumi.getter(name="networkInterfaces")
     def network_interfaces(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GuestOsCustomizationSpecNetworkInterfaceArgs']]]]:
+        """
+        A specification of network interface configuration options.
+        """
         return pulumi.get(self, "network_interfaces")
 
     @network_interfaces.setter
     def network_interfaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GuestOsCustomizationSpecNetworkInterfaceArgs']]]]):
         pulumi.set(self, "network_interfaces", value)
 
     @property
     @pulumi.getter(name="windowsOptions")
     def windows_options(self) -> Optional[pulumi.Input['GuestOsCustomizationSpecWindowsOptionsArgs']]:
+        """
+        A list of configuration options specific to Windows virtual machines.
+        """
         return pulumi.get(self, "windows_options")
 
     @windows_options.setter
     def windows_options(self, value: Optional[pulumi.Input['GuestOsCustomizationSpecWindowsOptionsArgs']]):
         pulumi.set(self, "windows_options", value)
 
     @property
     @pulumi.getter(name="windowsSysprepText")
     def windows_sysprep_text(self) -> Optional[pulumi.Input[str]]:
+        """
+        Use this option to specify a windows sysprep file directly.
+        """
         return pulumi.get(self, "windows_sysprep_text")
 
     @windows_sysprep_text.setter
     def windows_sysprep_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "windows_sysprep_text", value)
 
 
@@ -834,62 +888,84 @@
 class GuestOsCustomizationSpecLinuxOptionsArgs:
     def __init__(__self__, *,
                  domain: pulumi.Input[str],
                  host_name: pulumi.Input[str],
                  hw_clock_utc: Optional[pulumi.Input[bool]] = None,
                  script_text: Optional[pulumi.Input[str]] = None,
                  time_zone: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] domain: The domain name for this virtual machine.
+        :param pulumi.Input[str] host_name: The hostname for this virtual machine.
+        :param pulumi.Input[bool] hw_clock_utc: Specifies whether or not the hardware clock should be in UTC or not.
+        :param pulumi.Input[str] script_text: The customization script to run before and or after guest customization
+        :param pulumi.Input[str] time_zone: Customize the time zone on the VM. This should be a time zone-style entry, like America/Los_Angeles.
+        """
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "host_name", host_name)
         if hw_clock_utc is not None:
             pulumi.set(__self__, "hw_clock_utc", hw_clock_utc)
         if script_text is not None:
             pulumi.set(__self__, "script_text", script_text)
         if time_zone is not None:
             pulumi.set(__self__, "time_zone", time_zone)
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Input[str]:
+        """
+        The domain name for this virtual machine.
+        """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: pulumi.Input[str]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter(name="hostName")
     def host_name(self) -> pulumi.Input[str]:
+        """
+        The hostname for this virtual machine.
+        """
         return pulumi.get(self, "host_name")
 
     @host_name.setter
     def host_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "host_name", value)
 
     @property
     @pulumi.getter(name="hwClockUtc")
     def hw_clock_utc(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Specifies whether or not the hardware clock should be in UTC or not.
+        """
         return pulumi.get(self, "hw_clock_utc")
 
     @hw_clock_utc.setter
     def hw_clock_utc(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "hw_clock_utc", value)
 
     @property
     @pulumi.getter(name="scriptText")
     def script_text(self) -> Optional[pulumi.Input[str]]:
+        """
+        The customization script to run before and or after guest customization
+        """
         return pulumi.get(self, "script_text")
 
     @script_text.setter
     def script_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "script_text", value)
 
     @property
     @pulumi.getter(name="timeZone")
     def time_zone(self) -> Optional[pulumi.Input[str]]:
+        """
+        Customize the time zone on the VM. This should be a time zone-style entry, like America/Los_Angeles.
+        """
         return pulumi.get(self, "time_zone")
 
     @time_zone.setter
     def time_zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "time_zone", value)
 
 
@@ -898,14 +974,22 @@
     def __init__(__self__, *,
                  dns_domain: Optional[pulumi.Input[str]] = None,
                  dns_server_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv4_address: Optional[pulumi.Input[str]] = None,
                  ipv4_netmask: Optional[pulumi.Input[int]] = None,
                  ipv6_address: Optional[pulumi.Input[str]] = None,
                  ipv6_netmask: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[str] dns_domain: A DNS search domain to add to the DNS configuration on the virtual machine.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_server_lists: Network-interface specific DNS settings for Windows operating systems. Ignored on Linux.
+        :param pulumi.Input[str] ipv4_address: The IPv4 address assigned to this network adapter. If left blank, DHCP is used.
+        :param pulumi.Input[int] ipv4_netmask: The IPv4 CIDR netmask for the supplied IP address. Ignored if DHCP is selected.
+        :param pulumi.Input[str] ipv6_address: The IPv6 address assigned to this network adapter. If left blank, default auto-configuration is used.
+        :param pulumi.Input[int] ipv6_netmask: The IPv6 CIDR netmask for the supplied IP address. Ignored if auto-configuration is selected.
+        """
         if dns_domain is not None:
             pulumi.set(__self__, "dns_domain", dns_domain)
         if dns_server_lists is not None:
             pulumi.set(__self__, "dns_server_lists", dns_server_lists)
         if ipv4_address is not None:
             pulumi.set(__self__, "ipv4_address", ipv4_address)
         if ipv4_netmask is not None:
@@ -914,59 +998,77 @@
             pulumi.set(__self__, "ipv6_address", ipv6_address)
         if ipv6_netmask is not None:
             pulumi.set(__self__, "ipv6_netmask", ipv6_netmask)
 
     @property
     @pulumi.getter(name="dnsDomain")
     def dns_domain(self) -> Optional[pulumi.Input[str]]:
+        """
+        A DNS search domain to add to the DNS configuration on the virtual machine.
+        """
         return pulumi.get(self, "dns_domain")
 
     @dns_domain.setter
     def dns_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_domain", value)
 
     @property
     @pulumi.getter(name="dnsServerLists")
     def dns_server_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Network-interface specific DNS settings for Windows operating systems. Ignored on Linux.
+        """
         return pulumi.get(self, "dns_server_lists")
 
     @dns_server_lists.setter
     def dns_server_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_server_lists", value)
 
     @property
     @pulumi.getter(name="ipv4Address")
     def ipv4_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv4 address assigned to this network adapter. If left blank, DHCP is used.
+        """
         return pulumi.get(self, "ipv4_address")
 
     @ipv4_address.setter
     def ipv4_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv4_address", value)
 
     @property
     @pulumi.getter(name="ipv4Netmask")
     def ipv4_netmask(self) -> Optional[pulumi.Input[int]]:
+        """
+        The IPv4 CIDR netmask for the supplied IP address. Ignored if DHCP is selected.
+        """
         return pulumi.get(self, "ipv4_netmask")
 
     @ipv4_netmask.setter
     def ipv4_netmask(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ipv4_netmask", value)
 
     @property
     @pulumi.getter(name="ipv6Address")
     def ipv6_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv6 address assigned to this network adapter. If left blank, default auto-configuration is used.
+        """
         return pulumi.get(self, "ipv6_address")
 
     @ipv6_address.setter
     def ipv6_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv6_address", value)
 
     @property
     @pulumi.getter(name="ipv6Netmask")
     def ipv6_netmask(self) -> Optional[pulumi.Input[int]]:
+        """
+        The IPv6 CIDR netmask for the supplied IP address. Ignored if auto-configuration is selected.
+        """
         return pulumi.get(self, "ipv6_netmask")
 
     @ipv6_netmask.setter
     def ipv6_netmask(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ipv6_netmask", value)
 
 
@@ -982,14 +1084,29 @@
                  full_name: Optional[pulumi.Input[str]] = None,
                  join_domain: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  product_key: Optional[pulumi.Input[str]] = None,
                  run_once_command_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  time_zone: Optional[pulumi.Input[int]] = None,
                  workgroup: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] computer_name: The host name for this virtual machine.
+        :param pulumi.Input[str] admin_password: The new administrator password for this virtual machine.
+        :param pulumi.Input[bool] auto_logon: Specifies whether or not the VM automatically logs on as Administrator.
+        :param pulumi.Input[int] auto_logon_count: Specifies how many times the VM should auto-logon the Administrator account when auto_logon is true.
+        :param pulumi.Input[str] domain_admin_password: The password of the domain administrator used to join this virtual machine to the domain.
+        :param pulumi.Input[str] domain_admin_user: The user account of the domain administrator used to join this virtual machine to the domain.
+        :param pulumi.Input[str] full_name: The full name of the user of this virtual machine.
+        :param pulumi.Input[str] join_domain: The domain that the virtual machine should join.
+        :param pulumi.Input[str] organization_name: The organization name this virtual machine is being installed for.
+        :param pulumi.Input[str] product_key: The product key for this virtual machine.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] run_once_command_lists: A list of commands to run at first user logon, after guest customization.
+        :param pulumi.Input[int] time_zone: The new time zone for the virtual machine. This is a sysprep-dictated timezone code.
+        :param pulumi.Input[str] workgroup: The workgroup for this virtual machine if not joining a domain.
+        """
         pulumi.set(__self__, "computer_name", computer_name)
         if admin_password is not None:
             pulumi.set(__self__, "admin_password", admin_password)
         if auto_logon is not None:
             pulumi.set(__self__, "auto_logon", auto_logon)
         if auto_logon_count is not None:
             pulumi.set(__self__, "auto_logon_count", auto_logon_count)
@@ -1011,122 +1128,161 @@
             pulumi.set(__self__, "time_zone", time_zone)
         if workgroup is not None:
             pulumi.set(__self__, "workgroup", workgroup)
 
     @property
     @pulumi.getter(name="computerName")
     def computer_name(self) -> pulumi.Input[str]:
+        """
+        The host name for this virtual machine.
+        """
         return pulumi.get(self, "computer_name")
 
     @computer_name.setter
     def computer_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "computer_name", value)
 
     @property
     @pulumi.getter(name="adminPassword")
     def admin_password(self) -> Optional[pulumi.Input[str]]:
+        """
+        The new administrator password for this virtual machine.
+        """
         return pulumi.get(self, "admin_password")
 
     @admin_password.setter
     def admin_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "admin_password", value)
 
     @property
     @pulumi.getter(name="autoLogon")
     def auto_logon(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Specifies whether or not the VM automatically logs on as Administrator.
+        """
         return pulumi.get(self, "auto_logon")
 
     @auto_logon.setter
     def auto_logon(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_logon", value)
 
     @property
     @pulumi.getter(name="autoLogonCount")
     def auto_logon_count(self) -> Optional[pulumi.Input[int]]:
+        """
+        Specifies how many times the VM should auto-logon the Administrator account when auto_logon is true.
+        """
         return pulumi.get(self, "auto_logon_count")
 
     @auto_logon_count.setter
     def auto_logon_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "auto_logon_count", value)
 
     @property
     @pulumi.getter(name="domainAdminPassword")
     def domain_admin_password(self) -> Optional[pulumi.Input[str]]:
+        """
+        The password of the domain administrator used to join this virtual machine to the domain.
+        """
         return pulumi.get(self, "domain_admin_password")
 
     @domain_admin_password.setter
     def domain_admin_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_admin_password", value)
 
     @property
     @pulumi.getter(name="domainAdminUser")
     def domain_admin_user(self) -> Optional[pulumi.Input[str]]:
+        """
+        The user account of the domain administrator used to join this virtual machine to the domain.
+        """
         return pulumi.get(self, "domain_admin_user")
 
     @domain_admin_user.setter
     def domain_admin_user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_admin_user", value)
 
     @property
     @pulumi.getter(name="fullName")
     def full_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The full name of the user of this virtual machine.
+        """
         return pulumi.get(self, "full_name")
 
     @full_name.setter
     def full_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "full_name", value)
 
     @property
     @pulumi.getter(name="joinDomain")
     def join_domain(self) -> Optional[pulumi.Input[str]]:
+        """
+        The domain that the virtual machine should join.
+        """
         return pulumi.get(self, "join_domain")
 
     @join_domain.setter
     def join_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "join_domain", value)
 
     @property
     @pulumi.getter(name="organizationName")
     def organization_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The organization name this virtual machine is being installed for.
+        """
         return pulumi.get(self, "organization_name")
 
     @organization_name.setter
     def organization_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "organization_name", value)
 
     @property
     @pulumi.getter(name="productKey")
     def product_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        The product key for this virtual machine.
+        """
         return pulumi.get(self, "product_key")
 
     @product_key.setter
     def product_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product_key", value)
 
     @property
     @pulumi.getter(name="runOnceCommandLists")
     def run_once_command_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of commands to run at first user logon, after guest customization.
+        """
         return pulumi.get(self, "run_once_command_lists")
 
     @run_once_command_lists.setter
     def run_once_command_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "run_once_command_lists", value)
 
     @property
     @pulumi.getter(name="timeZone")
     def time_zone(self) -> Optional[pulumi.Input[int]]:
+        """
+        The new time zone for the virtual machine. This is a sysprep-dictated timezone code.
+        """
         return pulumi.get(self, "time_zone")
 
     @time_zone.setter
     def time_zone(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "time_zone", value)
 
     @property
     @pulumi.getter
     def workgroup(self) -> Optional[pulumi.Input[str]]:
+        """
+        The workgroup for this virtual machine if not joining a domain.
+        """
         return pulumi.get(self, "workgroup")
 
     @workgroup.setter
     def workgroup(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workgroup", value)
 
 
@@ -1134,14 +1290,16 @@
 class HostPortGroupPortArgs:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
                  mac_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] key: The key for this port group as returned from the vSphere API.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] mac_addresses: The MAC addresses of the network service of the virtual machine connected on this port.
+        :param pulumi.Input[str] type: Type type of the entity connected on this port. Possible values are host (VMKkernel), systemManagement (service console), virtualMachine, or unknown.
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
         if mac_addresses is not None:
             pulumi.set(__self__, "mac_addresses", mac_addresses)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -1157,23 +1315,29 @@
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter(name="macAddresses")
     def mac_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The MAC addresses of the network service of the virtual machine connected on this port.
+        """
         return pulumi.get(self, "mac_addresses")
 
     @mac_addresses.setter
     def mac_addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "mac_addresses", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Type type of the entity connected on this port. Possible values are host (VMKkernel), systemManagement (service console), virtualMachine, or unknown.
+        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
@@ -1184,14 +1348,15 @@
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  device_address: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[int]] = None,
                  path: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] client_device: Indicates whether the device should be backed by remote client device. Conflicts with `datastore_id` and `path`.
         :param pulumi.Input[str] datastore_id: The datastore ID that on which the ISO is located. Required for using a datastore ISO. Conflicts with `client_device`.
+        :param pulumi.Input[str] device_address: The internally-computed address of this device, such as scsi:0:1, denoting scsi bus #0 and device unit 1.
         :param pulumi.Input[int] key: The ID of the device within the virtual machine.
         :param pulumi.Input[str] path: The path to the ISO file. Required for using a datastore ISO. Conflicts with `client_device`.
                
                > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
                
                > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
@@ -1229,14 +1394,17 @@
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
     @property
     @pulumi.getter(name="deviceAddress")
     def device_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The internally-computed address of this device, such as scsi:0:1, denoting scsi bus #0 and device unit 1.
+        """
         return pulumi.get(self, "device_address")
 
     @device_address.setter
     def device_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "device_address", value)
 
     @property
@@ -1274,14 +1442,23 @@
                  template_uuid: pulumi.Input[str],
                  customization_spec: Optional[pulumi.Input['VirtualMachineCloneCustomizationSpecArgs']] = None,
                  customize: Optional[pulumi.Input['VirtualMachineCloneCustomizeArgs']] = None,
                  linked_clone: Optional[pulumi.Input[bool]] = None,
                  ovf_network_map: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  ovf_storage_map: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  timeout: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[str] template_uuid: The UUID of the source virtual machine or template.
+        :param pulumi.Input['VirtualMachineCloneCustomizationSpecArgs'] customization_spec: The customization specification for the virtual machine post-clone.
+        :param pulumi.Input['VirtualMachineCloneCustomizeArgs'] customize: The customization specification for the virtual machine post-clone.
+        :param pulumi.Input[bool] linked_clone: Whether or not to create a linked clone when cloning. When this option is used, the source VM must have a single snapshot associated with it.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] ovf_network_map: Mapping of ovf networks to the networks to use in vSphere.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] ovf_storage_map: Mapping of ovf storage to the datastores to use in vSphere.
+        :param pulumi.Input[int] timeout: The timeout, in minutes, to wait for the virtual machine clone to complete.
+        """
         pulumi.set(__self__, "template_uuid", template_uuid)
         if customization_spec is not None:
             pulumi.set(__self__, "customization_spec", customization_spec)
         if customize is not None:
             pulumi.set(__self__, "customize", customize)
         if linked_clone is not None:
             pulumi.set(__self__, "linked_clone", linked_clone)
@@ -1291,82 +1468,104 @@
             pulumi.set(__self__, "ovf_storage_map", ovf_storage_map)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter(name="templateUuid")
     def template_uuid(self) -> pulumi.Input[str]:
+        """
+        The UUID of the source virtual machine or template.
+        """
         return pulumi.get(self, "template_uuid")
 
     @template_uuid.setter
     def template_uuid(self, value: pulumi.Input[str]):
         pulumi.set(self, "template_uuid", value)
 
     @property
     @pulumi.getter(name="customizationSpec")
     def customization_spec(self) -> Optional[pulumi.Input['VirtualMachineCloneCustomizationSpecArgs']]:
+        """
+        The customization specification for the virtual machine post-clone.
+        """
         return pulumi.get(self, "customization_spec")
 
     @customization_spec.setter
     def customization_spec(self, value: Optional[pulumi.Input['VirtualMachineCloneCustomizationSpecArgs']]):
         pulumi.set(self, "customization_spec", value)
 
     @property
     @pulumi.getter
     def customize(self) -> Optional[pulumi.Input['VirtualMachineCloneCustomizeArgs']]:
+        """
+        The customization specification for the virtual machine post-clone.
+        """
         return pulumi.get(self, "customize")
 
     @customize.setter
     def customize(self, value: Optional[pulumi.Input['VirtualMachineCloneCustomizeArgs']]):
         pulumi.set(self, "customize", value)
 
     @property
     @pulumi.getter(name="linkedClone")
     def linked_clone(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether or not to create a linked clone when cloning. When this option is used, the source VM must have a single snapshot associated with it.
+        """
         return pulumi.get(self, "linked_clone")
 
     @linked_clone.setter
     def linked_clone(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "linked_clone", value)
 
     @property
     @pulumi.getter(name="ovfNetworkMap")
     def ovf_network_map(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Mapping of ovf networks to the networks to use in vSphere.
+        """
         return pulumi.get(self, "ovf_network_map")
 
     @ovf_network_map.setter
     def ovf_network_map(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "ovf_network_map", value)
 
     @property
     @pulumi.getter(name="ovfStorageMap")
     def ovf_storage_map(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Mapping of ovf storage to the datastores to use in vSphere.
+        """
         return pulumi.get(self, "ovf_storage_map")
 
     @ovf_storage_map.setter
     def ovf_storage_map(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "ovf_storage_map", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
+        """
+        The timeout, in minutes, to wait for the virtual machine clone to complete.
+        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
 
 @pulumi.input_type
 class VirtualMachineCloneCustomizationSpecArgs:
     def __init__(__self__, *,
                  id: pulumi.Input[str],
                  timeout: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] id: The UUID of the virtual machine.
+        :param pulumi.Input[int] timeout: The amount of time, in minutes, to wait for guest OS customization to complete before returning with an error. Setting this value to 0 or a negative value skips the waiter. Default: 10.
         """
         pulumi.set(__self__, "id", id)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
@@ -1379,14 +1578,17 @@
     @id.setter
     def id(self, value: pulumi.Input[str]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
+        """
+        The amount of time, in minutes, to wait for guest OS customization to complete before returning with an error. Setting this value to 0 or a negative value skips the waiter. Default: 10.
+        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
 
@@ -1399,15 +1601,23 @@
                  ipv6_gateway: Optional[pulumi.Input[str]] = None,
                  linux_options: Optional[pulumi.Input['VirtualMachineCloneCustomizeLinuxOptionsArgs']] = None,
                  network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineCloneCustomizeNetworkInterfaceArgs']]]] = None,
                  timeout: Optional[pulumi.Input[int]] = None,
                  windows_options: Optional[pulumi.Input['VirtualMachineCloneCustomizeWindowsOptionsArgs']] = None,
                  windows_sysprep_text: Optional[pulumi.Input[str]] = None):
         """
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_server_lists: The list of DNS servers for a virtual network adapter with a static IP address.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_suffix_lists: A list of DNS search domains to add to the DNS configuration on the virtual machine.
+        :param pulumi.Input[str] ipv4_gateway: The IPv4 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        :param pulumi.Input[str] ipv6_gateway: The IPv6 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        :param pulumi.Input['VirtualMachineCloneCustomizeLinuxOptionsArgs'] linux_options: A list of configuration options specific to Linux virtual machines.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineCloneCustomizeNetworkInterfaceArgs']]] network_interfaces: A specification for a virtual NIC on the virtual machine. See network interface options for more information.
+        :param pulumi.Input[int] timeout: The amount of time, in minutes, to wait for guest OS customization to complete before returning with an error. Setting this value to 0 or a negative value skips the waiter. Default: 10.
+        :param pulumi.Input['VirtualMachineCloneCustomizeWindowsOptionsArgs'] windows_options: A list of configuration options specific to Windows virtual machines.
+        :param pulumi.Input[str] windows_sysprep_text: Use this option to specify a windows sysprep file directly.
         """
         if dns_server_lists is not None:
             pulumi.set(__self__, "dns_server_lists", dns_server_lists)
         if dns_suffix_lists is not None:
             pulumi.set(__self__, "dns_suffix_lists", dns_suffix_lists)
         if ipv4_gateway is not None:
             pulumi.set(__self__, "ipv4_gateway", ipv4_gateway)
@@ -1423,50 +1633,65 @@
             pulumi.set(__self__, "windows_options", windows_options)
         if windows_sysprep_text is not None:
             pulumi.set(__self__, "windows_sysprep_text", windows_sysprep_text)
 
     @property
     @pulumi.getter(name="dnsServerLists")
     def dns_server_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The list of DNS servers for a virtual network adapter with a static IP address.
+        """
         return pulumi.get(self, "dns_server_lists")
 
     @dns_server_lists.setter
     def dns_server_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_server_lists", value)
 
     @property
     @pulumi.getter(name="dnsSuffixLists")
     def dns_suffix_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of DNS search domains to add to the DNS configuration on the virtual machine.
+        """
         return pulumi.get(self, "dns_suffix_lists")
 
     @dns_suffix_lists.setter
     def dns_suffix_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_suffix_lists", value)
 
     @property
     @pulumi.getter(name="ipv4Gateway")
     def ipv4_gateway(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv4 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        """
         return pulumi.get(self, "ipv4_gateway")
 
     @ipv4_gateway.setter
     def ipv4_gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv4_gateway", value)
 
     @property
     @pulumi.getter(name="ipv6Gateway")
     def ipv6_gateway(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv6 default gateway when using network_interface customization on the virtual machine. This address must be local to a static IPv4 address configured in an interface sub-resource.
+        """
         return pulumi.get(self, "ipv6_gateway")
 
     @ipv6_gateway.setter
     def ipv6_gateway(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv6_gateway", value)
 
     @property
     @pulumi.getter(name="linuxOptions")
     def linux_options(self) -> Optional[pulumi.Input['VirtualMachineCloneCustomizeLinuxOptionsArgs']]:
+        """
+        A list of configuration options specific to Linux virtual machines.
+        """
         return pulumi.get(self, "linux_options")
 
     @linux_options.setter
     def linux_options(self, value: Optional[pulumi.Input['VirtualMachineCloneCustomizeLinuxOptionsArgs']]):
         pulumi.set(self, "linux_options", value)
 
     @property
@@ -1480,32 +1705,41 @@
     @network_interfaces.setter
     def network_interfaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineCloneCustomizeNetworkInterfaceArgs']]]]):
         pulumi.set(self, "network_interfaces", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
+        """
+        The amount of time, in minutes, to wait for guest OS customization to complete before returning with an error. Setting this value to 0 or a negative value skips the waiter. Default: 10.
+        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
     @property
     @pulumi.getter(name="windowsOptions")
     def windows_options(self) -> Optional[pulumi.Input['VirtualMachineCloneCustomizeWindowsOptionsArgs']]:
+        """
+        A list of configuration options specific to Windows virtual machines.
+        """
         return pulumi.get(self, "windows_options")
 
     @windows_options.setter
     def windows_options(self, value: Optional[pulumi.Input['VirtualMachineCloneCustomizeWindowsOptionsArgs']]):
         pulumi.set(self, "windows_options", value)
 
     @property
     @pulumi.getter(name="windowsSysprepText")
     def windows_sysprep_text(self) -> Optional[pulumi.Input[str]]:
+        """
+        Use this option to specify a windows sysprep file directly.
+        """
         return pulumi.get(self, "windows_sysprep_text")
 
     @windows_sysprep_text.setter
     def windows_sysprep_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "windows_sysprep_text", value)
 
 
@@ -1513,62 +1747,84 @@
 class VirtualMachineCloneCustomizeLinuxOptionsArgs:
     def __init__(__self__, *,
                  domain: pulumi.Input[str],
                  host_name: pulumi.Input[str],
                  hw_clock_utc: Optional[pulumi.Input[bool]] = None,
                  script_text: Optional[pulumi.Input[str]] = None,
                  time_zone: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] domain: The domain name for this virtual machine.
+        :param pulumi.Input[str] host_name: The hostname for this virtual machine.
+        :param pulumi.Input[bool] hw_clock_utc: Specifies whether or not the hardware clock should be in UTC or not.
+        :param pulumi.Input[str] script_text: The customization script to run before and or after guest customization
+        :param pulumi.Input[str] time_zone: Customize the time zone on the VM. This should be a time zone-style entry, like America/Los_Angeles.
+        """
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "host_name", host_name)
         if hw_clock_utc is not None:
             pulumi.set(__self__, "hw_clock_utc", hw_clock_utc)
         if script_text is not None:
             pulumi.set(__self__, "script_text", script_text)
         if time_zone is not None:
             pulumi.set(__self__, "time_zone", time_zone)
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Input[str]:
+        """
+        The domain name for this virtual machine.
+        """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: pulumi.Input[str]):
         pulumi.set(self, "domain", value)
 
     @property
     @pulumi.getter(name="hostName")
     def host_name(self) -> pulumi.Input[str]:
+        """
+        The hostname for this virtual machine.
+        """
         return pulumi.get(self, "host_name")
 
     @host_name.setter
     def host_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "host_name", value)
 
     @property
     @pulumi.getter(name="hwClockUtc")
     def hw_clock_utc(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Specifies whether or not the hardware clock should be in UTC or not.
+        """
         return pulumi.get(self, "hw_clock_utc")
 
     @hw_clock_utc.setter
     def hw_clock_utc(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "hw_clock_utc", value)
 
     @property
     @pulumi.getter(name="scriptText")
     def script_text(self) -> Optional[pulumi.Input[str]]:
+        """
+        The customization script to run before and or after guest customization
+        """
         return pulumi.get(self, "script_text")
 
     @script_text.setter
     def script_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "script_text", value)
 
     @property
     @pulumi.getter(name="timeZone")
     def time_zone(self) -> Optional[pulumi.Input[str]]:
+        """
+        Customize the time zone on the VM. This should be a time zone-style entry, like America/Los_Angeles.
+        """
         return pulumi.get(self, "time_zone")
 
     @time_zone.setter
     def time_zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "time_zone", value)
 
 
@@ -1577,14 +1833,22 @@
     def __init__(__self__, *,
                  dns_domain: Optional[pulumi.Input[str]] = None,
                  dns_server_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv4_address: Optional[pulumi.Input[str]] = None,
                  ipv4_netmask: Optional[pulumi.Input[int]] = None,
                  ipv6_address: Optional[pulumi.Input[str]] = None,
                  ipv6_netmask: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[str] dns_domain: A DNS search domain to add to the DNS configuration on the virtual machine.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_server_lists: Network-interface specific DNS settings for Windows operating systems. Ignored on Linux.
+        :param pulumi.Input[str] ipv4_address: The IPv4 address assigned to this network adapter. If left blank, DHCP is used.
+        :param pulumi.Input[int] ipv4_netmask: The IPv4 CIDR netmask for the supplied IP address. Ignored if DHCP is selected.
+        :param pulumi.Input[str] ipv6_address: The IPv6 address assigned to this network adapter. If left blank, default auto-configuration is used.
+        :param pulumi.Input[int] ipv6_netmask: The IPv6 CIDR netmask for the supplied IP address. Ignored if auto-configuration is selected.
+        """
         if dns_domain is not None:
             pulumi.set(__self__, "dns_domain", dns_domain)
         if dns_server_lists is not None:
             pulumi.set(__self__, "dns_server_lists", dns_server_lists)
         if ipv4_address is not None:
             pulumi.set(__self__, "ipv4_address", ipv4_address)
         if ipv4_netmask is not None:
@@ -1593,59 +1857,77 @@
             pulumi.set(__self__, "ipv6_address", ipv6_address)
         if ipv6_netmask is not None:
             pulumi.set(__self__, "ipv6_netmask", ipv6_netmask)
 
     @property
     @pulumi.getter(name="dnsDomain")
     def dns_domain(self) -> Optional[pulumi.Input[str]]:
+        """
+        A DNS search domain to add to the DNS configuration on the virtual machine.
+        """
         return pulumi.get(self, "dns_domain")
 
     @dns_domain.setter
     def dns_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_domain", value)
 
     @property
     @pulumi.getter(name="dnsServerLists")
     def dns_server_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Network-interface specific DNS settings for Windows operating systems. Ignored on Linux.
+        """
         return pulumi.get(self, "dns_server_lists")
 
     @dns_server_lists.setter
     def dns_server_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_server_lists", value)
 
     @property
     @pulumi.getter(name="ipv4Address")
     def ipv4_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv4 address assigned to this network adapter. If left blank, DHCP is used.
+        """
         return pulumi.get(self, "ipv4_address")
 
     @ipv4_address.setter
     def ipv4_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv4_address", value)
 
     @property
     @pulumi.getter(name="ipv4Netmask")
     def ipv4_netmask(self) -> Optional[pulumi.Input[int]]:
+        """
+        The IPv4 CIDR netmask for the supplied IP address. Ignored if DHCP is selected.
+        """
         return pulumi.get(self, "ipv4_netmask")
 
     @ipv4_netmask.setter
     def ipv4_netmask(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ipv4_netmask", value)
 
     @property
     @pulumi.getter(name="ipv6Address")
     def ipv6_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IPv6 address assigned to this network adapter. If left blank, default auto-configuration is used.
+        """
         return pulumi.get(self, "ipv6_address")
 
     @ipv6_address.setter
     def ipv6_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ipv6_address", value)
 
     @property
     @pulumi.getter(name="ipv6Netmask")
     def ipv6_netmask(self) -> Optional[pulumi.Input[int]]:
+        """
+        The IPv6 CIDR netmask for the supplied IP address. Ignored if auto-configuration is selected.
+        """
         return pulumi.get(self, "ipv6_netmask")
 
     @ipv6_netmask.setter
     def ipv6_netmask(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ipv6_netmask", value)
 
 
@@ -1661,14 +1943,29 @@
                  full_name: Optional[pulumi.Input[str]] = None,
                  join_domain: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  product_key: Optional[pulumi.Input[str]] = None,
                  run_once_command_lists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  time_zone: Optional[pulumi.Input[int]] = None,
                  workgroup: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] computer_name: The host name for this virtual machine.
+        :param pulumi.Input[str] admin_password: The new administrator password for this virtual machine.
+        :param pulumi.Input[bool] auto_logon: Specifies whether or not the VM automatically logs on as Administrator.
+        :param pulumi.Input[int] auto_logon_count: Specifies how many times the VM should auto-logon the Administrator account when auto_logon is true.
+        :param pulumi.Input[str] domain_admin_password: The password of the domain administrator used to join this virtual machine to the domain.
+        :param pulumi.Input[str] domain_admin_user: The user account of the domain administrator used to join this virtual machine to the domain.
+        :param pulumi.Input[str] full_name: The full name of the user of this virtual machine.
+        :param pulumi.Input[str] join_domain: The domain that the virtual machine should join.
+        :param pulumi.Input[str] organization_name: The organization name this virtual machine is being installed for.
+        :param pulumi.Input[str] product_key: The product key for this virtual machine.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] run_once_command_lists: A list of commands to run at first user logon, after guest customization.
+        :param pulumi.Input[int] time_zone: The new time zone for the virtual machine. This is a sysprep-dictated timezone code.
+        :param pulumi.Input[str] workgroup: The workgroup for this virtual machine if not joining a domain.
+        """
         pulumi.set(__self__, "computer_name", computer_name)
         if admin_password is not None:
             pulumi.set(__self__, "admin_password", admin_password)
         if auto_logon is not None:
             pulumi.set(__self__, "auto_logon", auto_logon)
         if auto_logon_count is not None:
             pulumi.set(__self__, "auto_logon_count", auto_logon_count)
@@ -1690,122 +1987,161 @@
             pulumi.set(__self__, "time_zone", time_zone)
         if workgroup is not None:
             pulumi.set(__self__, "workgroup", workgroup)
 
     @property
     @pulumi.getter(name="computerName")
     def computer_name(self) -> pulumi.Input[str]:
+        """
+        The host name for this virtual machine.
+        """
         return pulumi.get(self, "computer_name")
 
     @computer_name.setter
     def computer_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "computer_name", value)
 
     @property
     @pulumi.getter(name="adminPassword")
     def admin_password(self) -> Optional[pulumi.Input[str]]:
+        """
+        The new administrator password for this virtual machine.
+        """
         return pulumi.get(self, "admin_password")
 
     @admin_password.setter
     def admin_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "admin_password", value)
 
     @property
     @pulumi.getter(name="autoLogon")
     def auto_logon(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Specifies whether or not the VM automatically logs on as Administrator.
+        """
         return pulumi.get(self, "auto_logon")
 
     @auto_logon.setter
     def auto_logon(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_logon", value)
 
     @property
     @pulumi.getter(name="autoLogonCount")
     def auto_logon_count(self) -> Optional[pulumi.Input[int]]:
+        """
+        Specifies how many times the VM should auto-logon the Administrator account when auto_logon is true.
+        """
         return pulumi.get(self, "auto_logon_count")
 
     @auto_logon_count.setter
     def auto_logon_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "auto_logon_count", value)
 
     @property
     @pulumi.getter(name="domainAdminPassword")
     def domain_admin_password(self) -> Optional[pulumi.Input[str]]:
+        """
+        The password of the domain administrator used to join this virtual machine to the domain.
+        """
         return pulumi.get(self, "domain_admin_password")
 
     @domain_admin_password.setter
     def domain_admin_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_admin_password", value)
 
     @property
     @pulumi.getter(name="domainAdminUser")
     def domain_admin_user(self) -> Optional[pulumi.Input[str]]:
+        """
+        The user account of the domain administrator used to join this virtual machine to the domain.
+        """
         return pulumi.get(self, "domain_admin_user")
 
     @domain_admin_user.setter
     def domain_admin_user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_admin_user", value)
 
     @property
     @pulumi.getter(name="fullName")
     def full_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The full name of the user of this virtual machine.
+        """
         return pulumi.get(self, "full_name")
 
     @full_name.setter
     def full_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "full_name", value)
 
     @property
     @pulumi.getter(name="joinDomain")
     def join_domain(self) -> Optional[pulumi.Input[str]]:
+        """
+        The domain that the virtual machine should join.
+        """
         return pulumi.get(self, "join_domain")
 
     @join_domain.setter
     def join_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "join_domain", value)
 
     @property
     @pulumi.getter(name="organizationName")
     def organization_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The organization name this virtual machine is being installed for.
+        """
         return pulumi.get(self, "organization_name")
 
     @organization_name.setter
     def organization_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "organization_name", value)
 
     @property
     @pulumi.getter(name="productKey")
     def product_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        The product key for this virtual machine.
+        """
         return pulumi.get(self, "product_key")
 
     @product_key.setter
     def product_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product_key", value)
 
     @property
     @pulumi.getter(name="runOnceCommandLists")
     def run_once_command_lists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        A list of commands to run at first user logon, after guest customization.
+        """
         return pulumi.get(self, "run_once_command_lists")
 
     @run_once_command_lists.setter
     def run_once_command_lists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "run_once_command_lists", value)
 
     @property
     @pulumi.getter(name="timeZone")
     def time_zone(self) -> Optional[pulumi.Input[int]]:
+        """
+        The new time zone for the virtual machine. This is a sysprep-dictated timezone code.
+        """
         return pulumi.get(self, "time_zone")
 
     @time_zone.setter
     def time_zone(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "time_zone", value)
 
     @property
     @pulumi.getter
     def workgroup(self) -> Optional[pulumi.Input[str]]:
+        """
+        The workgroup for this virtual machine if not joining a domain.
+        """
         return pulumi.get(self, "workgroup")
 
     @workgroup.setter
     def workgroup(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workgroup", value)
 
 
@@ -1830,19 +2166,21 @@
                  size: Optional[pulumi.Input[int]] = None,
                  storage_policy_id: Optional[pulumi.Input[str]] = None,
                  thin_provisioned: Optional[pulumi.Input[bool]] = None,
                  unit_number: Optional[pulumi.Input[int]] = None,
                  uuid: Optional[pulumi.Input[str]] = None,
                  write_through: Optional[pulumi.Input[bool]] = None):
         """
+        :param pulumi.Input[str] label: A unique label for this disk.
         :param pulumi.Input[bool] attach: Attach an external disk instead of creating a new one. Implies and conflicts with `keep_on_remove`. If set, you cannot set `size`, `eagerly_scrub`, or `thin_provisioned`. Must set `path` if used.
                
                > **NOTE:** External disks cannot be attached when `datastore_cluster_id` is used.
         :param pulumi.Input[str] controller_type: The type of storage controller to attach the  disk to. Can be `scsi`, `sata`, or `ide`. You must have the appropriate number of controllers enabled for the selected type. Default `scsi`.
         :param pulumi.Input[str] datastore_id: The datastore ID that on which the ISO is located. Required for using a datastore ISO. Conflicts with `client_device`.
+        :param pulumi.Input[str] device_address: The internally-computed address of this device, such as scsi:0:1, denoting scsi bus #0 and device unit 1.
         :param pulumi.Input[str] disk_mode: The mode of this this virtual disk for purposes of writes and snapshots. One of `append`, `independent_nonpersistent`, `independent_persistent`, `nonpersistent`, `persistent`, or `undoable`. Default: `persistent`. For more information on these option, please refer to the [product documentation][vmware-docs-disk-mode].
                
                [vmware-docs-disk-mode]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/da47f910-60ac-438b-8b9b-6122f4d14524/16b7274a-bf8b-4b4c-a05e-746f2aa93c8c/doc/vim.vm.device.VirtualDiskOption.DiskMode.html
         :param pulumi.Input[str] disk_sharing: The sharing mode of this virtual disk. One of `sharingMultiWriter` or `sharingNone`. Default: `sharingNone`.
                
                > **NOTE:** Disk sharing is only available on vSphere 6.0 and later.
         :param pulumi.Input[bool] eagerly_scrub: If set to `true`, the disk space is zeroed out when the virtual machine is created. This will delay the creation of the virtual disk. Cannot be set to `true` when `thin_provisioned` is `true`.  See the section on picking a disk type for more information.  Default: `false`.
@@ -1905,14 +2243,17 @@
             pulumi.set(__self__, "uuid", uuid)
         if write_through is not None:
             pulumi.set(__self__, "write_through", write_through)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
+        """
+        A unique label for this disk.
+        """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
     @property
@@ -1952,14 +2293,17 @@
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
     @property
     @pulumi.getter(name="deviceAddress")
     def device_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The internally-computed address of this device, such as scsi:0:1, denoting scsi bus #0 and device unit 1.
+        """
         return pulumi.get(self, "device_address")
 
     @device_address.setter
     def device_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "device_address", value)
 
     @property
@@ -2181,17 +2525,19 @@
         """
         :param pulumi.Input[str] network_id: The [managed object reference ID][docs-about-morefs] of the network on which to connect the virtual machine network interface.
         :param pulumi.Input[str] adapter_type: The network interface type. One of `e1000`, `e1000e`, `sriov`, or `vmxnet3`. Default: `vmxnet3`.
         :param pulumi.Input[int] bandwidth_limit: The upper bandwidth limit of the network interface, in Mbits/sec. The default is no limit. Ignored if `adapter_type` is set to `sriov`.
         :param pulumi.Input[int] bandwidth_reservation: The bandwidth reservation of the network interface, in Mbits/sec. The default is no reservation.
         :param pulumi.Input[int] bandwidth_share_count: The share count for the network interface when the share level is `custom`. Ignored if `adapter_type` is set to `sriov`.
         :param pulumi.Input[str] bandwidth_share_level: The bandwidth share allocation level for the network interface. One of `low`, `normal`, `high`, or `custom`. Default: `normal`. Ignored if `adapter_type` is set to `sriov`.
+        :param pulumi.Input[str] device_address: The internally-computed address of this device, such as scsi:0:1, denoting scsi bus #0 and device unit 1.
         :param pulumi.Input[int] key: The ID of the device within the virtual machine.
         :param pulumi.Input[str] mac_address: The MAC address of the network interface. Can only be manually set if `use_static_mac` is `true`. Otherwise, the value is computed and presents the assigned MAC address for the interface.
         :param pulumi.Input[str] ovf_mapping: Specifies which NIC in an OVF/OVA the `network_interface` should be associated. Only applies at creation when deploying from an OVF/OVA.
+        :param pulumi.Input[str] physical_function: The ID of the Physical SR-IOV NIC to attach to, e.g. '0000:d8:00.0'
         :param pulumi.Input[bool] use_static_mac: If true, the `mac_address` field is treated as a static MAC address and set accordingly. Setting this to `true` requires `mac_address` to be set. Default: `false`.
         """
         pulumi.set(__self__, "network_id", network_id)
         if adapter_type is not None:
             pulumi.set(__self__, "adapter_type", adapter_type)
         if bandwidth_limit is not None:
             pulumi.set(__self__, "bandwidth_limit", bandwidth_limit)
@@ -2285,14 +2631,17 @@
     @bandwidth_share_level.setter
     def bandwidth_share_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bandwidth_share_level", value)
 
     @property
     @pulumi.getter(name="deviceAddress")
     def device_address(self) -> Optional[pulumi.Input[str]]:
+        """
+        The internally-computed address of this device, such as scsi:0:1, denoting scsi bus #0 and device unit 1.
+        """
         return pulumi.get(self, "device_address")
 
     @device_address.setter
     def device_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "device_address", value)
 
     @property
@@ -2330,14 +2679,17 @@
     @ovf_mapping.setter
     def ovf_mapping(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ovf_mapping", value)
 
     @property
     @pulumi.getter(name="physicalFunction")
     def physical_function(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the Physical SR-IOV NIC to attach to, e.g. '0000:d8:00.0'
+        """
         return pulumi.get(self, "physical_function")
 
     @physical_function.setter
     def physical_function(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "physical_function", value)
 
     @property
@@ -2361,14 +2713,25 @@
                  disk_provisioning: Optional[pulumi.Input[str]] = None,
                  enable_hidden_properties: Optional[pulumi.Input[bool]] = None,
                  ip_allocation_policy: Optional[pulumi.Input[str]] = None,
                  ip_protocol: Optional[pulumi.Input[str]] = None,
                  local_ovf_path: Optional[pulumi.Input[str]] = None,
                  ovf_network_map: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  remote_ovf_url: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[bool] allow_unverified_ssl_cert: Allow unverified ssl certificates while deploying ovf/ova from url.
+        :param pulumi.Input[str] deployment_option: The Deployment option to be chosen. If empty, the default option is used.
+        :param pulumi.Input[str] disk_provisioning: An optional disk provisioning. If set, all the disks in the deployed ovf will have the same specified disk type (e.g., thin provisioned).
+        :param pulumi.Input[bool] enable_hidden_properties: Allow properties with ovf:userConfigurable=false to be set.
+        :param pulumi.Input[str] ip_allocation_policy: The IP allocation policy.
+        :param pulumi.Input[str] ip_protocol: The IP protocol.
+        :param pulumi.Input[str] local_ovf_path: The absolute path to the ovf/ova file in the local system.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] ovf_network_map: The mapping of name of network identifiers from the ovf descriptor to network UUID in the VI infrastructure.
+        :param pulumi.Input[str] remote_ovf_url: URL to the remote ovf/ova file to be deployed.
+        """
         if allow_unverified_ssl_cert is not None:
             pulumi.set(__self__, "allow_unverified_ssl_cert", allow_unverified_ssl_cert)
         if deployment_option is not None:
             pulumi.set(__self__, "deployment_option", deployment_option)
         if disk_provisioning is not None:
             pulumi.set(__self__, "disk_provisioning", disk_provisioning)
         if enable_hidden_properties is not None:
@@ -2383,103 +2746,136 @@
             pulumi.set(__self__, "ovf_network_map", ovf_network_map)
         if remote_ovf_url is not None:
             pulumi.set(__self__, "remote_ovf_url", remote_ovf_url)
 
     @property
     @pulumi.getter(name="allowUnverifiedSslCert")
     def allow_unverified_ssl_cert(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allow unverified ssl certificates while deploying ovf/ova from url.
+        """
         return pulumi.get(self, "allow_unverified_ssl_cert")
 
     @allow_unverified_ssl_cert.setter
     def allow_unverified_ssl_cert(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_unverified_ssl_cert", value)
 
     @property
     @pulumi.getter(name="deploymentOption")
     def deployment_option(self) -> Optional[pulumi.Input[str]]:
+        """
+        The Deployment option to be chosen. If empty, the default option is used.
+        """
         return pulumi.get(self, "deployment_option")
 
     @deployment_option.setter
     def deployment_option(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "deployment_option", value)
 
     @property
     @pulumi.getter(name="diskProvisioning")
     def disk_provisioning(self) -> Optional[pulumi.Input[str]]:
+        """
+        An optional disk provisioning. If set, all the disks in the deployed ovf will have the same specified disk type (e.g., thin provisioned).
+        """
         return pulumi.get(self, "disk_provisioning")
 
     @disk_provisioning.setter
     def disk_provisioning(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_provisioning", value)
 
     @property
     @pulumi.getter(name="enableHiddenProperties")
     def enable_hidden_properties(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allow properties with ovf:userConfigurable=false to be set.
+        """
         return pulumi.get(self, "enable_hidden_properties")
 
     @enable_hidden_properties.setter
     def enable_hidden_properties(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_hidden_properties", value)
 
     @property
     @pulumi.getter(name="ipAllocationPolicy")
     def ip_allocation_policy(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IP allocation policy.
+        """
         return pulumi.get(self, "ip_allocation_policy")
 
     @ip_allocation_policy.setter
     def ip_allocation_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_allocation_policy", value)
 
     @property
     @pulumi.getter(name="ipProtocol")
     def ip_protocol(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IP protocol.
+        """
         return pulumi.get(self, "ip_protocol")
 
     @ip_protocol.setter
     def ip_protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_protocol", value)
 
     @property
     @pulumi.getter(name="localOvfPath")
     def local_ovf_path(self) -> Optional[pulumi.Input[str]]:
+        """
+        The absolute path to the ovf/ova file in the local system.
+        """
         return pulumi.get(self, "local_ovf_path")
 
     @local_ovf_path.setter
     def local_ovf_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "local_ovf_path", value)
 
     @property
     @pulumi.getter(name="ovfNetworkMap")
     def ovf_network_map(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        The mapping of name of network identifiers from the ovf descriptor to network UUID in the VI infrastructure.
+        """
         return pulumi.get(self, "ovf_network_map")
 
     @ovf_network_map.setter
     def ovf_network_map(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "ovf_network_map", value)
 
     @property
     @pulumi.getter(name="remoteOvfUrl")
     def remote_ovf_url(self) -> Optional[pulumi.Input[str]]:
+        """
+        URL to the remote ovf/ova file to be deployed.
+        """
         return pulumi.get(self, "remote_ovf_url")
 
     @remote_ovf_url.setter
     def remote_ovf_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "remote_ovf_url", value)
 
 
 @pulumi.input_type
 class VirtualMachineVappArgs:
     def __init__(__self__, *,
                  properties: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] properties: A map of customizable vApp properties and their values. Allows customization of VMs cloned from OVF templates which have customizable vApp properties.
+        """
         if properties is not None:
             pulumi.set(__self__, "properties", properties)
 
     @property
     @pulumi.getter
     def properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        A map of customizable vApp properties and their values. Allows customization of VMs cloned from OVF templates which have customizable vApp properties.
+        """
         return pulumi.get(self, "properties")
 
     @properties.setter
     def properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "properties", value)
 
 
@@ -2678,20 +3074,26 @@
         pulumi.set(self, "gw", value)
 
 
 @pulumi.input_type
 class GetVirtualMachineVappArgs:
     def __init__(__self__, *,
                  properties: Optional[Mapping[str, str]] = None):
+        """
+        :param Mapping[str, str] properties: A map of customizable vApp properties and their values. Allows customization of VMs cloned from OVF templates which have customizable vApp properties.
+        """
         if properties is not None:
             pulumi.set(__self__, "properties", properties)
 
     @property
     @pulumi.getter
     def properties(self) -> Optional[Mapping[str, str]]:
+        """
+        A map of customizable vApp properties and their values. Allows customization of VMs cloned from OVF templates which have customizable vApp properties.
+        """
         return pulumi.get(self, "properties")
 
     @properties.setter
     def properties(self, value: Optional[Mapping[str, str]]):
         pulumi.set(self, "properties", value)
```

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/_utilities.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
 import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
 from pulumi.runtime.sync_await import _sync_await
 
@@ -68,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
```

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_host_group.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_host_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_affinity_rule.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_affinity_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_dependency_rule.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_dependency_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_group.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/compute_cluster_vm_host_rule.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/compute_cluster_vm_host_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/config/__init__.pyi` & `pulumi_vsphere-4.9.2/pulumi_vsphere/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/config/vars.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/content_library.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/content_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/content_library_item.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/content_library_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/custom_attribute.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/datacenter.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/datastore_cluster.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/datastore_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/distributed_port_group.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/distributed_port_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/distributed_virtual_switch.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/distributed_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/dpm_host_override.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/dpm_host_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/drs_vm_override.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/drs_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/entity_permissions.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/entity_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/file.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/folder.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_compute_cluster.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_compute_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_compute_cluster_host_group.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_compute_cluster_host_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_content_library.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_content_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_content_library_item.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_content_library_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_custom_attribute.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_datacenter.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_datastore.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_datastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_datastore_cluster.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_datastore_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_distributed_virtual_switch.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_distributed_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_dynamic.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_dynamic.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_folder.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_guest_os_customization.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_guest_os_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_host.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_host_pci_device.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_host_pci_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_host_thumbprint.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_host_thumbprint.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_license.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_license.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_network.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_ovf_vm_template.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_ovf_vm_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_policy.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_resource_pool.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_resource_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_role.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_tag.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_tag_category.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_tag_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_vapp_container.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_vapp_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_virtual_machine.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/get_vmfs_disks.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/get_vmfs_disks.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/guest_os_customization.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/guest_os_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/ha_vm_override.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/ha_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/host.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/host.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/host_port_group.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/host_port_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/host_virtual_switch.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/host_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/license.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/license.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/nas_datastore.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/nas_datastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/provider.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/resource_pool.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/resource_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/role.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/storage_drs_vm_override.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/storage_drs_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/tag.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/tag_category.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/tag_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/vapp_container.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/vapp_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/vapp_entity.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/vapp_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/virtual_disk.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/virtual_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/virtual_machine.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/virtual_machine_snapshot.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/virtual_machine_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/vm_storage_policy.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/vm_storage_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/vmfs_datastore.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/vmfs_datastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere/vnic.py` & `pulumi_vsphere-4.9.2/pulumi_vsphere/vnic.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/PKG-INFO` & `pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: pulumi-vsphere
-Version: 4.9.1
+Name: pulumi_vsphere
+Version: 4.9.2
 Summary: A Pulumi package for creating vsphere resources
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-vsphere
 Keywords: pulumi,vsphere
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0
 Requires-Dist: semver>=2.8.1
 
 [![Actions Status](https://github.com/pulumi/pulumi-vsphere/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-vsphere/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_vsphere-4.9.1/pulumi_vsphere.egg-info/SOURCES.txt` & `pulumi_vsphere-4.9.2/pulumi_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.9.1/pyproject.toml` & `pulumi_vsphere-4.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_vsphere"
   description = "A Pulumi package for creating vsphere resources"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "vsphere"]
   readme = "README.md"
-  requires-python = ">=3.7"
-  version = "4.9.1"
+  requires-python = ">=3.8"
+  version = "4.9.2"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-vsphere"
 
 [build-system]
```

