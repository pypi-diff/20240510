# Comparing `tmp/nautobot_bgp_models-2.0.0.tar.gz` & `tmp/nautobot_bgp_models-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_bgp_models-2.0.0.tar", max compression
+gzip compressed data, was "nautobot_bgp_models-2.1.0.tar", max compression
```

## Comparing `nautobot_bgp_models-2.0.0.tar` & `nautobot_bgp_models-2.1.0.tar`

### file list

```diff
@@ -1,55 +1,155 @@
--rw-r--r--   0        0        0      591 2024-02-28 17:58:03.579184 nautobot_bgp_models-2.0.0/LICENSE
--rw-r--r--   0        0        0     4588 2024-02-28 17:58:03.579184 nautobot_bgp_models-2.0.0/README.md
--rw-r--r--   0        0        0     1516 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/__init__.py
--rw-r--r--   0        0        0       51 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/__init__.py
--rw-r--r--   0        0        0      748 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/filter_backends.py
--rw-r--r--   0        0        0     5573 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/serializers.py
--rw-r--r--   0        0        0      908 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/urls.py
--rw-r--r--   0        0        0     4019 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/views.py
--rw-r--r--   0        0        0     1461 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/choices.py
--rw-r--r--   0        0        0     1111 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/dolt_compat.py
--rw-r--r--   0        0        0     1276 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/filter_extensions.py
--rw-r--r--   0        0        0     9788 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/filters.py
--rw-r--r--   0        0        0    19200 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/forms.py
--rw-r--r--   0        0        0    20990 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0001_initial.py
--rw-r--r--   0        0        0      953 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0002_viewsets_migration.py
--rw-r--r--   0        0        0     6716 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0003_peergroupaddressfamily_peerendpointaddressfamily.py
--rw-r--r--   0        0        0     1685 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0004_use_upstream_role_part1.py
--rw-r--r--   0        0        0     4870 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0005_use_upstream_role_part2.py
--rw-r--r--   0        0        0     1181 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0006_use_upstream_role_part3.py
--rw-r--r--   0        0        0     1508 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0007_use_upstream_role_part4.py
--rw-r--r--   0        0        0     4533 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0008_nautobotv2_updates.py
--rw-r--r--   0        0        0        0 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/__init__.py
--rw-r--r--   0        0        0    25851 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/models.py
--rw-r--r--   0        0        0     7051 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/navigation.py
--rw-r--r--   0        0        0     1148 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/signals.py
--rw-r--r--   0        0        0     9054 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tables.py
--rw-r--r--   0        0        0     2025 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/template_content.py
--rw-r--r--   0        0        0     2261 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily_retrieve.html
--rw-r--r--   0        0        0     1309 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem_retrieve.html
--rw-r--r--   0        0        0     3741 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance_retrieve.html
--rw-r--r--   0        0        0     1507 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html
--rw-r--r--   0        0        0      761 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html
--rw-r--r--   0        0        0      839 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html
--rw-r--r--   0        0        0      918 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html
--rw-r--r--   0        0        0      793 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html
--rw-r--r--   0        0        0      876 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html
--rw-r--r--   0        0        0     3146 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html
--rw-r--r--   0        0        0     6326 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint_retrieve.html
--rw-r--r--   0        0        0     3557 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpointaddressfamily_retrieve.html
--rw-r--r--   0        0        0     6556 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup_retrieve.html
--rw-r--r--   0        0        0     3128 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroupaddressfamily_retrieve.html
--rw-r--r--   0        0        0     2782 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate_retrieve.html
--rw-r--r--   0        0        0     2504 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_add.html
--rw-r--r--   0        0        0     1085 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_retrieve.html
--rw-r--r--   0        0        0       46 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/__init__.py
--rw-r--r--   0        0        0    53254 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_api.py
--rw-r--r--   0        0        0     1525 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_basic.py
--rw-r--r--   0        0        0    36686 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_filters.py
--rw-r--r--   0        0        0    15185 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_forms.py
--rw-r--r--   0        0        0    19149 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_models.py
--rw-r--r--   0        0        0    23948 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_views.py
--rw-r--r--   0        0        0     2591 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/urls.py
--rw-r--r--   0        0        0     9942 2024-02-28 17:58:03.595184 nautobot_bgp_models-2.0.0/nautobot_bgp_models/views.py
--rw-r--r--   0        0        0     2943 2024-02-28 17:58:18.375168 nautobot_bgp_models-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5422 1970-01-01 00:00:00.000000 nautobot_bgp_models-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-05-10 19:13:24.299508 nautobot_bgp_models-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4589 2024-05-10 19:13:24.299508 nautobot_bgp_models-2.1.0/README.md
+-rw-r--r--   0        0        0     1618 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/__init__.py
+-rw-r--r--   0        0        0      748 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/filter_backends.py
+-rw-r--r--   0        0        0     5972 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/serializers.py
+-rw-r--r--   0        0        0      988 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/urls.py
+-rw-r--r--   0        0        0     4328 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/views.py
+-rw-r--r--   0        0        0        5 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/app-config-schema.json
+-rw-r--r--   0        0        0     1461 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/choices.py
+-rw-r--r--   0        0        0     1111 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/dolt_compat.py
+-rw-r--r--   0        0        0     1276 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/filter_extensions.py
+-rw-r--r--   0        0        0    11423 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/filters.py
+-rw-r--r--   0        0        0    20445 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/forms.py
+-rw-r--r--   0        0        0     1190 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/helpers.py
+-rw-r--r--   0        0        0    20990 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0      953 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0002_viewsets_migration.py
+-rw-r--r--   0        0        0     6716 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0003_peergroupaddressfamily_peerendpointaddressfamily.py
+-rw-r--r--   0        0        0     1685 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0004_use_upstream_role_part1.py
+-rw-r--r--   0        0        0     4870 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0005_use_upstream_role_part2.py
+-rw-r--r--   0        0        0     1181 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0006_use_upstream_role_part3.py
+-rw-r--r--   0        0        0     1508 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0007_use_upstream_role_part4.py
+-rw-r--r--   0        0        0     4533 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0008_nautobotv2_updates.py
+-rw-r--r--   0        0        0     2248 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0009_autonomoussystemrange.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/__init__.py
+-rw-r--r--   0        0        0    27413 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/models.py
+-rw-r--r--   0        0        0     7938 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/navigation.py
+-rw-r--r--   0        0        0     1148 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/signals.py
+-rw-r--r--   0        0        0    31978 2024-05-10 19:13:48.367522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/404.html
+-rw-r--r--   0        0        0    34883 2024-05-10 19:13:48.391522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    42537 2024-05-10 19:13:48.399522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/install.html
+-rw-r--r--   0        0        0    34205 2024-05-10 19:13:48.403522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    35112 2024-05-10 19:13:48.407522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_0.20.html
+-rw-r--r--   0        0        0    40839 2024-05-10 19:13:48.411522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_0.7.html
+-rw-r--r--   0        0        0    38346 2024-05-10 19:13:48.415522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_0.8.html
+-rw-r--r--   0        0        0    40174 2024-05-10 19:13:48.415522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_0.9.html
+-rw-r--r--   0        0        0    33651 2024-05-10 19:13:48.419522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    33875 2024-05-10 19:13:48.419522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_2.0.html
+-rw-r--r--   0        0        0    33979 2024-05-10 19:13:48.423522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/release_notes/version_2.1.html
+-rw-r--r--   0        0        0    37019 2024-05-10 19:13:48.399522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    35596 2024-05-10 19:13:48.403522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     5135 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-05-10 19:13:48.255522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0     9204 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   113505 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/stylesheets/main.26e3688c.min.css
+-rw-r--r--   0        0        0    38975 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/stylesheets/main.26e3688c.min.css.map
+-rw-r--r--   0        0        0    12245 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/stylesheets/palette.ecc896b0.min.css
+-rw-r--r--   0        0        0     3639 2024-05-10 19:13:48.259522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/assets/stylesheets/palette.ecc896b0.min.css.map
+-rw-r--r--   0        0        0   171578 2024-05-10 19:13:48.527522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    34139 2024-05-10 19:13:48.459522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0    49609 2024-05-10 19:13:48.535522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    41776 2024-05-10 19:13:48.427522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/contributing.html
+-rw-r--r--   0        0        0    97013 2024-05-10 19:13:48.447522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    34287 2024-05-10 19:13:48.447522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/extending.html
+-rw-r--r--   0        0        0    54496 2024-05-10 19:13:48.455522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/dev/models.html
+-rw-r--r--   0        0        0   189432 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/add_asn_12345.png
+-rw-r--r--   0        0        0   244087 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/add_external_peering.png
+-rw-r--r--   0        0        0   244888 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/add_internal_peering.png
+-rw-r--r--   0        0        0   216570 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/add_new_ri.png
+-rw-r--r--   0        0        0   191048 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/autonomous_system_01.png
+-rw-r--r--   0        0        0   279343 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/external_peering_created.png
+-rw-r--r--   0        0        0    74601 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/icon-nautobot-bgp-models.png
+-rw-r--r--   0        0        0   275694 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/internal_peering_created.png
+-rw-r--r--   0        0        0   295878 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/main-page-menu.png
+-rw-r--r--   0        0        0    53679 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/menu.png
+-rw-r--r--   0        0        0   284671 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/peer_endpoint_01.png
+-rw-r--r--   0        0        0   277452 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/peer_group_01.png
+-rw-r--r--   0        0        0   269366 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/peering_01.png
+-rw-r--r--   0        0        0   173632 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/peering_list.png
+-rw-r--r--   0        0        0   265084 2024-05-10 19:13:48.251522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/images/ri_list_view.png
+-rw-r--r--   0        0        0    41740 2024-05-10 19:13:48.391522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/index.html
+-rw-r--r--   0        0        0      579 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/objects.inv
+-rw-r--r--   0        0        0      120 2024-05-10 19:13:48.247522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/requirements.txt
+-rw-r--r--   0        0        0   117814 2024-05-10 19:13:48.599522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/search/search_index.json
+-rw-r--r--   0        0        0     5393 2024-05-10 19:13:48.371522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/sitemap.xml
+-rw-r--r--   0        0        0      438 2024-05-10 19:13:48.371522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    45576 2024-05-10 19:13:48.539522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    39764 2024-05-10 19:13:48.543522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/user/app_overview.html
+-rw-r--r--   0        0        0    40525 2024-05-10 19:13:48.547522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0   107572 2024-05-10 19:13:48.571522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/user/cisco_use_case.html
+-rw-r--r--   0        0        0    34193 2024-05-10 19:13:48.575522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/user/faq.html
+-rw-r--r--   0        0        0   107203 2024-05-10 19:13:48.599522 nautobot_bgp_models-2.1.0/nautobot_bgp_models/static/nautobot_bgp_models/docs/user/juniper_use_case.html
+-rw-r--r--   0        0        0    10169 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tables.py
+-rw-r--r--   0        0        0     2025 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/template_content.py
+-rw-r--r--   0        0        0     2261 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily_retrieve.html
+-rw-r--r--   0        0        0     1309 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem_retrieve.html
+-rw-r--r--   0        0        0     1366 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystemrange_retrieve.html
+-rw-r--r--   0        0        0     3741 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance_retrieve.html
+-rw-r--r--   0        0        0     1507 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html
+-rw-r--r--   0        0        0      761 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html
+-rw-r--r--   0        0        0      839 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html
+-rw-r--r--   0        0        0      918 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html
+-rw-r--r--   0        0        0      793 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html
+-rw-r--r--   0        0        0      876 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html
+-rw-r--r--   0        0        0     3146 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html
+-rw-r--r--   0        0        0     6326 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint_retrieve.html
+-rw-r--r--   0        0        0     3557 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpointaddressfamily_retrieve.html
+-rw-r--r--   0        0        0     6556 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup_retrieve.html
+-rw-r--r--   0        0        0     3128 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroupaddressfamily_retrieve.html
+-rw-r--r--   0        0        0     2782 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate_retrieve.html
+-rw-r--r--   0        0        0     2504 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_add.html
+-rw-r--r--   0        0        0     1085 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_retrieve.html
+-rw-r--r--   0        0        0       46 2024-05-10 19:13:24.319508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/__init__.py
+-rw-r--r--   0        0        0    54399 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_api.py
+-rw-r--r--   0        0        0     1042 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_basic.py
+-rw-r--r--   0        0        0    40247 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_filters.py
+-rw-r--r--   0        0        0    16172 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_forms.py
+-rw-r--r--   0        0        0     2759 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_helpers.py
+-rw-r--r--   0        0        0    20775 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_models.py
+-rw-r--r--   0        0        0    25283 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_views.py
+-rw-r--r--   0        0        0     2673 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/urls.py
+-rw-r--r--   0        0        0    11695 2024-05-10 19:13:24.323508 nautobot_bgp_models-2.1.0/nautobot_bgp_models/views.py
+-rw-r--r--   0        0        0     5866 2024-05-10 19:13:32.211517 nautobot_bgp_models-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5634 1970-01-01 00:00:00.000000 nautobot_bgp_models-2.1.0/PKG-INFO
```

### Comparing `nautobot_bgp_models-2.0.0/LICENSE` & `nautobot_bgp_models-2.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache Software License 2.0
 
-Copyright (c) 2021, Network to Code, LLC
+Copyright (c) 2024, Network to Code, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nautobot_bgp_models-2.0.0/README.md` & `nautobot_bgp_models-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BGP Models
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-bgp-models/develop/docs/images/icon-nautobot-bgp-models.png" class="logo" height="200px">
   <br>
   <a href="https://github.com/nautobot/nautobot-app-bgp-models/actions"><img src="https://github.com/nautobot/nautobot-app-bgp-models/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/bgp-models/en/latest"><img src="https://readthedocs.org/projects/nautobot-plugin-bgp-models/badge/"></a>
+  <a href="https://docs.nautobot.com/projects/bgp-models/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-bgp-models/badge/"></a>
   <a href="https://pypi.org/project/nautobot-bgp-models/"><img src="https://img.shields.io/pypi/v/nautobot-bgp-models"></a>
   <a href="https://pypi.org/project/nautobot-bgp-models/"><img src="https://img.shields.io/pypi/dm/nautobot-bgp-models"></a>
   <br>
   An <a href="https://www.networktocode.com/nautobot/apps/">App</a> for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
 
 ## Overview
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/__init__.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """App declaration for nautobot_bgp_models."""
 
+# Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
 from importlib import metadata
 
 from django.db.models.signals import post_migrate
-from nautobot.extras.plugins import PluginConfig
-
+from nautobot.apps import NautobotAppConfig
 
 __version__ = metadata.version(__name__)
 
 
-class NautobotBGPModelsConfig(PluginConfig):
+class NautobotBGPModelsConfig(NautobotAppConfig):
     """App configuration for the nautobot_bgp_models app."""
 
     name = "nautobot_bgp_models"
     verbose_name = "BGP Models"
     version = __version__
     author = "Network to Code, LLC"
     description = "Nautobot BGP Models App."
     base_url = "bgp"
     required_settings = []
     min_version = "2.0.3"
-    max_version = "2.999.999"
+    max_version = "2.9999"
     default_settings = {
         "default_statuses": {
             "AutonomousSystem": ["Active", "Available", "Planned"],
             "BGPRoutingInstance": ["Planned", "Active", "Decommissioned"],
             "Peering": ["Active", "Decommissioned", "Deprovisioning", "Offline", "Planned", "Provisioning"],
         }
     }
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/filter_backends.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/serializers.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,29 @@
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_bgp_models-api:autonomoussystem-detail")
 
     class Meta:
         model = models.AutonomousSystem
         fields = "__all__"
 
 
+class AutonomousSystemRangeSerializer(
+    NautobotModelSerializer,
+    TaggedModelSerializerMixin,
+):
+    """REST API serializer for AutonomousSystemRange records."""
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:nautobot_bgp_models-api:autonomoussystemrange-detail"
+    )
+
+    class Meta:
+        model = models.AutonomousSystemRange
+        fields = "__all__"
+
+
 class InheritableFieldsSerializerMixin:
     """Common mixin for Serializers that support an additional `include_inherited` query parameter."""
 
     def to_representation(self, instance):
         """Render the model instance to a Python dict.
 
         If `include_inherited` is specified as a request parameter, include inherited field values as appropriate.
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/urls.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from . import views
 
 # Use instead of rest_framework.routers.DefaultRouter so that we get bulk-update/bulk-delete features
 router = OrderedDefaultRouter()
 
 router.register("autonomous-systems", views.AutonomousSystemViewSet)
+router.register("autonomous-system-ranges", views.AutonomousSystemRangeViewSet)
 router.register("peer-groups", views.PeerGroupViewSet)
 router.register("peer-group-templates", views.PeerGroupTemplateViewSet)
 router.register("peer-endpoints", views.PeerEndpointViewSet)
 router.register("peerings", views.PeeringViewSet)
 router.register("address-families", views.AddressFamilyViewSet)
 router.register("peer-group-address-families", views.PeerGroupAddressFamilyViewSet)
 router.register("peer-endpoint-address-families", views.PeerEndpointAddressFamilyViewSet)
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/api/views.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/api/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,22 @@
     """REST API viewset for AutonomousSystem records."""
 
     queryset = models.AutonomousSystem.objects.all()
     serializer_class = serializers.AutonomousSystemSerializer
     filterset_class = filters.AutonomousSystemFilterSet
 
 
+class AutonomousSystemRangeViewSet(NautobotModelViewSet):
+    """REST API viewset for AutonomousSystemRange records."""
+
+    queryset = models.AutonomousSystemRange.objects.all()
+    serializer_class = serializers.AutonomousSystemRangeSerializer
+    filterset_class = filters.AutonomousSystemRangeFilterSet
+
+
 include_inherited = OpenApiParameter(
     name="include_inherited",
     required=False,
     location=OpenApiParameter.QUERY,
     description="Include inherited configuration values",
     type=OpenApiTypes.BOOL,
 )
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/choices.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/dolt_compat.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/dolt_compat.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/filter_extensions.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/filter_extensions.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/filters.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,40 @@
         return queryset.filter(Q(asn__icontains=value) | Q(description__icontains=value)).distinct()
 
     class Meta:
         model = models.AutonomousSystem
         fields = ["id", "asn", "status", "tags"]
 
 
+class AutonomousSystemRangeFilterSet(
+    BaseFilterSet,
+    CreatedUpdatedModelFilterSetMixin,
+    CustomFieldModelFilterSetMixin,
+):
+    """Filtering of AutonomousSystemRange records."""
+
+    q = django_filters.CharFilter(
+        method="search",
+        label="Search",
+    )
+
+    def search(self, queryset, name, value):  # pylint: disable=unused-argument
+        """Free-text search method implementation."""
+        if not value.strip():
+            return queryset
+
+        return queryset.filter(
+            Q(name=value) | Q(asn_max__icontains=value) | Q(asn_min__icontains=value) | Q(description__icontains=value)
+        ).distinct()
+
+    class Meta:
+        model = models.AutonomousSystemRange
+        fields = ["id", "name", "asn_min", "asn_max", "tags"]
+
+
 class BGPRoutingInstanceFilterSet(
     BaseFilterSet, CreatedUpdatedModelFilterSetMixin, CustomFieldModelFilterSetMixin, StatusModelFilterSetMixin
 ):
     """Filtering of BGPRoutingInstance records."""
 
     q = django_filters.CharFilter(
         method="search",
@@ -98,14 +124,28 @@
     routing_instance = django_filters.ModelMultipleChoiceFilter(
         field_name="routing_instance__id",
         queryset=models.BGPRoutingInstance.objects.all(),
         to_field_name="id",
         label="BGP Routing Instance ID",
     )
 
+    device = django_filters.ModelMultipleChoiceFilter(
+        field_name="routing_instance__device__name",
+        queryset=Device.objects.all(),
+        to_field_name="name",
+        label="Device (name)",
+    )
+
+    device_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="routing_instance__device__id",
+        queryset=Device.objects.all(),
+        to_field_name="id",
+        label="Device (ID)",
+    )
+
     class Meta:
         model = models.PeerGroup
         fields = ["id", "name", "enabled"]
 
     def search(self, queryset, name, value):  # pylint: disable=unused-argument
         """Free-text search method implementation."""
         if not value.strip():
@@ -150,14 +190,21 @@
     device = django_filters.ModelMultipleChoiceFilter(
         field_name="routing_instance__device__name",
         queryset=Device.objects.all(),
         to_field_name="name",
         label="Device (name)",
     )
 
+    device_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="routing_instance__device__id",
+        queryset=Device.objects.all(),
+        to_field_name="id",
+        label="Device (ID)",
+    )
+
     autonomous_system = django_filters.ModelMultipleChoiceFilter(
         field_name="autonomous_system__asn",
         queryset=models.AutonomousSystem.objects.all(),
         to_field_name="asn",
         label="Autonomous System Number",
     )
 
@@ -193,14 +240,21 @@
     device = django_filters.ModelMultipleChoiceFilter(
         field_name="endpoints__routing_instance__device__name",
         queryset=Device.objects.all(),
         to_field_name="name",
         label="Device (name)",
     )
 
+    device_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="endpoints__routing_instance__device__id",
+        queryset=Device.objects.all(),
+        to_field_name="id",
+        label="Device (ID)",
+    )
+
     device_role = django_filters.ModelMultipleChoiceFilter(
         field_name="endpoints__routing_instance__device__role__name",
         queryset=Role.objects.all(),
         to_field_name="name",
         label="Device Role (name)",
     )
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/forms.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TagsBulkEditFormMixin,
 )
 from nautobot.circuits.models import Provider
 from nautobot.dcim.models import Device, Interface
 from nautobot.extras.forms import NautobotFilterForm, RoleModelFilterFormMixin
 from nautobot.extras.models import Tag, Secret, Role
 from nautobot.ipam.models import VRF, IPAddress
+from nautobot.tenancy.models import Tenant
 
 from . import choices, models
 
 
 class AutonomousSystemForm(NautobotModelForm):
     """Form for creating/updating AutonomousSystem records."""
 
@@ -49,14 +50,47 @@
 
     class Meta:
         nullable_fields = [
             "description",
         ]
 
 
+class AutonomousSystemRangeForm(NautobotModelForm):
+    """Form for creating/updating AutonomousSystem records."""
+
+    tags = DynamicModelMultipleChoiceField(queryset=Tag.objects.all(), required=False)
+    tenant = DynamicModelChoiceField(queryset=Tenant.objects.all(), required=False)
+
+    class Meta:
+        model = models.AutonomousSystemRange
+        fields = ("name", "asn_min", "asn_max", "description", "tenant", "tags")
+
+
+class AutonomousSystemRangeFilterForm(NautobotFilterForm):
+    """Form for filtering AutonomousSystem records in combination with AutonomousSystemFilterSet."""
+
+    model = models.AutonomousSystemRange
+    field_order = ["name", "asn_min", "asn_max", "tenant", "tags"]
+    tag = TagFilterField(model)
+
+
+class AutonomousSystemRangeBulkEditForm(TagsBulkEditFormMixin, NautobotBulkEditForm):
+    """Form for bulk-editing multiple AutonomousSystem records."""
+
+    pk = forms.ModelMultipleChoiceField(
+        queryset=models.AutonomousSystemRange.objects.all(), widget=forms.MultipleHiddenInput()
+    )
+    description = forms.CharField(max_length=200, required=False)
+
+    class Meta:
+        nullable_fields = [
+            "description",
+        ]
+
+
 class BGPRoutingInstanceForm(NautobotModelForm):
     """Form for creating/updating BGPRoutingInstance records."""
 
     def __init__(self, *args, **kwargs):
         """Init."""
         super().__init__(*args, **kwargs)
 
@@ -258,14 +292,15 @@
         fields = (
             "name",
             "description",
             "enabled",
             "role",
             "autonomous_system",
             "extra_attributes",
+            "tags",
         )
 
 
 class PeerGroupTemplateBulkEditForm(NautobotBulkEditForm):
     """Form for bulk-editing multiple PeerGroupTemplate records."""
 
     pk = forms.ModelMultipleChoiceField(
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0001_initial.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0002_viewsets_migration.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0002_viewsets_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0003_peergroupaddressfamily_peerendpointaddressfamily.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0003_peergroupaddressfamily_peerendpointaddressfamily.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0004_use_upstream_role_part1.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0004_use_upstream_role_part1.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0005_use_upstream_role_part2.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0005_use_upstream_role_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0006_use_upstream_role_part3.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0006_use_upstream_role_part3.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0007_use_upstream_role_part4.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0007_use_upstream_role_part4.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/migrations/0008_nautobotv2_updates.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/migrations/0008_nautobotv2_updates.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/models.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nautobot.circuits.models import Provider
 from nautobot.core.models.generics import PrimaryModel, OrganizationalModel
 from nautobot.dcim.fields import ASNField
 from nautobot.extras.models import StatusModel, RoleField
 from nautobot.apps.models import extras_features
 from nautobot.ipam.models import IPAddress, IPAddressToInterface
 from nautobot.core.utils.data import deepmerge
+from nautobot.tenancy.models import Tenant
 
 from nautobot_bgp_models.choices import AFISAFIChoices
 
 
 def rgetattr(obj, attr, *args):
     """Recursive getattr helper."""
 
@@ -144,14 +145,57 @@
 
 
 @extras_features(
     "custom_fields",
     "custom_links",
     "custom_validators",
     "export_templates",
+    "graphql",
+    "relationships",
+    "webhooks",
+)
+class AutonomousSystemRange(PrimaryModel):
+    """Autonomous System Range information."""
+
+    name = models.CharField(max_length=255, unique=True, blank=False)
+    asn_min = ASNField(verbose_name="Start", help_text="Min value for 32-bit autonomous system number")
+    asn_max = ASNField(verbose_name="End", help_text="Max value for 32-bit autonomous system number")
+    description = models.CharField(max_length=255, blank=True)
+    tenant = models.ForeignKey(to=Tenant, on_delete=models.PROTECT, blank=True, null=True)
+
+    class Meta:
+        ordering = ["asn_min"]
+        verbose_name = "Autonomous System Range"
+
+    def __str__(self):
+        """String representation of an AutonomousSystemRange."""
+        return f"ASN Range {self.asn_min}-{self.asn_max}"
+
+    def clean(self):
+        """Clean."""
+        if self.asn_min >= self.asn_max:
+            raise ValidationError("asn_min value must be lower than asn_max value.")
+
+    def get_next_available_asn(self):
+        """Return the first available ASN number in the range, or None if none are available."""
+        asn_nums = AutonomousSystem.objects.filter(asn__gte=self.asn_min, asn__lte=self.asn_max).values_list(
+            "asn", flat=True
+        )
+        for i in range(self.asn_min, self.asn_max + 1):
+            if i not in asn_nums:
+                return i
+
+        return None
+
+
+@extras_features(
+    "custom_fields",
+    "custom_links",
+    "custom_validators",
+    "export_templates",
     "graphql",
     "relationships",
     "statuses",
     "webhooks",
 )
 class BGPRoutingInstance(PrimaryModel, StatusModel, BGPExtraAttributesMixin):
     """BGP instance definition."""
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/navigation.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/navigation.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,29 @@
                             NavMenuImportButton(
                                 link="plugins:nautobot_bgp_models:autonomoussystem_import",
                                 permissions=["nautobot_bgp_models.add_autonomoussystem"],
                             ),
                         ),
                     ),
                     NavMenuItem(
+                        link="plugins:nautobot_bgp_models:autonomoussystemrange_list",
+                        name="Autonomous System Ranges",
+                        permissions=["nautobot_bgp_models.view_autonomoussystemrange"],
+                        buttons=(
+                            NavMenuAddButton(
+                                link="plugins:nautobot_bgp_models:autonomoussystemrange_add",
+                                permissions=["nautobot_bgp_models.add_autonomoussystemrange"],
+                            ),
+                            NavMenuImportButton(
+                                link="plugins:nautobot_bgp_models:autonomoussystemrange_import",
+                                permissions=["nautobot_bgp_models.add_autonomoussystemrange"],
+                            ),
+                        ),
+                    ),
+                    NavMenuItem(
                         link="plugins:nautobot_bgp_models:peergrouptemplate_list",
                         name="Peer Group Templates",
                         permissions=["nautobot_bgp_models.view_peergrouptemplate"],
                         buttons=(
                             NavMenuAddButton(
                                 link="plugins:nautobot_bgp_models:peergrouptemplate_add",
                                 permissions=["nautobot_bgp_models.add_peergrouptemplate"],
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/signals.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/tables.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,29 +11,58 @@
     TagColumn,
     ToggleColumn,
     StatusTableMixin,
 )
 
 from . import models
 
+ASN_LINK = """
+{% if record.present_in_database %}
+<a href="{{ record.get_absolute_url }}">{{ record.asn }}</a>
+{% elif perms.nautobot_bgp_models.autonomoussystem_add %}
+<a href="\
+{% url 'plugins:nautobot_bgp_models:autonomoussystem_add' %}\
+?asn={{ record.asn }}\
+" class="btn btn-xs btn-success">{{ record.available }} ASN{{ record.available|pluralize }} available</a>\
+{% else %}
+{{ record.available }} ASN{{ record.available|pluralize }} available
+{% endif %}
+"""
+
 
 class AutonomousSystemTable(StatusTableMixin, BaseTable):
     """Table representation of AutonomousSystem records."""
 
     pk = ToggleColumn()
-    asn = tables.LinkColumn()
+    asn = tables.TemplateColumn(template_code=ASN_LINK, verbose_name="ASN")
     provider = tables.LinkColumn()
     tags = TagColumn(url_name="plugins:nautobot_bgp_models:autonomoussystem_list")
     actions = ButtonsColumn(model=models.AutonomousSystem)
 
     class Meta(BaseTable.Meta):
         model = models.AutonomousSystem
         fields = ("pk", "asn", "status", "provider", "description", "tags")
 
 
+class AutonomousSystemRangeTable(StatusTableMixin, BaseTable):
+    """Table representation of AutonomousSystem records."""
+
+    pk = ToggleColumn()
+    name = tables.LinkColumn()
+    asn_min = tables.LinkColumn()
+    asn_max = tables.LinkColumn()
+    tenant = tables.LinkColumn()
+    tags = TagColumn(url_name="plugins:nautobot_bgp_models:autonomoussystemrange_list")
+    actions = ButtonsColumn(model=models.AutonomousSystemRange)
+
+    class Meta(BaseTable.Meta):
+        model = models.AutonomousSystemRange
+        fields = ("pk", "name", "asn_min", "asn_max", "tenant", "description", "tags")
+
+
 class BGPRoutingInstanceTable(StatusTableMixin, BaseTable):
     """Table representation of BGPRoutingInstance records."""
 
     pk = ToggleColumn()
     routing_instance = tables.LinkColumn(
         viewname="plugins:nautobot_bgp_models:bgproutinginstance",
         args=[A("pk")],
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/template_content.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpointaddressfamily_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpointaddressfamily_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroupaddressfamily_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroupaddressfamily_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_add.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_add.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_retrieve.html` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_api.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,43 @@
         cls.create_data = [
             {"asn": 64496, "status": status_active.pk},
             {"asn": 65551, "status": status_active.pk},
             {"asn": 4294967294, "status": status_active.pk, "description": "Reserved for private use"},
         ]
 
 
+class AutonomousSystemRangeAPITestCase(APIViewTestCases.APIViewTestCase):
+    """Test the AutonomousSystemRange API."""
+
+    model = models.AutonomousSystemRange
+    view_namespace = "plugins-api:nautobot_bgp_models"
+    bulk_update_data = {
+        "description": "Reserved for use in documentation/sample code",
+    }
+    choices_fields = []
+
+    @classmethod
+    def setUpTestData(cls):
+        models.AutonomousSystemRange.objects.create(
+            name="Test 1", asn_min=100, asn_max=200, description="Test Description 1"
+        )
+        models.AutonomousSystemRange.objects.create(
+            name="Test 2", asn_min=201, asn_max=300, description="Test Description 2"
+        )
+        models.AutonomousSystemRange.objects.create(
+            name="Test 3", asn_min=301, asn_max=400, description="Test Description 3"
+        )
+
+        cls.create_data = [
+            {"name": "Test 4", "asn_min": 401, "asn_max": 500, "description": "Test 4"},
+            {"name": "Test 5", "asn_min": 501, "asn_max": 600, "description": "Test 5"},
+            {"name": "Test 6", "asn_min": 601, "asn_max": 700, "description": "Test 6"},
+        ]
+
+
 class PeerGroupTemplateAPITestCase(APIViewTestCases.APIViewTestCase):
     """Test the PeerGroupTemplate API."""
 
     model = models.PeerGroupTemplate
     view_namespace = "plugins-api:nautobot_bgp_models"
 
     # TODO(mzb): Fix bulk update via #96 - ViewSets migration
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_filters.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,53 @@
 
     def test_status(self):
         """Test filtering by status."""
         params = {"status": [self.status_primary_asn.name, self.status_remote_asn.name]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
 
+class AutonomousSystemRangeTestCase(TestCase):
+    """Test filtering of AutonomousSystemRange records."""
+
+    queryset = models.AutonomousSystemRange.objects.all()
+    filterset = filters.AutonomousSystemRangeFilterSet
+
+    @classmethod
+    def setUpTestData(cls):
+        """One-time class setup to prepopulate required data for tests."""
+        cls.asn_range_1 = models.AutonomousSystemRange.objects.create(
+            name="Public asns", asn_min=100, asn_max=125, description="Test Range 1"
+        )
+
+        cls.asn_range_2 = models.AutonomousSystemRange.objects.create(
+            name="DC asns", asn_min=1000, asn_max=2000, description="asns for dc"
+        )
+
+        cls.asn_range_3 = models.AutonomousSystemRange.objects.create(
+            name="DC asns 2", asn_min=2001, asn_max=3000, description="asns for dc"
+        )
+
+    def test_id(self):
+        """Test filtering by ID."""
+        params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_name(self):
+        """Test filtering by Name."""
+        params = {"name": ["DC asns", "DC asns 2"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_min_max(self):
+        """Test filtering by ASN Min."""
+        params = {"asn_min": [1000]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+        params = {"asn_max": [3000]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 1)
+
+
 class PeerGroupTestCase(TestCase):
     """Test filtering of PeerGroup records."""
 
     queryset = models.PeerGroup.objects.all()
     filterset = filters.PeerGroupFilterSet
 
     @classmethod
@@ -75,86 +114,113 @@
         location_status = Status.objects.get_for_model(Location).first()
         location = Location.objects.create(name="Site 1", location_type=location_type, status=location_status)
         devicerole = Role.objects.create(name="Router", color="ff0000")
         devicerole.content_types.add(ContentType.objects.get_for_model(Device))
         cls.device_1 = Device.objects.create(
             device_type=devicetype, role=devicerole, name="Device 1", location=location, status=status_active
         )
+        cls.device_2 = Device.objects.create(
+            device_type=devicetype, role=devicerole, name="Device 2", location=location, status=status_active
+        )
 
         cls.asn_1 = models.AutonomousSystem.objects.create(asn=4294967294, status=status_active)
         asn_2 = models.AutonomousSystem.objects.create(asn=4294967295, status=status_active)
 
         cls.peeringrole_internal = Role.objects.create(name="Internal", color="333333")
         cls.peeringrole_internal.content_types.add(ContentType.objects.get_for_model(models.PeerGroup))
         peeringrole_external = Role.objects.create(name="External", color="ffffff")
         peeringrole_external.content_types.add(ContentType.objects.get_for_model(models.PeerGroup))
 
-        cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
+        cls.bgp_routing_instance_1 = models.BGPRoutingInstance.objects.create(
             description="Hello World!",
             autonomous_system=cls.asn_1,
             device=cls.device_1,
             status=status_active,
         )
+        cls.bgp_routing_instance_2 = models.BGPRoutingInstance.objects.create(
+            description="Hello World!",
+            autonomous_system=asn_2,
+            device=cls.device_2,
+            status=status_active,
+        )
 
         models.PeerGroup.objects.create(
-            routing_instance=cls.bgp_routing_instance,
+            routing_instance=cls.bgp_routing_instance_1,
             name="Group A",
             role=cls.peeringrole_internal,
             autonomous_system=cls.asn_1,
             description="Internal Group",
         )
         models.PeerGroup.objects.create(
-            routing_instance=cls.bgp_routing_instance,
+            routing_instance=cls.bgp_routing_instance_1,
             name="Group B",
             role=peeringrole_external,
             autonomous_system=cls.asn_1,
             enabled=False,
             description="External Group",
         )
         models.PeerGroup.objects.create(
-            routing_instance=cls.bgp_routing_instance,
+            routing_instance=cls.bgp_routing_instance_1,
+            name="Group C",
+            role=cls.peeringrole_internal,
+            autonomous_system=asn_2,
+            description="Internal Group",
+            # vrf=cls.vrf
+        )
+        models.PeerGroup.objects.create(
+            routing_instance=cls.bgp_routing_instance_2,
             name="Group C",
             role=cls.peeringrole_internal,
             autonomous_system=asn_2,
             description="Internal Group",
             # vrf=cls.vrf
         )
 
     def test_search(self):
         """Test text search."""
         # Match on name (case-insensitive)
         self.assertEqual(self.filterset({"q": "Group A"}, self.queryset).qs.count(), 1)
         self.assertEqual(self.filterset({"q": "group a"}, self.queryset).qs.count(), 1)
-        self.assertEqual(self.filterset({"q": "Internal Group"}, self.queryset).qs.count(), 2)
+        self.assertEqual(self.filterset({"q": "Internal Group"}, self.queryset).qs.count(), 3)
         self.assertEqual(self.filterset({"q": "External Group"}, self.queryset).qs.count(), 1)
 
     def test_id(self):
         """Test filtering by ID (primary key)."""
         params = {"id": self.queryset.values_list("pk", flat=True)[:2]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_enabled(self):
         """Test filtering by enabled status."""
         params = {"enabled": True}
-        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+    def test_device(self):
+        """Test filtering by device name."""
+        params = {"device": [self.device_1.name]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+    def test_device_id(self):
+        """Test filtering by device ID."""
+        params = {"device_id": [self.device_1.id]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
 
     def test_role(self):
         """Test filtering by peering role."""
         params = {"role": [self.peeringrole_internal.name]}
-        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
 
     def test_autonomous_system(self):
         """Test filtering by autonomous system."""
         params = {"autonomous_system": [4294967294]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_routing_instance(self):
         """Test Routing Instance."""
         self.assertEqual(
-            self.filterset({"routing_instance": self.bgp_routing_instance.pk}, self.queryset).qs.count(), 3
+            self.filterset({"routing_instance": [self.bgp_routing_instance_1.pk]}, self.queryset).qs.count(), 3
         )
 
 
 class PeerEndpointTestCase(TestCase):
     """Test filtering of PeerEndpoint records."""
 
     queryset = models.PeerEndpoint.objects.all()
@@ -176,24 +242,24 @@
         manufacturer = Manufacturer.objects.create(name="Cisco")
         cls.devicetype = DeviceType.objects.create(manufacturer=manufacturer, model="CSR 1000V")
         location_type = LocationType.objects.create(name="site")
         location_status = Status.objects.get_for_model(Location).first()
         cls.location = Location.objects.create(name="Site 1", location_type=location_type, status=location_status)
         cls.devicerole = Role.objects.create(name="Router", color="ff0000")
         cls.devicerole.content_types.add(ContentType.objects.get_for_model(Device))
-        device = Device.objects.create(
+        cls.device = Device.objects.create(
             device_type=cls.devicetype,
             role=cls.devicerole,
             name="Device 1",
             location=cls.location,
             status=status_active,
         )
         interface_status = Status.objects.get_for_model(Interface).first()
         interface = Interface.objects.create(
-            device=device, name="Loopback1", type=InterfaceTypeChoices.TYPE_VIRTUAL, status=interface_status
+            device=cls.device, name="Loopback1", type=InterfaceTypeChoices.TYPE_VIRTUAL, status=interface_status
         )
 
         namespace = Namespace.objects.first()
         prefix_status = Status.objects.get_for_model(Prefix).first()
         Prefix.objects.create(prefix="1.0.0.0/8", namespace=namespace, status=prefix_status)
 
         addresses = [
@@ -203,15 +269,15 @@
         ]
 
         interface.add_ip_addresses([addresses[0], addresses[1]])
 
         cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
             description="Hello World!",
             autonomous_system=asn,
-            device=device,
+            device=cls.device,
             status=status_active,
         )
 
         cls.peergroup = models.PeerGroup.objects.create(
             name="Group B",
             role=peeringrole,
             routing_instance=cls.bgp_routing_instance,
@@ -262,14 +328,24 @@
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_peer_group(self):
         """Test filtering by peer-group."""
         params = {"peer_group": [self.peergroup.pk]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
+    def test_device(self):
+        """Test filtering by device name."""
+        params = {"device": ["Device 1"]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+    def test_device_id(self):
+        """Test filtering by device ID."""
+        params = {"device_id": [self.device.pk]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
 
 class PeeringTestCase(TestCase):
     """Test filtering of Peering records."""
 
     queryset = models.Peering.objects.all()
     filterset = filters.PeeringFilterSet
 
@@ -291,51 +367,51 @@
         manufacturer = Manufacturer.objects.create(name="Cisco")
         devicetype = DeviceType.objects.create(manufacturer=manufacturer, model="CSR 1000V")
         location_type = LocationType.objects.create(name="site")
         location_status = Status.objects.get_for_model(Location).first()
         location = Location.objects.create(name="Site 1", location_type=location_type, status=location_status)
         devicerole_router = Role.objects.create(name="Router", color="ff0000")
         devicerole_switch = Role.objects.create(name="Switch", color="ff0000")
-        device1 = Device.objects.create(
+        cls.device1 = Device.objects.create(
             device_type=devicetype,
             role=devicerole_router,
             name="device1",
             location=location,
             status=status_active,
         )
-        device2 = Device.objects.create(
+        cls.device2 = Device.objects.create(
             device_type=devicetype,
             role=devicerole_switch,
             name="device2",
             location=location,
             status=status_active,
         )
         cls.bgp_routing_instance = models.BGPRoutingInstance.objects.create(
             description="Device 1 RI",
             autonomous_system=asn1,
-            device=device1,
+            device=cls.device1,
             status=status_active,
         )
 
         cls.bgp_routing_instance_device_2 = models.BGPRoutingInstance.objects.create(
             description="Device 2 RI",
             autonomous_system=asn1,
-            device=device2,
+            device=cls.device2,
             status=status_active,
         )
 
         interface_status = Status.objects.get_for_model(Interface).first()
         interfaces_device1 = [
-            Interface.objects.create(device=device1, name="Loopback0", status=interface_status),
-            Interface.objects.create(device=device1, name="Loopback1", status=interface_status),
-            Interface.objects.create(device=device1, name="Loopback2", status=interface_status),
+            Interface.objects.create(device=cls.device1, name="Loopback0", status=interface_status),
+            Interface.objects.create(device=cls.device1, name="Loopback1", status=interface_status),
+            Interface.objects.create(device=cls.device1, name="Loopback2", status=interface_status),
         ]
         interfaces_device2 = [
-            Interface.objects.create(device=device2, name="Loopback0", status=interface_status),
-            Interface.objects.create(device=device2, name="Loopback1", status=interface_status),
+            Interface.objects.create(device=cls.device2, name="Loopback0", status=interface_status),
+            Interface.objects.create(device=cls.device2, name="Loopback1", status=interface_status),
         ]
 
         namespace = Namespace.objects.first()
         prefix_status = Status.objects.get_for_model(Prefix).first()
         Prefix.objects.create(prefix="10.0.0.0/8", namespace=namespace, status=prefix_status)
 
         addresses = [
@@ -515,14 +591,25 @@
 
         params = {"device": ["device2"]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
         params = {"device": ["device1", "device2"]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 5)
 
+    def test_device_id(self):
+        """Test filtering by device id."""
+        params = {"device_id": [self.device1.id]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
+
+        params = {"device_id": [self.device2.id]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
+
+        params = {"device_id": [self.device1.pk, self.device2.id]}
+        self.assertEqual(self.filterset(params, self.queryset).qs.count(), 5)
+
     def test_device_role(self):
         """Test filtering by device role name."""
         params = {"device_role": ["Router"]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 3)
 
         params = {"device_role": ["Switch"]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_forms.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,42 @@
     def test_status_required(self):
         data = {"asn": 4200000001}
         form = self.form_class(data)
         self.assertFalse(form.is_valid())
         self.assertEqual("This field is required.", form.errors["status"][0])
 
 
+class AutonomousSystemRangeFormTestCase(TestCase):
+    """Test the AutonomousSystemRange create/edit form."""
+
+    form_class = forms.AutonomousSystemRangeForm
+
+    @classmethod
+    def setUpTestData(cls):
+        """Set up class-wide data for the test."""
+
+    def test_valid_asnrange(self):
+        data = {"asn_min": 1, "asn_max": 10, "name": "test"}
+        form = self.form_class(data)
+        self.assertTrue(form.is_valid())
+        self.assertTrue(form.save())
+
+    def test_invalid_asn(self):
+        data = {"asn_min": 10, "asn_max": 1, "name": "test"}
+        form = self.form_class(data)
+        self.assertFalse(form.is_valid())
+        self.assertEqual("asn_min value must be lower than asn_max value.", form.errors["__all__"][0])
+
+    def test_name_required(self):
+        data = {"asn_min": 1000, "asn_max": 2000}
+        form = self.form_class(data)
+        self.assertFalse(form.is_valid())
+        self.assertEqual("This field is required.", form.errors["name"][0])
+
+
 class BGPRoutingInstanceTestCase(TestCase):
     """Test the BGPRoutingInstance create/edit form."""
 
     form_class = forms.BGPRoutingInstanceForm
 
     @classmethod
     def setUpTestData(cls):
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_models.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,54 @@
         )
 
     def test_str(self):
         """Test string representation of an AutonomousSystem."""
         self.assertEqual(str(self.autonomous_system), "AS 15521")
 
 
+class AutonomousSystemRangeTestCase(TestCase):
+    """Test the AutonomousSystemRange model."""
+
+    @classmethod
+    def setUpTestData(cls):
+        """One-time class data setup."""
+        status_active = Status.objects.get(name__iexact="active")
+        status_active.content_types.add(ContentType.objects.get_for_model(models.AutonomousSystem))
+
+        cls.autonomous_system_100 = models.AutonomousSystem.objects.create(
+            asn=100, status=status_active, description="AS100"
+        )
+        cls.autonomous_system_101 = models.AutonomousSystem.objects.create(
+            asn=101, status=status_active, description="AS101"
+        )
+        cls.autonomous_system_120 = models.AutonomousSystem.objects.create(
+            asn=120, status=status_active, description="AS120"
+        )
+        cls.autonomous_system_150 = models.AutonomousSystem.objects.create(
+            asn=150, status=status_active, description="AS150"
+        )
+        cls.asn_range = models.AutonomousSystemRange.objects.create(
+            name="Test Range", asn_min=100, asn_max=125, description="Test Range"
+        )
+
+    def test_str(self):
+        """Test string representation of an AutonomousSystemRange."""
+        self.assertEqual(str(self.asn_range), "ASN Range 100-125")
+
+    def test_max_gt_min(self):
+        with self.assertRaises(ValidationError) as context:
+            self.asn_range.asn_min = 100
+            self.asn_range.asn_max = 90
+            self.asn_range.validated_save()
+        self.assertIn(
+            "asn_min value must be lower than asn_max value.",
+            context.exception.messages[0],
+        )
+
+
 class BGPRoutingInstanceTestCase(TestCase):
     """Test the BGPRoutingInstance model."""
 
     @classmethod
     def setUpTestData(cls):
         """One-time class data setup."""
         cls.status_active = Status.objects.get(name__iexact="active")
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/tests/test_views.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,54 @@
         )
 
         cls.bulk_edit_data = {
             "description": "New description",
         }
 
 
+class AutonomousSystemRangeTestCase(ViewTestCases.PrimaryObjectViewTestCase):
+    """Test views related to the AutonomousSystemRange model."""
+
+    model = models.AutonomousSystemRange
+
+    @classmethod
+    def setUpTestData(cls):
+        """One-time class data setup."""
+        models.AutonomousSystemRange.objects.create(
+            asn_min=1, asn_max=10, name="Private", description="Reserved for private use"
+        )
+        models.AutonomousSystemRange.objects.create(
+            asn_min=11, asn_max=20, name="Private 2", description="Also reserved for private use"
+        )
+        models.AutonomousSystemRange.objects.create(
+            asn_min=21, asn_max=30, name="Private 3", description="Another reserved for private use"
+        )
+
+        tags = cls.create_tags("Alpha", "Beta", "Gamma")
+
+        cls.form_data = {
+            "name": "Hello World",
+            "asn_min": 100,
+            "asn_max": 500,
+            "description": "Hello, world!",
+            "tags": [tag.pk for tag in tags],
+        }
+
+        cls.csv_data = (
+            "asn_min,asn_max,name,description",
+            "1000,2000,range1,range1 descr",
+            "2000,4000,range2,range2 descr",
+            "5000,9999,range3,range3 descr",
+        )
+
+        cls.bulk_edit_data = {
+            "description": "New description",
+        }
+
+
 class PeerGroupTestCase(
     ViewTestCases.GetObjectViewTestCase,
     ViewTestCases.GetObjectChangelogViewTestCase,
     ViewTestCases.CreateObjectViewTestCase,
     ViewTestCases.EditObjectViewTestCase,
     ViewTestCases.DeleteObjectViewTestCase,
     ViewTestCases.ListObjectsViewTestCase,
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/urls.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from nautobot.core.views.routers import NautobotUIViewSetRouter
 
 from . import models, views
 
 router = NautobotUIViewSetRouter()
 router.register("autonomous-systems", views.AutonomousSystemUIViewSet)
+router.register("autonomous-system-ranges", views.AutonomousSystemRangeUIViewSet)
 router.register("routing-instances", views.BGPRoutingInstanceUIViewSet)
 router.register("peer-groups", views.PeerGroupUIViewSet)
 router.register("peer-group-templates", views.PeerGroupTemplateUIViewSet)
 router.register("peer-endpoints", views.PeerEndpointUIViewSet)
 router.register("peerings", views.PeeringUIViewSet)
 router.register("address-families", views.AddressFamilyUIViewSet)
 router.register("peer-group-address-families", views.PeerGroupAddressFamilyUIViewSet)
```

### Comparing `nautobot_bgp_models-2.0.0/nautobot_bgp_models/views.py` & `nautobot_bgp_models-2.1.0/nautobot_bgp_models/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """View classes for nautobot_bgp_models."""
 
 from django.core.exceptions import ValidationError
 from django.db import transaction
 from django.shortcuts import get_object_or_404, redirect, render
 from django.views.generic import View
+from django_tables2 import RequestConfig
 
 from nautobot.apps.views import NautobotUIViewSet
 from nautobot.core.views import mixins
 from nautobot.core.views import generic
 from nautobot.extras.utils import get_base_template
+from nautobot.core.views.paginator import EnhancedPaginator, get_paginate_count
 
-from . import filters, forms, models, tables
+from . import filters, forms, helpers, models, tables
 from .api import serializers
 
 
 class AutonomousSystemUIViewSet(NautobotUIViewSet):
     """UIViewset for AutonomousSystem model."""
 
     bulk_update_form_class = forms.AutonomousSystemBulkEditForm
@@ -23,14 +25,53 @@
     form_class = forms.AutonomousSystemForm
     lookup_field = "pk"
     queryset = models.AutonomousSystem.objects.all()
     serializer_class = serializers.AutonomousSystemSerializer
     table_class = tables.AutonomousSystemTable
 
 
+class AutonomousSystemRangeUIViewSet(NautobotUIViewSet):
+    """UIViewset for AutonomousSystemRange model."""
+
+    bulk_update_form_class = forms.AutonomousSystemRangeBulkEditForm
+    filterset_class = filters.AutonomousSystemRangeFilterSet
+    filterset_form_class = forms.AutonomousSystemRangeFilterForm
+    form_class = forms.AutonomousSystemRangeForm
+    lookup_field = "pk"
+    queryset = models.AutonomousSystemRange.objects.all()
+    serializer_class = serializers.AutonomousSystemRangeSerializer
+    table_class = tables.AutonomousSystemRangeTable
+
+    def get_extra_context(self, request, instance):  # pylint: disable=signature-differs
+        """Return any additional context data for the template."""
+        context = super().get_extra_context(request, instance)
+        if self.action == "retrieve":
+            asns = models.AutonomousSystem.objects.filter(asn__gte=instance.asn_min, asn__lte=instance.asn_max)
+            asns = helpers.add_available_asns(instance, asns)
+
+            asn_table = tables.AutonomousSystemTable(asns)
+            asn_table.columns.hide("actions")
+
+            if request.user.has_perm("nautobot_bgp_models.change_autonomoussystem") or request.user.has_perm(
+                "nautobot_bgp_models.delete_autonomoussystem"
+            ):
+                asn_table.columns.show("pk")
+
+            paginate = {
+                "paginator_class": EnhancedPaginator,
+                "per_page": get_paginate_count(request),
+            }
+
+            RequestConfig(request, paginate).configure(asn_table)
+
+            context["asn_range_table"] = asn_table
+
+        return context
+
+
 class BGPRoutingInstanceUIViewSet(NautobotUIViewSet):
     """UIViewset for BGPRoutingInstance model."""
 
     bulk_update_form_class = forms.BGPRoutingInstanceBulkEditForm
     filterset_class = filters.BGPRoutingInstanceFilterSet
     filterset_form_class = forms.BGPRoutingInstanceFilterForm
     form_class = forms.BGPRoutingInstanceForm
```

### Comparing `nautobot_bgp_models-2.0.0/PKG-INFO` & `nautobot_bgp_models-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: nautobot-bgp-models
-Version: 2.0.0
+Version: 2.1.0
 Summary: Nautobot BGP Models App
 Home-page: https://github.com/nautobot/nautobot-app-bgp-models
 License: Apache-2.0
-Keywords: nautobot,nautobot-plugin,nautobot-app
+Keywords: nautobot,nautobot-app,nautobot-plugin
 Author: Network to Code, LLC
-Author-email: info@networktocode.com
+Author-email: opensource@networktocode.com
 Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Requires-Dist: nautobot (>=2.0.3,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://docs.nautobot.com/projects/bgp-models/en/latest/
 Project-URL: Repository, https://github.com/nautobot/nautobot-app-bgp-models
 Description-Content-Type: text/markdown
 
 # BGP Models
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-bgp-models/develop/docs/images/icon-nautobot-bgp-models.png" class="logo" height="200px">
   <br>
   <a href="https://github.com/nautobot/nautobot-app-bgp-models/actions"><img src="https://github.com/nautobot/nautobot-app-bgp-models/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/bgp-models/en/latest"><img src="https://readthedocs.org/projects/nautobot-plugin-bgp-models/badge/"></a>
+  <a href="https://docs.nautobot.com/projects/bgp-models/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-bgp-models/badge/"></a>
   <a href="https://pypi.org/project/nautobot-bgp-models/"><img src="https://img.shields.io/pypi/v/nautobot-bgp-models"></a>
   <a href="https://pypi.org/project/nautobot-bgp-models/"><img src="https://img.shields.io/pypi/dm/nautobot-bgp-models"></a>
   <br>
   An <a href="https://www.networktocode.com/nautobot/apps/">App</a> for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1 Name: nautobot-bgp-models Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: nautobot-bgp-models Version: 2.1.0 Summary:
 Nautobot BGP Models App Home-page: https://github.com/nautobot/nautobot-app-
-bgp-models License: Apache-2.0 Keywords: nautobot,nautobot-plugin,nautobot-app
-Author: Network to Code, LLC Author-email: info@networktocode.com Requires-
-Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: nautobot (>=2.0.3,<3.0.0) Requires-
-Dist: toml (>=0.10.2,<0.11.0) Project-URL: Repository, https://github.com/
-nautobot/nautobot-app-bgp-models Description-Content-Type: text/markdown # BGP
-Models
+bgp-models License: Apache-2.0 Keywords: nautobot,nautobot-app,nautobot-plugin
+Author: Network to Code, LLC Author-email: opensource@networktocode.com
+Requires-Python: >=3.8,<3.12 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
+Requires-Dist: nautobot (>=2.0.3,<3.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://docs.nautobot.com/projects/bgp-models/en/
+latest/ Project-URL: Repository, https://github.com/nautobot/nautobot-app-bgp-
+models Description-Content-Type: text/markdown # BGP Models
  [https://raw.githubusercontent.com/nautobot/nautobot-app-bgp-models/develop/
                    docs/images/icon-nautobot-bgp-models.png]
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_b_g_p_-_m_o_d_e_l_s_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/
  _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_b_g_p_-
   _m_o_d_e_l_s_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_b_g_p_-_m_o_d_e_l_s_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_b_g_p_-_m_o_d_e_l_s_]
                              An _A_p_p for _N_a_u_t_o_b_o_t.
```

