# Comparing `tmp/cognite_neat-0.69.1.tar.gz` & `tmp/cognite_neat-0.69.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.69.1.tar", max compression
+gzip compressed data, was "cognite_neat-0.69.2.tar", max compression
```

## Comparing `cognite_neat-0.69.1.tar` & `cognite_neat-0.69.2.tar`

### file list

```diff
@@ -1,232 +1,232 @@
--rw-r--r--   0        0        0    11351 2024-04-08 14:25:38.785308 cognite_neat-0.69.1/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/README.md
--rw-r--r--   0        0        0       61 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1855 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     4646 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     6369 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    11564 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      629 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13345 2024-04-08 14:25:38.789308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1403536 2024-04-08 14:25:38.797308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js
--rw-r--r--   0        0        0     2667 2024-04-08 14:25:38.797308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt
--rw-r--r--   0        0        0  6235494 2024-04-08 14:25:38.821308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map
--rw-r--r--   0        0        0   240334 2024-04-08 14:25:38.837308 cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-08 14:25:38.845308 cognite_neat-0.69.1/cognite/neat/config.py
--rw-r--r--   0        0        0     1228 2024-04-08 14:25:38.845308 cognite_neat-0.69.1/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-08 14:25:38.845308 cognite_neat-0.69.1/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-08 14:25:38.845308 cognite_neat-0.69.1/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-08 14:25:38.849308 cognite_neat-0.69.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11232 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17408 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14969 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5377 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/rules/_analysis/__init__.py
--rw-r--r--   0        0        0      674 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/rules/_analysis/_base.py
--rw-r--r--   0        0        0    19613 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/rules/_analysis/_information_rules.py
--rw-r--r--   0        0        0      177 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-04-08 14:25:38.853309 cognite_neat-0.69.1/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5501 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    37099 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8220 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0     9688 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     9067 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19768 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7890 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-04-08 14:25:38.857308 cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0     8775 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7674 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7304 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     5594 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    10573 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     5856 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    11161 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     6916 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    16180 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0    10195 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     6079 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    10635 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    49231 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    29927 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     2051 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    20501 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7344 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4316 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2468 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26223 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-08 14:25:38.861308 cognite_neat-0.69.1/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    15674 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6528 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6040 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18272 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12274 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-08 14:25:38.865309 cognite_neat-0.69.1/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4543 2024-04-08 14:25:39.253311 cognite_neat-0.69.1/pyproject.toml
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.69.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/README.md
+-rw-r--r--   0        0        0       61 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1855 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     4646 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13653 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     6369 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    11564 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      629 2024-04-09 08:22:33.830274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-09 08:22:33.834274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-09 08:22:33.834274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-09 08:22:33.834274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-09 08:22:33.834274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13345 2024-04-09 08:22:33.834274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1403536 2024-04-09 08:22:33.838274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js
+-rw-r--r--   0        0        0     2667 2024-04-09 08:22:33.838274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt
+-rw-r--r--   0        0        0  6235494 2024-04-09 08:22:33.862274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map
+-rw-r--r--   0        0        0   240334 2024-04-09 08:22:33.882274 cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-09 08:22:33.890274 cognite_neat-0.69.2/cognite/neat/config.py
+-rw-r--r--   0        0        0     1228 2024-04-09 08:22:33.890274 cognite_neat-0.69.2/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-09 08:22:33.890274 cognite_neat-0.69.2/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-09 08:22:33.890274 cognite_neat-0.69.2/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-09 08:22:33.890274 cognite_neat-0.69.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/extractor/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/extractor/_base.py
+-rw-r--r--   0        0        0    11232 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/extractor/_dexpi.py
+-rw-r--r--   0        0        0    17408 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/extractor/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14872 2024-04-09 08:22:33.894274 cognite_neat-0.69.2/cognite/neat/graph/extractor/_mock_graph_generator.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14969 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      693 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/__init__.py
+-rw-r--r--   0        0        0    23838 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/_asset_loader.py
+-rw-r--r--   0        0        0     2370 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/core/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/core/labels.py
+-rw-r--r--   0        0        0     5016 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/core/models.py
+-rw-r--r--   0        0        0    40458 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22678 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12957 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/loader/validator.py
+-rw-r--r--   0        0        0      149 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14254 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5377 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/transformation/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/transformation/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/transformation/query_generator/__init__.py
+-rw-r--r--   0        0        0    18659 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/transformation/query_generator/sparql.py
+-rw-r--r--   0        0        0    14673 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/graph/transformation/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/_analysis/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/_analysis/_base.py
+-rw-r--r--   0        0        0    19613 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/_analysis/_information_rules.py
+-rw-r--r--   0        0        0      177 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0     8596 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5501 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-09 08:22:33.898274 cognite_neat-0.69.2/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_base.py
+-rw-r--r--   0        0        0      102 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_core/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_core/rules2labels.py
+-rw-r--r--   0        0        0    37099 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2dms.py
+-rw-r--r--   0        0        0     8220 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2excel.py
+-rw-r--r--   0        0        0     6215 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2graphql.py
+-rw-r--r--   0        0        0    18414 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2ontology.py
+-rw-r--r--   0        0        0    28745 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3866 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2rules.py
+-rw-r--r--   0        0        0     1104 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2triples.py
+-rw-r--r--   0        0        0     5769 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporter/_validation.py
+-rw-r--r--   0        0        0      413 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0     9688 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     9067 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19768 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4092 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_base.py
+-rw-r--r--   0        0        0     6469 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_dict2rules.py
+-rw-r--r--   0        0        0     7890 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_dms2rules.py
+-rw-r--r--   0        0        0    12097 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9320 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10521 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1529 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      448 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_xsd2rules.py
+-rw-r--r--   0        0        0     1628 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importer/_yaml2rules.py
+-rw-r--r--   0        0        0      408 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4268 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0     9138 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12554 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6925 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11926 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7674 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7304 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     5594 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    10573 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4198 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     5856 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    11167 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      127 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0      517 2024-04-09 08:22:33.902274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/__init__.py
+-rw-r--r--   0        0        0    17145 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/_base.py
+-rw-r--r--   0        0        0    10195 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/_field.py
+-rw-r--r--   0        0        0     6079 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/_value.py
+-rw-r--r--   0        0        0    10635 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/base.py
+-rw-r--r--   0        0        0    49323 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/dms_architect_rules.py
+-rw-r--r--   0        0        0    30010 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/dms_schema.py
+-rw-r--r--   0        0        0     2051 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/domain_rules.py
+-rw-r--r--   0        0        0    20657 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/_rules/information_rules.py
+-rw-r--r--   0        0        0    12368 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7344 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51063 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/tables.py
+-rw-r--r--   0        0        0     4316 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/rules/models/value_types.py
+-rw-r--r--   0        0        0       68 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2699 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26223 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Export DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Import DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
+-rw-r--r--   0        0        0    15674 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6528 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6040 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18272 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7327 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4785 2024-04-09 08:22:33.906274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29390 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27269 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12274 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2345 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20657 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28072 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-09 08:22:33.910274 cognite_neat-0.69.2/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4543 2024-04-09 08:22:34.294273 cognite_neat-0.69.2/pyproject.toml
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.69.2/PKG-INFO
```

### Comparing `cognite_neat-0.69.1/LICENSE` & `cognite_neat-0.69.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/README.md` & `cognite_neat-0.69.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/configuration.py` & `cognite_neat-0.69.2/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.69.2/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.69.2/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/explorer.py` & `cognite_neat-0.69.2/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.69.2/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.69.2/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.69.2/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.69.2/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.69.2/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.69.2/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.69.2/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.69.2/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.69.2/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.69.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/config.py` & `cognite_neat-0.69.2/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/constants.py` & `cognite_neat-0.69.2/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/exceptions.py` & `cognite_neat-0.69.2/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.69.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.69.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.69.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/exceptions.py` & `cognite_neat-0.69.2/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.69.2/cognite/neat/graph/extractor/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.69.2/cognite/neat/graph/extractor/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.69.2/cognite/neat/graph/extractor/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.69.2/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.69.2/cognite/neat/graph/loader/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.69.2/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.69.2/cognite/neat/graph/transformation/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.69.2/cognite/neat/graph/transformation/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.69.2/cognite/neat/graph/transformation/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/_analysis/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/_analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/_analysis/_information_rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/_analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/analysis.py` & `cognite_neat-0.69.2/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.69.2/cognite/neat/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.69.2/cognite/neat/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.69.2/cognite/neat/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.69.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.69.2/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exceptions.py` & `cognite_neat-0.69.2/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporter/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.69.2/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importer/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import DataModelIdentifier
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex, InvertedIndex
 from cognite.client.data_classes.data_modeling.data_types import ListablePropertyType
 
+from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models._rules import DMSRules, DMSSchema, RoleTypes
 from cognite.neat.rules.models._rules._types import (
     ClassEntity,
     ContainerEntity,
     DMSValueType,
+    Undefined,
+    Unknown,
     ViewEntity,
     ViewPropEntity,
 )
 from cognite.neat.rules.models._rules.dms_architect_rules import (
     DMSContainer,
     DMSMetadata,
     DMSProperty,
@@ -59,20 +62,22 @@
         self,
         errors: Literal["raise", "continue"] = "continue",
         role: RoleTypes | None = None,
         is_reference: bool = False,
     ) -> tuple[Rules | None, IssueList] | Rules:
         if role is RoleTypes.domain_expert:
             raise ValueError(f"Role {role} is not supported for DMSImporter")
+        issue_list = IssueList()
         data_model = self.schema.data_models[0]
 
         container_by_id = {container.as_id(): container for container in self.schema.containers}
 
         properties = SheetList[DMSProperty]()
         for view in self.schema.views:
+            class_entity = ClassEntity(prefix=view.space, suffix=view.external_id, version=view.version)
             for prop_id, prop in (view.properties or {}).items():
                 if isinstance(prop, dm.MappedPropertyApply):
                     if prop.container not in container_by_id:
                         raise ValueError(f"Container {prop.container} not found")
                     container = container_by_id[prop.container]
                     if prop.container_property_identifier not in container.properties:
                         raise ValueError(
@@ -99,20 +104,23 @@
                             continue
                         else:
                             raise NotImplementedError(f"Constraint type {type(constraint_obj)} not implemented")
 
                     if isinstance(container_prop.type, dm.DirectRelation):
                         direct_value_type: str | ViewEntity | DMSValueType
                         if prop.source is None:
-                            direct_value_type = "UNKNOWN"
+                            issue_list.append(
+                                issues.importing.UnknownValueTypeWarning(class_entity.versioned_id, prop_id)
+                            )
+                            direct_value_type = ViewPropEntity(prefix=Undefined, suffix=Unknown)
                         else:
                             direct_value_type = ViewPropEntity.from_id(prop.source)
 
                         dms_property = DMSProperty(
-                            class_=ClassEntity(prefix=view.space, suffix=view.external_id, version=view.version),
+                            class_=class_entity,
                             property_=prop_id,
                             description=prop.description,
                             value_type=cast(ViewPropEntity | DMSValueType, direct_value_type),
                             relation="direct",
                             nullable=container_prop.nullable,
                             default=container_prop.default_value,
                             is_list=False,
@@ -176,8 +184,8 @@
         if role is RoleTypes.information_architect:
             output_rules = dms_rules.as_information_architect_rules()
         else:
             output_rules = dms_rules
         if errors == "raise":
             return output_rules
         else:
-            return output_rules, IssueList()
+            return output_rules, issue_list
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/base.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "MissingContainerError",
     "MissingContainerPropertyError",
     "MissingViewError",
     "MissingParentViewError",
     "MissingSourceViewError",
     "MissingEdgeViewError",
     "DuplicatedViewInDataModelError",
-    "DirectRelationMissingSourceError",
+    "DirectRelationMissingSourceWarning",
     "ContainerPropertyUsedMultipleTimesError",
     "DirectRelationListWarning",
     "ReverseOfDirectRelationListWarning",
     "EmptyContainerWarning",
     "UnsupportedRelationWarning",
     "MultipleReferenceWarning",
 ]
@@ -179,15 +179,15 @@
         output = super().dump()
         output["referred_by"] = self.referred_by
         output["view"] = self.view
         return output
 
 
 @dataclass(frozen=True)
-class DirectRelationMissingSourceError(DMSSchemaError):
+class DirectRelationMissingSourceWarning(DMSSchemaWarning):
     description = "The source view referred to by the DirectRelation does not exist"
     fix = "Create the source view"
     error_name: ClassVar[str] = "DirectRelationMissingSource"
     view_id: dm.ViewId
     property: str
 
     def message(self) -> str:
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/importing.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 __all__ = [
     "ModelImportWarning",
     "UnknownComponentWarning",
     "UnknownSubComponentWarning",
     "IgnoredComponentWarning",
     "UnknownPropertyWarning",
+    "UnknownValueTypeWarning",
     "ModelImportError",
     "InvalidComponentError",
     "MissingParentDefinitionError",
     "MissingIdentifierError",
     "UnsupportedPropertyTypeError",
 ]
 
@@ -111,14 +112,31 @@
             )
         else:
             prefix = f"Unknown property '{self.property_name}' of component '{self.component_type}'"
         return f"{prefix} This will be ignored in the imports."
 
 
 @dataclass(frozen=True)
+class UnknownValueTypeWarning(ModelImportWarning):
+    description = "Unknown value type. This limits validation done by NEAT. "
+    fix = "Set the value type"
+    class_id: str
+    property_id: str
+
+    def dump(self) -> dict[str, str]:
+        return {"class_id": self.class_id, "property_id": self.property_id}
+
+    def message(self) -> str:
+        return (
+            f"Unknown value type for property '{self.property_id}' of class '{self.class_id}'. "
+            "This limits validation done by NEAT."
+        )
+
+
+@dataclass(frozen=True)
 class ModelImportError(NeatValidationError, ABC):
     description = "An error was raised during importing."
     fix = "No fix is available."
 
 
 @dataclass(frozen=True)
 class InvalidComponentError(ModelImportError, ABC):
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.69.2/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     ContainerEntity,
     DataModelEntity,
     Entity,
     EntityTypes,
     ParentClassEntity,
     ReferenceEntity,
     Undefined,
+    Unknown,
     ViewEntity,
     ViewPropEntity,
 )
 from ._field import (
     CdfValueType,
     ClassType,
     ContainerListType,
@@ -28,14 +29,15 @@
     ViewListType,
     ViewType,
 )
 from ._value import DMS_VALUE_TYPE_MAPPINGS, XSD_VALUE_TYPE_MAPPINGS, DMSValueType, XSDValueType
 
 __all__ = [
     "Undefined",
+    "Unknown",
     "Entity",
     "EntityTypes",
     "ClassEntity",
     "ParentClassEntity",
     "ContainerEntity",
     "ViewEntity",
     "ViewPropEntity",
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import sys
 from functools import total_ordering
-from typing import Any, ClassVar, cast
+from typing import Any, ClassVar, Literal, cast, overload
 
 from cognite.client.data_classes.data_modeling import ContainerId, DataModelId, PropertyId, ViewId
 from pydantic import BaseModel
 
 from cognite.neat.rules.models.rdfpath import (
     SINGLE_PROPERTY_REGEX_COMPILED,
     AllReferences,
@@ -85,26 +85,27 @@
 )
 CLASS_ID_COMPLIANCE_REGEX = r"(?!^(Class|class)$)(^[a-zA-Z][a-zA-Z0-9._-]{0,253}[a-zA-Z0-9]?$)"
 PROPERTY_ID_COMPLIANCE_REGEX = r"^(\*)|(?!^(Property|property)$)(^[a-zA-Z][a-zA-Z0-9._-]{0,253}[a-zA-Z0-9]?$)"
 VERSION_COMPLIANCE_REGEX = r"^[a-zA-Z0-9]([.a-zA-Z0-9_-]{0,41}[a-zA-Z0-9])?$"
 
 
 Undefined = type(object())
+Unknown = type(object())
 
 
 # mypy does not like the sentinel value, and it is not possible to ignore only the line with it below.
 # so we ignore all errors beyond this point.
 # mypy: ignore-errors
 @total_ordering
 class Entity(BaseModel, arbitrary_types_allowed=True):
     """Entity is a class or property in OWL/RDF sense."""
 
     type_: ClassVar[EntityTypes] = EntityTypes.undefined
     prefix: str | Undefined = Undefined
-    suffix: str
+    suffix: str | Unknown
     version: str | None = None
     name: str | None = None
     description: str | None = None
 
     def __lt__(self, other: object) -> bool:
         if type(self) is not type(other) or not isinstance(other, Entity):
             return NotImplemented
@@ -119,15 +120,17 @@
         return hash(self.versioned_id)
 
     def as_non_versioned_entity(self) -> Self:
         return self.from_string(f"{self.prefix}:{self.suffix}")
 
     @property
     def id(self) -> str:
-        if self.prefix is Undefined:
+        if self.suffix is Unknown:
+            return "#N/A"
+        elif self.prefix is Undefined:
             return self.suffix
         else:
             return f"{self.prefix}:{self.suffix}"
 
     @property
     def versioned_id(self) -> str:
         if self.version is None:
@@ -149,15 +152,17 @@
         return self.versioned_id
 
     def __str__(self):
         return self.versioned_id
 
     @classmethod
     def from_string(cls, entity_string: str, base_prefix: str | None = None) -> Self:
-        if result := VERSIONED_ENTITY_REGEX_COMPILED.match(entity_string):
+        if entity_string == "#N/A":
+            return cls(prefix=Undefined, suffix=Unknown)
+        elif result := VERSIONED_ENTITY_REGEX_COMPILED.match(entity_string):
             return cls(
                 prefix=result.group("prefix"),
                 suffix=result.group("suffix"),
                 version=result.group("version"),
             )
         elif result := ENTITY_ID_REGEX_COMPILED.match(entity_string):
             return cls(prefix=result.group("prefix"), suffix=result.group("suffix"))
@@ -218,25 +223,52 @@
         else:
             return cls(prefix=Undefined, suffix=value)
 
     @classmethod
     def from_id(cls, view_id: ViewId) -> Self:
         return cls(prefix=view_id.space, suffix=view_id.external_id, version=view_id.version)
 
+    @overload
     def as_id(
-        self, default_space: str | None = None, default_version: str | None = None, standardize_casing: bool = True
+        self,
+        allow_none: Literal[False] = False,
+        default_space: str | None = None,
+        default_version: str | None = None,
+        standardize_casing: bool = True,
     ) -> ViewId:
+        ...
+
+    @overload
+    def as_id(
+        self,
+        allow_none: Literal[True],
+        default_space: str | None = None,
+        default_version: str | None = None,
+        standardize_casing: bool = True,
+    ) -> ViewId | None:
+        ...
+
+    def as_id(
+        self,
+        allow_none: bool = False,
+        default_space: str | None = None,
+        default_version: str | None = None,
+        standardize_casing: bool = True,
+    ) -> ViewId | None:
+        if self.suffix is Unknown and allow_none:
+            return None
+        elif self.suffix is Unknown:
+            raise ValueError("suffix is Unknown and cannot be converted to ViewId")
         space = default_space if self.space is Undefined else self.space
         version = self.version or default_version
 
         if space is None or space is Undefined:
             raise ValueError("space is required")
         if version is None:
             raise ValueError("version is required")
-
         external_id = to_pascal(self.external_id) if standardize_casing else self.external_id
         return ViewId(space=space, external_id=external_id, version=version)
 
 
 class ViewPropEntity(ViewEntity):
     type_: ClassVar[EntityTypes] = EntityTypes.view_prop
     property_: str | None = None
@@ -273,15 +305,15 @@
 
     def as_prop_id(
         self, default_space: str | None = None, default_version: str | None = None, standardize_casing: bool = True
     ) -> PropertyId:
         if self.property_ is None:
             raise ValueError("property is required to create PropertyId")
         return PropertyId(
-            source=self.as_id(default_space, default_version, standardize_casing), property=self.property_
+            source=self.as_id(False, default_space, default_version, standardize_casing), property=self.property_
         )
 
     @property
     def versioned_id(self) -> str:
         if self.version is None and self.property_ is None:
             output = self.id
         elif self.version is None:
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/dms_architect_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,23 +242,24 @@
 class DMSView(SheetEntity):
     view: ViewType = Field(alias="View")
     implements: ViewListType | None = Field(None, alias="Implements")
     reference: ReferenceType = Field(alias="Reference", default=None)
     in_model: bool = Field(True, alias="InModel")
 
     def as_view(self, default_space: str, default_version: str, standardize_casing: bool = True) -> dm.ViewApply:
-        view_id = self.view.as_id(default_space, default_version, standardize_casing)
+        view_id = self.view.as_id(False, default_space, default_version, standardize_casing)
         return dm.ViewApply(
             space=view_id.space,
             external_id=view_id.external_id,
             version=view_id.version or default_version,
             name=self.name or None,
             description=self.description,
             implements=[
-                parent.as_id(default_space, default_version, standardize_casing) for parent in self.implements or []
+                parent.as_id(False, default_space, default_version, standardize_casing)
+                for parent in self.implements or []
             ]
             or None,
             properties={},
         )
 
     @classmethod
     def from_view(cls, view: dm.ViewApply, data_model_view_ids: set[dm.ViewId]) -> "DMSView":
@@ -433,21 +434,21 @@
         if errors:
             raise issues.MultiValueError(errors)
         return self
 
     @model_validator(mode="after")
     def referenced_views_and_containers_are_existing(self) -> "DMSRules":
         # There two checks are done in the same method to raise all the errors at once.
-        defined_views = {view.view.as_id(self.metadata.space, self.metadata.version) for view in self.views}
+        defined_views = {view.view.as_id(False, self.metadata.space, self.metadata.version) for view in self.views}
 
         errors: list[issues.NeatValidationError] = []
         for prop_no, prop in enumerate(self.properties):
             if (
                 prop.view
-                and (view_id := prop.view.as_id(self.metadata.space, self.metadata.version)) not in defined_views
+                and (view_id := prop.view.as_id(False, self.metadata.space, self.metadata.version)) not in defined_views
             ):
                 errors.append(
                     cognite.neat.rules.issues.spreadsheet.NonExistingViewError(
                         column="View",
                         row=prop_no,
                         type="value_error.missing",
                         view_id=view_id,
@@ -622,15 +623,15 @@
         containers = self._create_containers(rules.containers, container_properties_by_id, default_space)
 
         views, node_types = self._create_views_with_node_types(
             rules.views, view_properties_by_id, default_space, default_version
         )
 
         views_not_in_model = {
-            view.view.as_id(default_space, default_version, self.standardize_casing)
+            view.view.as_id(False, default_space, default_version, self.standardize_casing)
             for view in rules.views
             if not view.in_model
         }
         data_model = rules.metadata.as_data_model()
         data_model.views = [view_id for view_id in views.as_ids() if view_id not in views_not_in_model]
 
         spaces = self._create_spaces(rules.metadata, containers, views, data_model)
@@ -681,15 +682,15 @@
                 continue
             for prop in view_properties:
                 view_property: ViewPropertyApply
                 if prop.is_list and prop.relation == "direct":
                     # This is not yet supported in the CDF API, a warning has already been issued, here we convert it to
                     # a multi-edge connection.
                     if isinstance(prop.value_type, ViewEntity):
-                        source = prop.value_type.as_id(default_space, default_version, self.standardize_casing)
+                        source = prop.value_type.as_id(False, default_space, default_version, self.standardize_casing)
                     else:
                         raise ValueError(
                             "Direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MultiEdgeConnectionApply(
                         type=dm.DirectRelationReference(
@@ -702,29 +703,29 @@
                 elif prop.container and prop.container_property and prop.view_property:
                     container_prop_identifier = (
                         to_camel(prop.container_property) if self.standardize_casing else prop.container_property
                     )
                     extra_args: dict[str, Any] = {}
                     if prop.relation == "direct" and isinstance(prop.value_type, ViewEntity):
                         extra_args["source"] = prop.value_type.as_id(
-                            default_space, default_version, self.standardize_casing
+                            True, default_space, default_version, self.standardize_casing
                         )
                     elif prop.relation == "direct" and not isinstance(prop.value_type, ViewEntity):
                         raise ValueError(
                             "Direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MappedPropertyApply(
                         container=prop.container.as_id(default_space, self.standardize_casing),
                         container_property_identifier=container_prop_identifier,
                         **extra_args,
                     )
                 elif prop.view and prop.view_property and prop.relation == "multiedge":
                     if isinstance(prop.value_type, ViewEntity):
-                        source = prop.value_type.as_id(default_space, default_version, self.standardize_casing)
+                        source = prop.value_type.as_id(False, default_space, default_version, self.standardize_casing)
                     else:
                         raise ValueError(
                             "Multiedge relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MultiEdgeConnectionApply(
                         type=dm.DirectRelationReference(
@@ -732,15 +733,15 @@
                             external_id=f"{prop.view.external_id}.{prop.view_property}",
                         ),
                         source=source,
                         direction="outwards",
                     )
                 elif prop.view and prop.view_property and prop.relation == "reversedirect":
                     if isinstance(prop.value_type, ViewPropEntity):
-                        source = prop.value_type.as_id(default_space, default_version, self.standardize_casing)
+                        source = prop.value_type.as_id(False, default_space, default_version, self.standardize_casing)
                     else:
                         raise ValueError(
                             "Reverse direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     source_prop = prop.value_type.property_
                     if source_prop is None:
@@ -900,23 +901,23 @@
 
     def _gather_properties(
         self, rules: DMSRules, default_space: str, default_version: str
     ) -> tuple[dict[dm.ContainerId, list[DMSProperty]], dict[dm.ViewId, list[DMSProperty]]]:
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]] = defaultdict(list)
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]] = defaultdict(list)
         for prop in rules.properties:
-            view_id = prop.view.as_id(default_space, default_version, self.standardize_casing)
+            view_id = prop.view.as_id(False, default_space, default_version, self.standardize_casing)
             view_properties_by_id[view_id].append(prop)
 
             if prop.container and prop.container_property:
                 if prop.relation == "direct" and prop.is_list:
                     warnings.warn(
                         issues.dms.DirectRelationListWarning(
                             container_id=prop.container.as_id(default_space, self.standardize_casing),
-                            view_id=prop.view.as_id(default_space, default_version, self.standardize_casing),
+                            view_id=prop.view.as_id(False, default_space, default_version, self.standardize_casing),
                             property=prop.container_property,
                         ),
                         stacklevel=2,
                     )
                     continue
                 container_id = prop.container.as_id(default_space, self.standardize_casing)
                 container_properties_by_id[container_id].append(prop)
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/dms_schema.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/dms_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes import DatabaseWrite, DatabaseWriteList, TransformationWrite, TransformationWriteList
 from cognite.client.data_classes.data_modeling import ViewApply
 from cognite.client.data_classes.transformations.common import Edges, EdgeType, Nodes, ViewInfo
 
 from cognite.neat.rules.issues.dms import (
     ContainerPropertyUsedMultipleTimesError,
-    DirectRelationMissingSourceError,
+    DirectRelationMissingSourceWarning,
     DMSSchemaError,
     DuplicatedViewInDataModelError,
     MissingContainerError,
     MissingContainerPropertyError,
     MissingEdgeViewError,
     MissingParentViewError,
     MissingSourceViewError,
@@ -307,15 +307,17 @@
                                 referred_by=view_id,
                             )
                         )
                     else:
                         container_property = ref_container.properties[prop.container_property_identifier]
 
                         if isinstance(container_property.type, dm.DirectRelation) and prop.source is None:
-                            errors.add(DirectRelationMissingSourceError(view_id=view_id, property=prop_name))
+                            warnings.warn(
+                                DirectRelationMissingSourceWarning(view_id=view_id, property=prop_name), stacklevel=2
+                            )
 
                 if isinstance(prop, dm.EdgeConnectionApply) and prop.source not in defined_views:
                     errors.add(MissingSourceViewError(view=prop.source, property=prop_name, referred_by=view_id))
 
                 if (
                     isinstance(prop, dm.EdgeConnectionApply)
                     and prop.edge_source is not None
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/_rules/information_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     Traversal,
     parse_rule,
 )
 
 from ._types import (
     ClassEntity,
     ContainerEntity,
+    Entity,
     EntityTypes,
     NamespaceType,
     ParentClassEntity,
     ParentClassType,
     PrefixType,
     PropertyType,
     ReferenceEntity,
@@ -38,14 +39,15 @@
     StrListType,
     Undefined,
     VersionType,
     ViewEntity,
     ViewPropEntity,
     XSDValueType,
 )
+from ._types._base import Unknown
 from .base import (
     BaseMetadata,
     ExtensionCategory,
     MatchType,
     RoleTypes,
     RuleModel,
     SchemaCompleteness,
@@ -268,14 +270,15 @@
             referred_classes = {property_.class_.versioned_id for property_ in self.properties} | {
                 parent.versioned_id for class_ in self.classes for parent in class_.parent or []
             }
             referred_types = {
                 property_.value_type.versioned_id
                 for property_ in self.properties
                 if property_.type_ == EntityTypes.object_property
+                and not (isinstance(property_.value_type, Entity) and property_.value_type.suffix is Unknown)
             }
             if not referred_classes.issubset(defined_classes) or not referred_types.issubset(defined_classes):
                 missing_classes = referred_classes.difference(defined_classes).union(
                     referred_types.difference(defined_classes)
                 )
                 raise exceptions.IncompleteSchema(missing_classes).to_pydantic_custom_error()
```

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/rules.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.69.2/cognite/neat/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/cdf.py` & `cognite_neat-0.69.2/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.69.2/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/exceptions.py` & `cognite_neat-0.69.2/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.69.2/cognite/neat/utils/spreadsheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,17 +63,21 @@
     else:
         skiprows = 0
 
     raw = pd.read_excel(excel_file, sheet_name, skiprows=skiprows)
     is_na = raw.isnull().all(axis=1)
     empty_rows = is_na[is_na].index.tolist()
 
-    output = raw.dropna(axis=0, how="all").replace(float("nan"), None).to_dict(orient="records")
+    raw.dropna(axis=0, how="all", inplace=True)
+    if "Value Type" in raw.columns:
+        # Special handling for Value Type column, #N/A is treated specially by NEAT it means Unknown
+        raw["Value Type"] = raw["Value Type"].replace(float("nan"), "#N/A")
+    output = raw.replace(float("nan"), None).to_dict(orient="records")
     if return_read_info:
-        return output, SpreadsheetRead(header_row=skiprows + 1, empty_rows=empty_rows, is_one_indexed=True)
+        return output, SpreadsheetRead(header_row=skiprows, empty_rows=empty_rows, is_one_indexed=True)
     return output
 
 
 def _get_row_number(sheet: Worksheet, values_to_find: list[str]) -> int | None:
     for row_number, row in enumerate(sheet.iter_rows(values_only=True), start=1):
         if any(value in row for value in values_to_find):
             return row_number
```

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/text.py` & `cognite_neat-0.69.2/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/utils.py` & `cognite_neat-0.69.2/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/utils/xml.py` & `cognite_neat-0.69.2/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.69.2/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/base.py` & `cognite_neat-0.69.2/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.69.2/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Export DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Import DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Validate Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.69.2/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/manager.py` & `cognite_neat-0.69.2/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.69.2/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.69.2/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/model.py` & `cognite_neat-0.69.2/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.69.2/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/tasks.py` & `cognite_neat-0.69.2/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/cognite/neat/workflows/triggers.py` & `cognite_neat-0.69.2/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.69.1/pyproject.toml` & `cognite_neat-0.69.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.69.1"
+version = "0.69.2"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.69.1/PKG-INFO` & `cognite_neat-0.69.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.69.1
+Version: 0.69.2
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

