# Comparing `tmp/fabric_fim-1.6.2.tar.gz` & `tmp/fabric_fim-1.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.6.2.tar", last modified: Thu Feb 22 14:37:14 2024, max compression
+gzip compressed data, was "fabric_fim-1.7.0b1.tar", last modified: Fri May 10 20:46:41 2024, max compression
```

## Comparing `fabric_fim-1.6.2.tar` & `fabric_fim-1.7.0b1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     2208 2024-01-11 18:55:34.270187 fabric_fim-1.6.2/.gitignore
--rw-r--r--   0        0        0       26 2024-01-11 18:55:34.270301 fabric_fim-1.6.2/AUTHORS
--rw-r--r--   0        0        0     1071 2024-01-11 18:55:34.270496 fabric_fim-1.6.2/LICENSE
--rw-r--r--   0        0        0    11110 2024-01-11 18:55:34.270710 fabric_fim-1.6.2/README.md
--rw-r--r--   0        0        0    18690 2024-01-11 18:55:34.270959 fabric_fim-1.6.2/figs/fim-structure.png
--rw-r--r--   0        0        0      557 2024-01-11 18:55:34.271160 fabric_fim-1.6.2/fim/README.md
--rw-r--r--   0        0        0      103 2024-02-22 14:12:08.267541 fabric_fim-1.6.2/fim/__init__.py
--rw-r--r--   0        0        0        1 2024-01-11 18:55:34.271390 fabric_fim-1.6.2/fim/authz/__init__.py
--rw-r--r--   0        0        0    16139 2024-01-11 18:55:34.271567 fabric_fim-1.6.2/fim/authz/attribute_collector.py
--rw-r--r--   0        0        0      334 2024-01-11 18:55:34.271711 fabric_fim-1.6.2/fim/graph/README.md
--rw-r--r--   0        0        0        1 2024-01-11 18:55:34.271818 fabric_fim-1.6.2/fim/graph/__init__.py
--rw-r--r--   0        0        0    69855 2024-01-11 18:55:34.272100 fabric_fim-1.6.2/fim/graph/abc_property_graph.py
--rw-r--r--   0        0        0     4093 2024-01-11 18:55:34.272262 fabric_fim-1.6.2/fim/graph/abc_property_graph_constants.py
--rw-r--r--   0        0        0        1 2024-01-11 18:55:34.272433 fabric_fim-1.6.2/fim/graph/data/__init__.py
--rw-r--r--   0        0        0      283 2024-01-11 18:55:34.272544 fabric_fim-1.6.2/fim/graph/data/capacity_types.json
--rw-r--r--   0        0        0      100 2024-01-11 18:55:34.272648 fabric_fim-1.6.2/fim/graph/data/constraint_types.json
--rw-r--r--   0        0        0     3886 2024-01-11 18:55:34.272772 fabric_fim-1.6.2/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0        0        0     3845 2024-01-11 18:55:34.272867 fabric_fim-1.6.2/fim/graph/data/graph_validation_rules_neo4j_v4.json
--rw-r--r--   0        0        0      547 2024-01-11 18:55:34.272967 fabric_fim-1.6.2/fim/graph/data/label_types.json
--rw-r--r--   0        0        0       91 2024-01-11 18:55:34.273058 fabric_fim-1.6.2/fim/graph/data/location_types.json
--rw-r--r--   0        0        0      861 2024-01-11 18:55:34.273161 fabric_fim-1.6.2/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0        0        0     3320 2024-01-11 18:55:34.273265 fabric_fim-1.6.2/fim/graph/graph_util.py
--rw-r--r--   0        0        0    44293 2024-01-11 18:55:34.273658 fabric_fim-1.6.2/fim/graph/neo4j_property_graph.py
--rw-r--r--   0        0        0     6160 2024-01-11 18:55:34.273943 fabric_fim-1.6.2/fim/graph/networkx_mixin.py
--rw-r--r--   0        0        0    42211 2024-01-11 18:55:34.274154 fabric_fim-1.6.2/fim/graph/networkx_property_graph.py
--rw-r--r--   0        0        0     8354 2024-01-11 18:55:34.274397 fabric_fim-1.6.2/fim/graph/networkx_property_graph_disjoint.py
--rw-r--r--   0        0        0     1501 2024-01-11 18:55:34.274576 fabric_fim-1.6.2/fim/graph/resources/README.md
--rw-r--r--   0        0        0        1 2024-01-11 18:55:34.274687 fabric_fim-1.6.2/fim/graph/resources/__init__.py
--rw-r--r--   0        0        0     4484 2024-01-11 18:55:34.274831 fabric_fim-1.6.2/fim/graph/resources/abc_adm.py
--rw-r--r--   0        0        0    13570 2024-01-11 18:55:34.275071 fabric_fim-1.6.2/fim/graph/resources/abc_arm.py
--rw-r--r--   0        0        0     2991 2024-01-11 18:55:34.275270 fabric_fim-1.6.2/fim/graph/resources/abc_bqm.py
--rw-r--r--   0        0        0     5284 2024-01-11 18:55:34.275389 fabric_fim-1.6.2/fim/graph/resources/abc_cbm.py
--rw-r--r--   0        0        0     2297 2024-01-11 18:55:34.275506 fabric_fim-1.6.2/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0        0        0     2106 2024-01-11 18:55:34.275626 fabric_fim-1.6.2/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0        0        0    20998 2024-01-11 18:55:34.275750 fabric_fim-1.6.2/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0        0        0     5017 2024-01-11 18:55:34.275891 fabric_fim-1.6.2/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0        0        0     2341 2024-01-11 18:55:34.275996 fabric_fim-1.6.2/fim/graph/resources/networkx_adm.py
--rw-r--r--   0        0        0     2122 2024-01-11 18:55:34.276255 fabric_fim-1.6.2/fim/graph/resources/networkx_arm.py
--rw-r--r--   0        0        0      301 2024-01-11 18:55:34.276430 fabric_fim-1.6.2/fim/graph/slices/README.md
--rw-r--r--   0        0        0        1 2024-01-11 18:55:34.276533 fabric_fim-1.6.2/fim/graph/slices/__init__.py
--rw-r--r--   0        0        0     8223 2024-01-11 18:55:34.276686 fabric_fim-1.6.2/fim/graph/slices/abc_asm.py
--rw-r--r--   0        0        0     3733 2024-01-11 18:55:34.276801 fabric_fim-1.6.2/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0        0        0     4298 2024-01-11 18:55:34.276914 fabric_fim-1.6.2/fim/graph/slices/networkx_asm.py
--rw-r--r--   0        0        0     8615 2024-01-11 18:55:34.277077 fabric_fim-1.6.2/fim/graph/typed_tuples.py
--rw-r--r--   0        0        0        0 2024-01-11 18:55:34.277169 fabric_fim-1.6.2/fim/logging/__init__.py
--rw-r--r--   0        0        0     1526 2024-01-11 18:55:34.277334 fabric_fim-1.6.2/fim/logging/fim_logger.py
--rw-r--r--   0        0        0     9592 2024-02-21 18:52:51.130770 fabric_fim-1.6.2/fim/logging/log_collector.py
--rw-r--r--   0        0        0     9555 2024-01-11 18:55:34.277688 fabric_fim-1.6.2/fim/pluggable.py
--rw-r--r--   0        0        0      189 2024-01-11 18:55:34.277835 fabric_fim-1.6.2/fim/slivers/README.md
--rw-r--r--   0        0        0      217 2024-01-11 18:55:34.277935 fabric_fim-1.6.2/fim/slivers/__init__.py
--rw-r--r--   0        0        0     3641 2024-01-11 18:55:34.278046 fabric_fim-1.6.2/fim/slivers/attached_components.py
--rw-r--r--   0        0        0    13021 2024-01-11 18:55:34.278221 fabric_fim-1.6.2/fim/slivers/base_sliver.py
--rw-r--r--   0        0        0    26012 2024-01-11 18:55:34.278336 fabric_fim-1.6.2/fim/slivers/capacities_labels.py
--rw-r--r--   0        0        0    11537 2024-01-11 18:55:34.278527 fabric_fim-1.6.2/fim/slivers/component_catalog.py
--rw-r--r--   0        0        0        1 2024-01-11 18:55:34.278674 fabric_fim-1.6.2/fim/slivers/data/__init__.py
--rw-r--r--   0        0        0     1691 2024-01-11 18:55:34.278786 fabric_fim-1.6.2/fim/slivers/data/component_catalog.json
--rw-r--r--   0        0        0    77237 2024-02-21 18:52:51.131259 fabric_fim-1.6.2/fim/slivers/data/instance_sizes.json
--rw-r--r--   0        0        0    23524 2024-01-11 18:55:34.279223 fabric_fim-1.6.2/fim/slivers/delegations.py
--rw-r--r--   0        0        0     3593 2024-01-11 18:55:34.279360 fabric_fim-1.6.2/fim/slivers/gateway.py
--rw-r--r--   0        0        0      919 2024-01-11 18:55:34.279466 fabric_fim-1.6.2/fim/slivers/identifiers.py
--rw-r--r--   0        0        0     3444 2024-01-11 18:55:34.279604 fabric_fim-1.6.2/fim/slivers/instance_catalog.py
--rw-r--r--   0        0        0     3225 2024-02-21 18:55:59.087001 fabric_fim-1.6.2/fim/slivers/interface_info.py
--rw-r--r--   0        0        0     2702 2024-01-11 18:55:34.279979 fabric_fim-1.6.2/fim/slivers/json.py
--rw-r--r--   0        0        0     3869 2024-01-11 18:55:34.280106 fabric_fim-1.6.2/fim/slivers/json_data.py
--rw-r--r--   0        0        0     5983 2024-01-11 18:55:34.280231 fabric_fim-1.6.2/fim/slivers/maintenance_mode.py
--rw-r--r--   0        0        0     1566 2024-01-11 18:55:34.280381 fabric_fim-1.6.2/fim/slivers/network_attached_storage.py
--rw-r--r--   0        0        0     3910 2024-01-11 18:55:34.280512 fabric_fim-1.6.2/fim/slivers/network_link.py
--rw-r--r--   0        0        0    10283 2024-01-11 18:55:34.280667 fabric_fim-1.6.2/fim/slivers/network_node.py
--rw-r--r--   0        0        0    22076 2024-02-21 18:52:51.132196 fabric_fim-1.6.2/fim/slivers/network_service.py
--rw-r--r--   0        0        0     6795 2024-01-11 18:55:34.280955 fabric_fim-1.6.2/fim/slivers/path_info.py
--rw-r--r--   0        0        0     3024 2024-01-11 18:55:34.281125 fabric_fim-1.6.2/fim/slivers/tags.py
--rw-r--r--   0        0        0     2622 2024-01-11 18:55:34.281252 fabric_fim-1.6.2/fim/slivers/topology_diff.py
--rw-r--r--   0        0        0     8706 2024-01-11 18:55:34.281520 fabric_fim-1.6.2/fim/user/README.md
--rw-r--r--   0        0        0     1914 2024-01-11 18:55:34.281626 fabric_fim-1.6.2/fim/user/__init__.py
--rw-r--r--   0        0        0    11730 2024-01-11 18:55:34.281773 fabric_fim-1.6.2/fim/user/component.py
--rw-r--r--   0        0        0     6781 2024-02-21 18:52:51.132799 fabric_fim-1.6.2/fim/user/composite_node.py
--rw-r--r--   0        0        0     7660 2024-01-11 18:55:34.282052 fabric_fim-1.6.2/fim/user/interface.py
--rw-r--r--   0        0        0     8381 2024-01-11 18:55:34.282225 fabric_fim-1.6.2/fim/user/link.py
--rw-r--r--   0        0        0     1219 2024-01-11 18:55:34.282371 fabric_fim-1.6.2/fim/user/measurement.py
--rw-r--r--   0        0        0     9668 2024-01-11 18:55:34.282564 fabric_fim-1.6.2/fim/user/model_element.py
--rw-r--r--   0        0        0    28472 2024-02-21 18:52:51.133160 fabric_fim-1.6.2/fim/user/network_service.py
--rw-r--r--   0        0        0    22636 2024-01-11 18:55:34.282877 fabric_fim-1.6.2/fim/user/node.py
--rw-r--r--   0        0        0    60969 2024-02-21 18:52:51.133457 fabric_fim-1.6.2/fim/user/topology.py
--rw-r--r--   0        0        0        2 2024-01-11 18:55:34.283239 fabric_fim-1.6.2/fim/util/__init__.py
--rw-r--r--   0        0        0    14680 2024-01-11 18:55:34.283425 fabric_fim-1.6.2/fim/util/fim_util.py
--rw-r--r--   0        0        0      595 2024-01-11 18:55:34.283537 fabric_fim-1.6.2/fim/view_only_dict.py
--rw-r--r--   0        0        0        0 2024-01-11 18:55:34.283691 fabric_fim-1.6.2/neo4j/data/.empty
--rw-r--r--   0        0        0        0 2024-01-11 18:55:34.283780 fabric_fim-1.6.2/neo4j/imports/.empty
--rw-r--r--   0        0        0      861 2024-02-21 18:52:51.133848 fabric_fim-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     4632 2024-01-11 18:55:34.284036 fabric_fim-1.6.2/test/ad_topology_test.py
--rw-r--r--   0        0        0     4834 2024-01-11 18:55:34.284148 fabric_fim-1.6.2/test/after.graphml
--rw-r--r--   0        0        0    17550 2024-01-11 18:55:34.284274 fabric_fim-1.6.2/test/attribute_collector_test.py
--rw-r--r--   0        0        0     4696 2024-01-11 18:55:34.284424 fabric_fim-1.6.2/test/before.graphml
--rw-r--r--   0        0        0     2729 2024-01-11 18:55:34.284530 fabric_fim-1.6.2/test/catalog_test.py
--rw-r--r--   0        0        0     4319 2024-01-11 18:55:34.284652 fabric_fim-1.6.2/test/delegation_label_test.py
--rw-r--r--   0        0        0     1653 2024-01-11 18:55:34.284790 fabric_fim-1.6.2/test/maintenance_test.py
--rw-r--r--   0        0        0    51613 2024-01-11 18:55:34.285014 fabric_fim-1.6.2/test/models/advertised_topo.graphml
--rw-r--r--   0        0        0    49696 2024-01-11 18:55:34.285218 fabric_fim-1.6.2/test/models/graph-template.graphml
--rw-r--r--   0        0        0    82994 2024-01-11 18:55:34.285855 fabric_fim-1.6.2/test/models/network-am-ad.graphml
--rw-r--r--   0        0        0    57411 2024-01-11 18:55:34.286085 fabric_fim-1.6.2/test/models/site-2-am-1broker-ad.graphml
--rw-r--r--   0        0        0    52887 2024-01-11 18:55:34.286259 fabric_fim-1.6.2/test/models/site-3-am-1broker-ad.graphml
--rw-r--r--   0        0        0   131407 2024-01-11 18:55:34.286528 fabric_fim-1.6.2/test/models/site-am-2broker-ad.graphml
--rw-r--r--   0        0        0    18708 2024-01-11 18:55:34.286711 fabric_fim-1.6.2/test/modify_test.py
--rw-r--r--   0        0        0    13135 2024-01-11 18:55:34.286998 fabric_fim-1.6.2/test/networkxx_pg_disjoint_test.py
--rw-r--r--   0        0        0    14091 2024-01-11 18:55:34.287189 fabric_fim-1.6.2/test/networkxx_pg_test.py
--rw-r--r--   0        0        0     2572 2024-01-11 18:55:34.287323 fabric_fim-1.6.2/test/pluggable_test.py
--rw-r--r--   0        0        0    45658 2024-02-21 18:52:51.134218 fabric_fim-1.6.2/test/slice_topology_test.py
--rw-r--r--   0        0        0     1869 2024-01-11 18:55:34.287651 fabric_fim-1.6.2/test/sliver_json_test.py
--rw-r--r--   0        0        0     6030 2024-01-11 18:55:34.287801 fabric_fim-1.6.2/test/sliver_test.py
--rw-r--r--   0        0        0    97162 2024-01-11 18:55:34.288155 fabric_fim-1.6.2/test/substrate_topology_test.py
--rw-r--r--   0        0        0      654 2024-01-11 18:55:34.288297 fabric_fim-1.6.2/test/test_load.py
--rw-r--r--   0        0        0     2362 2024-01-11 18:55:34.288486 fabric_fim-1.6.2/test/tuple_test.py
--rw-r--r--   0        0        0    15663 2024-01-11 18:55:34.288738 fabric_fim-1.6.2/test/zz_neo4j_pg_test.py
--rw-r--r--   0        0        0    11888 1970-01-01 00:00:00.000000 fabric_fim-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2208 2024-05-10 20:24:43.795008 fabric_fim-1.7.0b1/.gitignore
+-rw-r--r--   0        0        0       26 2024-05-10 20:24:43.795488 fabric_fim-1.7.0b1/AUTHORS
+-rw-r--r--   0        0        0     1071 2024-05-10 20:24:43.795857 fabric_fim-1.7.0b1/LICENSE
+-rw-r--r--   0        0        0    11110 2024-05-10 20:24:43.796169 fabric_fim-1.7.0b1/README.md
+-rw-r--r--   0        0        0    18690 2024-05-10 20:24:43.796534 fabric_fim-1.7.0b1/figs/fim-structure.png
+-rw-r--r--   0        0        0      557 2024-05-10 20:24:43.796847 fabric_fim-1.7.0b1/fim/README.md
+-rw-r--r--   0        0        0      105 2024-05-10 20:26:11.510446 fabric_fim-1.7.0b1/fim/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.797256 fabric_fim-1.7.0b1/fim/authz/__init__.py
+-rw-r--r--   0        0        0    16139 2024-05-10 20:24:43.797491 fabric_fim-1.7.0b1/fim/authz/attribute_collector.py
+-rw-r--r--   0        0        0      334 2024-05-10 20:24:43.797655 fabric_fim-1.7.0b1/fim/graph/README.md
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.797759 fabric_fim-1.7.0b1/fim/graph/__init__.py
+-rw-r--r--   0        0        0    69855 2024-05-10 20:24:43.798121 fabric_fim-1.7.0b1/fim/graph/abc_property_graph.py
+-rw-r--r--   0        0        0     4093 2024-05-10 20:24:43.798314 fabric_fim-1.7.0b1/fim/graph/abc_property_graph_constants.py
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.798489 fabric_fim-1.7.0b1/fim/graph/data/__init__.py
+-rw-r--r--   0        0        0      283 2024-05-10 20:24:43.798716 fabric_fim-1.7.0b1/fim/graph/data/capacity_types.json
+-rw-r--r--   0        0        0      100 2024-05-10 20:24:43.798819 fabric_fim-1.7.0b1/fim/graph/data/constraint_types.json
+-rw-r--r--   0        0        0     3886 2024-05-10 20:24:43.798958 fabric_fim-1.7.0b1/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0        0        0     3845 2024-05-10 20:24:43.799082 fabric_fim-1.7.0b1/fim/graph/data/graph_validation_rules_neo4j_v4.json
+-rw-r--r--   0        0        0      547 2024-05-10 20:24:43.799191 fabric_fim-1.7.0b1/fim/graph/data/label_types.json
+-rw-r--r--   0        0        0       91 2024-05-10 20:24:43.799336 fabric_fim-1.7.0b1/fim/graph/data/location_types.json
+-rw-r--r--   0        0        0      861 2024-05-10 20:24:43.799537 fabric_fim-1.7.0b1/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0        0        0     3320 2024-05-10 20:24:43.799684 fabric_fim-1.7.0b1/fim/graph/graph_util.py
+-rw-r--r--   0        0        0    44293 2024-05-10 20:24:43.799917 fabric_fim-1.7.0b1/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0        0        0     6160 2024-05-10 20:24:43.800266 fabric_fim-1.7.0b1/fim/graph/networkx_mixin.py
+-rw-r--r--   0        0        0    42211 2024-05-10 20:24:43.800923 fabric_fim-1.7.0b1/fim/graph/networkx_property_graph.py
+-rw-r--r--   0        0        0     8354 2024-05-10 20:24:43.801320 fabric_fim-1.7.0b1/fim/graph/networkx_property_graph_disjoint.py
+-rw-r--r--   0        0        0     1501 2024-05-10 20:24:43.801540 fabric_fim-1.7.0b1/fim/graph/resources/README.md
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.801659 fabric_fim-1.7.0b1/fim/graph/resources/__init__.py
+-rw-r--r--   0        0        0     4484 2024-05-10 20:24:43.801834 fabric_fim-1.7.0b1/fim/graph/resources/abc_adm.py
+-rw-r--r--   0        0        0    13570 2024-05-10 20:24:43.802071 fabric_fim-1.7.0b1/fim/graph/resources/abc_arm.py
+-rw-r--r--   0        0        0     2991 2024-05-10 20:24:43.802244 fabric_fim-1.7.0b1/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0        0        0     5284 2024-05-10 20:24:43.802417 fabric_fim-1.7.0b1/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0        0        0     2297 2024-05-10 20:24:43.802620 fabric_fim-1.7.0b1/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0        0        0     2106 2024-05-10 20:24:43.802756 fabric_fim-1.7.0b1/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0        0        0    20998 2024-05-10 20:24:43.802902 fabric_fim-1.7.0b1/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0        0        0     5017 2024-05-10 20:24:43.803159 fabric_fim-1.7.0b1/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0        0        0     2341 2024-05-10 20:24:43.803301 fabric_fim-1.7.0b1/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0        0        0     2122 2024-05-10 20:24:43.803584 fabric_fim-1.7.0b1/fim/graph/resources/networkx_arm.py
+-rw-r--r--   0        0        0      301 2024-05-10 20:24:43.803783 fabric_fim-1.7.0b1/fim/graph/slices/README.md
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.803907 fabric_fim-1.7.0b1/fim/graph/slices/__init__.py
+-rw-r--r--   0        0        0     8223 2024-05-10 20:24:43.804168 fabric_fim-1.7.0b1/fim/graph/slices/abc_asm.py
+-rw-r--r--   0        0        0     3733 2024-05-10 20:24:43.804392 fabric_fim-1.7.0b1/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0        0        0     4298 2024-05-10 20:24:43.804598 fabric_fim-1.7.0b1/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0        0        0     8615 2024-05-10 20:24:43.804937 fabric_fim-1.7.0b1/fim/graph/typed_tuples.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:24:43.805038 fabric_fim-1.7.0b1/fim/logging/__init__.py
+-rw-r--r--   0        0        0     1526 2024-05-10 20:24:43.805280 fabric_fim-1.7.0b1/fim/logging/fim_logger.py
+-rw-r--r--   0        0        0     9592 2024-05-10 20:24:43.805573 fabric_fim-1.7.0b1/fim/logging/log_collector.py
+-rw-r--r--   0        0        0     9555 2024-05-10 20:24:43.805926 fabric_fim-1.7.0b1/fim/pluggable.py
+-rw-r--r--   0        0        0      189 2024-05-10 20:24:43.806235 fabric_fim-1.7.0b1/fim/slivers/README.md
+-rw-r--r--   0        0        0      217 2024-05-10 20:24:43.806437 fabric_fim-1.7.0b1/fim/slivers/__init__.py
+-rw-r--r--   0        0        0     3641 2024-05-10 20:24:43.806672 fabric_fim-1.7.0b1/fim/slivers/attached_components.py
+-rw-r--r--   0        0        0    13021 2024-05-10 20:24:43.806968 fabric_fim-1.7.0b1/fim/slivers/base_sliver.py
+-rw-r--r--   0        0        0    26012 2024-05-10 20:24:43.807097 fabric_fim-1.7.0b1/fim/slivers/capacities_labels.py
+-rw-r--r--   0        0        0    11537 2024-05-10 20:24:43.807400 fabric_fim-1.7.0b1/fim/slivers/component_catalog.py
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.807559 fabric_fim-1.7.0b1/fim/slivers/data/__init__.py
+-rw-r--r--   0        0        0     1691 2024-05-10 20:24:43.807676 fabric_fim-1.7.0b1/fim/slivers/data/component_catalog.json
+-rw-r--r--   0        0        0    77237 2024-05-10 20:24:43.807928 fabric_fim-1.7.0b1/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0        0        0    23524 2024-05-10 20:24:43.808314 fabric_fim-1.7.0b1/fim/slivers/delegations.py
+-rw-r--r--   0        0        0     3593 2024-05-10 20:24:43.808521 fabric_fim-1.7.0b1/fim/slivers/gateway.py
+-rw-r--r--   0        0        0     1193 2024-05-10 20:44:16.037631 fabric_fim-1.7.0b1/fim/slivers/identifiers.py
+-rw-r--r--   0        0        0     3444 2024-05-10 20:24:43.808901 fabric_fim-1.7.0b1/fim/slivers/instance_catalog.py
+-rw-r--r--   0        0        0     3225 2024-05-10 20:24:43.809015 fabric_fim-1.7.0b1/fim/slivers/interface_info.py
+-rw-r--r--   0        0        0     2702 2024-05-10 20:24:43.809319 fabric_fim-1.7.0b1/fim/slivers/json.py
+-rw-r--r--   0        0        0     3869 2024-05-10 20:24:43.809455 fabric_fim-1.7.0b1/fim/slivers/json_data.py
+-rw-r--r--   0        0        0     5983 2024-05-10 20:24:43.809634 fabric_fim-1.7.0b1/fim/slivers/maintenance_mode.py
+-rw-r--r--   0        0        0     1566 2024-05-10 20:24:43.809805 fabric_fim-1.7.0b1/fim/slivers/network_attached_storage.py
+-rw-r--r--   0        0        0     3910 2024-05-10 20:24:43.809960 fabric_fim-1.7.0b1/fim/slivers/network_link.py
+-rw-r--r--   0        0        0    10283 2024-05-10 20:24:43.810194 fabric_fim-1.7.0b1/fim/slivers/network_node.py
+-rw-r--r--   0        0        0    22076 2024-05-10 20:24:43.810476 fabric_fim-1.7.0b1/fim/slivers/network_service.py
+-rw-r--r--   0        0        0     6795 2024-05-10 20:24:43.810725 fabric_fim-1.7.0b1/fim/slivers/path_info.py
+-rw-r--r--   0        0        0     3024 2024-05-10 20:24:43.811079 fabric_fim-1.7.0b1/fim/slivers/tags.py
+-rw-r--r--   0        0        0     2622 2024-05-10 20:24:43.811250 fabric_fim-1.7.0b1/fim/slivers/topology_diff.py
+-rw-r--r--   0        0        0     8706 2024-05-10 20:24:43.811562 fabric_fim-1.7.0b1/fim/user/README.md
+-rw-r--r--   0        0        0     1914 2024-05-10 20:24:43.811680 fabric_fim-1.7.0b1/fim/user/__init__.py
+-rw-r--r--   0        0        0    11730 2024-05-10 20:24:43.811887 fabric_fim-1.7.0b1/fim/user/component.py
+-rw-r--r--   0        0        0     6781 2024-05-10 20:24:43.812130 fabric_fim-1.7.0b1/fim/user/composite_node.py
+-rw-r--r--   0        0        0     7660 2024-05-10 20:24:43.812358 fabric_fim-1.7.0b1/fim/user/interface.py
+-rw-r--r--   0        0        0     8381 2024-05-10 20:24:43.812688 fabric_fim-1.7.0b1/fim/user/link.py
+-rw-r--r--   0        0        0     1219 2024-05-10 20:24:43.812907 fabric_fim-1.7.0b1/fim/user/measurement.py
+-rw-r--r--   0        0        0     9668 2024-05-10 20:24:43.813172 fabric_fim-1.7.0b1/fim/user/model_element.py
+-rw-r--r--   0        0        0    28472 2024-05-10 20:24:43.813369 fabric_fim-1.7.0b1/fim/user/network_service.py
+-rw-r--r--   0        0        0    22636 2024-05-10 20:24:43.813557 fabric_fim-1.7.0b1/fim/user/node.py
+-rw-r--r--   0        0        0    63341 2024-05-10 20:26:26.617594 fabric_fim-1.7.0b1/fim/user/topology.py
+-rw-r--r--   0        0        0        2 2024-05-10 20:24:43.814024 fabric_fim-1.7.0b1/fim/util/__init__.py
+-rw-r--r--   0        0        0    14680 2024-05-10 20:24:43.814211 fabric_fim-1.7.0b1/fim/util/fim_util.py
+-rw-r--r--   0        0        0      595 2024-05-10 20:24:43.814379 fabric_fim-1.7.0b1/fim/view_only_dict.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:24:43.816925 fabric_fim-1.7.0b1/neo4j/data/.empty
+-rw-r--r--   0        0        0        0 2024-05-10 20:24:43.817057 fabric_fim-1.7.0b1/neo4j/imports/.empty
+-rw-r--r--   0        0        0      861 2024-05-10 20:24:43.817205 fabric_fim-1.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4632 2024-05-10 20:24:43.817434 fabric_fim-1.7.0b1/test/ad_topology_test.py
+-rw-r--r--   0        0        0     4834 2024-05-10 20:24:43.817571 fabric_fim-1.7.0b1/test/after.graphml
+-rw-r--r--   0        0        0    17550 2024-05-10 20:24:43.817695 fabric_fim-1.7.0b1/test/attribute_collector_test.py
+-rw-r--r--   0        0        0     4696 2024-05-10 20:24:43.817868 fabric_fim-1.7.0b1/test/before.graphml
+-rw-r--r--   0        0        0     2729 2024-05-10 20:24:43.818052 fabric_fim-1.7.0b1/test/catalog_test.py
+-rw-r--r--   0        0        0     4319 2024-05-10 20:24:43.818232 fabric_fim-1.7.0b1/test/delegation_label_test.py
+-rw-r--r--   0        0        0     1653 2024-05-10 20:24:43.818351 fabric_fim-1.7.0b1/test/maintenance_test.py
+-rw-r--r--   0        0        0    51613 2024-05-10 20:24:43.818614 fabric_fim-1.7.0b1/test/models/advertised_topo.graphml
+-rw-r--r--   0        0        0    49696 2024-05-10 20:24:43.818816 fabric_fim-1.7.0b1/test/models/graph-template.graphml
+-rw-r--r--   0        0        0    82994 2024-05-10 20:24:43.819152 fabric_fim-1.7.0b1/test/models/network-am-ad.graphml
+-rw-r--r--   0        0        0    57411 2024-05-10 20:24:43.819362 fabric_fim-1.7.0b1/test/models/site-2-am-1broker-ad.graphml
+-rw-r--r--   0        0        0    52887 2024-05-10 20:24:43.819564 fabric_fim-1.7.0b1/test/models/site-3-am-1broker-ad.graphml
+-rw-r--r--   0        0        0   131407 2024-05-10 20:24:43.819871 fabric_fim-1.7.0b1/test/models/site-am-2broker-ad.graphml
+-rw-r--r--   0        0        0    18708 2024-05-10 20:24:43.820055 fabric_fim-1.7.0b1/test/modify_test.py
+-rw-r--r--   0        0        0    13135 2024-05-10 20:24:43.820298 fabric_fim-1.7.0b1/test/networkxx_pg_disjoint_test.py
+-rw-r--r--   0        0        0    14091 2024-05-10 20:24:43.820588 fabric_fim-1.7.0b1/test/networkxx_pg_test.py
+-rw-r--r--   0        0        0     2572 2024-05-10 20:24:43.820714 fabric_fim-1.7.0b1/test/pluggable_test.py
+-rw-r--r--   0        0        0    48631 2024-05-10 20:26:50.309360 fabric_fim-1.7.0b1/test/slice_topology_test.py
+-rw-r--r--   0        0        0     1869 2024-05-10 20:24:43.821046 fabric_fim-1.7.0b1/test/sliver_json_test.py
+-rw-r--r--   0        0        0     6030 2024-05-10 20:24:43.821189 fabric_fim-1.7.0b1/test/sliver_test.py
+-rw-r--r--   0        0        0    98404 2024-05-10 20:27:01.881851 fabric_fim-1.7.0b1/test/substrate_topology_test.py
+-rw-r--r--   0        0        0      654 2024-05-10 20:24:43.821690 fabric_fim-1.7.0b1/test/test_load.py
+-rw-r--r--   0        0        0     2362 2024-05-10 20:24:43.821803 fabric_fim-1.7.0b1/test/tuple_test.py
+-rw-r--r--   0        0        0    15663 2024-05-10 20:24:43.821993 fabric_fim-1.7.0b1/test/zz_neo4j_pg_test.py
+-rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.7.0b1/PKG-INFO
```

### Comparing `fabric_fim-1.6.2/.gitignore` & `fabric_fim-1.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/LICENSE` & `fabric_fim-1.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/README.md` & `fabric_fim-1.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/figs/fim-structure.png` & `fabric_fim-1.7.0b1/figs/fim-structure.png`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/README.md` & `fabric_fim-1.7.0b1/fim/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/authz/attribute_collector.py` & `fabric_fim-1.7.0b1/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/abc_property_graph.py` & `fabric_fim-1.7.0b1/fim/graph/abc_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.7.0b1/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.7.0b1/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/data/graph_validation_rules_neo4j_v4.json` & `fabric_fim-1.7.0b1/fim/graph/data/graph_validation_rules_neo4j_v4.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/data/label_types.json` & `fabric_fim-1.7.0b1/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/data/neo4j_indexes.json` & `fabric_fim-1.7.0b1/fim/graph/data/neo4j_indexes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/graph_util.py` & `fabric_fim-1.7.0b1/fim/graph/graph_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.7.0b1/fim/graph/neo4j_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/networkx_mixin.py` & `fabric_fim-1.7.0b1/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/networkx_property_graph.py` & `fabric_fim-1.7.0b1/fim/graph/networkx_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.7.0b1/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/README.md` & `fabric_fim-1.7.0b1/fim/graph/resources/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/abc_adm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/abc_arm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/neo4j_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.7.0b1/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/slices/abc_asm.py` & `fabric_fim-1.7.0b1/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.7.0b1/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.7.0b1/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/graph/typed_tuples.py` & `fabric_fim-1.7.0b1/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/logging/fim_logger.py` & `fabric_fim-1.7.0b1/fim/logging/fim_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/logging/log_collector.py` & `fabric_fim-1.7.0b1/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/pluggable.py` & `fabric_fim-1.7.0b1/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/attached_components.py` & `fabric_fim-1.7.0b1/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/base_sliver.py` & `fabric_fim-1.7.0b1/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/capacities_labels.py` & `fabric_fim-1.7.0b1/fim/slivers/capacities_labels.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/component_catalog.py` & `fabric_fim-1.7.0b1/fim/slivers/component_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/data/component_catalog.json` & `fabric_fim-1.7.0b1/fim/slivers/data/component_catalog.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.7.0b1/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/delegations.py` & `fabric_fim-1.7.0b1/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/gateway.py` & `fabric_fim-1.7.0b1/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/identifiers.py` & `fabric_fim-1.7.0b1/fim/slivers/identifiers.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,8 +31,19 @@
 def dp_port_id(switch: str, port: str) -> str:
     """
     Return a unique id of a DP switch port based on switch name and port name
     :param switch:
     :param port:
     :return:
     """
-    return 'port+' + switch + ':' + port
+    return 'port+' + switch + ':' + port
+
+
+def p4_switch_name_id(site: str, ip: str) -> Tuple[str, str]:
+    """
+    Return a tuple of name and id of a p4 switch name and node id
+    :param site:
+    :param ip:
+    :return:
+    """
+    name = site.lower() + '-p4-sw'
+    return name,  'node+' + name + ':ip+' + ip
```

### Comparing `fabric_fim-1.6.2/fim/slivers/instance_catalog.py` & `fabric_fim-1.7.0b1/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/interface_info.py` & `fabric_fim-1.7.0b1/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/json.py` & `fabric_fim-1.7.0b1/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/json_data.py` & `fabric_fim-1.7.0b1/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/maintenance_mode.py` & `fabric_fim-1.7.0b1/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/network_attached_storage.py` & `fabric_fim-1.7.0b1/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/network_link.py` & `fabric_fim-1.7.0b1/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/network_node.py` & `fabric_fim-1.7.0b1/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/network_service.py` & `fabric_fim-1.7.0b1/fim/slivers/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/path_info.py` & `fabric_fim-1.7.0b1/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/tags.py` & `fabric_fim-1.7.0b1/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/slivers/topology_diff.py` & `fabric_fim-1.7.0b1/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/README.md` & `fabric_fim-1.7.0b1/fim/user/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/__init__.py` & `fabric_fim-1.7.0b1/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/component.py` & `fabric_fim-1.7.0b1/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/composite_node.py` & `fabric_fim-1.7.0b1/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/interface.py` & `fabric_fim-1.7.0b1/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/link.py` & `fabric_fim-1.7.0b1/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/measurement.py` & `fabric_fim-1.7.0b1/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/model_element.py` & `fabric_fim-1.7.0b1/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/network_service.py` & `fabric_fim-1.7.0b1/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/node.py` & `fabric_fim-1.7.0b1/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/user/topology.py` & `fabric_fim-1.7.0b1/fim/user/topology.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,14 +269,57 @@
         service as appropriate. Same as removing a node.
         """
         fac = self._get_node_by_name(name)
         if fac.type != NodeType.Facility:
             raise TopologyException(f'{name} is not a Facility node, cannot remove.')
         self.remove_node(name)
 
+    def add_switch(self, *, name: str, node_id: str = None, site: str,
+                   nstype: ServiceType = ServiceType.P4, nslabels: Labels or None = None,
+                   nports: int = 8, portlabels: Labels or None = None,
+                   portcapacities: Capacities or None = None,
+                   **kwargs) -> Node:
+        """
+        Add a switch (P4 type by default) with some number of ports (8 by default)
+        all given names and label local_names 'p1'-'p8'.
+        :param name:
+        :param node_id:
+        :param site:
+        :param nstype: network service type (defaults to P4)
+        :param nslabels: additional labels for switch network service
+        :param nports: number of ports (defaults to 8)
+        :param portlabels: labels to be added to each port (otherwise overridden with default)
+        :param portcapacities: capacities to be added to each port (otherwise overridden with default)
+        :param kwargs: pass additional parameters to add node (e.g. model)
+        """
+        switch = self.add_node(name=name, node_id=node_id, site=site, ntype=NodeType.Switch)
+        switch_ns = switch.add_network_service(name=name + '-ns',
+                                               node_id=node_id + '-ns' if node_id else None,
+                                               nstype=nstype, labels=nslabels)
+        # name them 'p1'-'p8'
+        for i in range(1, nports + 1):
+            labels = Labels(local_name=f'p{i}')
+            # 100G port
+            capacities = Capacities(bw=100)
+            switch_i = switch_ns.add_interface(name=f'p{i}', node_id=node_id + f'-int{i}' if node_id else None,
+                                               itype=InterfaceType.DedicatedPort,
+                                               labels=portlabels if portlabels else labels,
+                                               capacities=portcapacities if portcapacities else capacities)
+        return switch
+
+    def remove_switch(self, *, name: str):
+        """
+        Remove a switch and associated network service and interfaces, disconnecting it from a
+        service as appropriate. Same as removing a node.
+        """
+        fac = self._get_node_by_name(name)
+        if fac.type != NodeType.Switch:
+            raise TopologyException(f'{name} is not a Switch node, cannot remove.')
+        self.remove_node(name)
+
     def add_link(self, *, name: str, node_id: str = None, ltype: LinkType,
                  interfaces: List[Interface], technology: str = None,
                  **kwargs) -> Link:
         """
         Add link between listed interfaces with specified parameters (for experiment
         topologies you want add_network_service instead)
         :param name:
```

### Comparing `fabric_fim-1.6.2/fim/util/fim_util.py` & `fabric_fim-1.7.0b1/fim/util/fim_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/fim/view_only_dict.py` & `fabric_fim-1.7.0b1/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/pyproject.toml` & `fabric_fim-1.7.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/ad_topology_test.py` & `fabric_fim-1.7.0b1/test/ad_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/after.graphml` & `fabric_fim-1.7.0b1/test/after.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/attribute_collector_test.py` & `fabric_fim-1.7.0b1/test/attribute_collector_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/before.graphml` & `fabric_fim-1.7.0b1/test/before.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/catalog_test.py` & `fabric_fim-1.7.0b1/test/catalog_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/delegation_label_test.py` & `fabric_fim-1.7.0b1/test/delegation_label_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/maintenance_test.py` & `fabric_fim-1.7.0b1/test/maintenance_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/models/advertised_topo.graphml` & `fabric_fim-1.7.0b1/test/models/advertised_topo.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/models/graph-template.graphml` & `fabric_fim-1.7.0b1/test/models/graph-template.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/models/network-am-ad.graphml` & `fabric_fim-1.7.0b1/test/models/network-am-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/models/site-2-am-1broker-ad.graphml` & `fabric_fim-1.7.0b1/test/models/site-2-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/models/site-3-am-1broker-ad.graphml` & `fabric_fim-1.7.0b1/test/models/site-3-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/models/site-am-2broker-ad.graphml` & `fabric_fim-1.7.0b1/test/models/site-am-2broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/modify_test.py` & `fabric_fim-1.7.0b1/test/modify_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/networkxx_pg_disjoint_test.py` & `fabric_fim-1.7.0b1/test/networkxx_pg_disjoint_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/networkxx_pg_test.py` & `fabric_fim-1.7.0b1/test/networkxx_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/pluggable_test.py` & `fabric_fim-1.7.0b1/test/pluggable_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/slice_topology_test.py` & `fabric_fim-1.7.0b1/test/slice_topology_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,17 +254,14 @@
         n1.boot_script = None
         self.assertIsNone(n1.boot_script)
 
         gpu1 = n1.components['gpu1']
         nic1 = n1.components['nic1']
         nic2 = n2.components['nic2']
 
-        p1 = nic2.interfaces['nic2-p1']
-        p2 = nic2.interfaces['nic2-p2']
-
         cap = f.Capacities(bw=50, unit=1)
         nic1.capacities = cap
         lab = f.Labels(ipv4="192.168.1.12")
         nic1.labels = lab
         caphints = f.CapacityHints(instance_type='blah')
         n1.capacity_hints = caphints
 
@@ -276,14 +273,15 @@
         assert (caphints.instance_type == caphints1.instance_type)
 
         #s1 = self.topo.add_network_service(name='s1', nstype=f.ServiceType.L2Bridge, interfaces=self.topo.interface_list)
 
         s1 = self.topo.add_network_service(name='s1', nstype=f.ServiceType.L2STS, interfaces=[n1.interface_list[0],
                                                                                               n2.interface_list[0],
                                                                                               n3.interface_list[0]])
+        p1 = n1.interface_list[0]
 
         # facilities
         fac1 = self.topo.add_facility(name='RENCI-DTN', site='RENC', capacities=f.Capacities(bw=10),
                                       labels=f.Labels(vlan='100'))
         # facility needs to be connected via a service to something else
         sfac = self.topo.add_network_service(name='s-fac', nstype=f.ServiceType.L2STS,
                                              interfaces=[fac1.interface_list[0],
@@ -311,19 +309,18 @@
         asm_graph = Neo4jASMFactory.create(generic_graph)
         asm_graph.validate_graph()
         self.n4j_imp.delete_all_graphs()
 
         s1p = self.topo.network_services['s1']
 
         print(f'S1 has these interfaces: {s1p.interface_list}')
-
-        s1.disconnect_interface(interface=p1)
-
-        print(f'S1 has these interfaces: {s1.interface_list}')
-        self.assertEqual(len(s1.interface_list), 2)
+        print(f'Disconnecting {p1} from S1')
+        s1p.disconnect_interface(interface=p1)
+        print(f'Now S1 has these interfaces: {s1p.interface_list}')
+        self.assertEqual(len(s1p.interface_list), 2)
 
         # validate the topology
         self.topo.validate()
 
         # Import it in the neo4j as ASM
         generic_graph = self.n4j_imp.import_graph_from_string(graph_string=slice_graph)
         asm_graph = Neo4jASMFactory.create(generic_graph)
@@ -506,14 +503,15 @@
         topo.nodes['n2'].add_component(model_type=f.ComponentModelType.SmartNIC_ConnectX_6, name='nic1')
         topo.nodes['n2'].add_component(model_type=f.ComponentModelType.GPU_RTX6000, name='gpu1')
         topo.nodes['n3'].add_component(model_type=f.ComponentModelType.SmartNIC_ConnectX_5, name='nic1')
         topo.add_network_service(name='bridge1', nstype=f.ServiceType.L2Bridge,
                                       interfaces=topo.interface_list)
         topo.serialize(file_name='single-site-neo4jimp.graphml')
         topo.validate()
+        os.unlink('single-site-neo4jimp.graphml')
 
     def testBasicTwoSiteSlice(self):
         # create a basic slice and export to GraphML and JSON
         self.topo.add_node(name='n1', site='RENC', ntype=f.NodeType.VM, capacities=Capacities(core=4, disk=10))
         self.topo.add_node(name='n2', site='RENC', capacities=Capacities(core=8, ram=2))
         self.topo.add_node(name='n3', site='UKY', capacities=Capacities(core=8, ram=2))
         self.topo.nodes['n1'].add_component(model_type=f.ComponentModelType.SharedNIC_ConnectX_6, name='nic1')
@@ -628,14 +626,44 @@
         generic_graph = self.n4j_imp.import_graph_from_string(graph_string=slice_graph)
         asm_graph = Neo4jASMFactory.create(generic_graph)
         # the following validation just uses cypher or networkx_query and is not as capable
         # as self.topo.validate() but is much faster
         asm_graph.validate_graph()
         self.n4j_imp.delete_all_graphs()
 
+    def testL3ServiceFail2(self):
+        """
+        Test validaton of L3 service required per site
+        """
+        self.topo.add_node(name='n1', site='RENC', ntype=f.NodeType.VM)
+        self.topo.add_node(name='n2', site='RENC')
+        self.topo.add_node(name='n3', site='UKY')
+        self.topo.nodes['n1'].add_component(model_type=f.ComponentModelType.SharedNIC_ConnectX_6, name='nic1')
+        self.topo.nodes['n2'].add_component(model_type=f.ComponentModelType.SmartNIC_ConnectX_6, name='nic1')
+        self.topo.nodes['n3'].add_component(model_type=f.ComponentModelType.SmartNIC_ConnectX_5, name='nic1')
+
+        s1 = self.topo.add_network_service(name='globalL3', nstype=f.ServiceType.FABNetv4,
+                                           interfaces=[self.topo.nodes['n1'].interface_list[0],
+                                                       self.topo.nodes['n2'].interface_list[0],
+                                                       self.topo.nodes['n3'].interface_list[0]])
+
+        # site property is set automagically by validate
+        with self.assertRaises(TopologyException):
+            self.topo.validate()
+
+        slice_graph = self.topo.serialize()
+
+        # Import it in the neo4j as ASM
+        generic_graph = self.n4j_imp.import_graph_from_string(graph_string=slice_graph)
+        asm_graph = Neo4jASMFactory.create(generic_graph)
+        # the following validation just uses cypher or networkx_query and is not as capable
+        # as self.topo.validate() but is much faster
+        asm_graph.validate_graph()
+        self.n4j_imp.delete_all_graphs()
+
     def testPortMirrorService(self):
         t = self.topo
 
         n1 = t.add_node(name='n1', site='MASS')
         n1.add_component(name='nic1', model_type=ComponentModelType.SharedNIC_ConnectX_6)
         n2 = t.add_node(name='n2', site='RENC')
         n2.add_component(name='nic1', model_type=ComponentModelType.SharedNIC_ConnectX_6)
@@ -702,15 +730,14 @@
                               interfaces=[n1.interface_list[0], n2.interface_list[0]])
 
         t.validate()
 
         slice_graph = t.serialize(file_name='fpga_slice.graphml')
         slice_graph = t.serialize()
 
-
         # Import it in the neo4j as ASM
         generic_graph = self.n4j_imp.import_graph_from_string(graph_string=slice_graph)
         asm_graph = Neo4jASMFactory.create(generic_graph)
         asm_graph.validate_graph()
         self.n4j_imp.delete_all_graphs()
         os.unlink('fpga_slice.graphml')
 
@@ -719,17 +746,17 @@
 
         n1 = t.add_node(name='n1', site='MASS')
         n1.add_component(name='nic1', model_type=ComponentModelType.SmartNIC_ConnectX_6)
         n2 = t.add_node(name='n2', site='RENC')
         n2.add_component(name='nic1', model_type=ComponentModelType.SmartNIC_ConnectX_6)
 
         # add facility
-        fac1 = self.topo.add_facility(name='RENCI-DTN', site='RENC',
-                                      interfaces=[('to_mass', f.Labels(vlan='100'), f.Capacities(bw=10)),
-                                                  ('to_renc', f.Labels(vlan='101'), f.Capacities(bw=1))])
+        fac1 = t.add_facility(name='RENCI-DTN', site='RENC',
+                              interfaces=[('to_mass', f.Labels(vlan='100'), f.Capacities(bw=10)),
+                              ('to_renc', f.Labels(vlan='101'), f.Capacities(bw=1))])
 
         t.add_network_service(name='ns1', nstype=ServiceType.L2PTP,
                               interfaces=[n1.interface_list[0], fac1.interface_list[0]])
         t.add_network_service(name='ns2', nstype=ServiceType.L2PTP,
                               interfaces=[n2.interface_list[0], fac1.interface_list[1]])
 
         print(f'{fac1.interface_list[0].name=}')
@@ -737,14 +764,44 @@
         self.assertEqual(fac1.interface_list[0].name, 'to_mass')
         self.assertEqual(fac1.interface_list[1].name, 'to_renc')
 
         t.validate()
 
         self.n4j_imp.delete_all_graphs()
 
+    def testP4Switch(self):
+        t = self.topo
+
+        n1 = t.add_node(name='n1', site='MASS')
+        n1.add_component(name='nic1', model_type=ComponentModelType.SmartNIC_ConnectX_6)
+        n2 = t.add_node(name='n2', site='RENC')
+        n2.add_component(name='nic1', model_type=ComponentModelType.SmartNIC_ConnectX_6)
+        n3 = t.add_node(name='n3', site='MASS')
+        n3.add_component(name='nic1', model_type=ComponentModelType.SmartNIC_ConnectX_6)
+
+        # add P4 switch at another site
+        sw = t.add_switch(name='p4switch', site='STAR')
+
+        # instead of sw.interfaces['p1'] you can also use sw.list_interfaces[0] however
+        # for p4 switches referencing by name may be more appropriate for the users
+        t.add_network_service(name='ns1', nstype=ServiceType.L2PTP,
+                              interfaces=[n1.interface_list[0], sw.interfaces['p1']])
+        t.add_network_service(name='ns2', nstype=ServiceType.L2PTP,
+                              interfaces=[n2.interface_list[0], sw.interfaces['p2']])
+        t.add_network_service(name='ns3', nstype=ServiceType.L2PTP,
+                              interfaces=[n3.interface_list[0], sw.interfaces['p3']])
+
+        t.validate()
+
+        t.serialize(file_name='p4_switch_slice.graphml')
+
+        self.n4j_imp.delete_all_graphs()
+
+        os.unlink('p4_switch_slice.graphml')
+
     def testL3VPNWithCloudService(self):
         t = self.topo
 
         n1 = t.add_node(name='n1', site='MASS')
         n1.add_component(name='nic1', model_type=ComponentModelType.SharedNIC_ConnectX_6)
         n2 = t.add_node(name='n2', site='RENC')
         n2.add_component(name='nic1', model_type=ComponentModelType.SharedNIC_ConnectX_6)
```

### Comparing `fabric_fim-1.6.2/test/sliver_json_test.py` & `fabric_fim-1.7.0b1/test/sliver_json_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/sliver_test.py` & `fabric_fim-1.7.0b1/test/sliver_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/substrate_topology_test.py` & `fabric_fim-1.7.0b1/test/substrate_topology_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,25 @@
                                      details='Mellanox Technologies MT27800 Family [ConnectX-5]')
 
         # NAS
         nas_model = 'ME4084'
         nas = self.topo.add_node(name=site.lower() + '-nas', model=nas_model, site=site, ntype=f.NodeType.NAS,
                                  node_id='BDXTQ53',
                                  capacities=f.Capacities(unit=1, disk=100000))
+
+        # P4 switch
+        # FIXME: Need to have a unique ID for the P4 switch
+        p4sw = self.topo.add_switch(name=site.lower() + '-p4', site='RENC', node_id='p4-switch-at-RENC')
+        # list of DP switch ports connected to the P4 switch in the order of port IDs 0-8 -> p1-p8
+        # they would typically be 400G->100G breakouts
+        dp_to_p4_ports = ['HundredGigeE0/0/0/0/26.1', 'HundredGigeE0/0/0/0/26.2', 'HundredGigeE0/0/0/0/26.3',
+                          'HundredGigeE0/0/0/0/26.4',
+                          'HundredGigeE0/0/0/0/27.1', 'HundredGigeE0/0/0/0/27.2', 'HundredGigeE0/0/0/0/27.3',
+                          'HundredGigeE0/0/0/0/27.4']
+
         # DP switch
         switch_model = 'NCS 55A1-36H' # new switches have  NCS-57B1-6D24-SYS
         switch_ip = "192.168.11.3"
         switch = self.topo.add_node(name=dp_switch_name_id(site, switch_ip)[0],
                                     node_id=dp_switch_name_id(site, switch_ip)[1], site=site,
                                     ntype=f.NodeType.Switch, stitch_node=True)
         dp_ns = switch.add_network_service(name=switch.name+'-ns',
@@ -309,14 +320,23 @@
             sp = dp_ns.add_interface(name=dp, itype=f.InterfaceType.TrunkPort,
                                      node_id=dp_port_id(switch.name, dp), stitch_node=True)
             self.topo.add_link(name='l' + str(link_idx), ltype=f.LinkType.Patch,
                                interfaces=[sr[0].interfaces[sr[1]], sp],
                                node_id=sp.node_id + '-DAC')
             link_idx += 1
 
+        # add dp switch ports that link to P4 switch ports (note they are not stitch nodes!!)
+        for dp, p4idx in zip(dp_to_p4_ports, range(1, 8+1)):
+            sp = dp_ns.add_interface(name=dp, itype=f.InterfaceType.TrunkPort,
+                                     node_id=dp_port_id(switch.name, dp), stitch_node=False)
+            self.topo.add_link(name='l' + str(link_idx), ltype=f.LinkType.Patch,
+                               interfaces=[p4sw.interfaces[f'p{p4idx}'], sp],
+                               node_id=sp.node_id + '-DAC')
+            link_idx += 1
+
         self.topo.validate()
         #
         # delegations
         #
         # Capacity delegations go on network nodes (workers), components and interfaces.
         # They are not going on switches, switch fabrics. They are typically not pooled.
         # Label delegations and pools go on interfaces.
```

### Comparing `fabric_fim-1.6.2/test/test_load.py` & `fabric_fim-1.7.0b1/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/tuple_test.py` & `fabric_fim-1.7.0b1/test/tuple_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/test/zz_neo4j_pg_test.py` & `fabric_fim-1.7.0b1/test/zz_neo4j_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.6.2/PKG-INFO` & `fabric_fim-1.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.6.2
+Version: 1.7.0b1
 Summary: FABRIC Information Model library and utilities
 Keywords: Neo4j
 Author-email: Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

