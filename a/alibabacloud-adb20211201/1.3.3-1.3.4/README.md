# Comparing `tmp/alibabacloud_adb20211201-1.3.3.tar.gz` & `tmp/alibabacloud_adb20211201-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adb20211201-1.3.3.tar", last modified: Wed Apr 10 17:11:51 2024, max compression
+gzip compressed data, was "dist/alibabacloud_adb20211201-1.3.4.tar", last modified: Thu May  9 17:09:45 2024, max compression
```

## Comparing `alibabacloud_adb20211201-1.3.3.tar` & `alibabacloud_adb20211201-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/
--rw-r--r--   0 root         (0) root         (0)     2134 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   432974 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/client.py
--rw-r--r--   0 root         (0) root         (0)   920707 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-10 17:11:51.000000 alibabacloud_adb20211201-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)     2284 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   550774 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201/client.py
+-rw-r--r--   0 root         (0) root         (0)   937417 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 17:09:45.000000 alibabacloud_adb20211201-1.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-09 17:09:44.000000 alibabacloud_adb20211201-1.3.4/setup.py
```

### Comparing `alibabacloud_adb20211201-1.3.3/ChangeLog.md` & `alibabacloud_adb20211201-1.3.4/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-10 Version: 1.3.3
+- Update API DescribeApsResourceGroups: add param RegionId.
+- Update API DescribeApsResourceGroups: add param WorkloadId.
+
+
 2024-04-09 Version: 1.3.2
 - Generated python 2021-12-01 for adb.
 
 2024-03-25 Version: 1.3.1
 - Update API CreateDBResourceGroup: add param Rules.
 - Update API DescribeDBResourceGroup: update response param.
 - Update API ModifyDBResourceGroup: add param Rules.
```

### Comparing `alibabacloud_adb20211201-1.3.3/LICENSE` & `alibabacloud_adb20211201-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.3/PKG-INFO` & `alibabacloud_adb20211201-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_adb20211201
-Version: 1.3.3
+Version: 1.3.4
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201-1.3.3/README-CN.md` & `alibabacloud_adb20211201-1.3.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.3/README.md` & `alibabacloud_adb20211201-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201/models.py` & `alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2811,15 +2811,18 @@
         compute_resource: str = None,
         dbcluster_description: str = None,
         dbcluster_network_type: str = None,
         dbcluster_version: str = None,
         enable_default_resource_pool: bool = None,
         pay_type: str = None,
         period: str = None,
+        product_form: str = None,
         region_id: str = None,
+        reserved_node_count: int = None,
+        reserved_node_size: str = None,
         resource_group_id: str = None,
         restore_to_time: str = None,
         restore_type: str = None,
         source_db_cluster_id: str = None,
         storage_resource: str = None,
         tag: List[CreateDBClusterRequestTag] = None,
         used_time: str = None,
@@ -2857,18 +2860,21 @@
         # The subscription type of the subscription cluster. Valid values:
         # 
         # *   **Year**: subscription on a yearly basis.
         # *   **Month**: subscription on a monthly basis.
         # 
         # >  This parameter must be specified when PayType is set to Prepaid.
         self.period = period
+        self.product_form = product_form
         # The region ID.
         # 
         # >  You can call the [DescribeRegions](~~454314~~) operation to query the most recent region list.
         self.region_id = region_id
+        self.reserved_node_count = reserved_node_count
+        self.reserved_node_size = reserved_node_size
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The point in time to which you want to restore data from the backup set.
         self.restore_to_time = restore_to_time
         # The method that you want to use to restore data. Valid values:
         # 
         # *   **backup**: restores data from a backup set. You must also specify the **BackupSetId** and **SourceDBClusterId** parameters.
@@ -2922,16 +2928,22 @@
             result['DBClusterVersion'] = self.dbcluster_version
         if self.enable_default_resource_pool is not None:
             result['EnableDefaultResourcePool'] = self.enable_default_resource_pool
         if self.pay_type is not None:
             result['PayType'] = self.pay_type
         if self.period is not None:
             result['Period'] = self.period
+        if self.product_form is not None:
+            result['ProductForm'] = self.product_form
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.reserved_node_count is not None:
+            result['ReservedNodeCount'] = self.reserved_node_count
+        if self.reserved_node_size is not None:
+            result['ReservedNodeSize'] = self.reserved_node_size
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.restore_to_time is not None:
             result['RestoreToTime'] = self.restore_to_time
         if self.restore_type is not None:
             result['RestoreType'] = self.restore_type
         if self.source_db_cluster_id is not None:
@@ -2966,16 +2978,22 @@
             self.dbcluster_version = m.get('DBClusterVersion')
         if m.get('EnableDefaultResourcePool') is not None:
             self.enable_default_resource_pool = m.get('EnableDefaultResourcePool')
         if m.get('PayType') is not None:
             self.pay_type = m.get('PayType')
         if m.get('Period') is not None:
             self.period = m.get('Period')
+        if m.get('ProductForm') is not None:
+            self.product_form = m.get('ProductForm')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ReservedNodeCount') is not None:
+            self.reserved_node_count = m.get('ReservedNodeCount')
+        if m.get('ReservedNodeSize') is not None:
+            self.reserved_node_size = m.get('ReservedNodeSize')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('RestoreToTime') is not None:
             self.restore_to_time = m.get('RestoreToTime')
         if m.get('RestoreType') is not None:
             self.restore_type = m.get('RestoreType')
         if m.get('SourceDbClusterId') is not None:
@@ -3091,16 +3109,23 @@
 class CreateDBResourceGroupRequestRules(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         query_time: str = None,
         target_group_name: str = None,
     ):
+        # The name of the resource group.
+        # 
+        # *   The name can be up to 255 characters in length.
+        # *   The name must start with a letter or digit.
+        # *   The name can contain letters, digits, hyphens (\_), and underscores (\_).
         self.group_name = group_name
+        # The execution duration of the query. Unit: milliseconds.
         self.query_time = query_time
+        # The name of the destination resource group.
         self.target_group_name = target_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3145,14 +3170,18 @@
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
+        # Specifies whether to enable the preemptible instance feature for the resource group. After you enable the preemptible instance feature, you are charged for resources at a lower unit price but the resources are probably released. You can enable the preemptible instance feature only for job resource groups. Valid values:
+        # 
+        # *   **True**\
+        # *   **False**\
         self.enable_spot = enable_spot
         # The name of the resource group.
         # 
         # *   The name can be up to 255 characters in length.
         # *   The name must start with a letter or a digit.
         # *   The name can contain letters, digits, hyphens (\_), and underscores (\_).
         self.group_name = group_name
@@ -3177,14 +3206,15 @@
         # *   When GroupType is set to Interactive, set this parameter to 16 ACUs.
         # *   When GroupType is set to Job, set this parameter to 0 ACUs.
         self.min_compute_resource = min_compute_resource
         # The region ID of the cluster.
         # 
         # >  You can call the [DescribeRegions](~~612393~~) operation to query the most recent region list.
         self.region_id = region_id
+        # The job resubmission rules.
         self.rules = rules
 
     def validate(self):
         if self.rules:
             for k in self.rules:
                 if k:
                     k.validate()
@@ -3273,14 +3303,18 @@
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
+        # Specifies whether to enable the preemptible instance feature for the resource group. After you enable the preemptible instance feature, you are charged for resources at a lower unit price but the resources are probably released. You can enable the preemptible instance feature only for job resource groups. Valid values:
+        # 
+        # *   **True**\
+        # *   **False**\
         self.enable_spot = enable_spot
         # The name of the resource group.
         # 
         # *   The name can be up to 255 characters in length.
         # *   The name must start with a letter or a digit.
         # *   The name can contain letters, digits, hyphens (\_), and underscores (\_).
         self.group_name = group_name
@@ -3305,14 +3339,15 @@
         # *   When GroupType is set to Interactive, set this parameter to 16 ACUs.
         # *   When GroupType is set to Job, set this parameter to 0 ACUs.
         self.min_compute_resource = min_compute_resource
         # The region ID of the cluster.
         # 
         # >  You can call the [DescribeRegions](~~612393~~) operation to query the most recent region list.
         self.region_id = region_id
+        # The job resubmission rules.
         self.rules_shrink = rules_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7113,14 +7148,15 @@
         workload_id: str = None,
     ):
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         # 
         # >  You can call the [DescribeDBClusters](~~612397~~) operation to query the IDs of all AnalyticDB for MySQL Data Lakehouse Edition (V3.0) clusters within a region.
         self.dbcluster_id = dbcluster_id
         self.region_id = region_id
+        # The ID of the data synchronization job.
         self.workload_id = workload_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9820,16 +9856,19 @@
         expired: str = None,
         lock_mode: str = None,
         lock_reason: str = None,
         maintain_time: str = None,
         mode: str = None,
         pay_type: str = None,
         port: int = None,
+        product_form: str = None,
         region_id: str = None,
         reserved_acu: str = None,
+        reserved_node_count: int = None,
+        reserved_node_size: str = None,
         resource_group_id: str = None,
         storage_resource: str = None,
         storage_resource_total: str = None,
         supported_features: Dict[str, str] = None,
         tags: DescribeDBClusterAttributeResponseBodyItemsDBClusterTags = None,
         user_enistatus: bool = None,
         vpcid: str = None,
@@ -9881,19 +9920,17 @@
         # *   If the billing method of the cluster is pay-as-you-go, null is returned.
         self.expire_time = expire_time
         # Indicates whether the subscription cluster has expired. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
-        # > 
-        # 
-        # *   If the cluster has expired, the system locks or releases the cluster within a period of time. We recommend that you renew the expired cluster. For more information, see [Renewal policy](~~135248~~).
         # 
-        # *   This parameter is not returned for pay-as-you-go clusters.
+        # > - If the cluster has expired, the system locks or releases the cluster within a period of time. We recommend that you renew the expired cluster. For more information, see [Renewal policy](~~135248~~).
+        # > - This parameter is not returned for pay-as-you-go clusters.
         self.expired = expired
         # The lock mode of the cluster. Valid values:
         # 
         # *   **Unlock**: The cluster is not locked.
         # *   **ManualLock**: The cluster is manually locked.
         # *   **LockByExpiration**: The cluster is automatically locked due to cluster expiration.
         self.lock_mode = lock_mode
@@ -9910,18 +9947,21 @@
         # The billing method of the cluster. Valid values:
         # 
         # *   **Postpaid**: pay-as-you-go.
         # *   **Prepaid**: subscription.
         self.pay_type = pay_type
         # The port number that is used to connect to the cluster.
         self.port = port
+        self.product_form = product_form
         # The region ID of the cluster.
         self.region_id = region_id
         # The remaining reserved computing resources that are available in the cluster. Each ACU is equivalent to 1 core and 4 GB memory.
         self.reserved_acu = reserved_acu
+        self.reserved_node_count = reserved_node_count
+        self.reserved_node_size = reserved_node_size
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The specifications of reserved storage resources. Each AnalyticDB compute unit (ACU) is equivalent to 1 core and 4 GB memory. Storage resources are used to read and write data. The increase in the storage resources can improve the read and write performance of the cluster.
         self.storage_resource = storage_resource
         # The total amount of storage resources in the cluster. Each ACU is equivalent to 1 core and 4 GB memory.
         self.storage_resource_total = storage_resource_total
         # A reserved parameter.
@@ -9988,18 +10028,24 @@
             result['MaintainTime'] = self.maintain_time
         if self.mode is not None:
             result['Mode'] = self.mode
         if self.pay_type is not None:
             result['PayType'] = self.pay_type
         if self.port is not None:
             result['Port'] = self.port
+        if self.product_form is not None:
+            result['ProductForm'] = self.product_form
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.reserved_acu is not None:
             result['ReservedACU'] = self.reserved_acu
+        if self.reserved_node_count is not None:
+            result['ReservedNodeCount'] = self.reserved_node_count
+        if self.reserved_node_size is not None:
+            result['ReservedNodeSize'] = self.reserved_node_size
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.storage_resource is not None:
             result['StorageResource'] = self.storage_resource
         if self.storage_resource_total is not None:
             result['StorageResourceTotal'] = self.storage_resource_total
         if self.supported_features is not None:
@@ -10056,18 +10102,24 @@
             self.maintain_time = m.get('MaintainTime')
         if m.get('Mode') is not None:
             self.mode = m.get('Mode')
         if m.get('PayType') is not None:
             self.pay_type = m.get('PayType')
         if m.get('Port') is not None:
             self.port = m.get('Port')
+        if m.get('ProductForm') is not None:
+            self.product_form = m.get('ProductForm')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ReservedACU') is not None:
             self.reserved_acu = m.get('ReservedACU')
+        if m.get('ReservedNodeCount') is not None:
+            self.reserved_node_count = m.get('ReservedNodeCount')
+        if m.get('ReservedNodeSize') is not None:
+            self.reserved_node_size = m.get('ReservedNodeSize')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('StorageResource') is not None:
             self.storage_resource = m.get('StorageResource')
         if m.get('StorageResourceTotal') is not None:
             self.storage_resource_total = m.get('StorageResourceTotal')
         if m.get('SupportedFeatures') is not None:
@@ -10573,18 +10625,18 @@
         # 
         #     *   **AnalyticDB_Disk_IO_Avg_Usage_Percentage**: the average I/O utilization.
         #     *   **AnalyticDB_Disk_IO_Avg_Waiting_Time**: the average I/O wait time.
         #     *   **AnalyticDB_IO_Throughput**: the disk throughput.
         #     *   **AnalyticDB_IOPS**: the disk IOPS.
         #     *   **AnalyticDB_Disk_Usage**: the disk space that is used.
         #     *   **AnalyticDB_Disk_Usage_Percentage**: the disk usage.
-        #     *   **AnalyticDB_HotDataDiskUsage**: the disk space that is used by hot data.
-        #     *   **AnalyticDB_ColdDataDiskUsage**: the disk space that is used by hot data.
+        #     *   **AnalyticDB_Hot_Data_Usage**: the disk space that is used by hot data.
+        #     *   **AnalyticDB_Cold_Data_Usage**: the disk space that is used by code data.
         # 
-        # > This parameter must be specified.
+        # >  This parameter must be specified.
         self.key = key
         # The region ID of the cluster.
         # 
         # > You can call the [DescribeRegions](~~612393~~) operation to query the most recent region list.
         self.region_id = region_id
         # The resource group ID.
         self.resource_pools = resource_pools
@@ -10836,17 +10888,21 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
+        # The region ID.
+        # 
+        # >  You can call the [DescribeRegions](~~143074~~) operation to query the most recent region list.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -10892,18 +10948,25 @@
         self,
         data_size: int = None,
         index_size: int = None,
         other_size: int = None,
         primary_key_index_size: int = None,
         total_size: int = None,
     ):
+        # The data size of table records. Unit: bytes.
         self.data_size = data_size
+        # The data size of regular indexes. Unit: bytes.
         self.index_size = index_size
+        # The data size of other data. Unit: bytes.
         self.other_size = other_size
+        # The data size of primary key indexes. Unit: bytes.
         self.primary_key_index_size = primary_key_index_size
+        # The cold data size. Unit: bytes.
+        # 
+        # >  Formula: Cold data size = Data size of table records + Data size of regular indexes + Data size of primary key indexes + Data size of other data.
         self.total_size = total_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10940,15 +11003,21 @@
 
 class DescribeDBClusterSpaceSummaryResponseBodyDataDataGrowth(TeaModel):
     def __init__(
         self,
         day_growth: int = None,
         week_growth: int = None,
     ):
+        # The data growth within the last day. Unit: bytes.
+        # 
+        # >  Formula: Data growth within the last day = Current data size - Data size one day ago.
         self.day_growth = day_growth
+        # The daily data growth within the last seven days. Unit: bytes.
+        # 
+        # >  Formula: Daily data growth within the last seven days = (Current data size - Data size seven days ago)/7.
         self.week_growth = week_growth
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10976,18 +11045,25 @@
         self,
         data_size: int = None,
         index_size: int = None,
         other_size: int = None,
         primary_key_index_size: int = None,
         total_size: int = None,
     ):
+        # The data size of table records. Unit: bytes.
         self.data_size = data_size
+        # The data size of regular indexes. Unit: bytes.
         self.index_size = index_size
+        # The data size of other data. Unit: bytes.
         self.other_size = other_size
+        # The data size of primary key indexes. Unit: bytes.
         self.primary_key_index_size = primary_key_index_size
+        # The hot data size. Unit: bytes.
+        # 
+        # >  Formula: Hot data size = Data size of table records + Data size of regular indexes + Data size of primary key indexes + Data size of other data.
         self.total_size = total_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11026,17 +11102,23 @@
     def __init__(
         self,
         cold_data: DescribeDBClusterSpaceSummaryResponseBodyDataColdData = None,
         data_growth: DescribeDBClusterSpaceSummaryResponseBodyDataDataGrowth = None,
         hot_data: DescribeDBClusterSpaceSummaryResponseBodyDataHotData = None,
         total_size: str = None,
     ):
+        # The cold data.
         self.cold_data = cold_data
+        # The data growth.
         self.data_growth = data_growth
+        # The hot data.
         self.hot_data = hot_data
+        # The total data size. Unit: bytes.
+        # 
+        # >  Formula: Total data size = Hot data size+ Cold data size.
         self.total_size = total_size
 
     def validate(self):
         if self.cold_data:
             self.cold_data.validate()
         if self.data_growth:
             self.data_growth.validate()
@@ -11077,15 +11159,17 @@
 
 class DescribeDBClusterSpaceSummaryResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDBClusterSpaceSummaryResponseBodyData = None,
         request_id: str = None,
     ):
+        # The queried storage overview information.
         self.data = data
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -11294,16 +11378,18 @@
 
 class DescribeDBClustersRequest(TeaModel):
     def __init__(
         self,
         dbcluster_description: str = None,
         dbcluster_ids: str = None,
         dbcluster_status: str = None,
+        dbcluster_version: str = None,
         page_number: int = None,
         page_size: int = None,
+        product_version: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         tag: List[DescribeDBClustersRequestTag] = None,
     ):
         # The description of the cluster.
         # 
         # *   The description cannot start with `http://` or `https://`.
@@ -11330,22 +11416,24 @@
         # <!---->
         # 
         # *   **ClassChanging**\
         # *   **NetAddressCreating**\
         # *   **NetAddressDeleting**\
         # *   **NetAddressModifying**\
         self.dbcluster_status = dbcluster_status
+        self.dbcluster_version = dbcluster_version
         # The page number. Pages start from page 1. Default value: **1**.
         self.page_number = page_number
         # The number of entries per page. Valid values:
         # 
         # *   **30** (default)
         # *   **50**\
         # *   **100**\
         self.page_size = page_size
+        self.product_version = product_version
         # The region ID of the cluster.
         # 
         # >  You can call the [DescribeRegions](~~454314~~) operation to query the most recent region list.
         self.region_id = region_id
         # The resource group ID. If you do not specify this parameter, the information about all resource groups in the cluster is returned.
         self.resource_group_id = resource_group_id
         # The tags that are added to the cluster.
@@ -11365,18 +11453,22 @@
         result = dict()
         if self.dbcluster_description is not None:
             result['DBClusterDescription'] = self.dbcluster_description
         if self.dbcluster_ids is not None:
             result['DBClusterIds'] = self.dbcluster_ids
         if self.dbcluster_status is not None:
             result['DBClusterStatus'] = self.dbcluster_status
+        if self.dbcluster_version is not None:
+            result['DBClusterVersion'] = self.dbcluster_version
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        if self.product_version is not None:
+            result['ProductVersion'] = self.product_version
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
@@ -11387,18 +11479,22 @@
         m = m or dict()
         if m.get('DBClusterDescription') is not None:
             self.dbcluster_description = m.get('DBClusterDescription')
         if m.get('DBClusterIds') is not None:
             self.dbcluster_ids = m.get('DBClusterIds')
         if m.get('DBClusterStatus') is not None:
             self.dbcluster_status = m.get('DBClusterStatus')
+        if m.get('DBClusterVersion') is not None:
+            self.dbcluster_version = m.get('DBClusterVersion')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
+        if m.get('ProductVersion') is not None:
+            self.product_version = m.get('ProductVersion')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
@@ -11475,44 +11571,200 @@
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = DescribeDBClustersResponseBodyItemsDBClusterTagsTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
+class DescribeDBClustersResponseBodyItemsDBClusterTaskInfoStepListStepList(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        start_time: str = None,
+        step_desc: str = None,
+        step_name: str = None,
+        step_progress: str = None,
+        step_status: str = None,
+    ):
+        self.end_time = end_time
+        self.start_time = start_time
+        self.step_desc = step_desc
+        self.step_name = step_name
+        self.step_progress = step_progress
+        self.step_status = step_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.step_desc is not None:
+            result['StepDesc'] = self.step_desc
+        if self.step_name is not None:
+            result['StepName'] = self.step_name
+        if self.step_progress is not None:
+            result['StepProgress'] = self.step_progress
+        if self.step_status is not None:
+            result['StepStatus'] = self.step_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('StepDesc') is not None:
+            self.step_desc = m.get('StepDesc')
+        if m.get('StepName') is not None:
+            self.step_name = m.get('StepName')
+        if m.get('StepProgress') is not None:
+            self.step_progress = m.get('StepProgress')
+        if m.get('StepStatus') is not None:
+            self.step_status = m.get('StepStatus')
+        return self
+
+
+class DescribeDBClustersResponseBodyItemsDBClusterTaskInfoStepList(TeaModel):
+    def __init__(
+        self,
+        step_list: List[DescribeDBClustersResponseBodyItemsDBClusterTaskInfoStepListStepList] = None,
+    ):
+        self.step_list = step_list
+
+    def validate(self):
+        if self.step_list:
+            for k in self.step_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['StepList'] = []
+        if self.step_list is not None:
+            for k in self.step_list:
+                result['StepList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.step_list = []
+        if m.get('StepList') is not None:
+            for k in m.get('StepList'):
+                temp_model = DescribeDBClustersResponseBodyItemsDBClusterTaskInfoStepListStepList()
+                self.step_list.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeDBClustersResponseBodyItemsDBClusterTaskInfo(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        progress: str = None,
+        status: str = None,
+        step_list: DescribeDBClustersResponseBodyItemsDBClusterTaskInfoStepList = None,
+    ):
+        self.name = name
+        self.progress = progress
+        self.status = status
+        self.step_list = step_list
+
+    def validate(self):
+        if self.step_list:
+            self.step_list.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.progress is not None:
+            result['Progress'] = self.progress
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.step_list is not None:
+            result['StepList'] = self.step_list.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Progress') is not None:
+            self.progress = m.get('Progress')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('StepList') is not None:
+            temp_model = DescribeDBClustersResponseBodyItemsDBClusterTaskInfoStepList()
+            self.step_list = temp_model.from_map(m['StepList'])
+        return self
+
+
 class DescribeDBClustersResponseBodyItemsDBCluster(TeaModel):
     def __init__(
         self,
+        category: str = None,
         commodity_code: str = None,
         compute_resource: str = None,
         connection_string: str = None,
         create_time: str = None,
         dbcluster_description: str = None,
         dbcluster_id: str = None,
         dbcluster_network_type: str = None,
         dbcluster_status: str = None,
         dbcluster_type: str = None,
+        dbnode_class: str = None,
+        dbnode_count: int = None,
+        dbnode_storage: int = None,
         dbversion: str = None,
+        disk_type: str = None,
+        dts_job_id: str = None,
+        elastic_ioresource: int = None,
         engine: str = None,
+        executor_count: str = None,
         expire_time: str = None,
         expired: str = None,
+        inner_ip: str = None,
+        inner_port: str = None,
         lock_mode: str = None,
         lock_reason: str = None,
         mode: str = None,
         pay_type: str = None,
         port: str = None,
+        product_form: str = None,
+        rds_instance_id: str = None,
         region_id: str = None,
         reserved_acu: str = None,
+        reserved_node_count: int = None,
+        reserved_node_size: str = None,
         resource_group_id: str = None,
         storage_resource: str = None,
         tags: DescribeDBClustersResponseBodyItemsDBClusterTags = None,
+        task_info: DescribeDBClustersResponseBodyItemsDBClusterTaskInfo = None,
+        vpccloud_instance_id: str = None,
         vpcid: str = None,
         v_switch_id: str = None,
         zone_id: str = None,
     ):
+        self.category = category
         # The billing method of the cluster. Valid values:
         # 
         # *   **ads**: pay-as-you-go.
         # *   **ads_pre**: subscription.
         self.commodity_code = commodity_code
         # The specifications of reserved computing resources. Each ACU is equivalent to 1 core and 4 GB memory. Computing resources are used to compute data. The increase in the computing resources can accelerate queries. You can scale computing resources based on your business requirements.
         self.compute_resource = compute_resource
@@ -11545,31 +11797,40 @@
         # *   **ClassChanging**\
         # *   **NetAddressCreating**\
         # *   **NetAddressDeleting**\
         # *   **NetAddressModifying**\
         self.dbcluster_status = dbcluster_status
         # The type of the cluster. By default, **Common** is returned, which indicates a common cluster.
         self.dbcluster_type = dbcluster_type
+        self.dbnode_class = dbnode_class
+        self.dbnode_count = dbnode_count
+        self.dbnode_storage = dbnode_storage
         # The version of AnalyticDB for MySQL Data Lakehouse Edition. **5.0** is returned.
         self.dbversion = dbversion
+        self.disk_type = disk_type
+        self.dts_job_id = dts_job_id
+        self.elastic_ioresource = elastic_ioresource
         # The database engine of the cluster. **AnalyticDB** is returned.
         self.engine = engine
+        self.executor_count = executor_count
         # The time when the cluster expired. The time follows the ISO 8601 standard in the *yyyy-MM-ddTHH:mm:ssZ* format. The time is displayed in UTC.
         # 
         # > - The expiration time is returned for a subscription cluster.
         # > - Anempty string is returned for a pay-as-you-go cluster.
         self.expire_time = expire_time
         # Indicates whether the subscription cluster has expired. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
         # > - If the cluster has expired, the system locks or releases the cluster within a period of time. We recommend that you renew expired clusters. For more information, see [Renewal policy](~~135246~~).
         # > - This parameter is not returned for pay-as-you-go clusters.
         self.expired = expired
+        self.inner_ip = inner_ip
+        self.inner_port = inner_port
         # The lock state of the cluster. Valid values:
         # 
         # *   **Unlock**: The cluster is not locked.
         # *   **ManualLock**: The cluster is manually locked.
         # *   **LockByExpiration**: The cluster is automatically locked due to cluster expiration.
         self.lock_mode = lock_mode
         # The reason why the cluster is locked.
@@ -11581,41 +11842,51 @@
         # The billing method of the cluster. Valid values:
         # 
         # *   **Postpaid**: pay-as-you-go.
         # *   **Prepaid**: subscription.
         self.pay_type = pay_type
         # The port number that is used to connect to the cluster.
         self.port = port
+        self.product_form = product_form
+        self.rds_instance_id = rds_instance_id
         # The region ID of the cluster.
         self.region_id = region_id
         # The amount of remaining reserved computing resources that are available in the cluster. Each ACU is equivalent to 1 core and 4 GB memory.
         self.reserved_acu = reserved_acu
+        self.reserved_node_count = reserved_node_count
+        self.reserved_node_size = reserved_node_size
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The specifications of reserved storage resources. Each AnalyticDB compute unit (ACU) is equivalent to 1 core and 4 GB memory. Storage resources are used to read and write data. The increase in the storage resources can improve the read and write performance of the cluster.
         self.storage_resource = storage_resource
         # The tags that are added to the cluster.
         self.tags = tags
+        self.task_info = task_info
+        self.vpccloud_instance_id = vpccloud_instance_id
         # The virtual private cloud (VPC) ID of the cluster.
         self.vpcid = vpcid
         # The vSwitch ID of the cluster.
         self.v_switch_id = v_switch_id
         # The zone ID of the cluster.
         self.zone_id = zone_id
 
     def validate(self):
         if self.tags:
             self.tags.validate()
+        if self.task_info:
+            self.task_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.category is not None:
+            result['Category'] = self.category
         if self.commodity_code is not None:
             result['CommodityCode'] = self.commodity_code
         if self.compute_resource is not None:
             result['ComputeResource'] = self.compute_resource
         if self.connection_string is not None:
             result['ConnectionString'] = self.connection_string
         if self.create_time is not None:
@@ -11626,52 +11897,84 @@
             result['DBClusterId'] = self.dbcluster_id
         if self.dbcluster_network_type is not None:
             result['DBClusterNetworkType'] = self.dbcluster_network_type
         if self.dbcluster_status is not None:
             result['DBClusterStatus'] = self.dbcluster_status
         if self.dbcluster_type is not None:
             result['DBClusterType'] = self.dbcluster_type
+        if self.dbnode_class is not None:
+            result['DBNodeClass'] = self.dbnode_class
+        if self.dbnode_count is not None:
+            result['DBNodeCount'] = self.dbnode_count
+        if self.dbnode_storage is not None:
+            result['DBNodeStorage'] = self.dbnode_storage
         if self.dbversion is not None:
             result['DBVersion'] = self.dbversion
+        if self.disk_type is not None:
+            result['DiskType'] = self.disk_type
+        if self.dts_job_id is not None:
+            result['DtsJobId'] = self.dts_job_id
+        if self.elastic_ioresource is not None:
+            result['ElasticIOResource'] = self.elastic_ioresource
         if self.engine is not None:
             result['Engine'] = self.engine
+        if self.executor_count is not None:
+            result['ExecutorCount'] = self.executor_count
         if self.expire_time is not None:
             result['ExpireTime'] = self.expire_time
         if self.expired is not None:
             result['Expired'] = self.expired
+        if self.inner_ip is not None:
+            result['InnerIp'] = self.inner_ip
+        if self.inner_port is not None:
+            result['InnerPort'] = self.inner_port
         if self.lock_mode is not None:
             result['LockMode'] = self.lock_mode
         if self.lock_reason is not None:
             result['LockReason'] = self.lock_reason
         if self.mode is not None:
             result['Mode'] = self.mode
         if self.pay_type is not None:
             result['PayType'] = self.pay_type
         if self.port is not None:
             result['Port'] = self.port
+        if self.product_form is not None:
+            result['ProductForm'] = self.product_form
+        if self.rds_instance_id is not None:
+            result['RdsInstanceId'] = self.rds_instance_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.reserved_acu is not None:
             result['ReservedACU'] = self.reserved_acu
+        if self.reserved_node_count is not None:
+            result['ReservedNodeCount'] = self.reserved_node_count
+        if self.reserved_node_size is not None:
+            result['ReservedNodeSize'] = self.reserved_node_size
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.storage_resource is not None:
             result['StorageResource'] = self.storage_resource
         if self.tags is not None:
             result['Tags'] = self.tags.to_map()
+        if self.task_info is not None:
+            result['TaskInfo'] = self.task_info.to_map()
+        if self.vpccloud_instance_id is not None:
+            result['VPCCloudInstanceId'] = self.vpccloud_instance_id
         if self.vpcid is not None:
             result['VPCId'] = self.vpcid
         if self.v_switch_id is not None:
             result['VSwitchId'] = self.v_switch_id
         if self.zone_id is not None:
             result['ZoneId'] = self.zone_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
         if m.get('CommodityCode') is not None:
             self.commodity_code = m.get('CommodityCode')
         if m.get('ComputeResource') is not None:
             self.compute_resource = m.get('ComputeResource')
         if m.get('ConnectionString') is not None:
             self.connection_string = m.get('ConnectionString')
         if m.get('CreateTime') is not None:
@@ -11682,43 +11985,74 @@
             self.dbcluster_id = m.get('DBClusterId')
         if m.get('DBClusterNetworkType') is not None:
             self.dbcluster_network_type = m.get('DBClusterNetworkType')
         if m.get('DBClusterStatus') is not None:
             self.dbcluster_status = m.get('DBClusterStatus')
         if m.get('DBClusterType') is not None:
             self.dbcluster_type = m.get('DBClusterType')
+        if m.get('DBNodeClass') is not None:
+            self.dbnode_class = m.get('DBNodeClass')
+        if m.get('DBNodeCount') is not None:
+            self.dbnode_count = m.get('DBNodeCount')
+        if m.get('DBNodeStorage') is not None:
+            self.dbnode_storage = m.get('DBNodeStorage')
         if m.get('DBVersion') is not None:
             self.dbversion = m.get('DBVersion')
+        if m.get('DiskType') is not None:
+            self.disk_type = m.get('DiskType')
+        if m.get('DtsJobId') is not None:
+            self.dts_job_id = m.get('DtsJobId')
+        if m.get('ElasticIOResource') is not None:
+            self.elastic_ioresource = m.get('ElasticIOResource')
         if m.get('Engine') is not None:
             self.engine = m.get('Engine')
+        if m.get('ExecutorCount') is not None:
+            self.executor_count = m.get('ExecutorCount')
         if m.get('ExpireTime') is not None:
             self.expire_time = m.get('ExpireTime')
         if m.get('Expired') is not None:
             self.expired = m.get('Expired')
+        if m.get('InnerIp') is not None:
+            self.inner_ip = m.get('InnerIp')
+        if m.get('InnerPort') is not None:
+            self.inner_port = m.get('InnerPort')
         if m.get('LockMode') is not None:
             self.lock_mode = m.get('LockMode')
         if m.get('LockReason') is not None:
             self.lock_reason = m.get('LockReason')
         if m.get('Mode') is not None:
             self.mode = m.get('Mode')
         if m.get('PayType') is not None:
             self.pay_type = m.get('PayType')
         if m.get('Port') is not None:
             self.port = m.get('Port')
+        if m.get('ProductForm') is not None:
+            self.product_form = m.get('ProductForm')
+        if m.get('RdsInstanceId') is not None:
+            self.rds_instance_id = m.get('RdsInstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ReservedACU') is not None:
             self.reserved_acu = m.get('ReservedACU')
+        if m.get('ReservedNodeCount') is not None:
+            self.reserved_node_count = m.get('ReservedNodeCount')
+        if m.get('ReservedNodeSize') is not None:
+            self.reserved_node_size = m.get('ReservedNodeSize')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('StorageResource') is not None:
             self.storage_resource = m.get('StorageResource')
         if m.get('Tags') is not None:
             temp_model = DescribeDBClustersResponseBodyItemsDBClusterTags()
             self.tags = temp_model.from_map(m['Tags'])
+        if m.get('TaskInfo') is not None:
+            temp_model = DescribeDBClustersResponseBodyItemsDBClusterTaskInfo()
+            self.task_info = temp_model.from_map(m['TaskInfo'])
+        if m.get('VPCCloudInstanceId') is not None:
+            self.vpccloud_instance_id = m.get('VPCCloudInstanceId')
         if m.get('VPCId') is not None:
             self.vpcid = m.get('VPCId')
         if m.get('VSwitchId') is not None:
             self.v_switch_id = m.get('VSwitchId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
@@ -11876,14 +12210,17 @@
         # The type of the resource group. Valid values:
         # 
         # *   **Interactive**\
         # *   **Job**\
         # 
         # > For information about resource groups of Data Lakehouse Edition, see [Resource groups](~~428610~~).
         self.group_type = group_type
+        # The region ID of the cluster.
+        # 
+        # >  You can call the [DescribeRegions](~~612393~~) operation to query the most recent region list.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11922,16 +12259,19 @@
 class DescribeDBResourceGroupResponseBodyGroupsInfoRules(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         query_time: str = None,
         target_group_name: str = None,
     ):
+        # The name of the resource group.
         self.group_name = group_name
+        # The execution duration of the query. Unit: milliseconds.
         self.query_time = query_time
+        # The name of the destination resource group.
         self.target_group_name = target_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11980,36 +12320,43 @@
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
         # The time when the resource group was created. The time follows the ISO 8601 standard in the *yyyy-MM-ddTHH:mm:ssZ* format. The time is displayed in UTC.
         self.create_time = create_time
-        # The minimum amount of elastic computing resources. Unit: ACU.
+        # The minimum amount of elastic computing resources. Unit: ACUs.
         self.elastic_min_compute_resource = elastic_min_compute_resource
+        # Indicates whether the preemptible instance feature is enabled for the resource group. After the preemptible instance feature is enabled, you are charged for resources at a lower unit price but the resources are probably released. Valid values:
+        # 
+        # *   **True**\
+        # *   **False**\
+        # 
+        # The True value is returned only for job resource groups.
         self.enable_spot = enable_spot
         # The name of the resource group.
         self.group_name = group_name
         # The type of the resource group. Valid values:
         # 
         # *   **Interactive**\
         # *   **Job**\
         # 
         # >  For more information about resource groups, see [Resource groups](~~428610~~).
         self.group_type = group_type
         # The Resource Access Management (RAM) user that is associated with the resource group.
         self.group_users = group_users
         # A reserved parameter.
         self.max_cluster_count = max_cluster_count
-        # The maximum amount of reserved computing resources. Unit: ACU.
+        # The maximum amount of reserved computing resources. Unit: ACUs.
         self.max_compute_resource = max_compute_resource
         # A reserved parameter.
         self.min_cluster_count = min_cluster_count
-        # The minimum amount of reserved computing resources. Unit: AnalyticDB compute unit (ACU).
+        # The minimum amount of reserved computing resources. Unit: AnalyticDB compute units (ACUs).
         self.min_compute_resource = min_compute_resource
+        # The job resubmission rules.
         self.rules = rules
         # A reserved parameter.
         self.running_cluster_count = running_cluster_count
         # The status of the resource group. Valid values:
         # 
         # *   **creating**: The resource group is being created.
         # *   **ok**: The resource group is created.
@@ -12910,15 +13257,15 @@
         # 
         # >  You can call the [DescribeDiagnosisRecords](~~308207~~) operation to query the diagnostic information about SQL statements for an AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster, including the IP address and port number of the frontend node.
         self.process_rc_host = process_rc_host
         # The execution start time of the SQL statement. Set the time to a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         # 
         # >  You can call the [DescribeDiagnosisRecords](~~308207~~) operation to query the diagnostic information about SQL statements for an AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster, including the execution start time of the SQL statement.
         self.process_start_time = process_start_time
-        # The state of the SQL statement. Valid values:
+        # The status of the SQL statement. Valid values:
         # 
         # *   **running**\
         # *   **finished**\
         # *   **failed**\
         # 
         # >  You can call the [DescribeDiagnosisRecords](~~308207~~) operation to query the diagnostic information about SQL statements for an AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster, including the status of the SQL statement.
         self.process_state = process_state
@@ -13341,21 +13688,21 @@
 
 class DescribeElasticPlanAttributeRequest(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
         elastic_plan_name: str = None,
     ):
-        # The ID of the cluster.
+        # The cluster ID.
         # 
-        # >  You can call the [DescribeDBClusters](~~454250~~) operation to query the ID of an AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
+        # >  You can call the [DescribeDBClusters](~~454250~~) operation to query the IDs of all AnalyticDB for MySQL Data Lakehouse Edition (V3.0) clusters within a region.
         self.dbcluster_id = dbcluster_id
         # The name of the scaling plan.
         # 
-        # >  You can call the [DescribeElasticPlans](~~601334~~) operation to query the name of a scaling plan.
+        # >  You can call the [DescribeElasticPlans](~~601334~~) operation to query the names of scaling plans.
         self.elastic_plan_name = elastic_plan_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13387,35 +13734,29 @@
         enabled: bool = None,
         end_time: str = None,
         resource_group_name: str = None,
         start_time: str = None,
         target_size: str = None,
         type: str = None,
     ):
-        # Indicates whether **Proportional Default Scaling for EIUs** is enabled.
+        # Indicates whether **Default Proportional Scaling for EIUs** is enabled. Valid values: true: Default Proportional Scaling for EIUs is enabled. If you set this parameter to true, storage resources are scaled along with computing resources. false: Default Proportional Scaling for EIUs is not enabled.
         # 
-        # Valid values:
-        # 
-        # true: Proportional Default Scaling for EIUs is enabled. If you set this parameter to true, the amount of storage resources scales along with the computing resources.
-        # 
-        # false: Proportional Default Scaling for EIUs is not enabled.
-        # 
-        # >  You can enable Proportional Default Scaling for EIUs for only a single scaling plan of a cluster.
+        # >  You can enable Default Proportional Scaling for EIUs for only a single scaling plan of a cluster. After you enable a scaling plan of the Default Proportional Scaling for EIUs type, you cannot enable scaling plans of other types.
         self.auto_scale = auto_scale
         # A CORN expression that indicates the scaling cycle and time for the scaling plan.
         self.cron_expression = cron_expression
         # The name of the scaling plan.
         self.elastic_plan_name = elastic_plan_name
-        # Indicates whether the scaling plan was enabled.
+        # Indicates whether the scaling plan is enabled.
         self.enabled = enabled
         # The end time of the scaling plan.
         # 
         # >  The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         self.end_time = end_time
-        # The name of the resource group.
+        # The name of the resource group used by the scaling plan.
         self.resource_group_name = resource_group_name
         # The start time of the scaling plan.
         # 
         # >  The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         self.start_time = start_time
         # The amount of elastic resources after scaling.
         self.target_size = target_size
@@ -13476,17 +13817,17 @@
 
 class DescribeElasticPlanAttributeResponseBody(TeaModel):
     def __init__(
         self,
         elastic_plan: DescribeElasticPlanAttributeResponseBodyElasticPlan = None,
         request_id: str = None,
     ):
-        # Details of the scaling plan.
+        # The queried scaling plan.
         self.elastic_plan = elastic_plan
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.elastic_plan:
             self.elastic_plan.validate()
 
     def to_map(self):
@@ -15080,19 +15421,19 @@
         self,
         accept_language: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
-        # The language used for the region and zone names specified by the LocalName parameter. Default value: zh-CN. Valid values:
+        # The language that is used for the region and zone names indicated by the LocalName parameter in the response parameters. Valid values:
         # 
-        # *   **zh-CN**: simplified Chinese
-        # *   **en-US**: English
-        # *   **ja**: Japanese
+        # *   **zh-CN** (default): simplified Chinese.
+        # *   **en-US**: English.
+        # *   **ja**: Japanese.
         self.accept_language = accept_language
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -15138,18 +15479,18 @@
         vpc_enabled: bool = None,
         zone_id: str = None,
     ):
         # The name of the zone.
         self.local_name = local_name
         # Indicates whether Virtual Private Cloud (VPC) is supported in the zone. Valid values:
         # 
-        # *   **true**: VPC is supported.
-        # *   **false**: VPC is not supported.
+        # *   **true**\
+        # *   **false**\
         self.vpc_enabled = vpc_enabled
-        # The ID of the zone.
+        # The zone ID.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15219,17 +15560,17 @@
         region_id: str = None,
         zones: DescribeRegionsResponseBodyRegionsRegionZones = None,
     ):
         # The name of the region.
         self.local_name = local_name
         # The endpoint of the region.
         self.region_endpoint = region_endpoint
-        # The ID of the region.
+        # The region ID.
         self.region_id = region_id
-        # Details of the zones.
+        # The queried zones.
         self.zones = zones
 
     def validate(self):
         if self.zones:
             self.zones.validate()
 
     def to_map(self):
@@ -15299,17 +15640,17 @@
 
 class DescribeRegionsResponseBody(TeaModel):
     def __init__(
         self,
         regions: DescribeRegionsResponseBodyRegions = None,
         request_id: str = None,
     ):
-        # Details of the regions.
+        # The queried regions.
         self.regions = regions
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.regions:
             self.regions.validate()
 
     def to_map(self):
@@ -19191,15 +19532,15 @@
         message: str = None,
         state: str = None,
     ):
         # The Spark application ID.
         self.app_id = app_id
         # The name of the application.
         self.app_name = app_name
-        # The database ID.
+        # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
         # The alert message returned for the operation, such as task execution failure or insufficient resources. If no alert occurs, null is returned.
         self.message = message
         # The execution state of the application. Valid values:
         # 
         # *   **SUBMITTED**\
         # *   **STARTING**\
@@ -22937,15 +23278,15 @@
         # The description of the database account.
         # 
         # *   The description cannot start with `http://` or `https://`.
         # *   The description must be 2 to 256 characters in length.
         self.account_description = account_description
         # The name of the database account.
         # 
-        # > You can call the [DescribeAccounts](~~612430~~) operation to query the information about database accounts in a cluster, including the database account name.
+        # >  You can call the [DescribeAccounts](~~612430~~) operation to query the information about database accounts of an AnalyticDB for MySQL cluster, including database account names.
         self.account_name = account_name
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
 
     def validate(self):
         pass
 
@@ -23912,14 +24253,16 @@
         self,
         compute_resource: str = None,
         dbcluster_id: str = None,
         enable_default_resource_pool: bool = None,
         owner_account: str = None,
         owner_id: int = None,
         region_id: str = None,
+        reserved_node_count: int = None,
+        reserved_node_size: str = None,
         resource_owner_account: str = None,
         storage_resource: str = None,
     ):
         # The reserved computing resources. Unit: ACUs. Valid values: 0 to 4096. The value must be in increments of 16 ACUs. Each ACU is equivalent to 1 core and 4 GB memory.
         # 
         # >  This parameter must be specified with a unit.
         self.compute_resource = compute_resource
@@ -23934,14 +24277,16 @@
         self.enable_default_resource_pool = enable_default_resource_pool
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
         # 
         # >  You can call the [DescribeRegions](~~454314~~) operation to query the most recent region list.
         self.region_id = region_id
+        self.reserved_node_count = reserved_node_count
+        self.reserved_node_size = reserved_node_size
         self.resource_owner_account = resource_owner_account
         # The reserved storage resources. Unit: ACUs. Valid values: 0 to 2064. The value must be in increments of 24 ACUs. Each ACU is equivalent to 1 core and 4 GB memory.
         # 
         # >  This parameter must be specified with a unit.
         self.storage_resource = storage_resource
 
     def validate(self):
@@ -23961,14 +24306,18 @@
             result['EnableDefaultResourcePool'] = self.enable_default_resource_pool
         if self.owner_account is not None:
             result['OwnerAccount'] = self.owner_account
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.reserved_node_count is not None:
+            result['ReservedNodeCount'] = self.reserved_node_count
+        if self.reserved_node_size is not None:
+            result['ReservedNodeSize'] = self.reserved_node_size
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.storage_resource is not None:
             result['StorageResource'] = self.storage_resource
         return result
 
     def from_map(self, m: dict = None):
@@ -23981,14 +24330,18 @@
             self.enable_default_resource_pool = m.get('EnableDefaultResourcePool')
         if m.get('OwnerAccount') is not None:
             self.owner_account = m.get('OwnerAccount')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ReservedNodeCount') is not None:
+            self.reserved_node_count = m.get('ReservedNodeCount')
+        if m.get('ReservedNodeSize') is not None:
+            self.reserved_node_size = m.get('ReservedNodeSize')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('StorageResource') is not None:
             self.storage_resource = m.get('StorageResource')
         return self
 
 
@@ -24188,15 +24541,15 @@
         dbcluster_id: str = None,
         maintain_time: str = None,
     ):
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
         # The maintenance window of the cluster. It must be in the hh:mmZ-hh:mmZ format.
         # 
-        # > The interval must be 1 hour on the hour.
+        # > The interval must be 1 hour and start and end at the beginning of an hour.
         self.maintain_time = maintain_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24291,16 +24644,19 @@
 class ModifyDBResourceGroupRequestRules(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         query_time: str = None,
         target_group_name: str = None,
     ):
+        # The name of the resource group.
         self.group_name = group_name
+        # The execution duration of the query. Unit: milliseconds.
         self.query_time = query_time
+        # The name of the destination resource group.
         self.target_group_name = target_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24345,15 +24701,15 @@
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
-        # Specifies whether to enable the preemptible instance feature for the resource group. This feature can be enabled only for job resource groups. Valid values:
+        # Specifies whether to enable the spot instance feature for the resource group. After you enable the spot instance feature, you are charged for resources at a lower unit price but the resources are probably released. You can enable the spot instance feature only for job resource groups. Valid values:
         # 
         # *   **True**\
         # *   **False**\
         self.enable_spot = enable_spot
         # The name of the resource group.
         # 
         # > You can call the [DescribeDBResourceGroup](~~459446~~) operation to query the name of a resource group in a cluster.
@@ -24379,14 +24735,15 @@
         # *   If the GroupType parameter is set to Interactive, set the value to 16ACU.
         # *   If GroupType is set to Job, set the value to 0ACU.
         self.min_compute_resource = min_compute_resource
         # The region ID of the cluster.
         # 
         # >  You can call the [DescribeRegions](~~454314~~) operation to query the most recent region list.
         self.region_id = region_id
+        # The job resubmission rules.
         self.rules = rules
 
     def validate(self):
         if self.rules:
             for k in self.rules:
                 if k:
                     k.validate()
@@ -24475,15 +24832,15 @@
     ):
         # A reserved parameter.
         self.cluster_mode = cluster_mode
         # A reserved parameter.
         self.cluster_size_resource = cluster_size_resource
         # The ID of the AnalyticDB for MySQL Data Lakehouse Edition (V3.0) cluster.
         self.dbcluster_id = dbcluster_id
-        # Specifies whether to enable the preemptible instance feature for the resource group. This feature can be enabled only for job resource groups. Valid values:
+        # Specifies whether to enable the spot instance feature for the resource group. After you enable the spot instance feature, you are charged for resources at a lower unit price but the resources are probably released. You can enable the spot instance feature only for job resource groups. Valid values:
         # 
         # *   **True**\
         # *   **False**\
         self.enable_spot = enable_spot
         # The name of the resource group.
         # 
         # > You can call the [DescribeDBResourceGroup](~~459446~~) operation to query the name of a resource group in a cluster.
@@ -24509,14 +24866,15 @@
         # *   If the GroupType parameter is set to Interactive, set the value to 16ACU.
         # *   If GroupType is set to Job, set the value to 0ACU.
         self.min_compute_resource = min_compute_resource
         # The region ID of the cluster.
         # 
         # >  You can call the [DescribeRegions](~~454314~~) operation to query the most recent region list.
         self.region_id = region_id
+        # The job resubmission rules.
         self.rules_shrink = rules_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_adb20211201-1.3.3/alibabacloud_adb20211201.egg-info/PKG-INFO` & `alibabacloud_adb20211201-1.3.4/alibabacloud_adb20211201.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-adb20211201
-Version: 1.3.3
+Version: 1.3.4
 Summary: Alibaba Cloud adb (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adb20211201-1.3.3/setup.py` & `alibabacloud_adb20211201-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adb20211201.
 
-Created on 10/04/2024
+Created on 09/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adb20211201"
 NAME = "alibabacloud_adb20211201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adb (20211201) SDK Library for Python"
```

