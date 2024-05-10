# Comparing `tmp/cimsparql-3.2.1.tar.gz` & `tmp/cimsparql-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cimsparql-3.2.1.tar", max compression
+gzip compressed data, was "cimsparql-3.3.1.tar", max compression
```

## Comparing `cimsparql-3.2.1.tar` & `cimsparql-3.3.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1065 2024-04-12 12:58:00.770785 cimsparql-3.2.1/LICENSE
--rw-r--r--   0        0        0     5330 2024-04-12 12:58:00.770785 cimsparql-3.2.1/README.md
--rw-r--r--   0        0        0       61 2024-04-12 12:58:13.298711 cimsparql-3.2.1/cimsparql/__init__.py
--rw-r--r--   0        0        0     4263 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/adaptions.py
--rw-r--r--   0        0        0     1642 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/constants.py
--rw-r--r--   0        0        0     9685 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/data_models.py
--rw-r--r--   0        0        0    15851 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/graphdb.py
--rw-r--r--   0        0        0    28362 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/model.py
--rw-r--r--   0        0        0     5202 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/ac_lines.sparql
--rw-r--r--   0        0        0      221 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/add_mrid.sparql
--rw-r--r--   0        0        0     1761 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/borders.sparql
--rw-r--r--   0        0        0     2073 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/branch_node_withdraw.sparql
--rw-r--r--   0        0        0     1795 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/bus.sparql
--rw-r--r--   0        0        0      984 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/connections.sparql
--rw-r--r--   0        0        0     1291 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/connectivity_nodes.sparql
--rw-r--r--   0        0        0      737 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/converter_hvdc_bidzones.sparql
--rw-r--r--   0        0        0     2337 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/converters.sparql
--rw-r--r--   0        0        0      588 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/coordinates.sparql
--rw-r--r--   0        0        0     2521 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/dc_active_power_flow.sparql
--rw-r--r--   0        0        0      242 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/disconnected.sparql
--rw-r--r--   0        0        0     3063 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/exchange.sparql
--rw-r--r--   0        0        0      792 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/full_model.sparql
--rw-r--r--   0        0        0     2813 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/loads.sparql
--rw-r--r--   0        0        0      287 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/market_dates.sparql
--rw-r--r--   0        0        0      523 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/power_flow.sparql
--rw-r--r--   0        0        0      397 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/ras_equipment.sparql
--rw-r--r--   0        0        0      573 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/regions.sparql
--rw-r--r--   0        0        0     3655 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/series_compensators.sparql
--rw-r--r--   0        0        0      426 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/station_group_code_and_names.sparql
--rw-r--r--   0        0        0      645 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/substation_voltage_level.sparql
--rw-r--r--   0        0        0     2877 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/sv_branch.sparql
--rw-r--r--   0        0        0      245 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/sv_injection.sparql
--rw-r--r--   0        0        0      781 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/switches.sparql
--rw-r--r--   0        0        0     2725 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/synchronous_machines.sparql
--rw-r--r--   0        0        0      318 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
--rw-r--r--   0        0        0     3102 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/three_winding.sparql
--rw-r--r--   0        0        0     1953 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/three_winding_dummy_nodes.sparql
--rw-r--r--   0        0        0     1583 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/three_winding_loss.sparql
--rw-r--r--   0        0        0      363 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/transformer_windings.sparql
--rw-r--r--   0        0        0     1269 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/transformers.sparql
--rw-r--r--   0        0        0     1844 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/transformers_connected_to_converter.sparql
--rw-r--r--   0        0        0     4520 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/two_winding_transformer.sparql
--rw-r--r--   0        0        0     1049 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/two_winding_transformer_angle.sparql
--rw-r--r--   0        0        0      461 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/type_mapper.sparql
--rw-r--r--   0        0        0      814 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/wind_generating_units.sparql
--rw-r--r--   0        0        0      944 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql/winding.sparql
--rw-r--r--   0        0        0     2181 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/sparql_result_json.py
--rw-r--r--   0        0        0     3193 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/templates.py
--rw-r--r--   0        0        0     5627 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/type_mapper.py
--rw-r--r--   0        0        0     1878 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/url.py
--rw-r--r--   0        0        0      626 2024-04-12 12:58:00.770785 cimsparql-3.2.1/cimsparql/value_mapper.py
--rw-r--r--   0        0        0      459 2024-04-12 12:58:00.778785 cimsparql-3.2.1/pkg_data/blazegraph_repo_config.xml
--rw-r--r--   0        0        0      676 2024-04-12 12:58:00.778785 cimsparql-3.2.1/pkg_data/namespaces.json
--rw-r--r--   0        0        0      805 2024-04-12 12:58:00.778785 cimsparql-3.2.1/pkg_data/native_store_config_template.ttl
--rw-r--r--   0        0        0     4357 2024-04-12 12:58:13.298711 cimsparql-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     6104 1970-01-01 00:00:00.000000 cimsparql-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-10 12:53:02.992521 cimsparql-3.3.1/LICENSE
+-rw-r--r--   0        0        0     5195 2024-05-10 12:53:02.992521 cimsparql-3.3.1/README.md
+-rw-r--r--   0        0        0       60 2024-05-10 12:53:16.472606 cimsparql-3.3.1/cimsparql/__init__.py
+-rw-r--r--   0        0        0     4744 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/adaptions.py
+-rw-r--r--   0        0        0     1642 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/constants.py
+-rw-r--r--   0        0        0     9739 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/data_models.py
+-rw-r--r--   0        0        0    16044 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/graphdb.py
+-rw-r--r--   0        0        0    28376 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/model.py
+-rw-r--r--   0        0        0     5202 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/ac_lines.sparql
+-rw-r--r--   0        0        0      221 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/add_mrid.sparql
+-rw-r--r--   0        0        0     1761 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/borders.sparql
+-rw-r--r--   0        0        0     2073 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/branch_node_withdraw.sparql
+-rw-r--r--   0        0        0     1795 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/bus.sparql
+-rw-r--r--   0        0        0      984 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/connections.sparql
+-rw-r--r--   0        0        0     1291 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/connectivity_nodes.sparql
+-rw-r--r--   0        0        0      737 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/converter_hvdc_bidzones.sparql
+-rw-r--r--   0        0        0     2614 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/converters.sparql
+-rw-r--r--   0        0        0      588 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/coordinates.sparql
+-rw-r--r--   0        0        0     2521 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/dc_active_power_flow.sparql
+-rw-r--r--   0        0        0      242 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/disconnected.sparql
+-rw-r--r--   0        0        0     3063 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/exchange.sparql
+-rw-r--r--   0        0        0      792 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/full_model.sparql
+-rw-r--r--   0        0        0     2813 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/loads.sparql
+-rw-r--r--   0        0        0      287 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/market_dates.sparql
+-rw-r--r--   0        0        0      523 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/power_flow.sparql
+-rw-r--r--   0        0        0      397 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/ras_equipment.sparql
+-rw-r--r--   0        0        0      573 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/regions.sparql
+-rw-r--r--   0        0        0     3655 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/series_compensators.sparql
+-rw-r--r--   0        0        0      426 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/station_group_code_and_names.sparql
+-rw-r--r--   0        0        0      645 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/substation_voltage_level.sparql
+-rw-r--r--   0        0        0     2877 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/sv_branch.sparql
+-rw-r--r--   0        0        0      245 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/sv_injection.sparql
+-rw-r--r--   0        0        0      781 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/switches.sparql
+-rw-r--r--   0        0        0     3285 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/synchronous_machines.sparql
+-rw-r--r--   0        0        0      318 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/test_configuration_modifications/add_zero_sv_power.sparql
+-rw-r--r--   0        0        0     3102 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/three_winding.sparql
+-rw-r--r--   0        0        0     1953 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/three_winding_dummy_nodes.sparql
+-rw-r--r--   0        0        0     1583 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/three_winding_loss.sparql
+-rw-r--r--   0        0        0      363 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/transformer_windings.sparql
+-rw-r--r--   0        0        0     1269 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/transformers.sparql
+-rw-r--r--   0        0        0     1844 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/transformers_connected_to_converter.sparql
+-rw-r--r--   0        0        0     4520 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer.sparql
+-rw-r--r--   0        0        0     1049 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer_angle.sparql
+-rw-r--r--   0        0        0      461 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/type_mapper.sparql
+-rw-r--r--   0        0        0      814 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/wind_generating_units.sparql
+-rw-r--r--   0        0        0      944 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql/winding.sparql
+-rw-r--r--   0        0        0     2298 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/sparql_result_json.py
+-rw-r--r--   0        0        0     3193 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/templates.py
+-rw-r--r--   0        0        0     5650 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/type_mapper.py
+-rw-r--r--   0        0        0      768 2024-05-10 12:53:02.992521 cimsparql-3.3.1/cimsparql/url.py
+-rw-r--r--   0        0        0      616 2024-05-10 12:53:02.996521 cimsparql-3.3.1/cimsparql/value_mapper.py
+-rw-r--r--   0        0        0      459 2024-05-10 12:53:03.004521 cimsparql-3.3.1/pkg_data/blazegraph_repo_config.xml
+-rw-r--r--   0        0        0      676 2024-05-10 12:53:03.004521 cimsparql-3.3.1/pkg_data/namespaces.json
+-rw-r--r--   0        0        0      805 2024-05-10 12:53:03.004521 cimsparql-3.3.1/pkg_data/native_store_config_template.ttl
+-rw-r--r--   0        0        0     4219 2024-05-10 12:53:16.472606 cimsparql-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 cimsparql-3.3.1/PKG-INFO
```

### Comparing `cimsparql-3.2.1/LICENSE` & `cimsparql-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/README.md` & `cimsparql-3.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,14 @@
 ```python
 >>> from string import Template
 >>> query = 'PREFIX cim:<${cim}>\nPREFIX rdf: <${rdf}>\nSELECT ?mrid where {?mrid rdf:type cim:ACLineSegment}'
 >>> query_result = model.get_table_and_convert(model.template_to_query(Template(query)))
 >>> print(query_result)
 ```
 
-### List of available repos at the server
-
-```python
->>> from cimsparql.url import GraphDbConfig
->>> print(GraphDbConfig().repos)
-```
-
 ### Prefix and namespace
 
 Available namespace for current graphdb client (`gdbc` in the examples above),
 which can be used in queries (such as `rdf` and `cim`) can by found by
 
 ```python
 >>> print(model.prefixes)
```

### Comparing `cimsparql-3.2.1/cimsparql/adaptions.py` & `cimsparql-3.3.1/cimsparql/adaptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from __future__ import annotations
 
 import hashlib
 import re
 import uuid
-from collections.abc import Iterable
 from contextlib import suppress
 from pathlib import Path
 from string import Template
+from typing import TYPE_CHECKING
 
 from rdflib import ConjunctiveGraph
 from rdflib.namespace import XSD
 from rdflib.plugins.sparql import prepareUpdate
 from rdflib.term import BNode, Literal, URIRef
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from rdflib import Graph
+
 
 class XmlModelAdaptor:
     eq_predicate = "http://entsoe.eu/CIM/EquipmentCore/3/1"
 
     def __init__(self, filenames: Iterable[Path]) -> None:
         self.graph = ConjunctiveGraph()
         for filename in filenames:
@@ -24,16 +29,16 @@
             uri = URIRef(f"http://cimsparql/xml-adpator/{profile}")
             destination_graph = self.graph.get_context(uri)
             destination_graph.parse(filename, publicID="http://cim")
 
     def namespaces(self) -> dict[str, str]:
         return {str(prefix): str(name) for prefix, name in self.graph.namespaces()}
 
-    def graphs(self) -> set[URIRef]:
-        return {graph for _, _, _, graph in self.graph.quads()}
+    def graphs(self) -> set[Graph]:
+        return {graph for _, _, _, graph in self.graph.quads() if graph}
 
     @classmethod
     def from_folder(cls, folder: Path) -> XmlModelAdaptor:
         return XmlModelAdaptor(list(folder.glob("*.xml")))
 
     def add_mrid(self) -> None:
         """
@@ -44,18 +49,31 @@
         for result in self.graph.query(
             "select ?s ?g where {graph ?g {?s cim:IdentifiedObject.name ?name}}", initNs=ns
         ):
             mrid_str = str(result["s"]).rpartition("#_")[-1]
             mrid = mrid_str if is_uuid(mrid_str) else generate_uuid(mrid_str)
             self.graph.add((result["s"], identified_obj_mrid, Literal(mrid), result["g"]))
 
+    def set_generation_type(self) -> None:
+        self.graph.update(
+            """
+            delete {?gen_unit a ?gen_unit_type}
+            insert {?gen_unit a cim:ThermalGeneratingUnit}
+            where {
+              values ?gen_unit_type {cim:GeneratingUnit}
+              ?gen_unit a ?gen_unit_type
+            }
+            """
+        )
+
     def adapt(self, eq_uri: str) -> None:
         self.add_zero_sv_power_flow()
         self.add_mrid()
         self.add_dtypes()
+        self.set_generation_type()
         self.add_internal_eq_link(eq_uri)
 
     def add_zero_sv_power_flow(self) -> None:
         with open(
             Path(__file__).parent
             / "sparql/test_configuration_modifications/add_zero_sv_power.sparql"
         ) as f:
```

### Comparing `cimsparql-3.2.1/cimsparql/constants.py` & `cimsparql-3.3.1/cimsparql/constants.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/data_models.py` & `cimsparql-3.3.1/cimsparql/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,22 +100,24 @@
 
 class SynchronousMachinesSchema(NamedMarketResourceSchema):
     node: Series[str] = pa.Field()
     status: Series[bool] = pa.Field()
     station_group: Series[str] = pa.Field(nullable=True)
     station_group_name: Series[str] = pa.Field(nullable=True)
     substation_mrid: Series[str] = pa.Field()
-    maxP: Series[float] = pa.Field(nullable=True)  # noqa N815
-    minP: Series[float] = pa.Field(nullable=True)  # noqa N815
+    maxP: Series[float] = pa.Field()
+    minP: Series[float] = pa.Field()
     MO: Series[float] = pa.Field(nullable=True)
     bidzone: Series[str] = pa.Field(nullable=True)
     sn: Series[float] = pa.Field()
     p: Series[float] = pa.Field(nullable=True)
     q: Series[float] = pa.Field(nullable=True)
     connectivity_node: Series[str] = pa.Field()
+    generator_type: Series[str] = pa.Field()
+    schedule_resource: Series[str] = pa.Field(nullable=True)
 
 
 SynchronousMachinesDataFrame = DataFrame[SynchronousMachinesSchema]
 
 
 class ConnectionsSchema(MridResourceSchema):
     t_mrid_1: Series[str] = pa.Field()
```

### Comparing `cimsparql-3.2.1/cimsparql/graphdb.py` & `cimsparql-3.3.1/cimsparql/graphdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Graphdb CIM sparql client"""
+
 from __future__ import annotations
 
 import json
 import os
-from collections.abc import Callable
 from copy import deepcopy
 from dataclasses import dataclass, field
 from enum import auto
 from http import HTTPStatus
 from pathlib import Path
 from typing import TYPE_CHECKING, TypedDict, TypeVar
 
@@ -16,14 +16,17 @@
 import tenacity
 from SPARQLWrapper import JSON, POST, SPARQLWrapper
 from strenum import StrEnum
 
 from cimsparql.sparql_result_json import SparqlResultJson
 from cimsparql.url import service, service_blazegraph
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
 
 class SparqlResult(TypedDict):
     cols: list[str]
     data: list[dict[str, dict[str, str]]]
     out: list[dict[str, str]]
 
 
@@ -49,29 +52,26 @@
 class RestApi(StrEnum):
     RDF4J = auto()
     BLAZEGRAPH = auto()
     DIRECT_SPARQL_ENDPOINT = auto()
 
 
 def parse_namespaces_rdf4j(response: httpx.Response) -> dict[str, str]:
-    prefixes = {}
-    for line in response.text.split()[1:]:
-        prefix, uri = line.split(",")
-        prefixes[prefix] = uri
-    return prefixes
+    return dict(line.split(",") for line in response.text.split()[1:])
 
 
 @dataclass(frozen=True)
 class ServiceConfig:
     repo: str = field(default=os.getenv("GRAPHDB_REPO", "LATEST"))
     protocol: str = "https"
     server: str = field(default=os.getenv("GRAPHDB_SERVER", "127.0.0.1:7200"))
     path: str = ""
     user: str | None = field(default=os.getenv("GRAPHDB_USER"))
     passwd: str | None = field(default=os.getenv("GRAPHDB_USER_PASSWD"))
+    token: str | None = field(default=os.getenv("GRAPHDB_TOKEN"))
     rest_api: RestApi = field(default=RestApi(os.getenv("SPARQL_REST_API", "RDF4J")))
     ca_bundle: str | None = field(default=None)
 
     # Parameters for rest api
     # https://rdf4j.org/documentation/reference/rest-api/
     distinct: bool = False
     infer: bool = False
@@ -127,18 +127,18 @@
 
 if TYPE_CHECKING:
     from typing import Concatenate, ParamSpec
 
     P = ParamSpec("P")
     T = TypeVar("T")
 
-    RDF4J_DECORATED = Callable[Concatenate[GraphDBClient, P], T]
-
 
-def require_rdf4j(f: RDF4J_DECORATED) -> Callable[RDF4J_DECORATED]:
+def require_rdf4j(
+    f: Callable[Concatenate[GraphDBClient, P], T],
+) -> Callable[Concatenate[GraphDBClient, P], T]:
     def wrapper(cli: GraphDBClient, *args: P.args, **kwargs: P.kwargs) -> T:
         if cli.service_cfg.rest_api != RestApi.RDF4J:
             raise NotImplementedError("Function only implemented for RDF4J")
         return f(cli, *args, **kwargs)
 
     return wrapper
 
@@ -167,15 +167,18 @@
         custom_headers: dict[str, str] | None = None,
         sparql_wrapper: SPARQLWrapper | None = None,
     ) -> None:
         self.service_cfg = service_cfg or ServiceConfig()
         self.sparql = sparql_wrapper or SPARQLWrapper(self.service_cfg.url)
         self.sparql.setReturnFormat(JSON)
         self.sparql.setMethod(POST)
-        self.sparql.setCredentials(self.service_cfg.user, self.service_cfg.passwd)
+        if self.service_cfg.token:
+            self.sparql.addCustomHttpHeader("authorization", self.service_cfg.token)
+        else:
+            self.sparql.setCredentials(self.service_cfg.user, self.service_cfg.passwd)
         if self.service_cfg.timeout:
             self.sparql.setTimeout(self.service_cfg.timeout)
         self._update_sparql_parameters()
         if custom_headers:
             for name, value in custom_headers.items():
                 self.sparql.addCustomHttpHeader(name, value)
         self._prefixes = None
@@ -413,23 +416,27 @@
     response = httpx.put(url, content=config, headers={"Content-Type": "text/turtle"})
     if response.status_code not in ignored_errors:
         response.raise_for_status()
 
     return GraphDBClient(ServiceConfig(repo, protocol, server))
 
 
-def new_repo_blazegraph(url: str, repo: str, protocol: str = "https") -> GraphDBClient:
+def new_repo_blazegraph(
+    url: str, repo: str, protocol: str = "https", token: str | None = None
+) -> GraphDBClient:
     template = confpath() / "blazegraph_repo_config.xml"
     config = config_bytes_from_template(template, {"repo": repo})
 
     response = httpx.post(
         f"{protocol}://{url}", content=config, headers={"Content-type": "application/xml"}
     )
     response.raise_for_status()
-    client = GraphDBClient(ServiceConfig(repo, protocol, url, rest_api=RestApi.BLAZEGRAPH))
+    client = GraphDBClient(
+        ServiceConfig(repo, protocol, url, rest_api=RestApi.BLAZEGRAPH, token=token)
+    )
     return client
 
 
 def config_bytes_from_template(
     template: Path, params: dict[str, str], encoding: str = "utf-8"
 ) -> bytes:
     """
```

### Comparing `cimsparql-3.2.1/cimsparql/model.py` & `cimsparql-3.3.1/cimsparql/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """The cimsparql.model module contains the base class Model."""
+
 from __future__ import annotations
 
 import functools
 import logging
 import re
 import time
 from collections import defaultdict
-from collections.abc import Callable, Iterable
 from dataclasses import dataclass, field
 from functools import cached_property
-from string import Template
-from types import TracebackType
 from typing import TYPE_CHECKING, ParamSpec, TypeVar
 from uuid import uuid4
 
 import pandas as pd
 
 from cimsparql import templates
 from cimsparql.data_models import (
@@ -48,14 +46,18 @@
     TransformerWindingsDataFrame,
     WindGeneratingUnitsDataFrame,
 )
 from cimsparql.graphdb import GraphDBClient, ServiceConfig
 from cimsparql.type_mapper import TypeMapper
 
 if TYPE_CHECKING:
+    from collections.abc import Callable, Iterable
+    from string import Template
+    from types import TracebackType
+
     from cimsparql.value_mapper import ValueMapper
 
 
 @dataclass
 class ModelConfig:
     system_state_repo: str | None = None
     eq_repo: str | None = None
```

### Comparing `cimsparql-3.2.1/cimsparql/sparql/ac_lines.sparql` & `cimsparql-3.3.1/cimsparql/sparql/ac_lines.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/borders.sparql` & `cimsparql-3.3.1/cimsparql/sparql/borders.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/branch_node_withdraw.sparql` & `cimsparql-3.3.1/cimsparql/sparql/branch_node_withdraw.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/bus.sparql` & `cimsparql-3.3.1/cimsparql/sparql/bus.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/connections.sparql` & `cimsparql-3.3.1/cimsparql/sparql/connections.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/connectivity_nodes.sparql` & `cimsparql-3.3.1/cimsparql/sparql/connectivity_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/converter_hvdc_bidzones.sparql` & `cimsparql-3.3.1/cimsparql/sparql/converter_hvdc_bidzones.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/converters.sparql` & `cimsparql-3.3.1/cimsparql/sparql/converters.sparql`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Name: Converters
 PREFIX cim:<${cim}>
 PREFIX xsd:<${xsd}>
 PREFIX SN:<${SN}>
-select ?mrid ?name ?alias ?p ?q ?substation_mrid ?status ?node ?connectivity_node
+PREFIX ALG:<${ALG}>
+select ?mrid ?name ?alias ?p ?q ?substation_mrid ?status ?node ?connectivity_node ?controller ?controller_factor
 where {
   # Extract active and reactive power for the converter
   ?converter cim:ACDCConverter.p ?p;
              cim:ACDCConverter.q ?q .
 
   optional {?converter ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?in_service .}
 
@@ -15,33 +16,37 @@
   optional {?terminal cim:Terminal.TopologicalNode/cim:IdentifiedObject.mRID ?term_top_node_mrid .}
 
   # Extract the mrid of the topoligical node associated with the connectivity node for the terminal
   optional {?con_node cim:ConnectivityNode.TopologicalNode/cim:IdentifiedObject.mRID ?con_top_node_mrid .}
 
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
-  # Extract mrid, name, substation and optionally aliasName of the converter
-  ?converter cim:IdentifiedObject.mRID ?mrid;
-             cim:IdentifiedObject.name ?name;
-             cim:Equipment.EquipmentContainer/cim:VoltageLevel.Substation ?substation .
-  optional {?converter cim:IdentifiedObject.aliasName ?alias .}
-
-  # Find area and mRID for the substation
-  ?substation cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area;
-              cim:IdentifiedObject.mRID ?substation_mrid .
-
-  # Extract properties for the terminals for the converter
-  ?terminal cim:Terminal.ConductingEquipment ?converter;
-            cim:Terminal.ConnectivityNode ?con_node;
-            cim:Terminal.sequenceNumber|cim:ACDCTerminal.sequenceNumber 1 .
-  ?con_node cim:IdentifiedObject.mRID ?connectivity_node .
-  optional {?converter SN:Equipment.networkAnalysisEnable ?_analysis_enabled .}
-  filter regex(?area, '${region}')
-  bind(coalesce(?_analysis_enabled, True) as ?analysis_enabled)
-  filter(?analysis_enabled)
+    # Extract mrid, name, substation and optionally aliasName of the converter
+    ?converter cim:IdentifiedObject.mRID ?mrid;
+               cim:IdentifiedObject.name ?name;
+               cim:Equipment.EquipmentContainer/cim:VoltageLevel.Substation ?substation;
+	       ALG:VoltageSourceConverter.DCPole|ALG:DCConverter.DCPole ?pole.
+    ?pole ALG:DCPole.DCController/cim:IdentifiedObject.mRID ?controller;
+          ALG:DCPole.participationFactor ?controller_factor;
+
+    optional {?converter cim:IdentifiedObject.aliasName ?alias .}
+
+    # Find area and mRID for the substation
+    ?substation cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area;
+		cim:IdentifiedObject.mRID ?substation_mrid .
+
+    # Extract properties for the terminals for the converter
+    ?terminal cim:Terminal.ConductingEquipment ?converter;
+              cim:Terminal.ConnectivityNode ?con_node;
+              cim:Terminal.sequenceNumber|cim:ACDCTerminal.sequenceNumber 1 .
+    ?con_node cim:IdentifiedObject.mRID ?connectivity_node .
+    optional {?converter SN:Equipment.networkAnalysisEnable ?_analysis_enabled .}
+    filter regex(?area, '${region}')
+    bind(coalesce(?_analysis_enabled, True) as ?analysis_enabled)
+    filter(?analysis_enabled)
   }
 
   # Asiign an mrid to the ?node variable. The first that exists is choden
   # 1) mRID of the topological node associated with the connectivity node
   # 2) mRID of the topological node for the terminal
   # 3) mRID of the terminal
   bind(coalesce(?con_top_node_mrid, ?term_top_node_mrid) as ?node)
```

### Comparing `cimsparql-3.2.1/cimsparql/sparql/coordinates.sparql` & `cimsparql-3.3.1/cimsparql/sparql/coordinates.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/dc_active_power_flow.sparql` & `cimsparql-3.3.1/cimsparql/sparql/dc_active_power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/exchange.sparql` & `cimsparql-3.3.1/cimsparql/sparql/exchange.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/full_model.sparql` & `cimsparql-3.3.1/cimsparql/sparql/full_model.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/loads.sparql` & `cimsparql-3.3.1/cimsparql/sparql/loads.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/power_flow.sparql` & `cimsparql-3.3.1/cimsparql/sparql/power_flow.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/regions.sparql` & `cimsparql-3.3.1/cimsparql/sparql/regions.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/series_compensators.sparql` & `cimsparql-3.3.1/cimsparql/sparql/series_compensators.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/substation_voltage_level.sparql` & `cimsparql-3.3.1/cimsparql/sparql/substation_voltage_level.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/sv_branch.sparql` & `cimsparql-3.3.1/cimsparql/sparql/sv_branch.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/switches.sparql` & `cimsparql-3.3.1/cimsparql/sparql/switches.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/synchronous_machines.sparql` & `cimsparql-3.3.1/cimsparql/sparql/synchronous_machines.sparql`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 # Name: Synchronous machines
 PREFIX cim: <${cim}>
 PREFIX SN: <${SN}>
-select ?mrid ?name ?market_code ?node ?status ?station_group ?station_group_name ?substation_mrid ?maxP ?minP ?MO ?bidzone ?sn ?p ?q ?connectivity_node
+select ?mrid ?name ?market_code ?node ?status ?station_group ?station_group_name ?substation_mrid ?maxP ?minP ?MO ?bidzone ?sn ?p ?q ?connectivity_node ?generator_type ?schedule_resource
 where {
   ?terminal cim:ACDCTerminal.connected ?connected .
   optional {?terminal cim:Terminal.TopologicalNode/cim:IdentifiedObject.mRID ?term_top_node_mrid}
   optional {?con_node cim:ConnectivityNode.TopologicalNode/cim:IdentifiedObject.mRID ?con_top_node_mrid .}
   optional {?machine ^cim:SvStatus.ConductingEquipment/cim:SvStatus.inService ?in_service} .
   optional {?machine cim:RotatingMachine.p ?p;cim:RotatingMachine.q ?q .}
 
   # Extract properties for synchronous machines.
   ?_eq_subject <http://entsoe.eu/CIM/EquipmentCore/3/1> ?eq_repo .
   service ?eq_repo {
+    values ?gen_type {cim:NuclearGeneratingUnit cim:MktGeneratingUnit cim:HydroGeneratingUnit cim:WindGeneratingUnit cim:ThermalGeneratingUnit cim:SolarGeneratingUnit}
     ?machine a cim:SynchronousMachine;
           cim:IdentifiedObject.name ?name;
           cim:RotatingMachine.ratedS ?sn;
-          cim:IdentifiedObject.mRID ?mrid;
           ^cim:Terminal.ConductingEquipment ?terminal;
-          cim:Equipment.EquipmentContainer/cim:VoltageLevel.Substation ?substation .
+          cim:Equipment.EquipmentContainer/cim:VoltageLevel.Substation ?substation;
+	  # TODO: Seems like cim15 uses SynchronousMachine while cim16 uses RotatingMachine. Will fix this when we have a proper cim16 model
+          cim:SynchronousMachine.GeneratingUnit|cim:RotatingMachine.GeneratingUnit ?gen_unit.
+
+    ?gen_unit a ?gen_type;
+	 cim:IdentifiedObject.mRID ?mrid;
+	 cim:GeneratingUnit.minOperatingP ?minP;
+         cim:GeneratingUnit.maxOperatingP ?maxP.
+
     ?terminal cim:Terminal.ConnectivityNode ?con_node .
     ?con_node cim:IdentifiedObject.mRID ?connectivity_node .
 
     # Extract area and mrid for the substation associated with a sync machine
     ?substation cim:Substation.Region/cim:SubGeographicalRegion.Region/cim:IdentifiedObject.name ?area;
                 cim:IdentifiedObject.mRID ?substation_mrid .
 
     # Optionally extract min/max operating power for each machin
     optional {
-      ?machine cim:SynchronousMachine.GeneratingUnit ?gen_unit.
-      ?gen_unit cim:GeneratingUnit.minOperatingP ?minP;
-                cim:GeneratingUnit.maxOperatingP ?maxP .
-      optional {
-        ?gen_unit SN:GeneratingUnit.marketCode ?market_code;
-                  SN:GeneratingUnit.groupAllocationWeight ?MO;
-                  SN:GeneratingUnit.ScheduleResource ?ScheduleResource .
-        ?ScheduleResource SN:ScheduleResource.marketCode ?station_group;
-                          cim:IdentifiedObject.name ?station_group_name .
-      }
+      ?gen_unit	cim:GeneratingUnit.minOperatingP ?minP;
+		cim:GeneratingUnit.maxOperatingP ?maxP.
+
+    optional {
+	?gen_unit SN:GeneratingUnit.marketCode ?market_code;
+           SN:GeneratingUnit.groupAllocationWeight ?MO;
+           SN:GeneratingUnit.ScheduleResource ?ScheduleResource .
+	?ScheduleResource SN:ScheduleResource.marketCode ?station_group;
+                   cim:IdentifiedObject.mRID ?schedule_resource;
+                   cim:IdentifiedObject.name ?station_group_name .
     }
+      }
     filter regex(?area, '${region}')
 
     # Optionally extract bidzone for the substation associated with the sync machin
     optional {
       ?substation SN:Substation.MarketDeliveryPoint/SN:MarketDeliveryPoint.BiddingArea/SN:BiddingArea.marketCode ?bidzone
     } .
 
     # Opionally extract non-CIM standard properties generating units
     optional {?machine SN:Equipment.networkAnalysisEnable ?_network_analysis}
+    bind(replace(str(?gen_type), str(cim:), "") as ?generator_type)
   }
   bind(coalesce(?_network_analysis, True) as ?network_analysis)
   bind(coalesce(?con_top_node_mrid, ?term_top_node_mrid) as ?node)
   bind(coalesce(?in_service, ?connected) as ?status)
   filter(?network_analysis)
 }
```

### Comparing `cimsparql-3.2.1/cimsparql/sparql/three_winding.sparql` & `cimsparql-3.3.1/cimsparql/sparql/three_winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/three_winding_dummy_nodes.sparql` & `cimsparql-3.3.1/cimsparql/sparql/three_winding_dummy_nodes.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/three_winding_loss.sparql` & `cimsparql-3.3.1/cimsparql/sparql/three_winding_loss.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/transformers.sparql` & `cimsparql-3.3.1/cimsparql/sparql/transformers.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/transformers_connected_to_converter.sparql` & `cimsparql-3.3.1/cimsparql/sparql/transformers_connected_to_converter.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/two_winding_transformer.sparql` & `cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/two_winding_transformer_angle.sparql` & `cimsparql-3.3.1/cimsparql/sparql/two_winding_transformer_angle.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/wind_generating_units.sparql` & `cimsparql-3.3.1/cimsparql/sparql/wind_generating_units.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql/winding.sparql` & `cimsparql-3.3.1/cimsparql/sparql/winding.sparql`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/sparql_result_json.py` & `cimsparql-3.3.1/cimsparql/sparql_result_json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from polyfactory.decorators import post_generated
 from polyfactory.factories import pydantic_factory
 from pydantic import BaseModel, ConfigDict, Field
 
+if TYPE_CHECKING:
+    from typing import Self
+
 
 class CimsparqlBaseModel(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
 
 class SparqlResultHead(CimsparqlBaseModel):
     link: list[str] = Field(default_factory=list)
@@ -30,15 +37,15 @@
 
     https://www.w3.org/TR/sparql11-results-json/
     """
 
     head: SparqlResultHead
     results: SparqlData
 
-    def validate_column_consistency(self) -> None:
+    def validate_column_consistency(self) -> Self:
         """
         This is an quite expensive validation since it iterates over the entire result.
         Therefore, it is not implemented as a validator, but it must be explicitly called
         when it is desired to perform the validation
         """
         column_set = set(self.head.variables)
         for item in self.results.bindings:
```

### Comparing `cimsparql-3.2.1/cimsparql/templates.py` & `cimsparql-3.3.1/cimsparql/templates.py`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/cimsparql/type_mapper.py` & `cimsparql-3.3.1/cimsparql/type_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import dataclasses
-from collections.abc import Callable, Generator
 from contextlib import contextmanager
 from decimal import Decimal
 from typing import TYPE_CHECKING, Any
 
 import pandas as pd
 
 from cimsparql.graphdb import GraphDBClient, ServiceConfig
 from cimsparql.templates import TYPE_MAPPER_QUERY
 
+if TYPE_CHECKING:
+    from collections.abc import Callable, Generator
+
 # Type-caster that can be used with pandas. It can be python types, numpy dtypes or string
 # value. Examples: float, "int", int, "string"
 if TYPE_CHECKING:
     TYPE_CASTER = Callable[[Any], Any] | str
     SPARQL_TYPE = str
     COL_NAME = str
     PREFIX = str
```

### Comparing `cimsparql-3.2.1/cimsparql/value_mapper.py` & `cimsparql-3.3.1/cimsparql/value_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pandas as pd
 
 
 class ValueMapper:
-    def map(self, df: pd.DataFrame) -> pd.DataFrame:  # noqa A003
+    def map(self, df: pd.DataFrame) -> pd.DataFrame:  # A003
         return df
 
 
 class MridMapper(ValueMapper):
     """
     Mapper which replaces all matches of uri_regex with an empty string
     in columns which constains mrid in the name
     """
 
     def __init__(self, uri_regex: str = "^([^#_|^#]+)(#_|#)") -> None:
         self.uri_regex = uri_regex
 
-    def map(self, df: pd.DataFrame) -> pd.DataFrame:  # noqa A003
+    def map(self, df: pd.DataFrame) -> pd.DataFrame:  # A003
         for col in filter(lambda col: "mrid" in col, df.columns):
             df[col] = df[col].str.replace(self.uri_regex, "", regex=True)
         return df
```

### Comparing `cimsparql-3.2.1/pkg_data/namespaces.json` & `cimsparql-3.3.1/pkg_data/namespaces.json`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/pkg_data/native_store_config_template.ttl` & `cimsparql-3.3.1/pkg_data/native_store_config_template.ttl`

 * *Files identical despite different names*

### Comparing `cimsparql-3.2.1/pyproject.toml` & `cimsparql-3.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cimsparql"
-version = "3.2.1"
+version = "3.3.1"
 description = "CIM query utilities"
 readme = "README.md"
 authors = ["Statnett Datascience <Datascience.Drift@Statnett.no>"]
 repository = "https://github.com/statnett/cimsparql.git"
 include = ["pkg_data/*"]
 exclude = ["tests/*"]
 
@@ -27,15 +27,14 @@
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-httpserver = "*"
 pytest-integration = "*"
 pytest-profiling = "*"
 
 [tool.poetry.group.style.dependencies]
-black = "*"
 ruff = "*"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 ruff-lsp = "*"
 
 [tool.poetry.group.docs]
@@ -50,14 +49,19 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 pattern = '^(?P<base>\d+\.\d+\.\d+)(-?((?P<stage>[a-zA-Z]+)\.?(?P<revision>\d+)?))?$'
 
 [tool.ruff]
+# Assume Python 3.10
+target-version = "py310"
+line-length = 100
+
+[tool.ruff.lint]
 select = [
   "A", # flake8-builtins
   "ANN", # flake8-annotations
   "ARG", # flake8-unused-arguments
   "B", # flake8-bugbear
   "C4", # flake8-comprehensions
   "C90", # mccabe
@@ -72,15 +76,15 @@
   "NPY", # numpy specific rules
   "PERF", # Perflint
   "PIE", # flake8-pie
   "RUF", # Ruff specific rules
   "S", # flake8-bandit
   "SIM", # flake8-simplify
   "T20", # flake8-print
-  "TCH001", # flake8-type-checking
+  "TCH", # flake8-type-checking
   "TRY", # tryceratops
   "UP", # pyupgrade
   "YTT", # flake8-2020
 ]
 
 ignore = ['S101', 'COM812', 'ANN101', 'ANN102', 'ANN401', 'TRY003']
 
@@ -109,55 +113,34 @@
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
 
-# Same as Black.
-line-length = 100
-
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.10
-target-version = "py310"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
+"cimsparql/data_models.py" = ["N815"]
 "docs/conf.py" = ["A001"]
 "tests/test*.py" = ["ANN201"]
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 # Allow Pydantic's `@validator` decorator to trigger class method treatment.
 classmethod-decorators = ["pandera.dataframe_check"]
 
-[tool.ruff.flake8-import-conventions]
+[tool.ruff.lint.flake8-import-conventions]
 
-[tool.ruff.flake8-import-conventions.aliases]
+[tool.ruff.lint.flake8-import-conventions.aliases]
 # Declare the default aliases.
 pandas = "pd"
 pandera = "pa"
 
-[tool.black]
-line-length = 100
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.git
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-  | profiling
-)/
-'''
-
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_lines = [
               "pragma: no cover",
               "raise AssertionError",
               "raise NotImplementedError",
               "if verbose:",
```

### Comparing `cimsparql-3.2.1/PKG-INFO` & `cimsparql-3.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cimsparql
-Version: 3.2.1
+Version: 3.3.1
 Summary: CIM query utilities
 Home-page: https://github.com/statnett/cimsparql.git
 Author: Statnett Datascience
 Author-email: Datascience.Drift@Statnett.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -66,21 +66,14 @@
 ```python
 >>> from string import Template
 >>> query = 'PREFIX cim:<${cim}>\nPREFIX rdf: <${rdf}>\nSELECT ?mrid where {?mrid rdf:type cim:ACLineSegment}'
 >>> query_result = model.get_table_and_convert(model.template_to_query(Template(query)))
 >>> print(query_result)
 ```
 
-### List of available repos at the server
-
-```python
->>> from cimsparql.url import GraphDbConfig
->>> print(GraphDbConfig().repos)
-```
-
 ### Prefix and namespace
 
 Available namespace for current graphdb client (`gdbc` in the examples above),
 which can be used in queries (such as `rdf` and `cim`) can by found by
 
 ```python
 >>> print(model.prefixes)
```

