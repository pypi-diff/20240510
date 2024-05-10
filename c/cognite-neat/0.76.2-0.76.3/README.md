# Comparing `tmp/cognite_neat-0.76.2.tar.gz` & `tmp/cognite_neat-0.76.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.76.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.76.3.tar", max compression
```

## Comparing `cognite_neat-0.76.2.tar` & `cognite_neat-0.76.3.tar`

### file list

```diff
@@ -1,277 +1,277 @@
--rw-r--r--   0        0        0    11351 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/README.md
--rw-r--r--   0        0        0       61 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4232 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     1675 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      585 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3523 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4597 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13686 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8121 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12393 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-07 12:45:19.145602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-07 12:45:19.149602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-07 12:45:19.149602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-07 12:45:19.149602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-07 12:45:19.149602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-07 12:45:19.149602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423717 2024-05-07 12:45:19.153602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
--rw-r--r--   0        0        0     2667 2024-05-07 12:45:19.153602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
--rw-r--r--   0        0        0  6282875 2024-05-07 12:45:19.177602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
--rw-r--r--   0        0        0   240334 2024-05-07 12:45:19.181602 cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     6145 2024-05-07 12:45:19.189602 cognite_neat-0.76.2/cognite/neat/config.py
--rw-r--r--   0        0        0     1300 2024-05-07 12:45:19.189602 cognite_neat-0.76.2/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-07 12:45:19.189602 cognite_neat-0.76.2/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-07 12:45:19.189602 cognite_neat-0.76.2/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-07 12:45:19.189602 cognite_neat-0.76.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14961 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-07 12:45:19.193602 cognite_neat-0.76.2/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3401 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-07 12:45:19.197602 cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14908 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23823 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2383 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2835 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40464 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22707 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12979 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3328 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14737 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-07 12:45:19.201602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36813 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5767 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7697 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0     1898 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      170 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      669 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19584 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-07 12:45:19.205602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1976 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    13529 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13034 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    20120 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3026 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4078 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    16891 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12663 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6717 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11897 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7591 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7786 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7437 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6925 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11353 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4275 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6438 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    19178 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     5748 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3385 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0    12288 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13936 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      782 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0    10876 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0    11030 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/_rdfpath.py
--rw-r--r--   0        0        0      305 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/_types/__init__.py
--rw-r--r--   0        0        0      929 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/_types/_base.py
--rw-r--r--   0        0        0     3197 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/_types/_field.py
--rw-r--r--   0        0        0     6078 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0      491 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/__init__.py
--rw-r--r--   0        0        0     5706 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_converter.py
--rw-r--r--   0        0        0    18908 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_exporter.py
--rw-r--r--   0        0        0    15599 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_rules.py
--rw-r--r--   0        0        0    13147 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_rules_input.py
--rw-r--r--   0        0        0    36236 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_schema.py
--rw-r--r--   0        0        0     6619 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_serializer.py
--rw-r--r--   0        0        0    12960 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/dms/_validation.py
--rw-r--r--   0        0        0     2934 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/domain.py
--rw-r--r--   0        0        0    16395 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0      195 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/information/__init__.py
--rw-r--r--   0        0        0     7833 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/information/_converter.py
--rw-r--r--   0        0        0    15546 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/information/_rules.py
--rw-r--r--   0        0        0     6154 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/rules/models/wrapped_entities.py
--rw-r--r--   0        0        0       68 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11336 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6303 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2714 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12818 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-07 12:45:19.209602 cognite_neat-0.76.2/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26800 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    14102 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6570 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0        0 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0      225 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/graph_store.py
--rw-r--r--   0        0        0    22824 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/rules_exporter.py
--rw-r--r--   0        0        0    10338 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/rules_importer.py
--rw-r--r--   0        0        0     4729 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/rules_validator.py
--rw-r--r--   0        0        0       32 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/io/__init__.py
--rw-r--r--   0        0        0    16874 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/io/io_steps.py
--rw-r--r--   0        0        0      274 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/__init__.py
--rw-r--r--   0        0        0     3919 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
--rw-r--r--   0        0        0    29357 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
--rw-r--r--   0        0        0    27265 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
--rw-r--r--   0        0        0    12704 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_store.py
--rw-r--r--   0        0        0     2351 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
--rw-r--r--   0        0        0    20462 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
--rw-r--r--   0        0        0    28065 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
--rw-r--r--   0        0        0     2943 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    11007 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-07 12:45:19.213602 cognite_neat-0.76.2/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4591 2024-05-07 12:45:19.597603 cognite_neat-0.76.2/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.76.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/README.md
+-rw-r--r--   0        0        0       61 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4232 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     1675 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      585 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3523 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4597 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13686 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8121 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12393 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-10 13:52:00.036956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-10 13:52:00.040956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423717 2024-05-10 13:52:00.044956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js
+-rw-r--r--   0        0        0     2667 2024-05-10 13:52:00.044956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282875 2024-05-10 13:52:00.072956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map
+-rw-r--r--   0        0        0   240334 2024-05-10 13:52:00.072956 cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     6145 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/config.py
+-rw-r--r--   0        0        0     1300 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-10 13:52:00.080956 cognite_neat-0.76.3/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-10 13:52:00.084956 cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-10 13:52:00.084956 cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-10 13:52:00.084956 cognite_neat-0.76.3/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14961 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-10 13:52:00.088956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3401 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14908 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23823 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2383 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2835 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40464 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22707 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12979 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3328 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14737 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-10 13:52:00.092956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36813 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5767 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7697 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0     1898 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-10 13:52:00.096956 cognite_neat-0.76.3/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19584 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1976 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    13529 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    14934 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20120 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3026 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4078 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    16891 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12663 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6717 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11897 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7591 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7786 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7437 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6925 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11882 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4275 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6438 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    22035 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     5748 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3385 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0    12288 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13936 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      782 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0    10876 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0    11030 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_rdfpath.py
+-rw-r--r--   0        0        0      305 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/_types/_field.py
+-rw-r--r--   0        0        0     6078 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0      491 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/__init__.py
+-rw-r--r--   0        0        0     5706 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_converter.py
+-rw-r--r--   0        0        0    18908 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_exporter.py
+-rw-r--r--   0        0        0    15599 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules.py
+-rw-r--r--   0        0        0    13620 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules_input.py
+-rw-r--r--   0        0        0    37463 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_schema.py
+-rw-r--r--   0        0        0     6668 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_serializer.py
+-rw-r--r--   0        0        0    14290 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/dms/_validation.py
+-rw-r--r--   0        0        0     2993 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/domain.py
+-rw-r--r--   0        0        0    16395 2024-05-10 13:52:00.100956 cognite_neat-0.76.3/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0      195 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/information/__init__.py
+-rw-r--r--   0        0        0     7964 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/information/_converter.py
+-rw-r--r--   0        0        0    15546 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/information/_rules.py
+-rw-r--r--   0        0        0     6154 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/rules/models/wrapped_entities.py
+-rw-r--r--   0        0        0       68 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11336 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6303 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2714 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12818 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26800 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    14102 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6570 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_store.py
+-rw-r--r--   0        0        0    22898 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py
+-rw-r--r--   0        0        0    10338 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_importer.py
+-rw-r--r--   0        0        0     4729 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_validator.py
+-rw-r--r--   0        0        0       32 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/io/__init__.py
+-rw-r--r--   0        0        0    16874 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/io/io_steps.py
+-rw-r--r--   0        0        0      274 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/__init__.py
+-rw-r--r--   0        0        0     3919 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py
+-rw-r--r--   0        0        0    29357 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py
+-rw-r--r--   0        0        0    27265 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py
+-rw-r--r--   0        0        0    12704 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py
+-rw-r--r--   0        0        0     2351 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py
+-rw-r--r--   0        0        0    20462 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py
+-rw-r--r--   0        0        0    28065 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py
+-rw-r--r--   0        0        0     2943 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    11007 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-10 13:52:00.104956 cognite_neat-0.76.3/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4591 2024-05-10 13:52:00.492955 cognite_neat-0.76.3/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.76.3/PKG-INFO
```

### Comparing `cognite_neat-0.76.2/LICENSE` & `cognite_neat-0.76.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/README.md` & `cognite_neat-0.76.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/configuration.py` & `cognite_neat-0.76.3/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.76.3/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/explorer.py` & `cognite_neat-0.76.3/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.76.3/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.76.3/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.76.3/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.76.3/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.76.3/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.76.3/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.76.3/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.76.3/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.76.3/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.76.3/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/js/main.ec7f72e2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.76.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/config.py` & `cognite_neat-0.76.3/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/constants.py` & `cognite_neat-0.76.3/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/exceptions.py` & `cognite_neat-0.76.3/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.76.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.76.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/exceptions.py` & `cognite_neat-0.76.3/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.76.3/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.76.3/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.76.3/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.76.3/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/legacy/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.76.3/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.76.3/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exceptions.py` & `cognite_neat-0.76.3/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from openpyxl import Workbook
 from openpyxl.cell import MergedCell
 from openpyxl.styles import Alignment, Border, Font, PatternFill, Side
 from openpyxl.worksheet.worksheet import Worksheet
 
 from cognite.neat.rules._shared import Rules
 from cognite.neat.rules.models import (
+    DataModelType,
     DMSRules,
     DomainRules,
+    ExtensionCategory,
     InformationRules,
     RoleTypes,
     SchemaCompleteness,
     SheetEntity,
 )
 
 from ._base import BaseExporter
@@ -31,53 +33,63 @@
         styling: The styling to use for the Excel file. Defaults to "default". See below for details
             on the different styles.
         output_role: The role to use for the exported spreadsheet. If provided, the rules will be converted to
             this role formate before being written to excel. If not provided, the role from the rules will be used.
         new_model_id: The new model ID to use for the exported spreadsheet. This is only applicable if the input
             rules have 'is_reference' set. If provided, the model ID will be used to automatically create the
             new metadata sheet in the Excel file.
-        is_reference: If True, the rules are considered to be a reference model. The exported Excel file will
-            then contain empty sheets for the main rules and this data model will be dumped to the reference sheets.
-            This is useful when you are building a solution model based on an Enterprise model, then the
-            Enterprise model will serve as the reference model. It is also useful when you are extending an existing
-            model, then the existing model will serve as the reference model. Defaults to False.
+        dump_as: This determines how the rules are written to the Excel file. An Excel file has up to three sets of
+           sheets: user, last, and reference. The user sheets are used for inputting rules from a user. The last sheets
+           are used for the last version of the same model as the user, while the reference sheets are used for
+           the model the user is building on. The options are:
+             * "user": The rules are written to the user sheets. This is used when you want to modify the rules
+                directly and potentially change the model. This is useful when you have imported the data model
+                from outside CDF and you want to modify it before you write it to CDF.
+             * "last": The rules are written to the last sheets. This is used when you want to extend the rules,
+               but have validation that you are not breaking the existing model. This is used when you want to
+               change a model that has already been published to CDF and that model is in production.
+             * "reference": The rules are written to the reference sheets. This is typically used when you want to build
+               a new solution on top of an enterprise model.
 
     The following styles are available:
 
     - "none":    No styling is applied.
     - "minimal": Column widths are adjusted to fit the content, and the header row(s) is frozen.
     - "default": Minimal + headers are bold, increased size, and colored.
     - "maximal": Default + alternating row colors in the properties sheet for each class in addition to extra
                  blank rows between classes and borders
     """
 
     Style = Literal["none", "minimal", "default", "maximal"]
-
+    DumpOptions = Literal["user", "last", "reference"]
     _main_header_by_sheet_name: ClassVar[dict[str, str]] = {
         "Properties": "Definition of Properties per Class",
         "Classes": "Definition of Classes",
         "Views": "Definition of Views",
         "Containers": "Definition of Containers",
     }
     style_options = get_args(Style)
+    dump_options = get_args(DumpOptions)
 
     def __init__(
         self,
         styling: Style = "default",
         output_role: RoleTypes | None = None,
         new_model_id: tuple[str, str, str] | None = None,
-        is_reference: bool = False,
+        dump_as: DumpOptions = "user",
     ):
         if styling not in self.style_options:
             raise ValueError(f"Invalid styling: {styling}. Valid options are {self.style_options}")
+        if dump_as not in self.dump_options:
+            raise ValueError(f"Invalid dump_as: {dump_as}. Valid options are {self.dump_options}")
         self.styling = styling
         self._styling_level = self.style_options.index(styling)
         self.output_role = output_role
         self.new_model_id = new_model_id
-        self.is_reference = is_reference
+        self.dump_as = dump_as
 
     def export_to_file(self, rules: Rules, filepath: Path) -> None:
         """Exports transformation rules to excel file."""
         data = self.export(rules)
         try:
             data.save(filepath)
         finally:
@@ -86,49 +98,56 @@
 
     def export(self, rules: Rules) -> Workbook:
         rules = self._convert_to_output_role(rules, self.output_role)
         workbook = Workbook()
         # Remove default sheet named "Sheet"
         workbook.remove(workbook["Sheet"])
 
-        dumped_rules: dict[str, Any]
+        dumped_user_rules: dict[str, Any]
+        dumped_last_rules: dict[str, Any] | None = None
         dumped_reference_rules: dict[str, Any] | None = None
-        if self.is_reference:
+        if self.dump_as != "user":
             # Writes empty reference sheets
-            dumped_rules = {
+            dumped_user_rules = {
                 "Metadata": self._create_metadata_sheet_user_rules(rules),
             }
-            dumped_rules["Metadata"]["role"] = (
-                self.output_role and self.output_role.value
-            ) or rules.metadata.role.value
-            dumped_reference_rules = rules.reference_self().model_dump(by_alias=True)
+
+            if self.dump_as == "last":
+                dumped_last_rules = rules.model_dump(by_alias=True)
+                if rules.reference:
+                    dumped_reference_rules = rules.reference.model_dump(by_alias=True)
+            elif self.dump_as == "reference":
+                dumped_reference_rules = rules.reference_self().model_dump(by_alias=True)
         else:
-            dumped_rules = rules.model_dump(by_alias=True)
+            dumped_user_rules = rules.model_dump(by_alias=True)
+            if rules.last:
+                dumped_last_rules = rules.last.model_dump(by_alias=True)
             if rules.reference:
                 dumped_reference_rules = rules.reference.model_dump(by_alias=True)
 
-        self._write_metadata_sheet(workbook, dumped_rules["Metadata"])
-        self._write_sheets(workbook, dumped_rules, rules)
+        self._write_metadata_sheet(workbook, dumped_user_rules["Metadata"])
+        self._write_sheets(workbook, dumped_user_rules, rules)
+        if dumped_last_rules:
+            self._write_sheets(workbook, dumped_last_rules, rules, sheet_prefix="Last")
+
         if dumped_reference_rules:
-            self._write_sheets(workbook, dumped_reference_rules, rules, is_reference=True)
-            self._write_metadata_sheet(workbook, dumped_reference_rules["Metadata"], is_reference=True)
+            prefix = "Ref"
+            self._write_sheets(workbook, dumped_reference_rules, rules, sheet_prefix=prefix)
+            self._write_metadata_sheet(workbook, dumped_reference_rules["Metadata"], sheet_prefix=prefix)
 
         if self._styling_level > 0:
             self._adjust_column_widths(workbook)
 
         return workbook
 
-    def _write_sheets(self, workbook: Workbook, dumped_rules: dict[str, Any], rules: Rules, is_reference: bool = False):
+    def _write_sheets(self, workbook: Workbook, dumped_rules: dict[str, Any], rules: Rules, sheet_prefix: str = ""):
         for sheet_name, headers in rules.headers_by_sheet(by_alias=True).items():
             if sheet_name in ("Metadata", "prefixes", "Reference", "Last"):
                 continue
-            if is_reference:
-                sheet = workbook.create_sheet(f"Ref{sheet_name}")
-            else:
-                sheet = workbook.create_sheet(sheet_name)
+            sheet = workbook.create_sheet(f"{sheet_prefix}{sheet_name}")
 
             main_header = self._main_header_by_sheet_name[sheet_name]
             sheet.append([main_header] + [""] * (len(headers) - 1))
             sheet.merge_cells(start_row=1, start_column=1, end_row=1, end_column=len(headers))
             sheet.append(headers)
 
             fill_colors = itertools.cycle(["CADCFC", "FFFFFF"])
@@ -166,25 +185,22 @@
             if self._styling_level > 1:
                 # Make the header row bold, larger, and colored
                 sheet["A1"].font = Font(bold=True, size=20)
                 sheet["A1"].fill = PatternFill(fgColor="FFC000", patternType="solid")
                 for cell in sheet["2"]:
                     cell.font = Font(bold=True, size=14)
 
-    def _write_metadata_sheet(self, workbook: Workbook, metadata: dict[str, Any], is_reference: bool = False) -> None:
+    def _write_metadata_sheet(self, workbook: Workbook, metadata: dict[str, Any], sheet_prefix: str = "") -> None:
         # Excel does not support timezone in datetime strings
         if isinstance(metadata.get("created"), datetime):
             metadata["created"] = metadata["created"].replace(tzinfo=None)
         if isinstance(metadata.get("updated"), datetime):
             metadata["updated"] = metadata["updated"].replace(tzinfo=None)
 
-        if is_reference:
-            metadata_sheet = workbook.create_sheet("RefMetadata")
-        else:
-            metadata_sheet = workbook.create_sheet("Metadata")
+        metadata_sheet = workbook.create_sheet(f"{sheet_prefix}Metadata")
         for key, value in metadata.items():
             metadata_sheet.append([key, value])
 
         if self._styling_level > 1:
             for cell in metadata_sheet["A"]:
                 cell.font = Font(bold=True, size=12)
 
@@ -237,33 +253,37 @@
         if isinstance(existing_metadata["created"], datetime):
             metadata["created"] = existing_metadata["created"].replace(tzinfo=None)
         if isinstance(existing_metadata["updated"], datetime):
             metadata["updated"] = existing_metadata["updated"].replace(tzinfo=None)
         # Excel does not support timezone in datetime strings
         now_iso = datetime.now().replace(tzinfo=None).isoformat()
         is_info = isinstance(rules, InformationRules)
-        is_dms = not is_info
-        is_extension = self.new_model_id is not None
-        is_solution = is_extension and self.new_model_id != existing_model_id
+        is_dms = isinstance(rules, DMSRules)
+        is_extension = self.new_model_id is not None or rules.reference is not None
+        is_solution = rules.metadata.data_model_type == DataModelType.solution
 
-        if is_solution:
+        if is_solution and self.new_model_id:
             metadata["prefix" if is_info else "space"] = self.new_model_id[0]  # type: ignore[index]
             metadata["title" if is_info else "externalId"] = self.new_model_id[1]  # type: ignore[index]
             metadata["version"] = self.new_model_id[2]  # type: ignore[index]
+        elif is_solution and self.dump_as == "reference" and rules.reference:
+            metadata["prefix" if is_info else "space"] = "YOUR_PREFIX"
+            metadata["title" if is_info else "externalId"] = "YOUR_TITLE"
+            metadata["version"] = "1"
         else:
             metadata["prefix" if is_info else "space"] = existing_model_id[0]
             metadata["title" if is_info else "externalId"] = existing_model_id[1]
             metadata["version"] = existing_model_id[2]
 
-        if is_solution and is_info:
+        if is_solution and is_info and self.new_model_id:
             metadata["namespace"] = f"http://purl.org/{self.new_model_id[0]}/"  # type: ignore[index]
         elif is_info:
             metadata["namespace"] = existing_metadata["namespace"]
 
-        if is_solution and is_dms:
+        if is_solution and is_dms and self.new_model_id:
             metadata["name"] = self.new_model_id[1]  # type: ignore[index]
 
         if is_solution:
             metadata["created"] = now_iso
         else:
             metadata["created"] = existing_metadata["created"]
 
@@ -281,10 +301,15 @@
             metadata["description"] = existing_metadata["description"]
 
         if is_extension:
             metadata["schema"] = SchemaCompleteness.extended.value
         else:
             metadata["schema"] = SchemaCompleteness.complete.value
 
-        metadata["extension"] = "addition"
+        if is_solution:
+            metadata["dataModelType"] = DataModelType.solution.value
+        else:
+            metadata["dataModelType"] = DataModelType.enterprise.value
 
+        metadata["extension"] = ExtensionCategory.addition.value
+        metadata["role"] = (self.output_role and self.output_role.value) or rules.metadata.role.value
         return metadata
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.76.3/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,79 +83,103 @@
         return True
 
 
 @dataclass
 class ReadResult:
     sheets: dict[str, dict | list]
     read_info_by_sheet: dict[str, SpreadsheetRead]
-    role: RoleTypes
-    schema: SchemaCompleteness | None
+    metadata: MetadataRaw
+
+    @property
+    def role(self) -> RoleTypes:
+        return self.metadata.role
+
+    @property
+    def schema(self) -> SchemaCompleteness | None:
+        return self.metadata.schema
 
 
 class SpreadsheetReader:
-    def __init__(self, issue_list: IssueList, is_reference: bool = False):
+    def __init__(
+        self,
+        issue_list: IssueList,
+        required: bool = True,
+        metadata: MetadataRaw | None = None,
+        sheet_prefix: Literal["", "Last", "Ref"] = "",
+    ):
         self.issue_list = issue_list
-        self._is_reference = is_reference
+        self.required = required
+        self.metadata = metadata
+        self._sheet_prefix = sheet_prefix
 
     @property
     def metadata_sheet_name(self) -> str:
-        metadata_name = "Metadata"
-        return self.to_reference_sheet(metadata_name) if self._is_reference else metadata_name
+        return f"{self._sheet_prefix}Metadata"
 
     def sheet_names(self, role: RoleTypes) -> set[str]:
         names = MANDATORY_SHEETS_BY_ROLE[role]
-        return {self.to_reference_sheet(sheet_name) for sheet_name in names} if self._is_reference else names
-
-    @classmethod
-    def to_reference_sheet(cls, sheet_name: str) -> str:
-        return f"Ref{sheet_name}"
+        return {f"{self._sheet_prefix}{sheet_name}" for sheet_name in names if sheet_name != "Metadata"}
 
     def read(self, filepath: Path) -> None | ReadResult:
         with pd.ExcelFile(filepath) as excel_file:
-            if self.metadata_sheet_name not in excel_file.sheet_names:
+            metadata: MetadataRaw | None
+            if self.metadata is not None:
+                metadata = self.metadata
+            else:
+                metadata = self._read_metadata(excel_file, filepath)
+                if metadata is None:
+                    # The reading of metadata failed, so we can't continue
+                    return None
+
+            sheets, read_info_by_sheet = self._read_sheets(excel_file, metadata.role)
+            if sheets is None or self.issue_list.has_errors:
+                return None
+            sheets["Metadata"] = dict(metadata)
+
+            return ReadResult(sheets, read_info_by_sheet, metadata)
+
+    def _read_metadata(self, excel_file: ExcelFile, filepath: Path) -> MetadataRaw | None:
+        if self.metadata_sheet_name not in excel_file.sheet_names:
+            if self.required:
                 self.issue_list.append(
                     issues.spreadsheet_file.MetadataSheetMissingOrFailedError(
                         filepath, sheet_name=self.metadata_sheet_name
                     )
                 )
-                return None
-
-            metadata = MetadataRaw.from_excel(excel_file, self.metadata_sheet_name)
-
-            if not metadata.is_valid(self.issue_list, filepath):
-                return None
+            return None
 
-            sheets, read_info_by_sheet = self._read_sheets(metadata, excel_file)
-            if sheets is None or self.issue_list.has_errors:
-                return None
+        metadata = MetadataRaw.from_excel(excel_file, self.metadata_sheet_name)
 
-            return ReadResult(sheets, read_info_by_sheet, metadata.role, metadata.schema)
+        if not metadata.is_valid(self.issue_list, filepath):
+            return None
+        return metadata
 
     def _read_sheets(
-        self, metadata: MetadataRaw, excel_file: ExcelFile
+        self, excel_file: ExcelFile, read_role: RoleTypes
     ) -> tuple[dict[str, dict | list] | None, dict[str, SpreadsheetRead]]:
         read_info_by_sheet: dict[str, SpreadsheetRead] = defaultdict(SpreadsheetRead)
 
-        sheets: dict[str, dict | list] = {"Metadata": dict(metadata)}
+        sheets: dict[str, dict | list] = {}
 
-        expected_sheet_names = self.sheet_names(metadata.role)
+        expected_sheet_names = self.sheet_names(read_role)
 
         if missing_sheets := expected_sheet_names.difference(set(excel_file.sheet_names)):
-            self.issue_list.append(
-                issues.spreadsheet_file.SheetMissingError(cast(Path, excel_file.io), list(missing_sheets))
-            )
+            if self.required:
+                self.issue_list.append(
+                    issues.spreadsheet_file.SheetMissingError(cast(Path, excel_file.io), list(missing_sheets))
+                )
             return None, read_info_by_sheet
 
         for source_sheet_name, target_sheet_name, headers_input in SOURCE_SHEET__TARGET_FIELD__HEADERS:
-            source_sheet_name = self.to_reference_sheet(source_sheet_name) if self._is_reference else source_sheet_name
+            source_sheet_name = f"{self._sheet_prefix}{source_sheet_name}"
 
             if source_sheet_name not in excel_file.sheet_names:
                 continue
             if isinstance(headers_input, dict):
-                headers = headers_input[metadata.role]
+                headers = headers_input[read_role]
             else:
                 headers = headers_input
 
             try:
                 sheets[target_sheet_name], read_info_by_sheet[source_sheet_name] = read_individual_sheet(
                     excel_file, source_sheet_name, return_read_info=True, expected_headers=[headers]
                 )
@@ -184,50 +208,45 @@
         self, errors: Literal["raise", "continue"] = "continue", role: RoleTypes | None = None
     ) -> tuple[Rules | None, IssueList] | Rules:
         issue_list = IssueList(title=f"'{self.filepath.name}'")
         if not self.filepath.exists():
             issue_list.append(issues.spreadsheet_file.SpreadsheetNotFoundError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
-        user_result = SpreadsheetReader(issue_list, is_reference=False).read(self.filepath)
-        if user_result is None or issue_list.has_errors:
+        user_read = SpreadsheetReader(issue_list).read(self.filepath)
+        if user_read is None or issue_list.has_errors:
             return self._return_or_raise(issue_list, errors)
 
-        reference_result: ReadResult | None = None
-        if (
-            user_result
-            and user_result.role != RoleTypes.domain_expert
-            and user_result.schema == SchemaCompleteness.extended
-        ):
-            reference_result = SpreadsheetReader(issue_list, is_reference=True).read(self.filepath)
+        last_read: ReadResult | None = None
+        reference_read: ReadResult | None = None
+        if user_read.schema == SchemaCompleteness.extended:
+            # Last does not have its own metadata sheet. It is the same as the user's metadata sheet.
+            last_read = SpreadsheetReader(
+                issue_list, required=False, metadata=user_read.metadata, sheet_prefix="Last"
+            ).read(self.filepath)
+            reference_read = SpreadsheetReader(issue_list, sheet_prefix="Ref").read(self.filepath)
             if issue_list.has_errors:
                 return self._return_or_raise(issue_list, errors)
 
-        if user_result and reference_result and user_result.role != reference_result.role:
+        if reference_read and user_read.role != reference_read.role:
             issue_list.append(issues.spreadsheet_file.RoleMismatchError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
-        if user_result and reference_result:
-            user_result.sheets["reference"] = reference_result.sheets
-            sheets = user_result.sheets
-            original_role = user_result.role
-            read_info_by_sheet = user_result.read_info_by_sheet
-            read_info_by_sheet.update(reference_result.read_info_by_sheet)
-        elif user_result:
-            sheets = user_result.sheets
-            original_role = user_result.role
-            read_info_by_sheet = user_result.read_info_by_sheet
-        elif reference_result:
-            sheets = reference_result.sheets
-            original_role = reference_result.role
-            read_info_by_sheet = reference_result.read_info_by_sheet
-        else:
-            raise ValueError(
-                "No rules were generated. This should have been caught earlier. " f"Bug in {type(self).__name__}."
-            )
+        sheets = user_read.sheets
+        original_role = user_read.role
+        read_info_by_sheet = user_read.read_info_by_sheet
+        if last_read:
+            sheets["last"] = last_read.sheets
+            read_info_by_sheet.update(last_read.read_info_by_sheet)
+            if reference_read:
+                # The last rules will also be validated against the reference rules
+                sheets["last"]["reference"] = reference_read.sheets  # type: ignore[call-overload]
+        if reference_read:
+            sheets["reference"] = reference_read.sheets
+            read_info_by_sheet.update(reference_read.read_info_by_sheet)
 
         rules_cls = RULES_PER_ROLE[original_role]
         with _handle_issues(
             issue_list,
             error_cls=issues.spreadsheet.InvalidSheetError,
             error_args={"read_info_by_sheet": read_info_by_sheet},
         ) as future:
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/base.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/dms.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 from cognite.client.data_classes import data_modeling as dm
 
 from .base import NeatValidationError, ValidationWarning
 
 __all__ = [
     "DMSSchemaError",
     "DMSSchemaWarning",
+    "IncompleteSchemaError",
     "MissingSpaceError",
     "MissingContainerError",
     "MissingContainerPropertyError",
     "MissingViewError",
     "MissingParentViewError",
     "MissingSourceViewError",
     "MissingEdgeViewError",
     "DirectRelationMissingSourceWarning",
     "ViewModelVersionNotMatchingWarning",
     "ViewModelSpaceNotMatchingWarning",
+    "ViewMapsToTooManyContainersWarning",
     "DuplicatedViewInDataModelError",
     "ContainerPropertyUsedMultipleTimesError",
     "EmptyContainerWarning",
     "UnsupportedConnectionWarning",
     "MultipleReferenceWarning",
     "HasDataFilterOnNoPropertiesViewWarning",
+    "HasDataFilterAppliedToTooManyContainersWarning",
     "ReverseRelationMissingOtherSideWarning",
     "NodeTypeFilterOnParentViewWarning",
     "ChangingContainerError",
     "ChangingViewError",
 ]
 
 
@@ -37,14 +40,32 @@
 
 
 @dataclass(frozen=True)
 class DMSSchemaWarning(ValidationWarning, ABC): ...
 
 
 @dataclass(frozen=True)
+class IncompleteSchemaError(DMSSchemaError):
+    description = "This error is raised when the schema is claimed to be complete but missing some components"
+    fix = "Either provide the missing components or change the schema to partial"
+    missing_component: dm.ContainerId | dm.ViewId
+
+    def message(self) -> str:
+        return (
+            "The data model schema is set to be complete, however, "
+            f"the referred component {self.missing_component} is not preset."
+        )
+
+    def dump(self) -> dict[str, Any]:
+        output = super().dump()
+        output["missing_component"] = self.missing_component
+        return output
+
+
+@dataclass(frozen=True)
 class MissingSpaceError(DMSSchemaError):
     description = "The spaced referred to by the Container/View/Node/Edge/DataModel does not exist"
     fix = "Create the space"
     space: str
     referred_by: dm.ContainerId | dm.ViewId | dm.NodeId | dm.EdgeId | dm.DataModelId
 
     def message(self) -> str:
@@ -247,14 +268,36 @@
         output = super().dump()
         output["view_id"] = [view_id.dump() for view_id in self.view_ids]
         output["data_model_space"] = self.data_model_space
         return output
 
 
 @dataclass(frozen=True)
+class ViewMapsToTooManyContainersWarning(DMSSchemaWarning):
+    description = "The view maps to more than 10 containers which impacts read/write performance of data model"
+    fix = "Try to have as few containers as possible to which the view maps to"
+    error_name: ClassVar[str] = "ViewMapsToTooManyContainers"
+    view_id: dm.ViewId
+    container_ids: set[dm.ContainerId]
+
+    def message(self) -> str:
+        return (
+            f"The view {self.view_id} maps to total of {len(self.container_ids)},."
+            "Mapping to more than 10 containers is not recommended and can lead to poor performances."
+            "Re-iterate the data model design to reduce the number of containers to which the view maps to."
+        )
+
+    def dump(self) -> dict[str, Any]:
+        output = super().dump()
+        output["view_id"] = self.view_id.dump()
+        output["container_ids"] = [container_id.dump() for container_id in self.container_ids]
+        return output
+
+
+@dataclass(frozen=True)
 class ContainerPropertyUsedMultipleTimesError(DMSSchemaError):
     description = "The container property is used multiple times by the same view property"
     fix = "Use unique container properties for when mapping to the same container"
     error_name: ClassVar[str] = "ContainerPropertyUsedMultipleTimes"
     container: dm.ContainerId
     property: str
     referred_by: frozenset[tuple[dm.ViewId, str]]
@@ -439,14 +482,36 @@
     def dump(self) -> dict[str, Any]:
         output = super().dump()
         output["view_id"] = self.view_id.dump()
         return output
 
 
 @dataclass(frozen=True)
+class HasDataFilterAppliedToTooManyContainersWarning(DMSSchemaWarning):
+    description = "The view filter hasData applied to more than 10 containers this will cause DMS API Error"
+    fix = "Do not map to more than 10 containers, alternatively override the filter by using rawFilter"
+    error_name: ClassVar[str] = "HasDataFilterAppliedToTooManyContainers"
+    view_id: dm.ViewId
+    container_ids: set[dm.ContainerId]
+
+    def message(self) -> str:
+        return (
+            f"The view {self.view_id} HasData filter applied to total of {len(self.container_ids)},."
+            "Applying HasData filter to more than 10 containers is not recommended and can lead to DMS API error."
+            "Re-iterate the data model design to reduce the number of containers to which the view maps to."
+        )
+
+    def dump(self) -> dict[str, Any]:
+        output = super().dump()
+        output["view_id"] = self.view_id.dump()
+        output["container_ids"] = [container_id.dump() for container_id in self.container_ids]
+        return output
+
+
+@dataclass(frozen=True)
 class NodeTypeFilterOnParentViewWarning(DMSSchemaWarning):
     description = (
         "Setting a node type filter on a parent view. This is not "
         "recommended as parent views are typically used for multiple type of nodes."
     )
     fix = "Use a HasData filter instead"
     error_name: ClassVar[str] = "NodeTypeFilterOnParentViewWarning"
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.76.3/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/__init__.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/_base.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/_rdfpath.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/_rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/_types/_base.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/_types/_field.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_converter.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_exporter.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_rules_input.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_rules_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
 
 @dataclass
 class DMSRulesInput:
     metadata: DMSMetadataInput
     properties: Sequence[DMSPropertyInput]
     views: Sequence[DMSViewInput]
     containers: Sequence[DMSContainerInput] | None = None
+    last: "DMSRulesInput | DMSRules | None" = None
     reference: "DMSRulesInput | DMSRules | None" = None
 
     @classmethod
     @overload
     def load(cls, data: dict[str, Any]) -> "DMSRulesInput": ...
 
     @classmethod
@@ -319,14 +320,15 @@
             return None
         _add_alias(data, DMSRules)
         return cls(
             metadata=DMSMetadataInput.load(data.get("metadata")),  # type: ignore[arg-type]
             properties=DMSPropertyInput.load(data.get("properties")),  # type: ignore[arg-type]
             views=DMSViewInput.load(data.get("views")),  # type: ignore[arg-type]
             containers=DMSContainerInput.load(data.get("containers")) or [],
+            last=DMSRulesInput.load(data.get("last")),
             reference=DMSRulesInput.load(data.get("reference")),
         )
 
     def as_rules(self) -> DMSRules:
         return DMSRules.model_validate(self.dump())
 
     def dump(self) -> dict[str, Any]:
@@ -334,20 +336,27 @@
         default_version = self.metadata.version
         reference: dict[str, Any] | None = None
         if isinstance(self.reference, DMSRulesInput):
             reference = self.reference.dump()
         elif isinstance(self.reference, DMSRules):
             # We need to load through the DMSRulesInput to set the correct default space and version
             reference = DMSRulesInput.load(self.reference.model_dump()).dump()
+        last: dict[str, Any] | None = None
+        if isinstance(self.last, DMSRulesInput):
+            last = self.last.dump()
+        elif isinstance(self.last, DMSRules):
+            # We need to load through the DMSRulesInput to set the correct default space and version
+            last = DMSRulesInput.load(self.last.model_dump()).dump()
 
         return dict(
             Metadata=self.metadata.dump(),
             Properties=[prop.dump(default_space, default_version) for prop in self.properties],
             Views=[view.dump(default_space, default_version) for view in self.views],
             Containers=[container.dump(default_space) for container in self.containers or []] or None,
+            Last=last,
             Reference=reference,
         )
 
 
 def _add_alias(data: dict[str, Any], base_model: type[BaseModel]) -> None:
     for field_name, field_ in base_model.model_fields.items():
         if field_name not in data and field_.alias in data:
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_schema.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues.dms import (
     ContainerPropertyUsedMultipleTimesError,
     DirectRelationMissingSourceWarning,
     DMSSchemaError,
     DuplicatedViewInDataModelError,
+    IncompleteSchemaError,
     MissingContainerError,
     MissingContainerPropertyError,
     MissingEdgeViewError,
     MissingParentViewError,
     MissingSourceViewError,
     MissingSpaceError,
     MissingViewError,
 )
 from cognite.neat.rules.models.data_types import _DATA_TYPE_BY_DMS_TYPE
 from cognite.neat.utils.cdf_loaders import ViewLoader
 from cognite.neat.utils.cdf_loaders.data_classes import RawTableWrite, RawTableWriteList
 from cognite.neat.utils.text import to_camel
+from cognite.neat.utils.utils import get_inheritance_path
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
@@ -56,14 +58,38 @@
         "container": "containers",
         "view": "views",
         "datamodel": "data_models",
         "space": "spaces",
         "node": "node_types",
     }
 
+    def _get_mapped_container_from_view(self, view_id: dm.ViewId) -> set[dm.ContainerId]:
+        # index all views, including ones from reference
+        indexed_views = {
+            **{view.as_id(): view for view in self.views},
+            **({view.as_id(): view for view in self.reference.views} if self.reference else {}),
+        }
+
+        if view_id not in indexed_views:
+            raise ValueError(f"View {view_id} not found")
+
+        indexed_implemented_views = {id_: view.implements for id_, view in indexed_views.items()}
+        view_inheritance = get_inheritance_path(view_id, indexed_implemented_views)
+
+        directly_referenced_containers = indexed_views[view_id].referenced_containers()
+        inherited_referenced_containers = set()
+
+        for view_id in view_inheritance:
+            if implemented_view := indexed_views.get(view_id):
+                inherited_referenced_containers |= implemented_view.referenced_containers()
+            else:
+                raise IncompleteSchemaError(missing_component=view_id).as_exception()
+
+        return directly_referenced_containers | inherited_referenced_containers
+
     @classmethod
     def from_model_id(cls, client: CogniteClient, data_model_id: dm.DataModelIdentifier) -> "DMSSchema":
         data_models = client.data_modeling.data_models.retrieve(data_model_id, inline_views=True)
         if len(data_models) == 0:
             raise ValueError(f"Data model {data_model_id} not found")
         data_model = data_models.latest_version()
         return cls.from_data_model(client, data_model)
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_serializer.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,18 @@
 
     def clean(self, dumped: dict[str, Any]) -> dict[str, Any]:
         # Sorting to get a deterministic order
         dumped[self.prop_name] = sorted(
             dumped[self.prop_name]["data"], key=lambda p: (p[self.prop_view], p[self.prop_view_property])
         )
         dumped[self.view_name] = sorted(dumped[self.view_name]["data"], key=lambda v: v[self.view_view])
-        if self.container_name in dumped:
-            dumped[self.container_name] = sorted(
-                dumped[self.container_name]["data"], key=lambda c: c[self.container_container]
-            )
+        if container_data := dumped.get(self.container_name):
+            dumped[self.container_name] = sorted(container_data["data"], key=lambda c: c[self.container_container])
+        else:
+            dumped.pop(self.container_name, None)
 
         for prop in dumped[self.prop_name]:
             for field_name in self.properties_fields:
                 if value := prop.get(field_name):
                     prop[field_name] = value.removeprefix(self.default_space).removesuffix(self.default_version_wrapped)
             # Value type can have a property as well
             prop[self.prop_value_type] = prop[self.prop_value_type].replace(self.default_version, "")
@@ -101,15 +101,15 @@
                     parent.strip().removeprefix(self.default_space).removesuffix(self.default_version_wrapped)
                     for parent in value.split(",")
                 )
             if self.exclude_views:
                 for field in self.exclude_views:
                     view.pop(field, None)
 
-        for container in dumped[self.container_name]:
+        for container in dumped.get(self.container_name, []):
             for field_name in self.containers_fields:
                 if value := container.get(field_name):
                     container[field_name] = value.removeprefix(self.default_space)
 
             if value := container.get(self.container_constraint):
                 container[self.container_constraint] = ",".join(
                     constraint.strip().removeprefix(self.default_space) for constraint in value.split(",")
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/dms/_validation.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/dms/_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from collections import defaultdict
 from typing import Any
 
+from cognite.client import data_modeling as dm
+
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models._base import ExtensionCategory, SchemaCompleteness
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.entities import ContainerEntity
 
 from ._rules import DMSProperty, DMSRules
@@ -23,14 +25,15 @@
         self.issue_list = IssueList()
 
     def validate(self) -> IssueList:
         self._consistent_container_properties()
         self._referenced_views_and_containers_are_existing()
         self._validate_extension()
         self._validate_schema()
+        self._validate_performance()
         return self.issue_list
 
     def _consistent_container_properties(self) -> None:
         container_properties_by_id: dict[tuple[ContainerEntity, str], list[tuple[int, DMSProperty]]] = defaultdict(list)
         for prop_no, prop in enumerate(self.properties):
             if prop.container and prop.container_property:
                 container_properties_by_id[(prop.container, prop.container_property)].append((prop_no, prop))
@@ -204,14 +207,44 @@
                 issues.dms.ChangingViewError(
                     view_id=view_id,
                     changed_properties=changed_properties or None,
                     changed_attributes=changed_attributes or None,
                 )
             )
 
+    def _validate_performance(self) -> None:
+        # we can only validate performance on complete schemas due to the need
+        # to access all the container mappings
+        if self.metadata.schema_ is not SchemaCompleteness.complete:
+            return None
+
+        dms_schema = self.rules.as_schema()
+
+        for view in dms_schema.views:
+            mapped_containers = dms_schema._get_mapped_container_from_view(view.as_id())
+
+            if mapped_containers and len(mapped_containers) > 10:
+                self.issue_list.append(
+                    issues.dms.ViewMapsToTooManyContainersWarning(
+                        view_id=view.as_id(),
+                        container_ids=mapped_containers,
+                    )
+                )
+                if (
+                    view.filter
+                    and isinstance(view.filter, dm.filters.HasData)
+                    and len(view.filter.dump()["hasData"]) > 10
+                ):
+                    self.issue_list.append(
+                        issues.dms.HasDataFilterAppliedToTooManyContainersWarning(
+                            view_id=view.as_id(),
+                            container_ids=mapped_containers,
+                        )
+                    )
+
     @staticmethod
     def _changed_attributes_and_properties(
         new_dumped: dict[str, Any], existing_dumped: dict[str, Any]
     ) -> tuple[list[str], list[str]]:
         """Helper method to find the changed attributes and properties between two containers or views."""
         new_attributes = {key: value for key, value in new_dumped.items() if key != "properties"}
         existing_attributes = {key: value for key, value in existing_dumped.items() if key != "properties"}
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/domain.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     parent: ParentEntityList | None = Field(alias="Parent Class")
 
 
 class DomainRules(RuleModel):
     metadata: DomainMetadata = Field(alias="Metadata")
     properties: SheetList[DomainProperty] = Field(alias="Properties")
     classes: SheetList[DomainClass] | None = Field(None, alias="Classes")
+    last: "DomainRules | None" = Field(None, alias="Last")
     reference: "DomainRules | None" = Field(None, alias="Reference")
 
     @model_serializer(mode="plain", when_used="always")
     def domain_rules_serializer(self, info: SerializationInfo) -> dict[str, Any]:
         kwargs = vars(info)
         output: dict[str, Any] = {
             "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/entities.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/information/_converter.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/information/_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from collections import defaultdict
 from datetime import datetime
 from typing import Literal
 
 from cognite.neat.rules.models._base import (
+    DataModelType,
     SheetList,
 )
 from cognite.neat.rules.models.data_types import DataType
 from cognite.neat.rules.models.dms._rules import DMSProperty, DMSRules, DMSView
 from cognite.neat.rules.models.domain import DomainRules
 from cognite.neat.rules.models.entities import (
     ClassEntity,
@@ -41,14 +42,15 @@
         default_version = info_metadata.version
         default_space = self._to_space(info_metadata.prefix)
         space = self._to_space(info_metadata.prefix)
 
         metadata = DMSMetadata(
             schema_=info_metadata.schema_,
             space=space,
+            data_model_type=DataModelType.solution if self.information.reference else DataModelType.enterprise,
             version=info_metadata.version,
             external_id=info_metadata.name.replace(" ", "_").lower(),
             creator=info_metadata.creator,
             name=info_metadata.name,
             created=created or datetime.now(),
             updated=updated or datetime.now(),
         )
```

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/information/_rules.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/information/_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/rules/models/wrapped_entities.py` & `cognite_neat-0.76.3/cognite/neat/rules/models/wrapped_entities.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/cdf.py` & `cognite_neat-0.76.3/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.76.3/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/exceptions.py` & `cognite_neat-0.76.3/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.76.3/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/text.py` & `cognite_neat-0.76.3/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/utils.py` & `cognite_neat-0.76.3/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/utils/xml.py` & `cognite_neat-0.76.3/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.76.3/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/base.py` & `cognite_neat-0.76.3/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.76.3/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.76.3/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/manager.py` & `cognite_neat-0.76.3/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.76.3/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.76.3/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/model.py` & `cognite_neat-0.76.3/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/graph_extractor.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/graph_loader.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/graph_store.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/rules_exporter.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,16 @@
         is_reference = self.configs.get("Is Reference") == "True"
         styling = cast(exporters.ExcelExporter.Style, self.configs.get("Styling", "default"))
         role = self.configs.get("Output role format")
         output_role = None
         if role != "input" and role is not None:
             output_role = RoleTypes[role]
 
-        excel_exporter = exporters.ExcelExporter(styling=styling, output_role=output_role, is_reference=is_reference)
+        dump_as = "reference" if is_reference else "user"
+        excel_exporter = exporters.ExcelExporter(styling=styling, output_role=output_role, dump_as=dump_as)  # type: ignore[arg-type]
 
         rule_instance: Rules
         if rules.domain:
             rule_instance = rules.domain
         elif rules.information:
             rule_instance = rules.information
         elif rules.dms:
```

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/rules_importer.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/current/rules_validator.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/current/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/io/io_steps.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/io/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_loader.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_store.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/lib/legacy/rules_importer.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/lib/legacy/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.76.3/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/tasks.py` & `cognite_neat-0.76.3/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/cognite/neat/workflows/triggers.py` & `cognite_neat-0.76.3/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.76.2/pyproject.toml` & `cognite_neat-0.76.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.76.2"
+version = "0.76.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.76.2/PKG-INFO` & `cognite_neat-0.76.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.76.2
+Version: 0.76.3
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

