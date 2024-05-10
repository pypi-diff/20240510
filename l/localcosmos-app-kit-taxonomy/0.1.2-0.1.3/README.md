# Comparing `tmp/localcosmos_app_kit_taxonomy-0.1.2.tar.gz` & `tmp/localcosmos_app_kit_taxonomy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_app_kit_taxonomy-0.1.2.tar", last modified: Fri Apr 19 07:17:38 2024, max compression
+gzip compressed data, was "localcosmos_app_kit_taxonomy-0.1.3.tar", last modified: Fri May 10 07:12:48 2024, max compression
```

## Comparing `localcosmos_app_kit_taxonomy-0.1.2.tar` & `localcosmos_app_kit_taxonomy-0.1.3.tar`

### file list

```diff
@@ -1,87 +1,94 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/
--rw-r--r--   0 tom       (1000) tom       (1000)     1086 2024-04-05 12:51:29.000000 localcosmos_app_kit_taxonomy-0.1.2/LICENCE
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-04-10 13:12:47.000000 localcosmos_app_kit_taxonomy-0.1.2/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      649 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)       68 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      649 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2441 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      920 2024-04-19 07:15:54.000000 localcosmos_app_kit_taxonomy-0.1.2/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)     1251 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/DBRouter.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4361 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/TaxonSearch.py
--rw-r--r--   0 tom       (1000) tom       (1000)       73 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      149 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5980 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/lazy.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7625 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/taxonomy_recreate_indices.py
--rw-r--r--   0 tom       (1000) tom       (1000)      634 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/update_taxonomic_database.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     1298 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      553 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0002_auto_20220503_0747.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9825 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1664 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/signals.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/
--rw-r--r--   0 tom       (1000) tom       (1000)    37032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/TaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/
--rw-r--r--   0 tom       (1000) tom       (1000)    50987 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/AlgaebaseManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      110 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/apps.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4336 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/
--rw-r--r--   0 tom       (1000) tom       (1000)    10255 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8228 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager2015.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)       98 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/apps.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4207 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      928 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     5699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/TestColTaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      104 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2690 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4246 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      756 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10323 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.140642 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)      522 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/taxontreeview.html
--rw-r--r--   0 tom       (1000) tom       (1000)      324 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/treeview_children.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)       69 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1784 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)    49583 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/TestTaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5567 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/test_lazy.py
--rw-r--r--   0 tom       (1000) tom       (1000)      560 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2174 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3200 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.776780 localcosmos_app_kit_taxonomy-0.1.3/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1086 2024-04-05 12:51:29.000000 localcosmos_app_kit_taxonomy-0.1.3/LICENCE
+-rw-r--r--   0 tom       (1000) tom       (1000)       94 2024-05-10 06:54:26.000000 localcosmos_app_kit_taxonomy-0.1.3/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)      649 2024-05-10 07:12:48.776780 localcosmos_app_kit_taxonomy-0.1.3/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)       68 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.776780 localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      649 2024-05-10 07:12:48.000000 localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2790 2024-05-10 07:12:48.000000 localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-05-10 07:12:48.000000 localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2024-05-10 07:12:48.000000 localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-05-10 07:12:48.776780 localcosmos_app_kit_taxonomy-0.1.3/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      920 2024-05-10 07:12:43.000000 localcosmos_app_kit_taxonomy-0.1.3/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.770113 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1251 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/DBRouter.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4361 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/TaxonSearch.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       73 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      149 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5980 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/lazy.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.770113 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.770113 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/commands/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/commands/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7625 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/commands/taxonomy_recreate_indices.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      634 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/commands/update_taxonomic_database.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.770113 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1298 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      553 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/migrations/0002_auto_20220503_0747.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9825 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1664 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/signals.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.770113 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/
+-rw-r--r--   0 tom       (1000) tom       (1000)    37243 2024-05-08 13:14:17.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/TaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/
+-rw-r--r--   0 tom       (1000) tom       (1000)    50987 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/AlgaebaseManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      110 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/apps.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4336 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9459 2024-05-08 12:57:33.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/ColTaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8228 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/ColTaxonSourceManager2015.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10255 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/ColTaxonSourceManager2019.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       98 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/apps.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4207 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      928 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/tests/TestColTaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/tests/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      104 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2690 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4246 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      756 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.766779 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/templates/custom_taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1348 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/templates/custom_taxonomy/manage_custom_taxon.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      485 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/templates/custom_taxonomy/manage_custom_taxonomy.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1487 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/templates/custom_taxonomy/manage_tree_entry.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1458 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/templates/custom_taxonomy/move_custom_taxon.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10323 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.766779 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)      522 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/taxontreeview.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      324 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/treeview_children.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.773446 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1784 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-10 07:12:48.776780 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)    49583 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/tests/TestTaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/tests/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5567 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/tests/test_lazy.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      560 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2174 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3200 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.3/taxonomy/views.py
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/LICENCE` & `localcosmos_app_kit_taxonomy-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/PKG-INFO` & `localcosmos_app_kit_taxonomy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_app_kit_taxonomy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Local Cosmos Taxonomy django app
 Home-page: https://github.com/localcosmos/app-kit
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity,taxonomy
 Platform: OS Independent
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO` & `localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_app_kit_taxonomy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Local Cosmos Taxonomy django app
 Home-page: https://github.com/localcosmos/app-kit
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity,taxonomy
 Platform: OS Independent
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt` & `localcosmos_app_kit_taxonomy-0.1.3/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 taxonomy/sources/algaebase/models.py
 taxonomy/sources/algaebase/tests.py
 taxonomy/sources/algaebase/views.py
 taxonomy/sources/algaebase/migrations/0001_initial.py
 taxonomy/sources/algaebase/migrations/__init__.py
 taxonomy/sources/col/ColTaxonSourceManager.py
 taxonomy/sources/col/ColTaxonSourceManager2015.py
+taxonomy/sources/col/ColTaxonSourceManager2019.py
 taxonomy/sources/col/__init__.py
 taxonomy/sources/col/admin.py
 taxonomy/sources/col/apps.py
 taxonomy/sources/col/models.py
 taxonomy/sources/col/tests.py
 taxonomy/sources/col/views.py
 taxonomy/sources/col/migrations/0001_initial.py
@@ -53,14 +54,18 @@
 taxonomy/sources/custom/forms.py
 taxonomy/sources/custom/models.py
 taxonomy/sources/custom/tests.py
 taxonomy/sources/custom/urls.py
 taxonomy/sources/custom/views.py
 taxonomy/sources/custom/migrations/0001_initial.py
 taxonomy/sources/custom/migrations/__init__.py
+taxonomy/sources/custom/templates/custom_taxonomy/manage_custom_taxon.html
+taxonomy/sources/custom/templates/custom_taxonomy/manage_custom_taxonomy.html
+taxonomy/sources/custom/templates/custom_taxonomy/manage_tree_entry.html
+taxonomy/sources/custom/templates/custom_taxonomy/move_custom_taxon.html
 taxonomy/templates/taxonomy/taxontreeview.html
 taxonomy/templates/taxonomy/treeview_children.html
 taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget.html
 taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html
 taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html
 taxonomy/tests/TestTaxonSourceManager.py
 taxonomy/tests/__init__.py
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/setup.py` & `localcosmos_app_kit_taxonomy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 install_requires = [
 
 ]
 
 setup(
     name='localcosmos_app_kit_taxonomy',
-    version='0.1.2',
+    version='0.1.3',
     description='Local Cosmos Taxonomy django app',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, localcosmos, localcosmos server, biodiversity, taxonomy',
     author='Thomas Uher',
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/DBRouter.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/DBRouter.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/TaxonSearch.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/TaxonSearch.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/lazy.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/lazy.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/taxonomy_recreate_indices.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/commands/taxonomy_recreate_indices.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/update_taxonomic_database.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/management/commands/update_taxonomic_database.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0002_auto_20220503_0747.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/migrations/0002_auto_20220503_0747.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/models.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/signals.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/signals.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/TaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/TaxonSourceManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,22 @@
 '''
     Interface for managing taxonomic sources
 '''
 from django.db.models.functions import Length
 import sys, os, json
 import time
 
-from localcosmos_server.slugifier import create_unique_slug
-
 from django.db import transaction
 
 '''
     some vernacular names might contain html characters
 '''
 
 # Python 3
-from html.parser import HTMLParser
-
-import logging
+import logging, html
 
 
 '''
     base
 '''
 
 nuid36 = ['0','1','2','3','4','5','6','7','8','9',                                                                    
@@ -86,16 +82,15 @@
 
 '''
     vernacular names
 '''
 class VernacularName:
 
     def __init__(self, name, language, preferred=False, iso6392=None):
-        parser = HTMLParser()
-        self.name = parser.unescape(name.strip())
+        self.name = html.unescape(name.strip())
         self.language = language.strip().lower() # iso6391 en, fr, de
         self.preferred = preferred
         self.iso6392 = iso6392 # 3-digit
 
 '''
     SourceTaxon
     - superclass for SourceTreeTaxon, SourceSynonymTaxon
@@ -207,14 +202,16 @@
     def set_nuid_from_db(self):
 
         if self.nuid is None:
             print('setting nuid from db')
             db_entry = self.TreeModel.objects.filter(source_id=self.source_id).first()
             if db_entry:
                 self.nuid = db_entry.taxon_nuid
+            else:
+                print('No db entry found for source_id: {0}'.format(self.source_id))
 
         return self.nuid
 
     def get_nuid(self):
         if self.nuid is None:
             self.set_nuid_from_db()
 
@@ -433,15 +430,15 @@
             
         return next_parent
 
            
     def _build_upstream(self):
         
         if self.upstream_is_built:
-            raise ValueError('source_taxon %s not found in tree' % source_taxon.latname)
+            raise ValueError('Upstream already built')
 
         toplevel = self.cache[0]
 
         parent_taxon = toplevel['parent_taxon']
 
         root_taxon = None
 
@@ -687,30 +684,30 @@
     '''
     def update_database(self):
 
         root_taxa = self._get_sorted_root_source_taxa()
         
         # check for existing taxa and assign their nuids, needed for db update
         for taxon in root_taxa:
-            lc_db_taxon = self.TaxonTreeModel.objects.filter(is_root_taxon=True, taxon_latname=taxon.latname).first()
+            lc_db_taxon = self.TaxonTreeModel.objects.filter(is_root_taxon=True, taxon_latname=taxon.latname).order_by('taxon_latname').first()
             if lc_db_taxon:
                 # use the database nuid
                 taxon.set_nuid(lc_db_taxon.taxon_nuid)
             
 
         # this method assigns nuid - to the currently non existing root_taxa
         new_root_taxa = self._compare_new_children_with_existing_children(root_taxa)
 
         for root_taxon in new_root_taxa:
             self._save_new_taxon(root_taxon, is_root_taxon=True)
 
         # work ALL root_taxa, starting with the first one
         root_taxon = root_taxa[0]
 
-        print('working new root taxon: %s' % root_taxon.latname)            
+        print('working new root taxon: {0}'.format(root_taxon.latname))            
         self.state.set_current_root_taxon(root_taxon)
             
         self._climb_tree(root_taxon)
 
 
     '''
     if the creation of the taxonomic database crashed or was manually aborted, resume
@@ -747,15 +744,15 @@
             # last_child is the first child of the last group of children
             # during _climb_down (or methods used in it) nuids have to be set and saved for new taxa
             # the last_child as a SourceTreeTaxon instance either has a nuid set - or can fetch the nuid from the target db
             last_child = self._climb_down(start_taxon)
 
             message = 'last_child: {0}, nuid: {1}'.format(last_child.latname, last_child.get_nuid())
             print(message)
-            self.logger.info(message)
+            # self.logger.info(message)
 
             # search siblings of this childless taxon, or parent siblings if no siblings available
             # start_taxon is always the last child, which is the first child of the last group of children
             # climbing up always uses the new tree - but the taxa it walks already have been saved and have nuids
             # the nuids have to be fetched from the lc db
 
             # get next parent node
@@ -765,15 +762,15 @@
             next_parent = self.cache.get_next_downclimb_taxon(last_child)
 
 
             if next_parent:
                 start_taxon = next_parent
                 message = 'starting nuid (next_parent): {0}'.format(start_taxon.get_nuid())
                 print(message)
-                self.logger.info(message)
+                # self.logger.info(message)
                 
             else:
                 continue_climbing = False
 
 
             if downclimb_counter % 100 == 0:
                 print('downclimb_counter: %s' % downclimb_counter)
@@ -885,22 +882,23 @@
         # children that are in the db AND in the children list
         still_included_children = []
 
         # first, compare the latnames
         existing_children = []
         existing_children_map = {}
         
-        for taxon in existing_children_query:
-            existing_children.append({'author': taxon.taxon_author, 'latname': taxon.taxon_latname})
+        if self.first_run == False:
+            for taxon in existing_children_query:
+                existing_children.append({'author': taxon.taxon_author, 'latname': taxon.taxon_latname})
 
-            author = taxon.taxon_author
-            if not author:
-                author = 'None'
-            key = " ".join([taxon.taxon_latname, author])
-            existing_children_map[key] = taxon
+                author = taxon.taxon_author
+                if not author:
+                    author = 'None'
+                key = " ".join([taxon.taxon_latname, author])
+                existing_children_map[key] = taxon
 
         for child in children:
 
             child_dict = {'author' : child.author, 'latname' : child.latname}
             still_included_children.append(child_dict)
             
             if child_dict in existing_children:
@@ -912,15 +910,15 @@
                     raise ValueError('Found more than one child with the same latname/author combination in the children group: %s' % child.latname)
 
                 existing_taxon = existing_taxon[0]
                 self._check_existing_taxon_synonyms(existing_taxon, child)
                 self._check_existing_taxon_vernacular_names(existing_taxon, child)
 
                 existing_taxon_source_taxon = self.SourceTreeTaxonClass(
-                    existing_taxon.taxon_latname, existing_taxon.author, existing_taxon.rank,
+                    existing_taxon.taxon_latname, existing_taxon.taxon_author, existing_taxon.rank,
                     self.TaxonTreeModel.__class__.__name__, existing_taxon.source_id, nuid=existing_taxon.taxon_nuid
                 )
                 cache_children.append(existing_taxon_source_taxon)
                 
                 continue
             
             # skip duplicates with the same author AND name
@@ -1035,19 +1033,22 @@
 
             return True
 
         return False
         
     def _climb_down(self, parent_taxon):
 
-        self.logger.info('climb down: {0}'.format(parent_taxon.latname))
+        message = 'climb down: {0}'.format(parent_taxon.latname)
+        print(message)
+        # self.logger.info(message)
 
         # if no nuid is found, it might be a duplicate
         is_duplicate = self._check_taxon_duplicate(parent_taxon)
         if is_duplicate:
+            self.logger.info('Duplicate: {0}'.format(parent_taxon.latname))
             return parent_taxon
 
         self.state.set_last_parent(parent_taxon)
 
         has_children = True
 
         first_child = None
@@ -1062,19 +1063,19 @@
                 new_children = self._work_children(parent_taxon, children)
 
                 # do not use new_children here. all children are part of the tree
                 # assign first (leftmost) child as new parent taxon
                 parent_taxon = children[0]
                 first_child = children[0]
 
-                self.logger.info('first child: {0}'.format(first_child.latname))
+                # self.logger.info('first child: {0}'.format(first_child.latname))
 
             else:
 
-                self.logger.info('no more children found for: {0}'.format(parent_taxon.latname))
+                # self.logger.info('no more children found for: {0}'.format(parent_taxon.latname))
                 
                 if self.first_run == False:
                     # check if there are children in the database thet need to be deleted
                     # print("parent: %s %s" % (parent_taxon.latname, parent_taxon.get_nuid()))
                     # check if it is a duplicate
                     is_duplicate = self._check_taxon_duplicate(parent_taxon)
                     if not is_duplicate:
@@ -1082,12 +1083,12 @@
                             taxon_nuid__startswith=parent_taxon.get_nuid()).exclude(
                                 taxon_nuid=parent_taxon.get_nuid()).delete()
                 has_children = False
 
         # if a parent_taxon that has no children is passed, return the parent taxon
         # the tree climber will then go to the next sibling - as it would with the first_child
         if first_child is None:
-            self.logger.info('climb down returning: {0}'.format(parent_taxon.latname))
+            self.logger.info('[_climb_down] No first child found. Returning: {0}'.format(parent_taxon.latname))
             return parent_taxon
 
-        self.logger.info('climb down: {0}'.format(first_child.latname))
+        # self.logger.info('climb down: {0}'.format(first_child.latname))
         return first_child
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/AlgaebaseManager.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/AlgaebaseManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/models.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/algaebase/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/ColTaxonSourceManager2019.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager2015.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/ColTaxonSourceManager2015.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/models.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/TestColTaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/col/tests/TestColTaxonSourceManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/forms.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/models.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/urls.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/views.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/sources/custom/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/taxontreeview.html` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/taxontreeview.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/TestTaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/tests/TestTaxonSourceManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/test_lazy.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/tests/test_lazy.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/urls.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/utils.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/views.py` & `localcosmos_app_kit_taxonomy-0.1.3/taxonomy/views.py`

 * *Files identical despite different names*

