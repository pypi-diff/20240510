# Comparing `tmp/pulumi_civo-2.4.0a1715335912.tar.gz` & `tmp/pulumi_civo-2.4.0a1715356631.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1715335912.tar", last modified: Fri May 10 10:14:42 2024, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1715356631.tar", last modified: Fri May 10 16:01:23 2024, max compression
```

## Comparing `pulumi_civo-2.4.0a1715335912.tar` & `pulumi_civo-2.4.0a1715356631.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:14:42.800676 pulumi_civo-2.4.0a1715335912/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-10 10:14:42.800676 pulumi_civo-2.4.0a1715335912/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:14:42.796676 pulumi_civo-2.4.0a1715335912/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43299 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:14:42.800676 pulumi_civo-2.4.0a1715335912/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_database_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    49735 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    58435 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:14:42.800676 pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-10 10:14:42.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-10 10:14:42.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:14:42.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 10:14:42.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 10:14:42.000000 pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-10 10:14:33.000000 pulumi_civo-2.4.0a1715335912/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:14:42.800676 pulumi_civo-2.4.0a1715335912/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:23.940457 pulumi_civo-2.4.0a1715356631/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-10 16:01:23.940457 pulumi_civo-2.4.0a1715356631/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:23.940457 pulumi_civo-2.4.0a1715356631/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43299 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:23.940457 pulumi_civo-2.4.0a1715356631/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51800 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26333 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58435 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:01:23.940457 pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-10 16:01:23.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-10 16:01:23.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:01:23.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 16:01:23.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 16:01:23.000000 pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-10 16:01:17.000000 pulumi_civo-2.4.0a1715356631/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:01:23.940457 pulumi_civo-2.4.0a1715356631/setup.cfg
```

### Comparing `pulumi_civo-2.4.0a1715335912/PKG-INFO` & `pulumi_civo-2.4.0a1715356631/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1715335912
+Version: 2.4.0a1715356631
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1715335912/README.md` & `pulumi_civo-2.4.0a1715356631/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/config/__init__.pyi` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_database_version.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_database_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def __init__(__self__, *,
                  disk_image: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
+                 private_ipv4: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
@@ -33,14 +34,15 @@
         The set of arguments for constructing a Instance resource.
         :param pulumi.Input[str] disk_image: The ID for the disk image to use to build the instance
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] hostname: A fully qualified domain name that should be set as the instance's hostname
         :param pulumi.Input[str] initial_user: The name of the initial user created on the server (optional; this will default to the template's default_username and fallback to civo)
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
+        :param pulumi.Input[str] private_ipv4: The private IPv4 address for the instance (optional)
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
         :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
         :param pulumi.Input[str] size: The name of the size, from the current list, e.g. g3.xsmall
         :param pulumi.Input[str] sshkey_id: The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
@@ -55,14 +57,16 @@
             pulumi.set(__self__, "hostname", hostname)
         if initial_user is not None:
             pulumi.set(__self__, "initial_user", initial_user)
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
+        if private_ipv4 is not None:
+            pulumi.set(__self__, "private_ipv4", private_ipv4)
         if public_ip_required is not None:
             pulumi.set(__self__, "public_ip_required", public_ip_required)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if reserved_ipv4 is not None:
             pulumi.set(__self__, "reserved_ipv4", reserved_ipv4)
         if reverse_dns is not None:
@@ -150,14 +154,26 @@
         return pulumi.get(self, "notes")
 
     @notes.setter
     def notes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "notes", value)
 
     @property
+    @pulumi.getter(name="privateIpv4")
+    def private_ipv4(self) -> Optional[pulumi.Input[str]]:
+        """
+        The private IPv4 address for the instance (optional)
+        """
+        return pulumi.get(self, "private_ipv4")
+
+    @private_ipv4.setter
+    def private_ipv4(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "private_ipv4", value)
+
+    @property
     @pulumi.getter(name="publicIpRequired")
     def public_ip_required(self) -> Optional[pulumi.Input[str]]:
         """
         This should be either 'none' or 'create' (default: 'create')
         """
         return pulumi.get(self, "public_ip_required")
 
@@ -275,14 +291,15 @@
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_password: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
                  private_ip: Optional[pulumi.Input[str]] = None,
+                 private_ipv4: Optional[pulumi.Input[str]] = None,
                  public_ip: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  ram_mb: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
@@ -302,14 +319,15 @@
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] hostname: A fully qualified domain name that should be set as the instance's hostname
         :param pulumi.Input[str] initial_password: Initial password for login
         :param pulumi.Input[str] initial_user: The name of the initial user created on the server (optional; this will default to the template's default_username and fallback to civo)
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
         :param pulumi.Input[str] private_ip: Instance's private IP address
+        :param pulumi.Input[str] private_ipv4: The private IPv4 address for the instance (optional)
         :param pulumi.Input[str] public_ip: Instance's public IP address
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[int] ram_mb: Instance's RAM (MB)
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
         :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
@@ -339,14 +357,16 @@
             pulumi.set(__self__, "initial_user", initial_user)
         if network_id is not None:
             pulumi.set(__self__, "network_id", network_id)
         if notes is not None:
             pulumi.set(__self__, "notes", notes)
         if private_ip is not None:
             pulumi.set(__self__, "private_ip", private_ip)
+        if private_ipv4 is not None:
+            pulumi.set(__self__, "private_ipv4", private_ipv4)
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
         if public_ip_required is not None:
             pulumi.set(__self__, "public_ip_required", public_ip_required)
         if ram_mb is not None:
             pulumi.set(__self__, "ram_mb", ram_mb)
         if region is not None:
@@ -504,14 +524,26 @@
         return pulumi.get(self, "private_ip")
 
     @private_ip.setter
     def private_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "private_ip", value)
 
     @property
+    @pulumi.getter(name="privateIpv4")
+    def private_ipv4(self) -> Optional[pulumi.Input[str]]:
+        """
+        The private IPv4 address for the instance (optional)
+        """
+        return pulumi.get(self, "private_ipv4")
+
+    @private_ipv4.setter
+    def private_ipv4(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "private_ipv4", value)
+
+    @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[pulumi.Input[str]]:
         """
         Instance's public IP address
         """
         return pulumi.get(self, "public_ip")
 
@@ -686,14 +718,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  disk_image: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
+                 private_ipv4: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
@@ -715,14 +748,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] disk_image: The ID for the disk image to use to build the instance
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] hostname: A fully qualified domain name that should be set as the instance's hostname
         :param pulumi.Input[str] initial_user: The name of the initial user created on the server (optional; this will default to the template's default_username and fallback to civo)
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
+        :param pulumi.Input[str] private_ipv4: The private IPv4 address for the instance (optional)
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
         :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
         :param pulumi.Input[str] size: The name of the size, from the current list, e.g. g3.xsmall
         :param pulumi.Input[str] sshkey_id: The ID of an already uploaded SSH public key to use for login to the default user (optional; if one isn't provided a random password will be set and returned in the initial_password field)
@@ -763,14 +797,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  disk_image: Optional[pulumi.Input[str]] = None,
                  firewall_id: Optional[pulumi.Input[str]] = None,
                  hostname: Optional[pulumi.Input[str]] = None,
                  initial_user: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  notes: Optional[pulumi.Input[str]] = None,
+                 private_ipv4: Optional[pulumi.Input[str]] = None,
                  public_ip_required: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  reserved_ipv4: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  script: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  sshkey_id: Optional[pulumi.Input[str]] = None,
@@ -787,14 +822,15 @@
 
             __props__.__dict__["disk_image"] = disk_image
             __props__.__dict__["firewall_id"] = firewall_id
             __props__.__dict__["hostname"] = hostname
             __props__.__dict__["initial_user"] = initial_user
             __props__.__dict__["network_id"] = network_id
             __props__.__dict__["notes"] = notes
+            __props__.__dict__["private_ipv4"] = private_ipv4
             __props__.__dict__["public_ip_required"] = public_ip_required
             __props__.__dict__["region"] = region
             __props__.__dict__["reserved_ipv4"] = reserved_ipv4
             __props__.__dict__["reverse_dns"] = reverse_dns
             __props__.__dict__["script"] = script
             __props__.__dict__["size"] = size
             __props__.__dict__["sshkey_id"] = sshkey_id
@@ -829,14 +865,15 @@
             firewall_id: Optional[pulumi.Input[str]] = None,
             hostname: Optional[pulumi.Input[str]] = None,
             initial_password: Optional[pulumi.Input[str]] = None,
             initial_user: Optional[pulumi.Input[str]] = None,
             network_id: Optional[pulumi.Input[str]] = None,
             notes: Optional[pulumi.Input[str]] = None,
             private_ip: Optional[pulumi.Input[str]] = None,
+            private_ipv4: Optional[pulumi.Input[str]] = None,
             public_ip: Optional[pulumi.Input[str]] = None,
             public_ip_required: Optional[pulumi.Input[str]] = None,
             ram_mb: Optional[pulumi.Input[int]] = None,
             region: Optional[pulumi.Input[str]] = None,
             reserved_ipv4: Optional[pulumi.Input[str]] = None,
             reverse_dns: Optional[pulumi.Input[str]] = None,
             script: Optional[pulumi.Input[str]] = None,
@@ -861,14 +898,15 @@
         :param pulumi.Input[str] firewall_id: The ID of the firewall to use, from the current list. If left blank or not sent, the default firewall will be used (open to all)
         :param pulumi.Input[str] hostname: A fully qualified domain name that should be set as the instance's hostname
         :param pulumi.Input[str] initial_password: Initial password for login
         :param pulumi.Input[str] initial_user: The name of the initial user created on the server (optional; this will default to the template's default_username and fallback to civo)
         :param pulumi.Input[str] network_id: This must be the ID of the network from the network listing (optional; default network used when not specified)
         :param pulumi.Input[str] notes: Add some notes to the instance
         :param pulumi.Input[str] private_ip: Instance's private IP address
+        :param pulumi.Input[str] private_ipv4: The private IPv4 address for the instance (optional)
         :param pulumi.Input[str] public_ip: Instance's public IP address
         :param pulumi.Input[str] public_ip_required: This should be either 'none' or 'create' (default: 'create')
         :param pulumi.Input[int] ram_mb: Instance's RAM (MB)
         :param pulumi.Input[str] region: The region for the instance, if not declare we use the region in declared in the provider
         :param pulumi.Input[str] reserved_ipv4: Can be either the UUID, name, or the IP address of the reserved IP
         :param pulumi.Input[str] reverse_dns: A fully qualified domain name that should be used as the instance's IP's reverse DNS (optional, uses the hostname if unspecified)
         :param pulumi.Input[str] script: The contents of a script that will be uploaded to /usr/local/bin/civo-user-init-script on your instance, read/write/executable only by root and then will be executed at the end of the cloud initialization
@@ -891,14 +929,15 @@
         __props__.__dict__["firewall_id"] = firewall_id
         __props__.__dict__["hostname"] = hostname
         __props__.__dict__["initial_password"] = initial_password
         __props__.__dict__["initial_user"] = initial_user
         __props__.__dict__["network_id"] = network_id
         __props__.__dict__["notes"] = notes
         __props__.__dict__["private_ip"] = private_ip
+        __props__.__dict__["private_ipv4"] = private_ipv4
         __props__.__dict__["public_ip"] = public_ip
         __props__.__dict__["public_ip_required"] = public_ip_required
         __props__.__dict__["ram_mb"] = ram_mb
         __props__.__dict__["region"] = region
         __props__.__dict__["reserved_ipv4"] = reserved_ipv4
         __props__.__dict__["reverse_dns"] = reverse_dns
         __props__.__dict__["script"] = script
@@ -996,14 +1035,22 @@
     def private_ip(self) -> pulumi.Output[str]:
         """
         Instance's private IP address
         """
         return pulumi.get(self, "private_ip")
 
     @property
+    @pulumi.getter(name="privateIpv4")
+    def private_ipv4(self) -> pulumi.Output[Optional[str]]:
+        """
+        The private IPv4 address for the instance (optional)
+        """
+        return pulumi.get(self, "private_ipv4")
+
+    @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> pulumi.Output[str]:
         """
         Instance's public IP address
         """
         return pulumi.get(self, "public_ip")
```

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/volume.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,373 +5,360 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['NetworkArgs', 'Network']
+__all__ = ['VolumeArgs', 'Volume']
 
 @pulumi.input_type
-class NetworkArgs:
+class VolumeArgs:
     def __init__(__self__, *,
-                 label: pulumi.Input[str],
-                 cidr_v4: Optional[pulumi.Input[str]] = None,
-                 nameservers_v4s: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 network_id: pulumi.Input[str],
+                 size_gb: pulumi.Input[int],
+                 name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Network resource.
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] cidr_v4: The CIDR block for the network
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nameservers_v4s: List of nameservers for the network
-        :param pulumi.Input[str] region: The region of the network
-        """
-        pulumi.set(__self__, "label", label)
-        if cidr_v4 is not None:
-            pulumi.set(__self__, "cidr_v4", cidr_v4)
-        if nameservers_v4s is not None:
-            pulumi.set(__self__, "nameservers_v4s", nameservers_v4s)
+        The set of arguments for constructing a Volume resource.
+        :param pulumi.Input[str] network_id: The network that the volume belongs to
+        :param pulumi.Input[int] size_gb: A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
+        :param pulumi.Input[str] name: A name that you wish to use to refer to this volume
+        :param pulumi.Input[str] region: The region for the volume, if not declare we use the region in declared in the provider.
+        """
+        pulumi.set(__self__, "network_id", network_id)
+        pulumi.set(__self__, "size_gb", size_gb)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if region is not None:
             pulumi.set(__self__, "region", region)
 
     @property
-    @pulumi.getter
-    def label(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Input[str]:
         """
-        Name for the network
+        The network that the volume belongs to
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "network_id")
 
-    @label.setter
-    def label(self, value: pulumi.Input[str]):
-        pulumi.set(self, "label", value)
+    @network_id.setter
+    def network_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network_id", value)
 
     @property
-    @pulumi.getter(name="cidrV4")
-    def cidr_v4(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="sizeGb")
+    def size_gb(self) -> pulumi.Input[int]:
         """
-        The CIDR block for the network
+        A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
         """
-        return pulumi.get(self, "cidr_v4")
+        return pulumi.get(self, "size_gb")
 
-    @cidr_v4.setter
-    def cidr_v4(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cidr_v4", value)
+    @size_gb.setter
+    def size_gb(self, value: pulumi.Input[int]):
+        pulumi.set(self, "size_gb", value)
 
     @property
-    @pulumi.getter(name="nameserversV4s")
-    def nameservers_v4s(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        List of nameservers for the network
+        A name that you wish to use to refer to this volume
         """
-        return pulumi.get(self, "nameservers_v4s")
+        return pulumi.get(self, "name")
 
-    @nameservers_v4s.setter
-    def nameservers_v4s(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "nameservers_v4s", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the network
+        The region for the volume, if not declare we use the region in declared in the provider.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
 
 @pulumi.input_type
-class _NetworkState:
+class _VolumeState:
     def __init__(__self__, *,
-                 cidr_v4: Optional[pulumi.Input[str]] = None,
-                 default: Optional[pulumi.Input[bool]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
+                 mount_point: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 nameservers_v4s: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 region: Optional[pulumi.Input[str]] = None):
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 region: Optional[pulumi.Input[str]] = None,
+                 size_gb: Optional[pulumi.Input[int]] = None):
+        """
+        Input properties used for looking up and filtering Volume resources.
+        :param pulumi.Input[str] mount_point: The mount point of the volume (from instance's perspective)
+        :param pulumi.Input[str] name: A name that you wish to use to refer to this volume
+        :param pulumi.Input[str] network_id: The network that the volume belongs to
+        :param pulumi.Input[str] region: The region for the volume, if not declare we use the region in declared in the provider.
+        :param pulumi.Input[int] size_gb: A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
         """
-        Input properties used for looking up and filtering Network resources.
-        :param pulumi.Input[str] cidr_v4: The CIDR block for the network
-        :param pulumi.Input[bool] default: If the network is default, this will be `true`
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] name: The name of the network
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nameservers_v4s: List of nameservers for the network
-        :param pulumi.Input[str] region: The region of the network
-        """
-        if cidr_v4 is not None:
-            pulumi.set(__self__, "cidr_v4", cidr_v4)
-        if default is not None:
-            pulumi.set(__self__, "default", default)
-        if label is not None:
-            pulumi.set(__self__, "label", label)
+        if mount_point is not None:
+            pulumi.set(__self__, "mount_point", mount_point)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if nameservers_v4s is not None:
-            pulumi.set(__self__, "nameservers_v4s", nameservers_v4s)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
         if region is not None:
             pulumi.set(__self__, "region", region)
+        if size_gb is not None:
+            pulumi.set(__self__, "size_gb", size_gb)
 
     @property
-    @pulumi.getter(name="cidrV4")
-    def cidr_v4(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="mountPoint")
+    def mount_point(self) -> Optional[pulumi.Input[str]]:
         """
-        The CIDR block for the network
+        The mount point of the volume (from instance's perspective)
         """
-        return pulumi.get(self, "cidr_v4")
+        return pulumi.get(self, "mount_point")
 
-    @cidr_v4.setter
-    def cidr_v4(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cidr_v4", value)
-
-    @property
-    @pulumi.getter
-    def default(self) -> Optional[pulumi.Input[bool]]:
-        """
-        If the network is default, this will be `true`
-        """
-        return pulumi.get(self, "default")
-
-    @default.setter
-    def default(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "default", value)
-
-    @property
-    @pulumi.getter
-    def label(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name for the network
-        """
-        return pulumi.get(self, "label")
-
-    @label.setter
-    def label(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "label", value)
+    @mount_point.setter
+    def mount_point(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "mount_point", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the network
+        A name that you wish to use to refer to this volume
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="nameserversV4s")
-    def nameservers_v4s(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[pulumi.Input[str]]:
         """
-        List of nameservers for the network
+        The network that the volume belongs to
         """
-        return pulumi.get(self, "nameservers_v4s")
+        return pulumi.get(self, "network_id")
 
-    @nameservers_v4s.setter
-    def nameservers_v4s(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "nameservers_v4s", value)
+    @network_id.setter
+    def network_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_id", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
-        The region of the network
+        The region for the volume, if not declare we use the region in declared in the provider.
         """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
+    @property
+    @pulumi.getter(name="sizeGb")
+    def size_gb(self) -> Optional[pulumi.Input[int]]:
+        """
+        A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
+        """
+        return pulumi.get(self, "size_gb")
 
-class Network(pulumi.CustomResource):
+    @size_gb.setter
+    def size_gb(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size_gb", value)
+
+
+class Volume(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cidr_v4: Optional[pulumi.Input[str]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
-                 nameservers_v4s: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 size_gb: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Provides a Civo network resource. This can be used to create, modify, and delete networks.
+        Provides a Civo volume which can be attached to an instance in order to provide expanded storage.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        custom_net = civo.Network("custom_net", label="test_network")
+        # Get network
+        default_network = civo.get_network(label="Default")
+        # Create volume
+        db = civo.Volume("db",
+            name="backup-data",
+            size_gb=5,
+            network_id=default_network.id,
+            opts=pulumi.ResourceOptions(depends_on=[default_network]))
         ```
 
         ## Import
 
         using ID
 
         ```sh
-        $ pulumi import civo:index/network:Network custom_net b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
+        $ pulumi import civo:index/volume:Volume db 506f78a4-e098-11e5-ad9f-000f53306ae1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr_v4: The CIDR block for the network
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nameservers_v4s: List of nameservers for the network
-        :param pulumi.Input[str] region: The region of the network
+        :param pulumi.Input[str] name: A name that you wish to use to refer to this volume
+        :param pulumi.Input[str] network_id: The network that the volume belongs to
+        :param pulumi.Input[str] region: The region for the volume, if not declare we use the region in declared in the provider.
+        :param pulumi.Input[int] size_gb: A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NetworkArgs,
+                 args: VolumeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Civo network resource. This can be used to create, modify, and delete networks.
+        Provides a Civo volume which can be attached to an instance in order to provide expanded storage.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        custom_net = civo.Network("custom_net", label="test_network")
+        # Get network
+        default_network = civo.get_network(label="Default")
+        # Create volume
+        db = civo.Volume("db",
+            name="backup-data",
+            size_gb=5,
+            network_id=default_network.id,
+            opts=pulumi.ResourceOptions(depends_on=[default_network]))
         ```
 
         ## Import
 
         using ID
 
         ```sh
-        $ pulumi import civo:index/network:Network custom_net b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
+        $ pulumi import civo:index/volume:Volume db 506f78a4-e098-11e5-ad9f-000f53306ae1
         ```
 
         :param str resource_name: The name of the resource.
-        :param NetworkArgs args: The arguments to use to populate this resource's properties.
+        :param VolumeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NetworkArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VolumeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cidr_v4: Optional[pulumi.Input[str]] = None,
-                 label: Optional[pulumi.Input[str]] = None,
-                 nameservers_v4s: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
+                 size_gb: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NetworkArgs.__new__(NetworkArgs)
+            __props__ = VolumeArgs.__new__(VolumeArgs)
 
-            __props__.__dict__["cidr_v4"] = cidr_v4
-            if label is None and not opts.urn:
-                raise TypeError("Missing required property 'label'")
-            __props__.__dict__["label"] = label
-            __props__.__dict__["nameservers_v4s"] = nameservers_v4s
+            __props__.__dict__["name"] = name
+            if network_id is None and not opts.urn:
+                raise TypeError("Missing required property 'network_id'")
+            __props__.__dict__["network_id"] = network_id
             __props__.__dict__["region"] = region
-            __props__.__dict__["default"] = None
-            __props__.__dict__["name"] = None
-        super(Network, __self__).__init__(
-            'civo:index/network:Network',
+            if size_gb is None and not opts.urn:
+                raise TypeError("Missing required property 'size_gb'")
+            __props__.__dict__["size_gb"] = size_gb
+            __props__.__dict__["mount_point"] = None
+        super(Volume, __self__).__init__(
+            'civo:index/volume:Volume',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            cidr_v4: Optional[pulumi.Input[str]] = None,
-            default: Optional[pulumi.Input[bool]] = None,
-            label: Optional[pulumi.Input[str]] = None,
+            mount_point: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
-            nameservers_v4s: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            region: Optional[pulumi.Input[str]] = None) -> 'Network':
+            network_id: Optional[pulumi.Input[str]] = None,
+            region: Optional[pulumi.Input[str]] = None,
+            size_gb: Optional[pulumi.Input[int]] = None) -> 'Volume':
         """
-        Get an existing Network resource's state with the given name, id, and optional extra
+        Get an existing Volume resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr_v4: The CIDR block for the network
-        :param pulumi.Input[bool] default: If the network is default, this will be `true`
-        :param pulumi.Input[str] label: Name for the network
-        :param pulumi.Input[str] name: The name of the network
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] nameservers_v4s: List of nameservers for the network
-        :param pulumi.Input[str] region: The region of the network
+        :param pulumi.Input[str] mount_point: The mount point of the volume (from instance's perspective)
+        :param pulumi.Input[str] name: A name that you wish to use to refer to this volume
+        :param pulumi.Input[str] network_id: The network that the volume belongs to
+        :param pulumi.Input[str] region: The region for the volume, if not declare we use the region in declared in the provider.
+        :param pulumi.Input[int] size_gb: A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _NetworkState.__new__(_NetworkState)
+        __props__ = _VolumeState.__new__(_VolumeState)
 
-        __props__.__dict__["cidr_v4"] = cidr_v4
-        __props__.__dict__["default"] = default
-        __props__.__dict__["label"] = label
+        __props__.__dict__["mount_point"] = mount_point
         __props__.__dict__["name"] = name
-        __props__.__dict__["nameservers_v4s"] = nameservers_v4s
+        __props__.__dict__["network_id"] = network_id
         __props__.__dict__["region"] = region
-        return Network(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["size_gb"] = size_gb
+        return Volume(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="cidrV4")
-    def cidr_v4(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="mountPoint")
+    def mount_point(self) -> pulumi.Output[str]:
         """
-        The CIDR block for the network
+        The mount point of the volume (from instance's perspective)
         """
-        return pulumi.get(self, "cidr_v4")
+        return pulumi.get(self, "mount_point")
 
     @property
     @pulumi.getter
-    def default(self) -> pulumi.Output[bool]:
+    def name(self) -> pulumi.Output[str]:
         """
-        If the network is default, this will be `true`
+        A name that you wish to use to refer to this volume
         """
-        return pulumi.get(self, "default")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def label(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Output[str]:
         """
-        Name for the network
+        The network that the volume belongs to
         """
-        return pulumi.get(self, "label")
+        return pulumi.get(self, "network_id")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def region(self) -> pulumi.Output[Optional[str]]:
         """
-        The name of the network
+        The region for the volume, if not declare we use the region in declared in the provider.
         """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="nameserversV4s")
-    def nameservers_v4s(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        List of nameservers for the network
-        """
-        return pulumi.get(self, "nameservers_v4s")
+        return pulumi.get(self, "region")
 
     @property
-    @pulumi.getter
-    def region(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="sizeGb")
+    def size_gb(self) -> pulumi.Output[int]:
         """
-        The region of the network
+        A minimum of 1 and a maximum of your available disk space from your quota specifies the size of the volume in gigabytes
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "size_gb")
```

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1715356631/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1715335912
+Version: 2.4.0a1715356631
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1715335912/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1715356631/pulumi_civo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1715335912/pyproject.toml` & `pulumi_civo-2.4.0a1715356631/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_civo"
   description = "A Pulumi package for creating and managing Civo cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "civo"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1715335912"
+  version = "2.4.0a1715356631"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-civo"
 
 [build-system]
```

