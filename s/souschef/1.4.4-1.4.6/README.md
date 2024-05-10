# Comparing `tmp/souschef-1.4.4.tar.gz` & `tmp/souschef-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/souschef-1.4.4.tar", last modified: Fri May  3 15:49:59 2024, max compression
+gzip compressed data, was "dist/souschef-1.4.6.tar", last modified: Fri May 10 16:11:31 2024, max compression
```

## Comparing `souschef-1.4.4.tar` & `souschef-1.4.6.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/
--rw-r--r--   0 root         (0) root         (0)     5731 2024-02-17 22:37:08.000000 souschef-1.4.4/INSTALL.md
--rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.4.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2261 2024-05-03 15:49:59.000000 souschef-1.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.4.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.4.4/UPDATE.md
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-18 19:41:03.000000 souschef-1.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-03 15:49:59.000000 souschef-1.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1812 2024-05-03 15:48:16.000000 souschef-1.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/
--rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/admin.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/billing/apps.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/billing/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/migrations/
--rw-r--r--   0 root         (0) root         (0)     1201 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0002_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      370 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0003_auto_20161122_0515.py
--rw-r--r--   0 root         (0) root         (0)      374 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0004_auto_20201030_1540.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5211 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/templates/
--rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/base_billing.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/templates/billing/
--rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/add.html
--rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/billing_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/templates/billing/partials/
--rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/partials/statistics.html
--rw-r--r--   0 root         (0) root         (0)     5508 2021-07-16 15:48:25.000000 souschef-1.4.4/souschef/billing/templates/billing/partials/summary.html
--rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/print_summary.html
--rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/view.html
--rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.4.4/souschef/billing/templates/billing/view_orders.html
--rw-r--r--   0 root         (0) root         (0)     8556 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/tests.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/billing/urls.py
--rw-r--r--   0 root         (0) root         (0)    12279 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/configsamples/
--rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.4.4/souschef/configsamples/nginx.conf
--rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.4.4/souschef/configsamples/souschef.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/cronscripts/
--rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.4.4/souschef/cronscripts/souschef_daily.sh
--rw-r--r--   0 root         (0) root         (0)      350 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/dataexec.py
--rw-r--r--   0 root         (0) root         (0)    76889 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/dataload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/datamigration/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/admin.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.4.4/souschef/datamigration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.4.4/souschef/datamigration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2026 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importaddresses.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importclients.py
--rw-r--r--   0 root         (0) root         (0)     2890 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importcontactaddresses.py
--rw-r--r--   0 root         (0) root         (0)     4190 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importmeals.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importorders.py
--rw-r--r--   0 root         (0) root         (0)     3299 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importrelationships.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/datamigration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/models.py
--rw-r--r--   0 root         (0) root         (0)     6860 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/datamigration/tests.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/delivery/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/delivery/admin.py
--rwxr-xr-x   0 root         (0) root         (0)       91 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/delivery/apps.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/delivery/filters.py
--rw-r--r--   0 root         (0) root         (0)     1426 2024-02-17 22:36:40.000000 souschef-1.4.4/souschef/delivery/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/migrations/
--rw-r--r--   0 root         (0) root         (0)      690 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/delivery/migrations/0001_fix004a.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/delivery/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      232 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/delivery/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/templates/
--rw-r--r--   0 root         (0) root         (0)    12210 2024-02-19 02:15:16.000000 souschef-1.4.4/souschef/delivery/templates/edit_delivery_route.html
--rw-r--r--   0 root         (0) root         (0)     3686 2024-03-06 02:24:13.000000 souschef-1.4.4/souschef/delivery/templates/ingredients.html
--rw-r--r--   0 root         (0) root         (0)     4380 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/delivery/templates/kitchen_count.html
--rw-r--r--   0 root         (0) root         (0)     1360 2024-03-06 02:24:13.000000 souschef-1.4.4/souschef/delivery/templates/kitchen_count_steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/templates/partials/
--rw-r--r--   0 root         (0) root         (0)     2648 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/templates/partials/generated_orders.html
--rw-r--r--   0 root         (0) root         (0)     1777 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_order_row_content.html
--rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_table_head.html
--rw-r--r--   0 root         (0) root         (0)     5472 2024-03-06 02:24:13.000000 souschef-1.4.4/souschef/delivery/templates/review_orders.html
--rw-r--r--   0 root         (0) root         (0)     3407 2024-02-19 02:15:16.000000 souschef-1.4.4/souschef/delivery/templates/route_sheet.html
--rw-r--r--   0 root         (0) root         (0)     5284 2024-04-09 15:26:23.000000 souschef-1.4.4/souschef/delivery/templates/routes.html
--rwxr-xr-x   0 root         (0) root         (0)    53737 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/tests.py
--rw-r--r--   0 root         (0) root         (0)     2877 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/delivery/tsp.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-09 15:26:23.000000 souschef-1.4.4/souschef/delivery/urls.py
--rwxr-xr-x   0 root         (0) root         (0)    80975 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/frontend/images/
--rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/katrina.jpg
--rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/meal/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/meal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-01 00:23:07.000000 souschef-1.4.4/souschef/meal/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/apps.py
--rw-r--r--   0 root         (0) root         (0)     2269 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/meal/migrations/
--rw-r--r--   0 root         (0) root         (0)     7348 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0002_ingredient_ingredient_group.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0003_fix224a.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0004_fix004d.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0006_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0007_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0008_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/meal/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8100 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/meal/models.py
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/settings.py
--rw-r--r--   0 root         (0) root         (0)     8761 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/tests.py
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/urls.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/admin.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/apps.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/factories.py
--rw-r--r--   0 root         (0) root         (0)    20424 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/member/forms.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/formsets.py
--rw-r--r--   0 root         (0) root         (0)      964 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/formsfield.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.4.4/souschef/member/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.4.4/souschef/member/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/management/commands/createclients.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/management/commands/createnotes.py
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/member/management/commands/processscheduledstatuschange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/migrations/
--rw-r--r--   0 root         (0) root         (0)    15890 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0002_auto_20160605_1609.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0003_auto_20160615_2100.py
--rw-r--r--   0 root         (0) root         (0)     4445 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0005_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0006_client_meal_default_week.py
--rw-r--r--   0 root         (0) root         (0)      908 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0007_auto_20160726_1703.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0008_auto_20160727_2251.py
--rw-r--r--   0 root         (0) root         (0)      918 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0009_auto_20160728_1443.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0010_auto_20160803_2052.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0011_client_delivery_note.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0012_clientscheduledstatus.py
--rw-r--r--   0 root         (0) root         (0)      754 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0013_auto_20160820_2322.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0014_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0015_route_client_id_sequence.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0016_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0017_auto_20161020_2039.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0018_auto_20161110_2352.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0019_auto_20161111_1750.py
--rw-r--r--   0 root         (0) root         (0)      438 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0020_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0021_auto_20161125_2055.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0022_auto_20161215_1936.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0023_auto_20161220_1401.py
--rw-r--r--   0 root         (0) root         (0)     2680 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0024_auto_20161227_1819.py
--rw-r--r--   0 root         (0) root         (0)      672 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0025_route_vehicle.py
--rw-r--r--   0 root         (0) root         (0)     3723 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0026_change_to_emergency_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1372 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0027_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)     1904 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/member/migrations/0029_member_address_fk_to_1to1.py
--rw-r--r--   0 root         (0) root         (0)     2584 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0030_route_deliveryhistory.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0032_relationship.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0033_auto_20170801_1607.py
--rw-r--r--   0 root         (0) root         (0)      554 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0034_auto_20170816_0850.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0035_auto_20210115_1155.py
--rw-r--r--   0 root         (0) root         (0)     1449 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0036_member_addresses.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0037_one_address_per_member.py
--rw-r--r--   0 root         (0) root         (0)      601 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0038_member_verbose_names.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29870 2024-05-03 15:39:44.000000 souschef-1.4.4/souschef/member/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/signals/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/signals/__init__.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/signals/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/
--rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/create/
--rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/create/form.html
--rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/create/steps.html
--rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/partials/
--rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/birthdays.html
--rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/filters.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/
--rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/address_information.html
--rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/basic_information.html
--rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/dietary_restriction.html
--rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/meal_defaults.html
--rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/payment_information.html
--rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/relationship_form.html
--rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/relationships.html
--rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/menu.html
--rw-r--r--   0 root         (0) root         (0)     2017 2021-06-18 20:11:28.000000 souschef-1.4.4/souschef/member/templates/client/partials/order_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/update/
--rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.4.4/souschef/member/templates/client/update/base.html
--rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.4.4/souschef/member/templates/client/update/status.html
--rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/update/step.html
--rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/update/steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/view/
--rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/address.html
--rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/allergies.html
--rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/delete_status_confirmation.html
--rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/information.html
--rw-r--r--   0 root         (0) root         (0)     2716 2021-06-11 15:40:13.000000 souschef-1.4.4/souschef/member/templates/client/view/notes.html
--rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.4.4/souschef/member/templates/client/view/orders.html
--rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/payment.html
--rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/referent.html
--rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/status.html
--rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/route/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/delivered_route_detail.html
--rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/delivery_history_detail.html
--rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/detail.html
--rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/edit.html
--rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/list.html
--rw-r--r--   0 root         (0) root         (0)   165842 2024-05-03 15:46:57.000000 souschef-1.4.4/souschef/member/tests.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/urls.py
--rw-r--r--   0 root         (0) root         (0)    54776 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/member/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/note/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/note/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/note/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/note/apps.py
--rw-r--r--   0 root         (0) root         (0)      775 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/factories.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/note/migrations/
--rw-r--r--   0 root         (0) root         (0)     2230 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      607 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0002_auto_20160818_2104.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0003_auto_20160819_2037.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0004_notepriority.py
--rw-r--r--   0 root         (0) root         (0)     1286 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0005_note_priority_old_data_migration.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0006_change_priority_field.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0007_notecategory.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0008_auto_20170116_1441.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0009_auto_20170116_1543.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0010_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      987 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0011_auto_20170419_1109.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0012_note_is_deleted.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0013_date_modified.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0014_date_created.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/note/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/note/templates/
--rw-r--r--   0 root         (0) root         (0)      909 2021-07-09 19:21:52.000000 souschef-1.4.4/souschef/note/templates/note_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     1720 2021-07-09 19:00:25.000000 souschef-1.4.4/souschef/note/templates/note_edit.html
--rw-r--r--   0 root         (0) root         (0)     2186 2021-07-09 19:00:30.000000 souschef-1.4.4/souschef/note/templates/notes_add.html
--rw-r--r--   0 root         (0) root         (0)     4080 2021-06-11 15:41:01.000000 souschef-1.4.4/souschef/note/templates/notes_client_list.html
--rw-r--r--   0 root         (0) root         (0)     5780 2021-07-23 15:17:48.000000 souschef-1.4.4/souschef/note/templates/notes_list.html
--rw-r--r--   0 root         (0) root         (0)     9225 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/tests.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/note/urls.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/admin.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/notification/migrations/
--rw-r--r--   0 root         (0) root         (0)     1247 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/notification/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/notification/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2024-02-11 21:15:42.000000 souschef-1.4.4/souschef/notification/models.py
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/tests.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/urls.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/order/admin.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/order/apps.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/factories.py
--rw-r--r--   0 root         (0) root         (0)     5183 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.4.4/souschef/order/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.4.4/souschef/order/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/management/commands/createorders.py
--rw-r--r--   0 root         (0) root         (0)     1869 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/management/commands/generateorders.py
--rw-r--r--   0 root         (0) root         (0)     1330 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/management/commands/setordersdelivered.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/migrations/
--rw-r--r--   0 root         (0) root         (0)     4735 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      581 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0002_auto_20160614_1736.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0003_auto_20160615_1504.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      681 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0006_auto_20160803_2217.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0007_remove_order_item_component.py
--rw-r--r--   0 root         (0) root         (0)      633 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0008_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0009_auto_20161012_1919.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0010_auto_20161012_1921.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0011_auto_20161014_1901.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0012_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)     2226 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0013_orderstatuschange.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0014_auto_20161209_2045.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0015_auto_20170410_1029.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0016_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0017_total_quantity_not_nullable.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1268 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/mixins.py
--rw-r--r--   0 root         (0) root         (0)    47013 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/order/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/templates/
--rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/_form.html
--rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/_order_info.html
--rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/base_order.html
--rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/create.html
--rw-r--r--   0 root         (0) root         (0)     4481 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/order/templates/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/templates/order/
--rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/order/create_batch.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/templates/order/partials/
--rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/order/partials/filters.html
--rw-r--r--   0 root         (0) root         (0)     1070 2021-07-09 19:21:52.000000 souschef-1.4.4/souschef/order/templates/order_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.4.4/souschef/order/templates/order_update_status.html
--rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.4.4/souschef/order/templates/update.html
--rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.4.4/souschef/order/templates/view.html
--rw-r--r--   0 root         (0) root         (0)    66186 2024-02-24 23:48:36.000000 souschef-1.4.4/souschef/order/tests.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/order/urls.py
--rw-r--r--   0 root         (0) root         (0)    14652 2024-02-19 02:15:16.000000 souschef-1.4.4/souschef/order/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/page/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/page/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/page/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/templates/pages/
--rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/templates/pages/card.html
--rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/templates/pages/home.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/templates/registration/
--rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/templates/registration/login.html
--rw-r--r--   0 root         (0) root         (0)    10143 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/page/tests.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/page/urls.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/page/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/pycrons/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.4.4/souschef/pycrons/__init__.py
--rw-r--r--   0 root         (0) root         (0)      461 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/pycrons/cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/css/
--rw-r--r--   0 root         (0) root         (0)   655527 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/css/main.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/
--rw-r--r--   0 root         (0) root         (0)    98640 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.eot
--rw-r--r--   0 root         (0) root         (0)   507628 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.svg
--rw-r--r--   0 root         (0) root         (0)    98404 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    63728 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff
--rw-r--r--   0 root         (0) root         (0)    54488 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff2
--rw-r--r--   0 root         (0) root         (0)   106004 2024-05-03 15:49:33.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.eot
--rw-r--r--   0 root         (0) root         (0)    93888 2024-05-03 15:49:33.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.otf
--rw-r--r--   0 root         (0) root         (0)   390837 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.svg
--rw-r--r--   0 root         (0) root         (0)   105784 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.ttf
--rw-r--r--   0 root         (0) root         (0)    50524 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff
--rw-r--r--   0 root         (0) root         (0)    40148 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff2
--rw-r--r--   0 root         (0) root         (0)    31156 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.eot
--rw-r--r--   0 root         (0) root         (0)   107201 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.svg
--rw-r--r--   0 root         (0) root         (0)    30928 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    14712 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff
--rw-r--r--   0 root         (0) root         (0)    12240 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/images/
--rw-r--r--   0 root         (0) root         (0)   258972 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    11449 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/demo.png
--rw-r--r--   0 root         (0) root         (0)      608 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/favicon.png
--rw-r--r--   0 root         (0) root         (0)    28123 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/images/flags.png
--rw-r--r--   0 root         (0) root         (0)      490 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/images/geocoder.png
--rw-r--r--   0 root         (0) root         (0)     1374 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.png
--rw-r--r--   0 root         (0) root         (0)     1287 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.svg
--rw-r--r--   0 root         (0) root         (0)    21977 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    26952 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/katrina.jpg
--rw-r--r--   0 root         (0) root         (0)     2306 2024-05-03 15:49:36.000000 souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.png
--rw-r--r--   0 root         (0) root         (0)     4060 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
--rw-r--r--   0 root         (0) root         (0)     6363 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-coul.png
--rw-r--r--   0 root         (0) root         (0)     6033 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-nb.png
--rw-r--r--   0 root         (0) root         (0)      891 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/logo.png
--rw-r--r--   0 root         (0) root         (0)    14323 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte.png
--rw-r--r--   0 root         (0) root         (0)    30194 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte@2x.png
--rw-r--r--   0 root         (0) root         (0)     7946 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-plain.png
--rw-r--r--   0 root         (0) root         (0)      535 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow.png
--rw-r--r--   0 root         (0) root         (0)     1134 2024-05-03 15:49:46.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow@2x.png
--rw-r--r--   0 root         (0) root         (0)    36367 2024-05-03 15:49:46.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft.png
--rw-r--r--   0 root         (0) root         (0)   146362 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft@2x.png
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-03 15:49:37.000000 souschef-1.4.4/souschef/sous_chef/assets/images/routing-icon.png
--rw-r--r--   0 root         (0) root         (0)     4831 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/throbber.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/js/
--rw-r--r--   0 root         (0) root         (0)  1031323 2024-05-03 15:49:33.000000 souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.js
--rw-r--r--   0 root         (0) root         (0)   627692 2024-05-03 15:49:36.000000 souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.min.js
--rw-r--r--   0 root         (0) root         (0)    22295 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.js
--rw-r--r--   0 root         (0) root         (0)    10453 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.min.js
--rw-r--r--   0 root         (0) root         (0)  1111829 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.js
--rw-r--r--   0 root         (0) root         (0)   399694 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.min.js
--rw-r--r--   0 root         (0) root         (0)     1518 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/formats/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/formats/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/formats/en/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/formats/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/formats/en/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/formats/fr/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/formats/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      141 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/formats/fr/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/management/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/management/commands/makemessages.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/rules.py
--rw-r--r--   0 root         (0) root         (0)     7507 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/settings.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/settings_test.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/settings_test_fr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/
--rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/avatar/
--rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/avatar/change.html
--rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/avatar/confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3656 2021-07-23 15:25:58.000000 souschef-1.4.4/souschef/sous_chef/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/dashboard/
--rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/dashboard/statistics.html
--rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/splash.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/system/
--rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/system/_button_export.html
--rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/system/breadcrumb.html
--rw-r--r--   0 root         (0) root         (0)     2878 2021-07-09 19:03:35.000000 souschef-1.4.4/souschef/sous_chef/templates/system/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/templatetags/sous_chef_extras.py
--rw-r--r--   0 root         (0) root         (0)     3420 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/tests.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/urls.py
--rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2261 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15624 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      476 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/
+-rw-r--r--   0 root         (0) root         (0)     5731 2024-02-17 22:37:08.000000 souschef-1.4.6/INSTALL.md
+-rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.4.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-05-10 16:11:31.000000 souschef-1.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.4.6/README.md
+-rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.4.6/UPDATE.md
+-rw-r--r--   0 root         (0) root         (0)      249 2024-02-18 19:41:03.000000 souschef-1.4.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-10 16:11:31.000000 souschef-1.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-05-10 16:08:55.000000 souschef-1.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/
+-rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/admin.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/billing/apps.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/billing/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/billing/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      459 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/migrations/0002_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      370 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/migrations/0003_auto_20161122_0515.py
+-rw-r--r--   0 root         (0) root         (0)      374 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/migrations/0004_auto_20201030_1540.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/billing/templates/
+-rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/base_billing.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/billing/templates/billing/
+-rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/billing/add.html
+-rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/billing/billing_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/billing/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/billing/templates/billing/partials/
+-rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/billing/partials/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     5508 2021-07-16 15:48:25.000000 souschef-1.4.6/souschef/billing/templates/billing/partials/summary.html
+-rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/billing/print_summary.html
+-rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/billing/templates/billing/view.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.4.6/souschef/billing/templates/billing/view_orders.html
+-rw-r--r--   0 root         (0) root         (0)     8556 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/tests.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/billing/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12279 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/billing/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/configsamples/
+-rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.4.6/souschef/configsamples/nginx.conf
+-rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.4.6/souschef/configsamples/souschef.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/cronscripts/
+-rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.4.6/souschef/cronscripts/souschef_daily.sh
+-rw-r--r--   0 root         (0) root         (0)      350 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/dataexec.py
+-rw-r--r--   0 root         (0) root         (0)    76889 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/dataload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/datamigration/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/datamigration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/datamigration/admin.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/datamigration/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/datamigration/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.4.6/souschef/datamigration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/datamigration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.4.6/souschef/datamigration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/datamigration/management/commands/importaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/datamigration/management/commands/importclients.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/datamigration/management/commands/importcontactaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/datamigration/management/commands/importmeals.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/datamigration/management/commands/importorders.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/datamigration/management/commands/importrelationships.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/datamigration/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/datamigration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/datamigration/models.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/datamigration/tests.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/datamigration/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/delivery/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/delivery/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/delivery/admin.py
+-rwxr-xr-x   0 root         (0) root         (0)       91 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/delivery/apps.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/delivery/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2024-02-17 22:36:40.000000 souschef-1.4.6/souschef/delivery/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/delivery/migrations/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/delivery/migrations/0001_fix004a.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/delivery/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      232 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/delivery/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/delivery/templates/
+-rw-r--r--   0 root         (0) root         (0)    12210 2024-02-19 02:15:16.000000 souschef-1.4.6/souschef/delivery/templates/edit_delivery_route.html
+-rw-r--r--   0 root         (0) root         (0)     3686 2024-03-06 02:24:13.000000 souschef-1.4.6/souschef/delivery/templates/ingredients.html
+-rw-r--r--   0 root         (0) root         (0)     4380 2024-04-11 01:19:40.000000 souschef-1.4.6/souschef/delivery/templates/kitchen_count.html
+-rw-r--r--   0 root         (0) root         (0)     1360 2024-03-06 02:24:13.000000 souschef-1.4.6/souschef/delivery/templates/kitchen_count_steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/delivery/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/delivery/templates/partials/generated_orders.html
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/delivery/templates/partials/generated_orders_order_row_content.html
+-rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.4.6/souschef/delivery/templates/partials/generated_orders_table_head.html
+-rw-r--r--   0 root         (0) root         (0)     5472 2024-03-06 02:24:13.000000 souschef-1.4.6/souschef/delivery/templates/review_orders.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2024-02-19 02:15:16.000000 souschef-1.4.6/souschef/delivery/templates/route_sheet.html
+-rw-r--r--   0 root         (0) root         (0)     5284 2024-04-09 15:26:23.000000 souschef-1.4.6/souschef/delivery/templates/routes.html
+-rwxr-xr-x   0 root         (0) root         (0)    53737 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/delivery/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/delivery/tsp.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-09 15:26:23.000000 souschef-1.4.6/souschef/delivery/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)    80975 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/delivery/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/frontend/images/
+-rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/frontend/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/frontend/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/frontend/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/frontend/images/katrina.jpg
+-rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/meal/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/meal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2024-05-06 01:26:56.000000 souschef-1.4.6/souschef/meal/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/meal/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/meal/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7348 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0002_ingredient_ingredient_group.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0003_fix224a.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0004_fix004d.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0006_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0007_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/migrations/0008_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/meal/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2024-04-11 01:19:40.000000 souschef-1.4.6/souschef/meal/models.py
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/meal/settings.py
+-rw-r--r--   0 root         (0) root         (0)     8761 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/meal/tests.py
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/meal/urls.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/meal/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/admin.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/member/apps.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/factories.py
+-rw-r--r--   0 root         (0) root         (0)    20424 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/member/forms.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/member/formsets.py
+-rw-r--r--   0 root         (0) root         (0)      964 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/formsfield.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.4.6/souschef/member/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.4.6/souschef/member/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/member/management/commands/createclients.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/member/management/commands/createnotes.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-11 01:19:40.000000 souschef-1.4.6/souschef/member/management/commands/processscheduledstatuschange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/migrations/
+-rw-r--r--   0 root         (0) root         (0)    15890 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0002_auto_20160605_1609.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0003_auto_20160615_2100.py
+-rw-r--r--   0 root         (0) root         (0)     4445 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0005_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0006_client_meal_default_week.py
+-rw-r--r--   0 root         (0) root         (0)      908 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0007_auto_20160726_1703.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0008_auto_20160727_2251.py
+-rw-r--r--   0 root         (0) root         (0)      918 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0009_auto_20160728_1443.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0010_auto_20160803_2052.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0011_client_delivery_note.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0012_clientscheduledstatus.py
+-rw-r--r--   0 root         (0) root         (0)      754 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0013_auto_20160820_2322.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0014_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0015_route_client_id_sequence.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0016_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0017_auto_20161020_2039.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0018_auto_20161110_2352.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0019_auto_20161111_1750.py
+-rw-r--r--   0 root         (0) root         (0)      438 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0020_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0021_auto_20161125_2055.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0022_auto_20161215_1936.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0023_auto_20161220_1401.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0024_auto_20161227_1819.py
+-rw-r--r--   0 root         (0) root         (0)      672 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0025_route_vehicle.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0026_change_to_emergency_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0027_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-11 01:19:40.000000 souschef-1.4.6/souschef/member/migrations/0029_member_address_fk_to_1to1.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0030_route_deliveryhistory.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0032_relationship.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0033_auto_20170801_1607.py
+-rw-r--r--   0 root         (0) root         (0)      554 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0034_auto_20170816_0850.py
+-rw-r--r--   0 root         (0) root         (0)      866 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0035_auto_20210115_1155.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0036_member_addresses.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0037_one_address_per_member.py
+-rw-r--r--   0 root         (0) root         (0)      601 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/member/migrations/0038_member_verbose_names.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29870 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/member/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/signals/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/signals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/member/signals/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/member/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/client/
+-rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/client/create/
+-rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/create/form.html
+-rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/create/steps.html
+-rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/client/partials/
+-rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/birthdays.html
+-rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/filters.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/
+-rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/address_information.html
+-rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/basic_information.html
+-rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/dietary_restriction.html
+-rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/meal_defaults.html
+-rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/payment_information.html
+-rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/relationship_form.html
+-rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/forms/relationships.html
+-rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/partials/menu.html
+-rw-r--r--   0 root         (0) root         (0)     2017 2021-06-18 20:11:28.000000 souschef-1.4.6/souschef/member/templates/client/partials/order_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/client/update/
+-rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.4.6/souschef/member/templates/client/update/base.html
+-rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.4.6/souschef/member/templates/client/update/status.html
+-rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/update/step.html
+-rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/update/steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/client/view/
+-rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/address.html
+-rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/allergies.html
+-rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/delete_status_confirmation.html
+-rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/information.html
+-rw-r--r--   0 root         (0) root         (0)     2716 2021-06-11 15:40:13.000000 souschef-1.4.6/souschef/member/templates/client/view/notes.html
+-rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.4.6/souschef/member/templates/client/view/orders.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/payment.html
+-rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/referent.html
+-rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/status.html
+-rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/client/view/summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/member/templates/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/route/delivered_route_detail.html
+-rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/route/delivery_history_detail.html
+-rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/route/detail.html
+-rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/route/edit.html
+-rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/member/templates/route/list.html
+-rw-r--r--   0 root         (0) root         (0)   165842 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/member/tests.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/member/urls.py
+-rw-r--r--   0 root         (0) root         (0)    54776 2024-04-11 01:19:40.000000 souschef-1.4.6/souschef/member/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/note/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/note/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/note/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/note/apps.py
+-rw-r--r--   0 root         (0) root         (0)      775 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/factories.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/note/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      607 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0002_auto_20160818_2104.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0003_auto_20160819_2037.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0004_notepriority.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0005_note_priority_old_data_migration.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0006_change_priority_field.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0007_notecategory.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0008_auto_20170116_1441.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0009_auto_20170116_1543.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0010_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      987 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0011_auto_20170419_1109.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0012_note_is_deleted.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0013_date_modified.py
+-rw-r--r--   0 root         (0) root         (0)      495 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/migrations/0014_date_created.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/note/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/note/templates/
+-rw-r--r--   0 root         (0) root         (0)      909 2021-07-09 19:21:52.000000 souschef-1.4.6/souschef/note/templates/note_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     1720 2021-07-09 19:00:25.000000 souschef-1.4.6/souschef/note/templates/note_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2186 2021-07-09 19:00:30.000000 souschef-1.4.6/souschef/note/templates/notes_add.html
+-rw-r--r--   0 root         (0) root         (0)     4080 2021-06-11 15:41:01.000000 souschef-1.4.6/souschef/note/templates/notes_client_list.html
+-rw-r--r--   0 root         (0) root         (0)     5780 2021-07-23 15:17:48.000000 souschef-1.4.6/souschef/note/templates/notes_list.html
+-rw-r--r--   0 root         (0) root         (0)     9225 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/tests.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/note/urls.py
+-rw-r--r--   0 root         (0) root         (0)     5709 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/note/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/notification/admin.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/notification/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/notification/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/notification/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/notification/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2024-02-11 21:15:42.000000 souschef-1.4.6/souschef/notification/models.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/notification/tests.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/notification/urls.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/notification/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/order/admin.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/order/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/factories.py
+-rw-r--r--   0 root         (0) root         (0)     5183 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.4.6/souschef/order/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.4.6/souschef/order/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/management/commands/createorders.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/management/commands/generateorders.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/management/commands/setordersdelivered.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4735 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      581 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0002_auto_20160614_1736.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0003_auto_20160615_1504.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      681 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0006_auto_20160803_2217.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0007_remove_order_item_component.py
+-rw-r--r--   0 root         (0) root         (0)      633 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0008_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0009_auto_20161012_1919.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0010_auto_20161012_1921.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0011_auto_20161014_1901.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0012_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0013_orderstatuschange.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0014_auto_20161209_2045.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0015_auto_20170410_1029.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0016_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/migrations/0017_total_quantity_not_nullable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/order/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    47013 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/order/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/templates/
+-rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/templates/_form.html
+-rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/templates/_order_info.html
+-rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/templates/base_order.html
+-rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/templates/create.html
+-rw-r--r--   0 root         (0) root         (0)     4481 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/order/templates/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/templates/order/
+-rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/templates/order/create_batch.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/order/templates/order/partials/
+-rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/order/templates/order/partials/filters.html
+-rw-r--r--   0 root         (0) root         (0)     1070 2021-07-09 19:21:52.000000 souschef-1.4.6/souschef/order/templates/order_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.4.6/souschef/order/templates/order_update_status.html
+-rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.4.6/souschef/order/templates/update.html
+-rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.4.6/souschef/order/templates/view.html
+-rw-r--r--   0 root         (0) root         (0)    66186 2024-02-24 23:48:36.000000 souschef-1.4.6/souschef/order/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/order/urls.py
+-rw-r--r--   0 root         (0) root         (0)    14652 2024-02-19 02:15:16.000000 souschef-1.4.6/souschef/order/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/page/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/page/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/page/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/page/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/page/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/page/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/page/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/page/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/page/templates/pages/
+-rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/page/templates/pages/card.html
+-rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/page/templates/pages/home.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/page/templates/registration/
+-rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/page/templates/registration/login.html
+-rw-r--r--   0 root         (0) root         (0)    10143 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/page/tests.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/page/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-05-06 01:12:04.000000 souschef-1.4.6/souschef/page/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/pycrons/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.4.6/souschef/pycrons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/pycrons/cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef/sous_chef/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/assets/css/
+-rw-r--r--   0 root         (0) root         (0)   655527 2024-05-10 16:11:11.000000 souschef-1.4.6/souschef/sous_chef/assets/css/main.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/
+-rw-r--r--   0 root         (0) root         (0)    98640 2024-05-10 16:11:04.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   507628 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    98404 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    63728 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.woff
+-rw-r--r--   0 root         (0) root         (0)    54488 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)   106004 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.eot
+-rw-r--r--   0 root         (0) root         (0)    93888 2024-05-10 16:11:08.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.otf
+-rw-r--r--   0 root         (0) root         (0)   390837 2024-05-10 16:11:11.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.svg
+-rw-r--r--   0 root         (0) root         (0)   105784 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    50524 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.woff
+-rw-r--r--   0 root         (0) root         (0)    40148 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.woff2
+-rw-r--r--   0 root         (0) root         (0)    31156 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   107201 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    30928 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    14712 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.woff
+-rw-r--r--   0 root         (0) root         (0)    12240 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/assets/images/
+-rw-r--r--   0 root         (0) root         (0)   258972 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    11449 2024-05-10 16:11:20.000000 souschef-1.4.6/souschef/sous_chef/assets/images/demo.png
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    28123 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/images/flags.png
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/images/geocoder.png
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/glyph-marker-icon.png
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/glyph-marker-icon.svg
+-rw-r--r--   0 root         (0) root         (0)    21977 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    26952 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/katrina.jpg
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-05-10 16:11:09.000000 souschef-1.4.6/souschef/sous_chef/assets/images/leaflet.routing.icons.png
+-rw-r--r--   0 root         (0) root         (0)     4060 2024-05-10 16:11:11.000000 souschef-1.4.6/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
+-rw-r--r--   0 root         (0) root         (0)     6363 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/logo-souschef-coul.png
+-rw-r--r--   0 root         (0) root         (0)     6033 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/logo-souschef-nb.png
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-10 16:11:21.000000 souschef-1.4.6/souschef/sous_chef/assets/images/logo.png
+-rw-r--r--   0 root         (0) root         (0)    14323 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-matte.png
+-rw-r--r--   0 root         (0) root         (0)    30194 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-matte@2x.png
+-rw-r--r--   0 root         (0) root         (0)     7946 2024-05-10 16:11:19.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-plain.png
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-10 16:11:19.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-shadow.png
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-05-10 16:11:19.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-shadow@2x.png
+-rw-r--r--   0 root         (0) root         (0)    36367 2024-05-10 16:11:19.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-soft.png
+-rw-r--r--   0 root         (0) root         (0)   146362 2024-05-10 16:11:20.000000 souschef-1.4.6/souschef/sous_chef/assets/images/markers-soft@2x.png
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-10 16:11:09.000000 souschef-1.4.6/souschef/sous_chef/assets/images/routing-icon.png
+-rw-r--r--   0 root         (0) root         (0)     4831 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/images/throbber.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/assets/js/
+-rw-r--r--   0 root         (0) root         (0)  1031323 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/js/leaflet.js
+-rw-r--r--   0 root         (0) root         (0)   627692 2024-05-10 16:11:09.000000 souschef-1.4.6/souschef/sous_chef/assets/js/leaflet.min.js
+-rw-r--r--   0 root         (0) root         (0)    22295 2024-05-10 16:11:04.000000 souschef-1.4.6/souschef/sous_chef/assets/js/multidatespicker.js
+-rw-r--r--   0 root         (0) root         (0)    10453 2024-05-10 16:11:05.000000 souschef-1.4.6/souschef/sous_chef/assets/js/multidatespicker.min.js
+-rw-r--r--   0 root         (0) root         (0)  1111829 2024-05-10 16:11:11.000000 souschef-1.4.6/souschef/sous_chef/assets/js/sous-chef.js
+-rw-r--r--   0 root         (0) root         (0)   399694 2024-05-10 16:11:18.000000 souschef-1.4.6/souschef/sous_chef/assets/js/sous-chef.min.js
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/formats/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/formats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/formats/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/formats/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/formats/en/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/formats/fr/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/formats/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      141 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/formats/fr/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/management/commands/makemessages.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/rules.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/settings.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/sous_chef/settings_test.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/sous_chef/settings_test_fr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/templates/
+-rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/templates/avatar/
+-rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/avatar/change.html
+-rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/avatar/confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3656 2021-07-23 15:25:58.000000 souschef-1.4.6/souschef/sous_chef/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/templates/dashboard/
+-rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/dashboard/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/splash.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/templates/system/
+-rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/system/_button_export.html
+-rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templates/system/breadcrumb.html
+-rw-r--r--   0 root         (0) root         (0)     2878 2021-07-09 19:03:35.000000 souschef-1.4.6/souschef/sous_chef/templates/system/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:31.000000 souschef-1.4.6/souschef/sous_chef/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/sous_chef/templatetags/sous_chef_extras.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-02-18 19:41:03.000000 souschef-1.4.6/souschef/sous_chef/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-26 21:47:13.000000 souschef-1.4.6/souschef/sous_chef/urls.py
+-rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.4.6/souschef/sous_chef/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15624 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      476 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-10 16:11:30.000000 souschef-1.4.6/souschef.egg-info/top_level.txt
```

### Comparing `souschef-1.4.4/INSTALL.md` & `souschef-1.4.6/INSTALL.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/LICENSE.txt` & `souschef-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/PKG-INFO` & `souschef-1.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.4.4
+Version: 1.4.6
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/santropolroulant/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Keywords: meals-on-wheel
 Platform: UNKNOWN
```

### Comparing `souschef-1.4.4/README.md` & `souschef-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/UPDATE.md` & `souschef-1.4.6/UPDATE.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/setup.py` & `souschef-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="souschef",
-    version="1.4.4",
+    version="1.4.6",
     license="AGPL-3.0",
     author="Santropol Roulant and Savoir Faire Linux",
     author_email="info@santropolroulant.org",
     description="Webapp used to manage orders for meals-on-wheel delivery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/santropolroulant/sous-chef",
```

### Comparing `souschef-1.4.4/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg` & `souschef-1.4.6/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/migrations/0001_initial.py` & `souschef-1.4.6/souschef/billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/models.py` & `souschef-1.4.6/souschef/billing/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/add.html` & `souschef-1.4.6/souschef/billing/templates/billing/add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/billing_confirm_delete.html` & `souschef-1.4.6/souschef/billing/templates/billing/billing_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/list.html` & `souschef-1.4.6/souschef/billing/templates/billing/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/partials/statistics.html` & `souschef-1.4.6/souschef/billing/templates/billing/partials/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/partials/summary.html` & `souschef-1.4.6/souschef/billing/templates/billing/partials/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/print_summary.html` & `souschef-1.4.6/souschef/billing/templates/billing/print_summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/view.html` & `souschef-1.4.6/souschef/billing/templates/billing/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/templates/billing/view_orders.html` & `souschef-1.4.6/souschef/billing/templates/billing/view_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/tests.py` & `souschef-1.4.6/souschef/billing/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/urls.py` & `souschef-1.4.6/souschef/billing/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/billing/views.py` & `souschef-1.4.6/souschef/billing/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/configsamples/nginx.conf` & `souschef-1.4.6/souschef/configsamples/nginx.conf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/dataload.py` & `souschef-1.4.6/souschef/dataload.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/management/commands/importaddresses.py` & `souschef-1.4.6/souschef/datamigration/management/commands/importaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/management/commands/importclients.py` & `souschef-1.4.6/souschef/datamigration/management/commands/importclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/management/commands/importcontactaddresses.py` & `souschef-1.4.6/souschef/datamigration/management/commands/importcontactaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/management/commands/importmeals.py` & `souschef-1.4.6/souschef/datamigration/management/commands/importmeals.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/management/commands/importorders.py` & `souschef-1.4.6/souschef/datamigration/management/commands/importorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/management/commands/importrelationships.py` & `souschef-1.4.6/souschef/datamigration/management/commands/importrelationships.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/datamigration/tests.py` & `souschef-1.4.6/souschef/datamigration/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/filters.py` & `souschef-1.4.6/souschef/delivery/filters.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/forms.py` & `souschef-1.4.6/souschef/delivery/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/migrations/0001_fix004a.py` & `souschef-1.4.6/souschef/delivery/migrations/0001_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/edit_delivery_route.html` & `souschef-1.4.6/souschef/delivery/templates/edit_delivery_route.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/ingredients.html` & `souschef-1.4.6/souschef/delivery/templates/ingredients.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/kitchen_count.html` & `souschef-1.4.6/souschef/delivery/templates/kitchen_count.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/kitchen_count_steps.html` & `souschef-1.4.6/souschef/delivery/templates/kitchen_count_steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/partials/generated_orders.html` & `souschef-1.4.6/souschef/delivery/templates/partials/generated_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_order_row_content.html` & `souschef-1.4.6/souschef/delivery/templates/partials/generated_orders_order_row_content.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_table_head.html` & `souschef-1.4.6/souschef/delivery/templates/partials/generated_orders_table_head.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/review_orders.html` & `souschef-1.4.6/souschef/delivery/templates/review_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/route_sheet.html` & `souschef-1.4.6/souschef/delivery/templates/route_sheet.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/templates/routes.html` & `souschef-1.4.6/souschef/delivery/templates/routes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/tests.py` & `souschef-1.4.6/souschef/delivery/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/tsp.py` & `souschef-1.4.6/souschef/delivery/tsp.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/urls.py` & `souschef-1.4.6/souschef/delivery/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/delivery/views.py` & `souschef-1.4.6/souschef/delivery/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/frontend/images/bg1.jpg` & `souschef-1.4.6/souschef/frontend/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/frontend/images/jenny.jpg` & `souschef-1.4.6/souschef/frontend/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/frontend/images/joe.jpg` & `souschef-1.4.6/souschef/frontend/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/frontend/images/katrina.jpg` & `souschef-1.4.6/souschef/frontend/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/admin.py` & `souschef-1.4.6/souschef/meal/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 class ComponentsInline(admin.TabularInline):
     model = Menu.components.through
 
 
 class ComponentIngredientInline(admin.TabularInline):
     model = Component_ingredient
+    fields = ("ingredient",)
+
+    def get_queryset(self, request):
+        return super().get_queryset(request).filter(date=None)
 
 
 class IncompatibilityInline(admin.TabularInline):
     model = Incompatibility
 
 
 class MenuAdmin(admin.ModelAdmin):
```

### Comparing `souschef-1.4.4/souschef/meal/factories.py` & `souschef-1.4.6/souschef/meal/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0001_fix161f.py` & `souschef-1.4.6/souschef/meal/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0002_ingredient_ingredient_group.py` & `souschef-1.4.6/souschef/meal/migrations/0002_ingredient_ingredient_group.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0003_fix224a.py` & `souschef-1.4.6/souschef/meal/migrations/0003_fix224a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0005_fix241b.py` & `souschef-1.4.6/souschef/meal/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0006_auto_20160826_0007.py` & `souschef-1.4.6/souschef/meal/migrations/0006_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0007_auto_20170313_1442.py` & `souschef-1.4.6/souschef/meal/migrations/0007_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/migrations/0008_auto_20180704_1613.py` & `souschef-1.4.6/souschef/meal/migrations/0008_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/models.py` & `souschef-1.4.6/souschef/meal/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/meal/tests.py` & `souschef-1.4.6/souschef/meal/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/admin.py` & `souschef-1.4.6/souschef/member/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/factories.py` & `souschef-1.4.6/souschef/member/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/forms.py` & `souschef-1.4.6/souschef/member/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/formsfield.py` & `souschef-1.4.6/souschef/member/formsfield.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/management/commands/createclients.py` & `souschef-1.4.6/souschef/member/management/commands/createclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/management/commands/processscheduledstatuschange.py` & `souschef-1.4.6/souschef/member/management/commands/processscheduledstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0001_fix161f.py` & `souschef-1.4.6/souschef/member/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0002_auto_20160605_1609.py` & `souschef-1.4.6/souschef/member/migrations/0002_auto_20160605_1609.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0003_auto_20160615_2100.py` & `souschef-1.4.6/souschef/member/migrations/0003_auto_20160615_2100.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0004_fix004a.py` & `souschef-1.4.6/souschef/member/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0005_fix004a.py` & `souschef-1.4.6/souschef/member/migrations/0005_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0007_auto_20160726_1703.py` & `souschef-1.4.6/souschef/member/migrations/0007_auto_20160726_1703.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0009_auto_20160728_1443.py` & `souschef-1.4.6/souschef/member/migrations/0009_auto_20160728_1443.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0012_clientscheduledstatus.py` & `souschef-1.4.6/souschef/member/migrations/0012_clientscheduledstatus.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0013_auto_20160820_2322.py` & `souschef-1.4.6/souschef/member/migrations/0013_auto_20160820_2322.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0014_auto_20160826_0007.py` & `souschef-1.4.6/souschef/member/migrations/0014_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0016_auto_20160912_1509.py` & `souschef-1.4.6/souschef/member/migrations/0016_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0017_auto_20161020_2039.py` & `souschef-1.4.6/souschef/member/migrations/0017_auto_20161020_2039.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0018_auto_20161110_2352.py` & `souschef-1.4.6/souschef/member/migrations/0018_auto_20161110_2352.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0019_auto_20161111_1750.py` & `souschef-1.4.6/souschef/member/migrations/0019_auto_20161111_1750.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0022_auto_20161215_1936.py` & `souschef-1.4.6/souschef/member/migrations/0022_auto_20161215_1936.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0023_auto_20161220_1401.py` & `souschef-1.4.6/souschef/member/migrations/0023_auto_20161220_1401.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0024_auto_20161227_1819.py` & `souschef-1.4.6/souschef/member/migrations/0024_auto_20161227_1819.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0025_route_vehicle.py` & `souschef-1.4.6/souschef/member/migrations/0025_route_vehicle.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0026_change_to_emergency_contacts.py` & `souschef-1.4.6/souschef/member/migrations/0026_change_to_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0027_auto_20170313_1442.py` & `souschef-1.4.6/souschef/member/migrations/0027_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py` & `souschef-1.4.6/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0029_member_address_fk_to_1to1.py` & `souschef-1.4.6/souschef/member/migrations/0029_member_address_fk_to_1to1.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0030_route_deliveryhistory.py` & `souschef-1.4.6/souschef/member/migrations/0030_route_deliveryhistory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0031_client_option_allow_reverse_relation.py` & `souschef-1.4.6/souschef/member/migrations/0031_client_option_allow_reverse_relation.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0032_relationship.py` & `souschef-1.4.6/souschef/member/migrations/0032_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0033_auto_20170801_1607.py` & `souschef-1.4.6/souschef/member/migrations/0033_auto_20170801_1607.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0034_auto_20170816_0850.py` & `souschef-1.4.6/souschef/member/migrations/0034_auto_20170816_0850.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0035_auto_20210115_1155.py` & `souschef-1.4.6/souschef/member/migrations/0035_auto_20210115_1155.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0036_member_addresses.py` & `souschef-1.4.6/souschef/member/migrations/0036_member_addresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0037_one_address_per_member.py` & `souschef-1.4.6/souschef/member/migrations/0037_one_address_per_member.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/migrations/0038_member_verbose_names.py` & `souschef-1.4.6/souschef/member/migrations/0038_member_verbose_names.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/models.py` & `souschef-1.4.6/souschef/member/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/base.html` & `souschef-1.4.6/souschef/member/templates/client/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/create/form.html` & `souschef-1.4.6/souschef/member/templates/client/create/form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/create/steps.html` & `souschef-1.4.6/souschef/member/templates/client/create/steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/list.html` & `souschef-1.4.6/souschef/member/templates/client/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/birthdays.html` & `souschef-1.4.6/souschef/member/templates/client/partials/birthdays.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/filters.html` & `souschef-1.4.6/souschef/member/templates/client/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/address_information.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/address_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/basic_information.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/basic_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/dietary_restriction.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/dietary_restriction.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/meal_defaults.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/meal_defaults.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/payment_information.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/payment_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/relationship_form.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/relationship_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/forms/relationships.html` & `souschef-1.4.6/souschef/member/templates/client/partials/forms/relationships.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/menu.html` & `souschef-1.4.6/souschef/member/templates/client/partials/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/partials/order_list.html` & `souschef-1.4.6/souschef/member/templates/client/partials/order_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/update/base.html` & `souschef-1.4.6/souschef/member/templates/client/update/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/update/status.html` & `souschef-1.4.6/souschef/member/templates/client/update/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/allergies.html` & `souschef-1.4.6/souschef/member/templates/client/view/allergies.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/delete_status_confirmation.html` & `souschef-1.4.6/souschef/member/templates/client/view/delete_status_confirmation.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/information.html` & `souschef-1.4.6/souschef/member/templates/client/view/information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/notes.html` & `souschef-1.4.6/souschef/member/templates/client/view/notes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/orders.html` & `souschef-1.4.6/souschef/member/templates/client/view/orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/payment.html` & `souschef-1.4.6/souschef/member/templates/client/view/payment.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/referent.html` & `souschef-1.4.6/souschef/member/templates/client/view/referent.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/status.html` & `souschef-1.4.6/souschef/member/templates/client/view/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/client/view/summary.html` & `souschef-1.4.6/souschef/member/templates/client/view/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/route/delivery_history_detail.html` & `souschef-1.4.6/souschef/member/templates/route/delivery_history_detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/route/detail.html` & `souschef-1.4.6/souschef/member/templates/route/detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/route/edit.html` & `souschef-1.4.6/souschef/member/templates/route/edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/templates/route/list.html` & `souschef-1.4.6/souschef/member/templates/route/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/tests.py` & `souschef-1.4.6/souschef/member/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/urls.py` & `souschef-1.4.6/souschef/member/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/member/views.py` & `souschef-1.4.6/souschef/member/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/admin.py` & `souschef-1.4.6/souschef/note/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/factories.py` & `souschef-1.4.6/souschef/note/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/forms.py` & `souschef-1.4.6/souschef/note/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0001_initial.py` & `souschef-1.4.6/souschef/note/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0002_auto_20160818_2104.py` & `souschef-1.4.6/souschef/note/migrations/0002_auto_20160818_2104.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0004_notepriority.py` & `souschef-1.4.6/souschef/note/migrations/0004_notepriority.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0005_note_priority_old_data_migration.py` & `souschef-1.4.6/souschef/note/migrations/0005_note_priority_old_data_migration.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0007_notecategory.py` & `souschef-1.4.6/souschef/note/migrations/0007_notecategory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0008_auto_20170116_1441.py` & `souschef-1.4.6/souschef/note/migrations/0008_auto_20170116_1441.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0009_auto_20170116_1543.py` & `souschef-1.4.6/souschef/note/migrations/0009_auto_20170116_1543.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0010_auto_20170313_1442.py` & `souschef-1.4.6/souschef/note/migrations/0010_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0011_auto_20170419_1109.py` & `souschef-1.4.6/souschef/note/migrations/0011_auto_20170419_1109.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/migrations/0013_date_modified.py` & `souschef-1.4.6/souschef/note/migrations/0013_date_modified.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/models.py` & `souschef-1.4.6/souschef/note/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/templates/note_confirm_delete.html` & `souschef-1.4.6/souschef/note/templates/note_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/templates/note_edit.html` & `souschef-1.4.6/souschef/note/templates/note_edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/templates/notes_add.html` & `souschef-1.4.6/souschef/note/templates/notes_add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/templates/notes_client_list.html` & `souschef-1.4.6/souschef/note/templates/notes_client_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/templates/notes_list.html` & `souschef-1.4.6/souschef/note/templates/notes_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/tests.py` & `souschef-1.4.6/souschef/note/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/urls.py` & `souschef-1.4.6/souschef/note/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/note/views.py` & `souschef-1.4.6/souschef/note/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/notification/migrations/0001_fix161f.py` & `souschef-1.4.6/souschef/notification/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/notification/models.py` & `souschef-1.4.6/souschef/notification/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/admin.py` & `souschef-1.4.6/souschef/order/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/factories.py` & `souschef-1.4.6/souschef/order/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/forms.py` & `souschef-1.4.6/souschef/order/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/management/commands/generateorders.py` & `souschef-1.4.6/souschef/order/management/commands/generateorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/management/commands/setordersdelivered.py` & `souschef-1.4.6/souschef/order/management/commands/setordersdelivered.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0001_fix161f.py` & `souschef-1.4.6/souschef/order/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0002_auto_20160614_1736.py` & `souschef-1.4.6/souschef/order/migrations/0002_auto_20160614_1736.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0003_auto_20160615_1504.py` & `souschef-1.4.6/souschef/order/migrations/0003_auto_20160615_1504.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0004_fix004a.py` & `souschef-1.4.6/souschef/order/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0005_fix241b.py` & `souschef-1.4.6/souschef/order/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0006_auto_20160803_2217.py` & `souschef-1.4.6/souschef/order/migrations/0006_auto_20160803_2217.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0008_auto_20160912_1509.py` & `souschef-1.4.6/souschef/order/migrations/0008_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0009_auto_20161012_1919.py` & `souschef-1.4.6/souschef/order/migrations/0009_auto_20161012_1919.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0011_auto_20161014_1901.py` & `souschef-1.4.6/souschef/order/migrations/0011_auto_20161014_1901.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0013_orderstatuschange.py` & `souschef-1.4.6/souschef/order/migrations/0013_orderstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0014_auto_20161209_2045.py` & `souschef-1.4.6/souschef/order/migrations/0014_auto_20161209_2045.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0015_auto_20170410_1029.py` & `souschef-1.4.6/souschef/order/migrations/0015_auto_20170410_1029.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/migrations/0016_auto_20180704_1613.py` & `souschef-1.4.6/souschef/order/migrations/0016_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/mixins.py` & `souschef-1.4.6/souschef/order/mixins.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/models.py` & `souschef-1.4.6/souschef/order/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/_form.html` & `souschef-1.4.6/souschef/order/templates/_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/_order_info.html` & `souschef-1.4.6/souschef/order/templates/_order_info.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/create.html` & `souschef-1.4.6/souschef/order/templates/create.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/list.html` & `souschef-1.4.6/souschef/order/templates/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/order/create_batch.html` & `souschef-1.4.6/souschef/order/templates/order/create_batch.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/order/partials/filters.html` & `souschef-1.4.6/souschef/order/templates/order/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/order_confirm_delete.html` & `souschef-1.4.6/souschef/order/templates/order_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/order_update_status.html` & `souschef-1.4.6/souschef/order/templates/order_update_status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/update.html` & `souschef-1.4.6/souschef/order/templates/update.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/templates/view.html` & `souschef-1.4.6/souschef/order/templates/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/tests.py` & `souschef-1.4.6/souschef/order/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/urls.py` & `souschef-1.4.6/souschef/order/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/order/views.py` & `souschef-1.4.6/souschef/order/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/page/templates/pages/home.html` & `souschef-1.4.6/souschef/page/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/page/templates/registration/login.html` & `souschef-1.4.6/souschef/page/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/page/tests.py` & `souschef-1.4.6/souschef/page/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/page/views.py` & `souschef-1.4.6/souschef/page/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/css/main.min.css` & `souschef-1.4.6/souschef/sous_chef/assets/css/main.min.css`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.eot` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.svg` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.ttf` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff2` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.eot` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.otf` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.otf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.svg` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.ttf` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff2` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.eot` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.svg` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.ttf` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff2` & `souschef-1.4.6/souschef/sous_chef/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/bg1.jpg` & `souschef-1.4.6/souschef/sous_chef/assets/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/demo.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/demo.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/favicon.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/flags.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/glyph-marker-icon.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.svg` & `souschef-1.4.6/souschef/sous_chef/assets/images/glyph-marker-icon.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/jenny.jpg` & `souschef-1.4.6/souschef/sous_chef/assets/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/joe.jpg` & `souschef-1.4.6/souschef/sous_chef/assets/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/katrina.jpg` & `souschef-1.4.6/souschef/sous_chef/assets/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/leaflet.routing.icons.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.svg` & `souschef-1.4.6/souschef/sous_chef/assets/images/leaflet.routing.icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-coul.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/logo-souschef-coul.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-nb.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/logo-souschef-nb.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/logo.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-matte.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte@2x.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-matte@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-plain.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-plain.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-shadow.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow@2x.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-shadow@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-soft.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft@2x.png` & `souschef-1.4.6/souschef/sous_chef/assets/images/markers-soft@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/images/throbber.gif` & `souschef-1.4.6/souschef/sous_chef/assets/images/throbber.gif`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.js` & `souschef-1.4.6/souschef/sous_chef/assets/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.min.js` & `souschef-1.4.6/souschef/sous_chef/assets/js/leaflet.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.js` & `souschef-1.4.6/souschef/sous_chef/assets/js/multidatespicker.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.min.js` & `souschef-1.4.6/souschef/sous_chef/assets/js/multidatespicker.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.js` & `souschef-1.4.6/souschef/sous_chef/assets/js/sous-chef.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.min.js` & `souschef-1.4.6/souschef/sous_chef/assets/js/sous-chef.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/context_processors.py` & `souschef-1.4.6/souschef/sous_chef/context_processors.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/management/commands/makemessages.py` & `souschef-1.4.6/souschef/sous_chef/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/settings.py` & `souschef-1.4.6/souschef/sous_chef/settings.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/404.html` & `souschef-1.4.6/souschef/sous_chef/templates/404.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/avatar/change.html` & `souschef-1.4.6/souschef/sous_chef/templates/avatar/change.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/avatar/confirm_delete.html` & `souschef-1.4.6/souschef/sous_chef/templates/avatar/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/base.html` & `souschef-1.4.6/souschef/sous_chef/templates/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/dashboard/statistics.html` & `souschef-1.4.6/souschef/sous_chef/templates/dashboard/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/splash.html` & `souschef-1.4.6/souschef/sous_chef/templates/splash.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/templates/system/menu.html` & `souschef-1.4.6/souschef/sous_chef/templates/system/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/tests.py` & `souschef-1.4.6/souschef/sous_chef/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef/sous_chef/urls.py` & `souschef-1.4.6/souschef/sous_chef/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.4/souschef.egg-info/PKG-INFO` & `souschef-1.4.6/souschef.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.4.4
+Version: 1.4.6
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/santropolroulant/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Keywords: meals-on-wheel
 Platform: UNKNOWN
```

### Comparing `souschef-1.4.4/souschef.egg-info/SOURCES.txt` & `souschef-1.4.6/souschef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

