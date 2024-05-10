# Comparing `tmp/alas_ce0_client-5.0.82.tar.gz` & `tmp/alas_ce0_client-5.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alas_ce0_client-5.0.82.tar", last modified: Wed Apr 24 21:51:10 2024, max compression
+gzip compressed data, was "alas_ce0_client-5.0.83.tar", last modified: Wed May  8 14:47:19 2024, max compression
```

## Comparing `alas_ce0_client-5.0.82.tar` & `alas_ce0_client-5.0.83.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.733881 alas_ce0_client-5.0.82/
--rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/LICENSE.txt
--rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/MANIFEST.in
--rw-r--r--   0 lzambra    (501) staff       (20)      976 2024-04-24 21:51:10.733707 alas_ce0_client-5.0.82/PKG-INFO
--rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/README.rst
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.635870 alas_ce0_client-5.0.82/alas_ce0/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.638647 alas_ce0_client-5.0.82/alas_ce0/clients/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/clients/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)     6256 2024-04-24 15:18:04.000000 alas_ce0_client-5.0.82/alas_ce0/clients/api_client.py
--rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/clients/core.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.640607 alas_ce0_client-5.0.82/alas_ce0/common/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/common/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)    11080 2024-04-24 21:49:03.000000 alas_ce0_client-5.0.82/alas_ce0/common/client_base.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.644980 alas_ce0_client-5.0.82/alas_ce0/delivery/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/delivery/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/delivery/b2c.py
--rw-r--r--   0 lzambra    (501) staff       (20)    51663 2024-04-24 15:18:04.000000 alas_ce0_client-5.0.82/alas_ce0/delivery/delivery_order.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.650037 alas_ce0_client-5.0.82/alas_ce0/integration/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/integration/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/integration/device_magic.py
--rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/integration/shipper.py
--rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/integration/whatsapp.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.719347 alas_ce0_client-5.0.82/alas_ce0/management/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/barcode.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1511 2024-02-12 13:05:56.000000 alas_ce0_client-5.0.82/alas_ce0/management/bulk.py
--rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/configuration.py
--rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/contact.py
--rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/cross_docking.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/delivery_entity.py
--rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/distribution_zone.py
--rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/employee.py
--rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/feature.py
--rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas_ce0_client-5.0.82/alas_ce0/management/geographic_coverage.py
--rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/geographic_coverage_active.py
--rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/maintenance.py
--rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/notification.py
--rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/package_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/packaging.py
--rw-r--r--   0 lzambra    (501) staff       (20)      732 2024-02-12 13:05:56.000000 alas_ce0_client-5.0.82/alas_ce0/management/pallet.py
--rw-r--r--   0 lzambra    (501) staff       (20)      155 2024-02-12 13:10:27.000000 alas_ce0_client-5.0.82/alas_ce0/management/position.py
--rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/product_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/resource.py
--rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/role.py
--rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/roles_group.py
--rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/service_level.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/shelf.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/task.py
--rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/user.py
--rw-r--r--   0 lzambra    (501) staff       (20)      591 2024-02-12 13:05:56.000000 alas_ce0_client-5.0.82/alas_ce0/management/user_app.py
--rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/management/vehicle.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.723488 alas_ce0_client-5.0.82/alas_ce0/reporting/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/reporting/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/reporting/regional_partner_report.py
--rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/reporting/report.py
--rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/reporting/report_manager.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.725835 alas_ce0_client-5.0.82/alas_ce0/scheduling/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/scheduling/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/scheduling/route.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.730202 alas_ce0_client-5.0.82/alas_ce0/task/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/task/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.82/alas_ce0/task/data_job.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-24 21:51:10.732876 alas_ce0_client-5.0.82/alas_ce0_client.egg-info/
--rw-r--r--   0 lzambra    (501) staff       (20)      976 2024-04-24 21:51:10.000000 alas_ce0_client-5.0.82/alas_ce0_client.egg-info/PKG-INFO
--rw-r--r--   0 lzambra    (501) staff       (20)     1852 2024-04-24 21:51:10.000000 alas_ce0_client-5.0.82/alas_ce0_client.egg-info/SOURCES.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        1 2024-04-24 21:51:10.000000 alas_ce0_client-5.0.82/alas_ce0_client.egg-info/dependency_links.txt
--rw-r--r--   0 lzambra    (501) staff       (20)       55 2024-04-24 21:51:10.000000 alas_ce0_client-5.0.82/alas_ce0_client.egg-info/requires.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        9 2024-04-24 21:51:10.000000 alas_ce0_client-5.0.82/alas_ce0_client.egg-info/top_level.txt
--rw-r--r--   0 lzambra    (501) staff       (20)       67 2024-04-24 21:51:10.734557 alas_ce0_client-5.0.82/setup.cfg
--rw-r--r--   0 lzambra    (501) staff       (20)     3825 2024-04-24 21:50:21.000000 alas_ce0_client-5.0.82/setup.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.432904 alas_ce0_client-5.0.83/
+-rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/LICENSE.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/MANIFEST.in
+-rw-r--r--   0 lzambra    (501) staff       (20)      976 2024-05-08 14:47:19.432719 alas_ce0_client-5.0.83/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/README.rst
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.389610 alas_ce0_client-5.0.83/alas_ce0/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.391569 alas_ce0_client-5.0.83/alas_ce0/clients/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/clients/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     6256 2024-05-08 14:09:48.000000 alas_ce0_client-5.0.83/alas_ce0/clients/api_client.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/clients/core.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.392392 alas_ce0_client-5.0.83/alas_ce0/common/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/common/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    11080 2024-05-08 14:09:48.000000 alas_ce0_client-5.0.83/alas_ce0/common/client_base.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.393993 alas_ce0_client-5.0.83/alas_ce0/delivery/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/delivery/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/delivery/b2c.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    51931 2024-05-08 14:21:07.000000 alas_ce0_client-5.0.83/alas_ce0/delivery/delivery_order.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.397180 alas_ce0_client-5.0.83/alas_ce0/integration/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/integration/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/integration/device_magic.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/integration/shipper.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/integration/whatsapp.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.418351 alas_ce0_client-5.0.83/alas_ce0/management/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/barcode.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1511 2024-02-12 13:05:56.000000 alas_ce0_client-5.0.83/alas_ce0/management/bulk.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/configuration.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/contact.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/cross_docking.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/delivery_entity.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/distribution_zone.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/employee.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/feature.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas_ce0_client-5.0.83/alas_ce0/management/geographic_coverage.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/geographic_coverage_active.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/maintenance.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/notification.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/package_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/packaging.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      732 2024-02-12 13:05:56.000000 alas_ce0_client-5.0.83/alas_ce0/management/pallet.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2024-02-12 13:10:27.000000 alas_ce0_client-5.0.83/alas_ce0/management/position.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/product_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/resource.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/role.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/roles_group.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/service_level.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/shelf.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/task.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/user.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      591 2024-02-12 13:05:56.000000 alas_ce0_client-5.0.83/alas_ce0/management/user_app.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/management/vehicle.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.420705 alas_ce0_client-5.0.83/alas_ce0/reporting/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/reporting/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/reporting/regional_partner_report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/reporting/report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/reporting/report_manager.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.422050 alas_ce0_client-5.0.83/alas_ce0/scheduling/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/scheduling/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/scheduling/route.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.428860 alas_ce0_client-5.0.83/alas_ce0/task/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/task/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas_ce0_client-5.0.83/alas_ce0/task/data_job.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-05-08 14:47:19.431795 alas_ce0_client-5.0.83/alas_ce0_client.egg-info/
+-rw-r--r--   0 lzambra    (501) staff       (20)      976 2024-05-08 14:47:19.000000 alas_ce0_client-5.0.83/alas_ce0_client.egg-info/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)     1852 2024-05-08 14:47:19.000000 alas_ce0_client-5.0.83/alas_ce0_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        1 2024-05-08 14:47:19.000000 alas_ce0_client-5.0.83/alas_ce0_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       55 2024-05-08 14:47:19.000000 alas_ce0_client-5.0.83/alas_ce0_client.egg-info/requires.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        9 2024-05-08 14:47:19.000000 alas_ce0_client-5.0.83/alas_ce0_client.egg-info/top_level.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       67 2024-05-08 14:47:19.433432 alas_ce0_client-5.0.83/setup.cfg
+-rw-r--r--   0 lzambra    (501) staff       (20)     3825 2024-05-08 14:21:55.000000 alas_ce0_client-5.0.83/setup.py
```

### Comparing `alas_ce0_client-5.0.82/PKG-INFO` & `alas_ce0_client-5.0.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alas-ce0-client
-Version: 5.0.82
+Version: 5.0.83
 Summary: API client for Alas.Ce0 project
 Home-page: https://github.com/pypa/alas-ce0-client
 Author: Leonardo Zambra
 Author-email: lzambra@alasxpress.com
 License: MIT
 Keywords: alas-ce0 api client development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `alas_ce0_client-5.0.82/alas_ce0/clients/api_client.py` & `alas_ce0_client-5.0.83/alas_ce0/clients/api_client.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/clients/core.py` & `alas_ce0_client-5.0.83/alas_ce0/clients/core.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/common/client_base.py` & `alas_ce0_client-5.0.83/alas_ce0/common/client_base.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/delivery/delivery_order.py` & `alas_ce0_client-5.0.83/alas_ce0/delivery/delivery_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,21 @@
         DeliveryOrderStatusType.VirtuallyReceived.value,
     ],
     DeliveryOrderStatusType.VirtuallyReceived.value: [
         DeliveryOrderStatusType.PhysicallyReceived.value,
         #DeliveryOrderStatusType.B2BReceptionRejected.value, #rechazado b2b
         DeliveryOrderStatusType.DeliveryRejected.value, #entrega rechazada
     ],
+
+    DeliveryOrderStatusType.Packaging.value: [
+        DeliveryOrderStatusType.PhysicallyReceived.value,
+        # DeliveryOrderStatusType.B2BReceptionRejected.value, #rechazado b2b
+        DeliveryOrderStatusType.DeliveryRejected.value,  # entrega rechazada
+    ],
+
     DeliveryOrderStatusType.PhysicallyReceived.value: [
         DeliveryOrderStatusType.DistributionCenterReceived.value,
         DeliveryOrderStatusType.DeliveryRejected.value, #entrega rechazada
     ],
     DeliveryOrderStatusType.DistributionCenterReceived.value: [
         DeliveryOrderStatusType.DeliveryCourierPreAssigned.value,
         DeliveryOrderStatusType.SERTravelling.value,
```

### Comparing `alas_ce0_client-5.0.82/alas_ce0/integration/device_magic.py` & `alas_ce0_client-5.0.83/alas_ce0/integration/device_magic.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/barcode.py` & `alas_ce0_client-5.0.83/alas_ce0/management/barcode.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/bulk.py` & `alas_ce0_client-5.0.83/alas_ce0/management/bulk.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/configuration.py` & `alas_ce0_client-5.0.83/alas_ce0/management/configuration.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/delivery_entity.py` & `alas_ce0_client-5.0.83/alas_ce0/management/delivery_entity.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/employee.py` & `alas_ce0_client-5.0.83/alas_ce0/management/employee.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/notification.py` & `alas_ce0_client-5.0.83/alas_ce0/management/notification.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/pallet.py` & `alas_ce0_client-5.0.83/alas_ce0/management/pallet.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/user.py` & `alas_ce0_client-5.0.83/alas_ce0/management/user.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/management/user_app.py` & `alas_ce0_client-5.0.83/alas_ce0/management/user_app.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0/scheduling/route.py` & `alas_ce0_client-5.0.83/alas_ce0/scheduling/route.py`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/alas_ce0_client.egg-info/PKG-INFO` & `alas_ce0_client-5.0.83/alas_ce0_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alas-ce0-client
-Version: 5.0.82
+Version: 5.0.83
 Summary: API client for Alas.Ce0 project
 Home-page: https://github.com/pypa/alas-ce0-client
 Author: Leonardo Zambra
 Author-email: lzambra@alasxpress.com
 License: MIT
 Keywords: alas-ce0 api client development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `alas_ce0_client-5.0.82/alas_ce0_client.egg-info/SOURCES.txt` & `alas_ce0_client-5.0.83/alas_ce0_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alas_ce0_client-5.0.82/setup.py` & `alas_ce0_client-5.0.83/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
-API_CLIENT_VERSION = '5.0.82'
+API_CLIENT_VERSION = '5.0.83'
 
 setup(
     name='alas-ce0-client',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
```

