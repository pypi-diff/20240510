# Comparing `tmp/oaklib-0.6.5.tar.gz` & `tmp/oaklib-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.6.5.tar", max compression
+gzip compressed data, was "oaklib-0.6.6.tar", max compression
```

## Comparing `oaklib-0.6.5.tar` & `oaklib-0.6.6.tar`

### file list

```diff
@@ -1,316 +1,316 @@
--rw-r--r--   0        0        0    11357 2024-04-27 02:05:43.507818 oaklib-0.6.5/LICENSE
--rw-r--r--   0        0        0     7258 2024-04-27 02:05:43.507818 oaklib-0.6.5/README.md
--rw-r--r--   0        0        0     3522 2024-04-27 02:06:20.159785 oaklib-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      272 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/__init__.py
--rw-r--r--   0        0        0   231525 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     1011 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      529 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
--rw-r--r--   0        0        0      118 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4730 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      149 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1461 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2547 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2446 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12105 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     7719 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     6100 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    38339 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    13058 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13288 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3262 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24250 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35746 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14566 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15776 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17296 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26474 2024-04-27 02:05:43.671818 oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    33955 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     4155 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    51109 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    19600 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   116914 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    31452 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3348 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25157 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6684 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12826 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22645 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5690 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0    23481 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.py
--rw-r--r--   0        0        0     2476 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.yaml
--rw-r--r--   0        0        0     9909 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18432 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5880 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    21645 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4996 2024-04-27 02:05:43.675818 oaklib-0.6.5/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    33912 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     9005 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     6595 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     6452 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0    16195 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2180 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1055 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     3565 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30523 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0    28777 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/llm_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ncbi/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    17122 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     8071 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1250 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    13670 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pantherdb/__init__.py
--rw-r--r--   0        0        0    12625 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    37863 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      247 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0    11605 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    46328 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    23081 2024-04-27 02:05:43.679818 oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    38067 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2325 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   115796 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tabular/__init__.py
--rw-r--r--   0        0        0    19432 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tabular/robot_template_implementation.py
--rw-r--r--   0        0        0     3279 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tabular/tabular_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     5442 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    20090 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0    14740 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17267 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/indexes/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/indexes/edge_index.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/__init__.py
--rw-r--r--   0        0        0      748 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/owl_reasoner.py
--rw-r--r--   0        0        0      105 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/reasoner.py
--rw-r--r--   0        0        0     6960 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/inference/relation_graph_reasoner.py
--rw-r--r--   0        0        0      913 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    28686 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    55465 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     9243 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    21219 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     3222 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      788 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13680 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    24049 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      786 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/ontology_generator_interface.py
--rw-r--r--   0        0        0      784 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    13645 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8606 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2287 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    16173 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2113 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18295 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0    10076 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0    12915 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1565 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     9012 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2024-04-27 02:05:43.683818 oaklib-0.6.5/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0      785 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2672 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3485 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5126 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3956 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1979 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2363 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4732 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2148 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     2101 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1131 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0     1673 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/hpoa_g2d_association_parser.py
--rw-r--r--   0        0        0      603 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      654 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1672 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      526 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1433 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      708 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8681 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/resource.py
--rw-r--r--   0        0        0    15958 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/selector.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/__init__.py
--rw-r--r--   0        0        0      589 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/chained_ontology_transformer.py
--rw-r--r--   0        0        0     2757 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/edge_filter_transformer.py
--rw-r--r--   0        0        0     1257 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/graph_transformer.py
--rw-r--r--   0        0        0     1804 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/node_filter_transformer.py
--rw-r--r--   0        0        0      470 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/ontology_transformer.py
--rw-r--r--   0        0        0     6353 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/sep_transformer.py
--rw-r--r--   0        0        0     1768 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/transformers/transformers_factory.py
--rw-r--r--   0        0        0      177 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3427 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/__init__.py
--rw-r--r--   0        0        0     7694 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
--rw-r--r--   0        0        0     4093 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_analyzer.py
--rw-r--r--   0        0        0     8829 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_summarizer.py
--rw-r--r--   0        0        0     2436 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_utilities.py
--rw-r--r--   0        0        0     1540 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0     1356 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/format_utilities.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2857 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     1015 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/keyval_cache.py
--rw-r--r--   0        0        0     3425 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19249 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0    10235 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/patternizer.py
--rw-r--r--   0        0        0     6881 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/lexical/synonymizer.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14422 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15527 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0    10929 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2558 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      690 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    30409 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/__init__.py
--rw-r--r--   0        0        0     5283 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/doi_wrapper.py
--rw-r--r--   0        0        0      924 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
--rw-r--r--   0        0        0     6575 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
--rw-r--r--   0        0        0      380 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     2545 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.687818 oaklib-0.6.5/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    12015 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    18045 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    11118 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1275 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0      122 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/writers/__init__.py
--rw-r--r--   0        0        0    16522 2024-04-27 02:05:43.691818 oaklib-0.6.5/src/oaklib/utilities/writers/change_handler.py
--rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 oaklib-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 23:39:19.984135 oaklib-0.6.6/LICENSE
+-rw-r--r--   0        0        0     7258 2024-05-09 23:39:19.984135 oaklib-0.6.6/README.md
+-rw-r--r--   0        0        0     3599 2024-05-09 23:39:53.832227 oaklib-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      272 2024-05-09 23:39:20.152136 oaklib-0.6.6/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   231525 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0     1011 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      529 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      118 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4730 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      149 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1461 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2547 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2446 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12105 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     7719 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     6100 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    38339 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    13058 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13288 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3262 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24250 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35746 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14566 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15776 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17296 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26474 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33955 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     4155 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    51109 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    19600 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   116914 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    31452 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3348 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25157 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6684 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12826 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22645 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5690 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0    23481 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.py
+-rw-r--r--   0        0        0     2476 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18432 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5880 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    21645 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4996 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33912 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     9005 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     6549 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     6452 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     6377 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8848 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0    16195 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2180 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1055 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     3565 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30523 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0    28777 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/llm_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7034 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ncbi/__init__.py
+-rw-r--r--   0        0        0     7034 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    17122 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     8071 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2641 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1250 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    13670 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pantherdb/__init__.py
+-rw-r--r--   0        0        0    12625 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    37863 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      247 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0    11605 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    46328 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    23081 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    38067 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2325 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   115796 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tabular/__init__.py
+-rw-r--r--   0        0        0    19432 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tabular/robot_template_implementation.py
+-rw-r--r--   0        0        0     3279 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tabular/tabular_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     5442 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    20090 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0    14740 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17267 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/indexes/__init__.py
+-rw-r--r--   0        0        0     3089 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/indexes/edge_index.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/__init__.py
+-rw-r--r--   0        0        0      748 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/owl_reasoner.py
+-rw-r--r--   0        0        0      105 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/reasoner.py
+-rw-r--r--   0        0        0     6960 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/relation_graph_reasoner.py
+-rw-r--r--   0        0        0      913 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    28686 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    55465 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     9243 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    21219 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     3222 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      788 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13680 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    24049 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      786 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/ontology_generator_interface.py
+-rw-r--r--   0        0        0      784 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    13645 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8606 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2287 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    16173 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2113 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18295 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0    10076 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0    12915 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2091 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1565 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     9012 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0      785 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2672 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3485 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5101 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3956 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1979 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2363 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1525 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4732 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2148 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     2101 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1131 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0     1673 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/hpoa_g2d_association_parser.py
+-rw-r--r--   0        0        0      603 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      654 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1672 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      526 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1433 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      708 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8681 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/resource.py
+-rw-r--r--   0        0        0    15958 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/selector.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/__init__.py
+-rw-r--r--   0        0        0      589 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/chained_ontology_transformer.py
+-rw-r--r--   0        0        0     2757 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/edge_filter_transformer.py
+-rw-r--r--   0        0        0     1257 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/graph_transformer.py
+-rw-r--r--   0        0        0     1804 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/node_filter_transformer.py
+-rw-r--r--   0        0        0      470 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/ontology_transformer.py
+-rw-r--r--   0        0        0     6353 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/sep_transformer.py
+-rw-r--r--   0        0        0     1768 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/transformers_factory.py
+-rw-r--r--   0        0        0      177 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3427 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/__init__.py
+-rw-r--r--   0        0        0     7694 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
+-rw-r--r--   0        0        0     4093 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_analyzer.py
+-rw-r--r--   0        0        0     8829 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_summarizer.py
+-rw-r--r--   0        0        0     2436 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_utilities.py
+-rw-r--r--   0        0        0     1540 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0     1356 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/format_utilities.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2491 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2857 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     1015 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/keyval_cache.py
+-rw-r--r--   0        0        0     3425 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19249 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0    10235 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/patternizer.py
+-rw-r--r--   0        0        0     6881 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/synonymizer.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14422 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15527 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0    10929 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2558 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      690 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    30409 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/__init__.py
+-rw-r--r--   0        0        0     5283 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/doi_wrapper.py
+-rw-r--r--   0        0        0      960 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
+-rw-r--r--   0        0        0     6575 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
+-rw-r--r--   0        0        0      380 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     2545 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    12015 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    18045 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    11118 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1275 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0      122 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/writers/__init__.py
+-rw-r--r--   0        0        0    15885 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/writers/change_handler.py
+-rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 oaklib-0.6.6/PKG-INFO
```

### Comparing `oaklib-0.6.5/LICENSE` & `oaklib-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/README.md` & `oaklib-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/pyproject.toml` & `oaklib-0.6.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.6.5"
+version = "v0.6.6"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -19,15 +19,15 @@
 ratelimit = ">=2.2.1"
 appdirs = ">=1.4.4"
 semsql = ">=0.3.1"
 kgcl-schema = "^0.6.8"
 
 funowl = ">=0.2.0"
 gilda = {version = ">=1.0.0", optional = true}
-semsimian = {version = ">=0.2.15", optional = true}
+semsimian = {version = ">=0.2.16", optional = true}
 kgcl-rdflib = "0.5.0"
 llm = {version = "*", optional = true}
 html2text = {version = "*", optional = true}
 aiohttp = {version = "*", optional = true}
 pystow = ">=0.5.0"
 class-resolver = ">=0.4.2"
 ontoportal-client = ">=0.0.3"
@@ -101,14 +101,15 @@
     "D212",  # `multi-line-summary-first-line`
     "E731",  # Do not assign a `lambda` expression, use a `def`
     "B005",  # Using `.strip()` with multi-character strings is misleading the reader
     "S101",  # Use of `assert` detected
     "S607",  # Starting a process with a partial executable path
     "S608",  # Possible SQL injection vector through string-based query construction
     "S603",  # `subprocess` call: check for execution of untrusted input
+    "B024",  # XXX is an abstract base class, but it has no abstract methods
     ]
 lint.exclude = ["src/oaklib/datamodels/*"]
 line-length = 120
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 lint.fixable = ["ALL"]
```

### Comparing `oaklib-0.6.5/src/oaklib/cli.py` & `oaklib-0.6.6/src/oaklib/cli.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.6.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.6.6/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml` & `oaklib-0.6.6/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/conf/obograph-style.json` & `oaklib-0.6.6/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/converters/data_model_converter.py` & `oaklib-0.6.6/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.6.6/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/association.py` & `oaklib-0.6.6/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/association.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/cx.py` & `oaklib-0.6.6/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/cx.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/fhir.py` & `oaklib-0.6.6/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/input_specification.py` & `oaklib-0.6.6/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/item_list.py` & `oaklib-0.6.6/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/obograph.py` & `oaklib-0.6.6/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/oxo.py` & `oaklib-0.6.6/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/search.py` & `oaklib-0.6.6/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/similarity.py` & `oaklib-0.6.6/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.py` & `oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/synonymizer_datamodel.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.6.6/src/oaklib/datamodels/vocabulary.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,14 @@
 CREATED = "dcterms:created"
 IAO_TERM_EDITOR = "IAO:0000117"
 ALL_CONTRIBUTOR_PREDICATES = [OIO_CREATED_BY, CONTRIBUTOR, CREATOR, IAO_TERM_EDITOR]
 
 OWL_VERSION_INFO = "owl:versionInfo"
 OWL_VERSION_IRI = "owl:versionIRI"
 
-MAPPING_EDGE_DELETION = "MappingEdgeDeletion"
 CLASS_CREATION = "ClassCreation"
 NODE_CREATION = "NodeCreation"
 NODE_DELETION = "NodeDeletion"
 NODE_TEXT_DEFINITION_CHANGE = "NodeTextDefinitionChange"
 
 EXTENDED_SCOPE_TO_SYNONYM_PRED_MAP = {
     "LABEL": LABEL_PREDICATE,
```

### Comparing `oaklib-0.6.5/src/oaklib/implementations/__init__.py` & `oaklib-0.6.6/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/gilda.py` & `oaklib-0.6.6/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/llm_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/llm_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.6.6/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.6.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/pantherdb/pantherdb_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/pantherdb/pantherdb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.6.6/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/tabular/robot_template_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/tabular/robot_template_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/tabular/tabular_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/tabular/tabular_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.6.6/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/indexes/edge_index.py` & `oaklib-0.6.6/src/oaklib/indexes/edge_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/inference/owl_reasoner.py` & `oaklib-0.6.6/src/oaklib/inference/owl_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/inference/relation_graph_reasoner.py` & `oaklib-0.6.6/src/oaklib/inference/relation_graph_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/__init__.py` & `oaklib-0.6.6/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/ontology_generator_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/ontology_generator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/search_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.6.6/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/heatmap_writer.py` & `oaklib-0.6.6/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/html_writer.py` & `oaklib-0.6.6/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/obograph_writer.py` & `oaklib-0.6.6/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.6.6/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import atexit
 import logging
 import sys
-from abc import ABC
 from dataclasses import dataclass, field
 from typing import Any, ClassVar, Dict, Iterable, List, Mapping, Optional, Type, Union
 
 from linkml_runtime import SchemaView
 from linkml_runtime.dumpers import json_dumper
 from linkml_runtime.utils.yamlutils import YAMLRoot
 
@@ -16,15 +15,15 @@
 from oaklib.utilities.iterator_utils import chunk
 
 ID_KEY = "id"
 LABEL_KEY = "label"
 
 
 @dataclass
-class StreamingWriter(ABC):
+class StreamingWriter:
     """
     Base class for streaming writers.
     """
 
     file: Any = field(default_factory=lambda: sys.stdout)
     ontology_interface: BasicOntologyInterface = None
     display_options: List[str] = None
```

### Comparing `oaklib-0.6.5/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.6.6/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/mappers/base_mapper.py` & `oaklib-0.6.6/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.6.6/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/__init__.py` & `oaklib-0.6.6/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.6.6/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/hpoa_g2d_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/hpoa_g2d_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/parser_base.py` & `oaklib-0.6.6/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.6.6/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/resource.py` & `oaklib-0.6.6/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/selector.py` & `oaklib-0.6.6/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/transformers/chained_ontology_transformer.py` & `oaklib-0.6.6/src/oaklib/transformers/chained_ontology_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/transformers/edge_filter_transformer.py` & `oaklib-0.6.6/src/oaklib/transformers/edge_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/transformers/graph_transformer.py` & `oaklib-0.6.6/src/oaklib/transformers/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/transformers/node_filter_transformer.py` & `oaklib-0.6.6/src/oaklib/transformers/node_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/transformers/sep_transformer.py` & `oaklib-0.6.6/src/oaklib/transformers/sep_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/transformers/transformers_factory.py` & `oaklib-0.6.6/src/oaklib/transformers/transformers_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.6.6/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.6.6/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.6.6/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py` & `oaklib-0.6.6/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_analyzer.py` & `oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_summarizer.py` & `oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_summarizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/axioms/logical_definition_utilities.py` & `oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/basic_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/format_utilities.py` & `oaklib-0.6.6/src/oaklib/utilities/format_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.6.6/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.6.6/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/keyval_cache.py` & `oaklib-0.6.6/src/oaklib/utilities/keyval_cache.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.6.6/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/label_utilities.py` & `oaklib-0.6.6/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.6.6/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/lexical/patternizer.py` & `oaklib-0.6.6/src/oaklib/utilities/lexical/patternizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/lexical/synonymizer.py` & `oaklib-0.6.6/src/oaklib/utilities/lexical/synonymizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.6.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.6.6/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.6.6/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.6.6/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/publication_utils/doi_wrapper.py` & `oaklib-0.6.6/src/oaklib/utilities/publication_utils/doi_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubdb_wrapper.py` & `oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubdb_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import ClassVar, Dict, List, Optional
 
 import pystow
 import requests
 import requests_cache
 
@@ -28,9 +28,10 @@
             cache_path = pystow.join("oaklib", "session_cache", self.name, ensure_exists=True)
         self.set_cache(cache_path)
 
     def set_cache(self, name: str) -> None:
         self.session = requests_cache.CachedSession(name)
         self._uses_cache = True
 
+    @abstractmethod
     def objects_by_ids(self, object_ids: List[str]) -> List[Dict]:
         raise NotImplementedError
```

### Comparing `oaklib-0.6.5/src/oaklib/utilities/publication_utils/pubmed_wrapper.py` & `oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubmed_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.6.6/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.6.6/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.6.6/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.6.6/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/table_filler.py` & `oaklib-0.6.6/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.6.6/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.6.6/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.6.6/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.6.6/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.6.6/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.5/src/oaklib/utilities/writers/change_handler.py` & `oaklib-0.6.6/src/oaklib/utilities/writers/change_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,44 +63,30 @@
             for change in value
         ]
 
         # Define the header for the table
         header = "| Subject | Predicate | Object|"
 
         # Write the "Edges Created" section as a collapsible markdown table
-        self.write_markdown_table(f"Mappings added: {len(rows)}", header, rows)
+        self.write_markdown_table(f"Relationships added: {len(rows)}", header, rows)
 
     def handle_edge_change(self, value):
         # Create rows for the table
         rows = [
             f"| {self._format_entity_labels(change.about_edge.subject)} | \
                 {self._format_entity_labels(change.about_edge.predicate)} | \
                 {self._format_entity_labels(change.old_value)} | {self._format_entity_labels(change.new_value)} |"
             for change in value
         ]
 
         # Define the header for the table
         header = "| Subject | Predicate | Old Object | New Object |"
 
         # Write the "Edges Changed" section as a collapsible markdown table
-        self.write_markdown_table(f"Mappings changed: {len(rows)}", header, rows)
-
-    def handle_mapping_edge_deletion(self, value):
-        # Create rows for the table
-        rows = [
-            f"| {self._format_entity_labels(change.subject)} | {self._format_entity_labels(change.predicate)} |\
-                {self._format_entity_labels(change.object)} |"
-            for change in value
-        ]
-
-        # Define the header for the table
-        header = "| Subject | Predicate | Object |"
-
-        # Write the "Edges Deleted" section as a collapsible markdown table
-        self.write_markdown_table(f"Mappings removed: {len(rows)}", header, rows)
+        self.write_markdown_table(f"Relationships changed: {len(rows)}", header, rows)
 
     def handle_node_move(self, value):
         # Create rows for the table
         rows = [
             f"| {self._format_entity_labels(change.about_edge.subject)} | \
                 {self._format_entity_labels(change.about_edge.predicate)} |\
                 {self._format_entity_labels(change.about_edge.object)} |"
@@ -349,15 +335,14 @@
             "NewTextDefinition": self.handle_new_text_definition,  # ! same as NodeTextDefinition
             "RemoveTextDefinition": self.handle_remove_text_definition,
             "NodeObsoletionWithDirectReplacement": self.handle_node_obsoletion_with_direct_replacement,
             "NodeObsoletion": self.handle_node_obsoletion,
             "NodeDirectMerge": self.handle_node_direct_merge,
             "EdgeCreation": self.handle_edge_creation,
             "EdgeChange": self.handle_edge_change,
-            "MappingEdgeDeletion": self.handle_mapping_edge_deletion,
             "AddNodeToSubset": self.handle_add_node_to_subset,
             # "DatatypeOrLanguageTagChange": self.handle_datatype_or_language_tag_change,
             # "LanguageTagChange": self.handle_language_tag_change,
             # "DatatypeChange": self.handle_datatype_change,
             # "AllowsAutomaticReplacementOfEdges": self.handle_allows_automatic_replacement_of_edges,
             # "Unobsoletion": self.handle_unobsoletion,
             # "Deletion": self.handle_deletion,
```

### Comparing `oaklib-0.6.5/PKG-INFO` & `oaklib-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.6.5
+Version: 0.6.6
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -41,15 +41,15 @@
 Requires-Dist: prefixmaps (>=0.1.2)
 Requires-Dist: pronto (>=2.5.0)
 Requires-Dist: pydantic
 Requires-Dist: pysolr (>=3.9.0,<4.0.0)
 Requires-Dist: pystow (>=0.5.0)
 Requires-Dist: ratelimit (>=2.2.1)
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: semsimian (>=0.2.15) ; extra == "semsimian"
+Requires-Dist: semsimian (>=0.2.16) ; extra == "semsimian"
 Requires-Dist: semsql (>=0.3.1)
 Requires-Dist: sssom (>=0.4.4,<0.5.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: urllib3 (<2) ; extra == "gilda"
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
```

